<template>
  <div class="row welcome-background">
    <div class="q-mt-sm col-2 offset-1" align="left">
      <img
        src="~assets/logo-white.svg"
        alt="Rooster Grin White"
      >
    </div>

    <div class="full-width fade-in">
      <b class="text-h3 text-bold clear-outline">
        {{ 'Welcome To'.toUpperCase() }}
      </b><br>
      <b class="text-h4 text-white">Rooster Grin</b><br><br>
      <q-btn dense class="sharp" color="accent">
        <span class="text-small">
          button button
        </span>
      </q-btn>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ComponentWelcome',

  data () {
    return {
    }
  }
}
</script>
