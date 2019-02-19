<template>
  <div>
    <section class="hero">
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
                <p>Get started today!</p>

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
      <div class="columns">
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
        <div class="columns">
          <div class="column">
            <h1 class="title">Section 1</h1>
            <h2 class="subtitle">
              A simple container to divide your page into <strong>sections</strong>, like the one you're currently reading
            </h2>            
          </div>
          <div class="column">
            <img src="https://osmaviation.com/app/uploads/2018/06/24131305_10155971074998967_883996193735898811_n_c4yogu-850x494.jpg">
          </div>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container">
        <div class="columns">
          <div class="column">
            <img src="https://epicflightacademy.com/wp-content/uploads/2018/03/commercial-pilot-e1520909294533.jpg">
          </div>
          <div class="column">
            <h1 class="title">Section 2</h1>
            <h2 class="subtitle">
              A simple container to divide your page into <strong>sections</strong>, like the one you're currently reading
            </h2>            
          </div>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container">
        <div class="columns">
          <div class="column">
            <h1 class="title">Section 3</h1>
            <h2 class="subtitle">
              A simple container to divide your page into <strong>sections</strong>, like the one you're currently reading
            </h2>            
          </div>
          <div class="column">
            <img src="https://images.wsj.net/im-2890?width=620&aspect_ratio=1.5">
          </div>
        </div>
      </div>
    </section>
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

<style>
.hero {
  background: url('~assets/jet.jpg') left no-repeat;
  background-size: cover;
}
.hero .title {
  font-size: 4em;
  color: white;
}
.hero .subtitle {
  font-size: 2em;
  color: black;
}
form {
  border-radius: 10px;
  padding: 1em;
  background-color: rgba(0, 0, 0, 0.7);
}

form p {
  color: white;
  font-size: 1.2em;
  margin-bottom: 1em;
}

b-field {
  color: white;
}
form .label {
  color: white !important;
}
</style>
