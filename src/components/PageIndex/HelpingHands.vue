<template>
  <div class="row">
    <div class="col-12 col-sm-5 offset-sm-1 flex flex-center">
      <div class="q-px-xl q-my-xl" align="left">
        <div class="text-h5 text-accent text-bold">
          {{ 'Lorem Ipsum'.toUpperCase() }}
        </div>
        <div class="q-mt-sm" style="font-size: 10px;">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </div>
        <div>
          <q-btn rounded no-caps flat dense size=".5em" color="accent">
            > Lorem Ipsum
          </q-btn>
        </div>
      </div>
    </div>
    <div class="col-none col-sm helping-hands-background">
    </div>
  </div>
</template>

<script>
export default {
  name: 'ComponentHelpingHands',

  data () {
    return {
    }
  }
}
</script>
