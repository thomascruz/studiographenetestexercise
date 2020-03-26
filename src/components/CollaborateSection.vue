<template>
  <section class="landing-section" id="collaborate-section">
    <div class="decoration decor-plus"></div>

    <div class="wrapper">

      <div class="left-wrapper">

        <h2 class="crossed-title">Collaborate<br><span class="crossed">With Us</span></h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br><br>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore</p>

      </div>

      <div class="right-wrapper">
        <form class="collaborate-form">

          <div class="form-row">

            <div class="form-input">
              <label for="name">Name</label>
              <input type="text" name="name" placeholder="Name">
            </div>

            <div class="form-input">
              <label for="surname">Surname</label>
              <input type="text" name="surname" placeholder="Surname">
            </div>

          </div>

          <div class="form-row">

            <div class="form-input">
              <label for="phone">Phone</label>
              <input type="tel" name="phone" placeholder="Phone">
            </div>

            <div class="form-input">
              <label for="email">Email Address</label>
              <input type="email" name="email" placeholder="Email">
            </div>

          </div>

          <div class="form-row">

            <div class="form-input">
              <label for="experience">Experience</label>

              <div class="select-wrapper">
                <select name="experience">
                  <option value="" disabled selected>Select</option>
                  <option value="">Option</option>
                  <option value="">Option</option>
                </select>
              </div>

            </div>

            <div class="form-input">
              <label for="where">Where did you hear about us?</label>

              <div class="select-wrapper">
                <select name="where">
                  <option value="" disabled selected>Select</option>
                  <option value="">Option</option>
                  <option value="">Option</option>
                </select>
              </div>

            </div>

          </div>

          <div class="form-row right">

            <button class="btn btn-submit" type="submit" name="send">Send</button>

          </div>

        </form>
      </div>

    </div>
  </section>
</template>

<script>
export default {
  name: 'CollaborateSection',
  props: { },
  mounted: function () {
  }
}
</script>
