<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
          <md-list-item
                href="https://www.facebook.com/i8studio"
                target="_blank"
              >
                <i class="fab fa-instagram"></i>
                <p>Instagram</p>
                <md-tooltip md-direction="bottom"
                  >Follow Us on Instagram</md-tooltip
                >
            </md-list-item>
          </li>
          <li>
            <md-list-item
              href="https://www.facebook.com/i8studio"
              target="_blank"
            >
              <i class="fab fa-facebook-square"></i>
              <p>Facebook</p>
              <md-tooltip md-direction="bottom"
                >Like us on Facebook</md-tooltip
              >
            </md-list-item>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}
        <a href="https://www.i8studios.com/" target="_blank">i8 Studios</a>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String,
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style>
</style>
