<template>
  <div>
    <section class="hero is-info">
      <div class="hero-body">
        <div class="container">
          <div class="columns">
            <div class="column is-two-thirds">
              <h1 class="title">
                Become a Commercial Airline Pilot
              </h1>
              <h2 class="subtitle">
                Find the American flight school that’s right for you
              </h2>
            </div>
            <div class="column">
              <form>
                <p>Start your application now</p>

                <section>
                  <!-- <b-checkbox v-model="hasError">Show errors</b-checkbox> -->

                  <b-field
                    label="Full name"
                    :type="{ 'is-danger': hasError }"
                    :message="{ 'Username is not available': hasError }">
                    <b-input
                      type="text"
                      placeholder="Peter Young"
                      size="is-medium"
                      required>
                    </b-input>
                  </b-field>

                  <b-field
                    label="Email address"
                    :type="{ 'is-danger': hasError }"
                    :message="{ 'Username is not available': hasError }">
                    <b-input
                      placeholder="peter@example.com"
                      size="is-medium"
                      type="email"
                      required>
                    </b-input>
                  </b-field>

                  <b-field
                    label="Phone number"
                    :type="{ 'is-danger': hasError }"
                    :message="{ 'Username is not available': hasError }">
                    <b-input
                      placeholder="Foo"
                      size="is-medium">
                    </b-input>
                  </b-field>

                  <b-field
                    label="Expanded">
                    <b-select
                      placeholder="Select a country"
                      size="is-medium"
                      expanded>
                      <option value="flint">Flint</option>
                      <option value="silver">Silver</option>
                    </b-select>
                  </b-field>
                </section>
              </form>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- value props -->
    <section class="section">
      <div class="columns is-mobile">
        <card
          title="Free"
          icon="github-circle"
        >
          Open source on <a href="https://github.com/buefy/buefy"> GitHub</a>
        </card>

        <card
          title="Responsive"
          icon="cellphone-link"
        >
          <b class="has-text-grey">Every</b> component is responsive
        </card>

        <card
          title="Modern"
          icon="alert-decagram"
        >
          Built with <a href="https://vuejs.org/">Vue.js</a> and <a href="http://bulma.io/">Bulma</a>
        </card>

        <card
          title="Lightweight"
          icon="arrange-bring-to-front"
        >
          No other internal dependency
        </card>
      </div>
    </section>

    <section class="section">
      <div class="container">
        <h1 class="title">Section</h1>
        <h2 class="subtitle">
          A simple container to divide your page into <strong>sections</strong>, like the one you're currently reading
        </h2>
      </div>
    </section>

    <footer class="footer">
      <div class="content has-text-centered">
        <p>
          <strong>Bulma</strong> by <a href="https://jgthms.com">Jeremy Thomas</a>. The source code is licensed
          <a href="http://opensource.org/licenses/mit-license.php">MIT</a>. The website content
          is licensed <a href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY NC SA 4.0</a>.
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
import Card from '~/components/Card'

export default {
  layout: 'home',
  name: 'HomePage',
  components: {
    Card
  },
  data() {
    return {
      hasError: false
    }
  }
}
</script>

<style lang="scss">
.hero {
  background: url('~assets/jet.jpg') left no-repeat;
  background-size: cover;
}
.title {
  font-size: 3em;
}
.subtitle {
  font-size: 1.5em;
}
form {
  padding: 1em;
  background-color: rgba(0, 0, 0, 0.7);
}

b-field {
  color: white;
}
</style>
