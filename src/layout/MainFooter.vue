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
            <a href="https://www.i8studios.com">
              Creative Tim
            </a>
          </li>
          <li>
            <a href="https:///presentation.i8studios.com">
              About Us
            </a>
          </li>
          <li>
            <a href="https:///blog.i8studios.com">
              Blog
            </a>
          </li>
          <li>
            <a href="https://www.i8studios.com/license">
              Licenses
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, made with <md-icon>favorite</md-icon> by
        <a href="https://www.i8studios.com/" target="_blank">i8 Studios</a>
        for a better web.
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
