<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">
        julians-dope-website
      </h1>
      <h2 class="subtitle">
        My sweet website
      </h2>
      <div class="row">
        <div class="col-md-8">
          Hallo ich bin Julian, ich lerne gerade wie man Websiten macht!
        </div>
        <div class="col-md-4">
          <img id="flower" src="~/assets/folower.jpg" alt="flower">
        </div>
      </div>
      <div class="row">
        <div class="col-md">
          <button v-on:click="clickme">click mich zwei mal</button>
        </div>
      </div>
    </div>
  </div> 
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  methods: {
    clickme: function(event) {
      alert("hallo welt")
    }
  }
}
</script>

<style>

#flower {
  max-width: 100%;
  object-fit: contain;
}

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
