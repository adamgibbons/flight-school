<template>
  <div>
    <nav
      class="navbar header has-shadow is-transparent"
      role="navigation"
      aria-label="main navigation"
    >
      <div class="navbar-brand">
        <a
          class="navbar-item"
          href="/"
        >
          <img
            src="~assets/logo.png"
            alt="Buefy"
            height="28"
          >
          <span class="navbar-text">American Flight School Advisors</span>
        </a>

        <div class="navbar-burger">
          <span />
          <span />
          <span />
        </div>
      </div>
    </nav>

    <nuxt />

    <Footer />
  </div>
</template>

<script>
import Footer from '~/components/Footer'

export default {
  components: { Footer },
  data() {
    return {
      items: [
        {
          title: 'Home baz',
          icon: 'home',
          to: { name: 'index' }
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' }
        }
      ]
    }
  }
}
</script>

<style scoped>
.navbar-text {
  margin-left: 0.5em;
  font-size: 1.5em;
}
</style>
