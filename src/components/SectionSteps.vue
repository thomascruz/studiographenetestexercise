<template>
  <div id="section-steps">

    <span class="counter">
      01
    </span>

    <div class="lines">
      <div class="line" :class="{ active: activeClass }"></div>
      <div class="line"></div>
      <div class="line"></div>
    </div>

  </div>
</template>

<script>
import $ from 'jquery'

export default {
  name: 'SectionSteps',
  data: function() {
    return {
      activeClass: 'active'
    }
  },
  computed: {
    currentPage() {
      console.log(this.$route);
    }
  }
}
</script>
