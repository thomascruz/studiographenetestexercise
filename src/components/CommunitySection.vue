<template>
  <section id="community-section">
    <div class="wrapper flex flex-end">

      <div class="item item-1-4 item-filler"></div>

      <div class="item item-1-4">
        <h2 class="crossed-title"><span class="crossed">Meet our<br>Community</span></h2>
        <button class="btn btn-pink" type="button">Know more</button>

        <h3 class="subtitle">LOREM IPSUM DOLOR SIT AMET ERNUT TEMPARTERO SERTU PER NABORE EN TORNA ENTALTO</h3>
      </div>

      <div class="item item-1-4 community-card insta-card">
        <div id="decor-1" class="decoration decor-plus"></div>

        <div class="wrapper">
          <div class="insta-badge">
            <img src="../assets/insta-badge.svg">
          </div>
          <img class="insta-photo" src="../assets/insta1.png">
        </div>
      </div>

      <div class="item item-1-4 community-card text-card">
        <div id="decor-2" class="decoration decor-stripes"></div>

        <div class="wrapper">
          <h4 class="card-title">@buzzfeedfood</h4>
          <p class="card-text">It’s taco Tuesday! These tacos from @jesseszewczyk have no added sugars and are SO good 🌮. Find the recipe from the link in our bio! 📸: @taylormillerphoto</p>
          <div class="card-actions">
            <div class="action">
              <p class="icon like-icon">60</p>
            </div>
            <div class="action">
              <p class="icon comment-icon">14.7K</p>
            </div>
          </div>
        </div>
      </div>

      <div class="item item-1-4 community-card text-card">
        <div id="decor-3" class="decoration decor-dots"></div>

        <div class="wrapper">
          <h4 class="card-title">@love_food</h4>
          <p class="card-text">Waffle sticks in Copenhagen! 🇩🇰😍 Milk chocolate with sprinkles, dark chocolate with coconut and milk chocolate with peanuts! [📷: @foodwithmichel] #lovefood</p>
          <div class="card-actions">
            <div class="action">
              <p class="icon like-icon">789</p>
            </div>
            <div class="action">
              <p class="icon comment-icon">99.7K</p>
            </div>
          </div>
        </div>
      </div>

      <div class="item item-1-4 community-card insta-card">
        <div class="wrapper">
          <div class="insta-badge">
            <img src="../assets/insta-badge.svg">
          </div>
          <img class="insta-photo"src="../assets/insta2.png" alt="">
        </div>
      </div>

      <div class="item item-1-4 card">
        <div class="wrapper">
          <p class="text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Duis aute irure.</p>
        </div>
      </div>

      <div class="item item-1-4 item-filler"></div>

      <div class="item item-1-4 card">
        <div class="wrapper">
          <p class="text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Duis aute irure.</p>
        </div>
      </div>

      <div class="item item-1-4 item-filler"></div>

      <div class="item item-1-4 community-card text-card">
        <div class="wrapper">
          <h4 class="card-title">@buzzfeedfood</h4>
          <p class="card-text">Getting into long weekend mode like 🍤 #pancitpalabok (📷 @jeepneynyc)</p>
          <div class="card-actions">
            <div class="action">
              <p class="icon like-icon">152</p>
            </div>
            <div class="action">
              <p class="icon comment-icon">18.2K</p>
            </div>
          </div>
        </div>
      </div>

      <div class="item item-1-4 community-card insta-card">
        <div class="wrapper">
          <div class="insta-badge">
            <img src="../assets/insta-badge.svg">
          </div>
          <img class="insta-photo" src="../assets/insta3.png" alt="">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import $ from 'jquery'

export default {
  name: 'CommunitySection',
  props: { },
  mounted: function () {
  }
}
</script>
