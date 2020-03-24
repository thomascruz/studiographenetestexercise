<template>
  <div id="Landing">
    <Header/>

    <div class="sections">
      <SectionSteps/>

      <BannerSection/>
      <CommunitySection/>
      <LocationSection/>

      <CollaborateSection/>
    </div>

    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'

import BannerSection from '@/components/BannerSection.vue'
import CommunitySection from '@/components/CommunitySection.vue'
import LocationSection from '@/components/LocationSection.vue'
import CollaborateSection from '@/components/CollaborateSection.vue'
import SectionSteps from '@/components/SectionSteps.vue'

import Footer from '@/components/Footer.vue'

import $ from 'jquery';
import easyScroll from 'easy-scroll';

export default {
  name: 'Landing',
  components: {
    Header,
    SectionSteps,
    BannerSection,
    CommunitySection,
    LocationSection,
    CollaborateSection,
    Footer
  },
  data: function() {
    return {
      sections: [
        {
          id: 'banner-section'
        },
        {
          id: 'community-section'
        },
        {
          id: 'location-section'
        }
      ]
    }
  },
  mounted: function () {
    let scrollEvt = {
      event: {},
    };

    let position = $(window).scrollTop();

    $(window).scroll(function() {

      let scroll = $(window).scrollTop();

      if (scroll > position) {
        console.log('scrollDown');
        // easyScroll({
        //   'scrollableDomEle': window,
        //   'direction': 'bottom',
        //   'duration': 1000,
        //   'easingPreset': 'easeInOutCubic',
        //   'scrollAmount': 200
        // });
      } else {
        console.log('scrollUp');
      }
      position = scroll;
    });

  }
}
</script>
