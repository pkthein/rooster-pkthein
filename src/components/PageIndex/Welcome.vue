<template>
  <div class="row welcome-background">
    <div class="q-mt-sm col-2 offset-1" align="left">
      <img
        class="cursor-pointer logo"
        src="~assets/logo-white.svg"
        alt="Rooster Grin White"
        @click="roosterGrin"
      >
    </div>

    <div class="full-width fade-in">
      <b class="head-xl clear-outline">
        Welcome To
      </b><br>
      <b class="head-lg text-white">Rooster Grin</b><br><br>
      <q-btn
        dense class="sharp" color="accent"
        @click="roosterGrin"
      >
        <span class="text-sm">
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
  },

  methods: {
    roosterGrin: function () {
      const path = 'https://www.roostergrin.com/'
      window.open(path, '_blank', 'noopener')
    }
  }
}
</script>
