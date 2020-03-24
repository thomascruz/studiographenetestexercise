<template>
  <section id="banner-section">
    <div class="wrapper">

      <div id="gourmet-exp-badge">
        <div id="circle-text" text="GOURMET EXPERIENCE • GOURMET EXPERIENCE • "></div>
        <span id="text-inside">Logo</span>
      </div>

      <div class="center-title">
        <h1 class="title">
          The best foodie<br>
          <span class="large">experience</span>
        </h1>
        <p class="sub-title">now in London</p>
      </div>

    </div>
  </section>
</template>

<script>
import $ from 'jquery'

export default {
  name: 'BannerSection',
  props: { },
  mounted: function () {
    let circleElement = $('#circle-text');
    let phrase = circleElement.attr('text');

    for (var i = 0; i < phrase.length; i++) {
      circleElement.append("<span class='circle-letter'>" + phrase[i] + "</span>");
    }

    let letters = $('.circle-letter');
    let step = 360 / letters.length;

    letters.each(function(index) {
      $(this).css('transform', 'rotate(' + (((index + 2) * step) + 90 )  + 'deg)');
    });
  }
}
</script>
