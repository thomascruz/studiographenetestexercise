<template>
  <header>
    <div class="wrapper">

      <div class="header-element logo">
        <h2>LOGO</h2>
      </div>

      <div class="header-element nav">
        <router-link class="link" to="/">About</router-link>
        <router-link class="link" to="/">Community</router-link>
        <router-link class="link" to="/">Location</router-link>
        <router-link class="link" to="/">Our Menu</router-link>
        <router-link class="link" to="/">Recipies</router-link>
      </div>

      <div class="header-element nav nav-right">
        <router-link class="link" to="/">Contact</router-link>
        <router-link class="link" to="/">Login</router-link>
      </div>

    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: { }
}
</script>
