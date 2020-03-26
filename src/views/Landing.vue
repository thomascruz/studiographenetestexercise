<template>
  <div id="Landing">
    <Header/>

    <div class="sections">
      <SectionSteps :sections="sections" :current-section="currentSection"/>

      <BannerSection/>
      <CommunitySection/>
      <LocationSection/>
      <MenuSection/>

      <CollaborateSection/>
    </div>

    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'

import BannerSection from '@/components/BannerSection.vue'
import CommunitySection from '@/components/CommunitySection.vue'
import LocationSection from '@/components/LocationSection.vue'
import MenuSection from '@/components/MenuSection.vue'
import CollaborateSection from '@/components/CollaborateSection.vue'
import SectionSteps from '@/components/SectionSteps.vue'

import Footer from '@/components/Footer.vue'

import ScrollMagic from 'scrollmagic';

export default {
  name: 'Landing',
  components: {
    Header,
    SectionSteps,
    BannerSection,
    CommunitySection,
    LocationSection,
    MenuSection,
    CollaborateSection,
    Footer
  },
  data: function() {
    return {
      currentSection: 0,
      sections: [
        {
          id: 'banner-section'
        },
        {
          id: 'community-section'
        },
        {
          id: 'location-section'
        },
        {
          id: 'menu-section'
        },
        {
          id: 'collaborate-section'
        },
      ]
    }
  },
  methods: {
    setSectionStep: function(section, interator) {
      console.log(section.id);
      var interatorVal = interator ? interator : 0;

      for (var i = 0; i < this.sections.length; i++) {
        this.currentSection = this.sections[i].id === section.id ? i + interatorVal : this.currentSection;
      }
    }
  },
  mounted: function () {
    let self = this;

    let controller = new ScrollMagic.Controller();
    let sections = document.querySelectorAll("section.landing-section");

    // INDICATOR ANIMATION
    for (var i = 0; i < sections.length; i++) {
      new ScrollMagic.Scene({
              triggerElement: sections[i],
              triggerHook: 0.95,
            })
            .on("enter", function (event) {
              console.log("enter");
              self.setSectionStep(event.target.triggerElement());
            })
            .addTo(controller);

      new ScrollMagic.Scene({
              triggerElement: sections[i],
              triggerHook: 0.4,
            })
            .on("leave", function (event) {
              console.log("leave");
              self.setSectionStep(event.target.triggerElement(), -1);
            })
            .addTo(controller);
    }

    // COMMUNITY CARDS ANIMATION
    new ScrollMagic.Scene({
            triggerElement: "#community-section",
            triggerHook: 0.6,
            reverse: false
          })
          .setClassToggle(".animated-card-1", "card-enter-scene")
          .addTo(controller);

    new ScrollMagic.Scene({
            triggerElement: "#community-section",
            triggerHook: 0.3,
            reverse: false
          })
          .setClassToggle(".animated-card-2", "card-enter-scene")
          .addTo(controller);

    new ScrollMagic.Scene({
            triggerElement: "#community-section",
            triggerHook: 0,
            reverse: false
          })
          .setClassToggle(".animated-card-3", "card-enter-scene")
          .addTo(controller);

    // MENU ANIMATION
  }
}
</script>
