<template>
  <div id="section-steps">

    <span class="counter" :style="{top: (27 * (currentSection)) - 6 + 'px'}">
      0{{currentSection+1}}
    </span>

    <div class="lines">
      <div v-for="(section, index) in sections" :id="index" :class="{active: index == currentSection}" class="line"></div>
    </div>

  </div>
</template>

<script>
import $ from 'jquery'

export default {
  name: 'SectionSteps',
  props: ['sections', 'currentSection'],
  data: function() {
    return {
      activeClass: 'active'
    }
  },
  computed: {
    isActive: function(element) {
      console.log(element);
      // return this.currentSection == element
    }
  }
}
</script>
