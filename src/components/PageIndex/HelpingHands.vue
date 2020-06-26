<template>
  <div class="row">
    <div class="col-12 col-md-5 offset-md-1 flex flex-center">
      <div class="q-px-xl q-my-xl" align="left">
        <div class="head-md text-accent text-bold">
          Lorem Ipsum
        </div>
        <div class="q-mt-sm">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </div>
        <div>
          <q-btn
            rounded no-caps flat dense color="accent"
            @click="personalWebsite"
          >
            > Lorem Ipsum
          </q-btn>
        </div>
      </div>
    </div>
    <div class="col-md-6 helping-hands-background">
    </div>
  </div>
</template>

<script>
export default {
  name: 'ComponentHelpingHands',

  data () {
    return {
    }
  },

  methods: {
    personalWebsite: function () {
      const path = 'https://pkthein.github.io/'
      window.open(path, '_self', 'noopener')
    }
  }
}
</script>
