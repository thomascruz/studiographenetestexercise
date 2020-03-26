<template>
  <section class="landing-section" id="menu-section">
    <div class="wrapper">

      <div class="section-title">
        <h2 class="crossed-title"><span class="crossed"><br>Our Menu</span></h2>
        <button class="btn btn-pink" type="button">Know more</button>
      </div>

      <div class="menu-sections">

        <section class="menu-section menu-odd" id="menu-section-1">
          <div class="wrapper animate-out">

            <h3 class="title">Starters</h3>

            <div class="menu-option">
              <h4 class="menu-option-title">Quinoa Croquettas</h4>
              <p class="menu-option-description">
                Quinoa and cheddar croquettas with aji rocotto & pineapple salsa (v)
              </p>
              <button class="btn btn-pink-border">£4.95</button>
            </div>

            <div class="menu-option">
              <h4 class="menu-option-title">CHIFA CHICHARRONES</h4>
              <p class="menu-option-description">
                Slow cooked, crispy pork belly with sweet soy sauce
              </p>
              <button class="btn btn-pink-border">£6.95</button>
            </div>

            <div class="menu-option">
              <h4 class="menu-option-title">CALAMARES</h4>
              <p class="menu-option-description">
                Crispy baby squid with pickled jalapeño miso salsa
              </p>
              <button class="btn btn-pink-border">£6.95</button>
            </div>

          </div>
        </section>

        <section class="menu-section menu-even" id="menu-section-2">
          <div class="wrapper animate-out">

            <h3 class="title">Main<br>Courses</h3>

            <div class="menu-option">
              <h4 class="menu-option-title">El Classico</h4>
              <p class="menu-option-description">
                Sea bass ceviche with aji limo tiger’s milk, sweet potato purée, choclo corn, red onion, coriander & plantain (gf)
              </p>
              <button class="btn btn-pink-border">£8.95</button>
            </div>

            <div class="menu-option">
              <h4 class="menu-option-title">TIRADITO CALLAO</h4>
              <p class="menu-option-description">
                Cobia tiradito with coriander tiger’s milk, black tobika, crème fraiche & sweet potato crunchies
              </p>
              <button class="btn btn-pink-border">£8.95</button>
            </div>

          </div>
        </section>

        <section class="menu-section menu-odd" id="menu-section-3">
          <div class="wrapper animate-out">
            <h3 class="title">Sides</h3>

            <div class="menu-option">
              <h4 class="menu-option-title">Super Pollo</h4>
              <p class="menu-option-description">
                Marinated corn fed chicken pieces with rocotto salsa
              </p>
              <button class="btn btn-pink-border">£4.95</button>
            </div>

            <div class="menu-option">
              <h4 class="menu-option-title">Patatas Fritas</h4>
              <p class="menu-option-description">
                Sweet potato fries with aji rocotto mayonnaise (v)
              </p>
              <button class="btn btn-pink-border">£3.95</button>
            </div>
          </div>
        </section>

        <section class="menu-section menu-even" id="menu-section-4">
          <div class="wrapper animate-out">

            <h3 class="title">Desserts</h3>

            <div class="menu-option">
              <h4 class="menu-option-title">Icecream</h4>
              <p class="menu-option-description">
                Lorem ipsum dolor sit amet salerma petrum sea
              </p>
              <button class="btn btn-pink-border">£3.95</button>
            </div>

            <div class="menu-option">
              <h4 class="menu-option-title">Tiramisu</h4>
              <p class="menu-option-description">
                Lorem ipsum dolor sit amet salerma petrum sea
              </p>
              <button class="btn btn-pink-border">£3.95</button>
            </div>

            <div class="menu-option">
              <h4 class="menu-option-title">Chocolate brownie</h4>
              <p class="menu-option-description">
                Lorem ipsum dolor sit amet salerma petrum sea
              </p>
              <button class="btn btn-pink-border">£3.95</button>
            </div>

          </div>
        </section>

      </div>

    </div>
  </section>
</template>

<script>
import $ from 'jquery'

export default {
  name: 'MenuSection',
  props: { },
  mounted: function () {
  }
}
</script>
