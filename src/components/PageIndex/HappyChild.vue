<template>
  <div class="row happy-child-background" align="center">
    <div class="col-5 offset-6 flex flex-center">
      <div class="q-mx-lg q-px-lg" align="left">
        <div class="text-h5 text-accent text-bold">
          {{ 'Lorem Ipsum'.toUpperCase() }}
        </div>
        <p class="q-mt-sm sm" style="font-size: 10px;">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        </p>
        <div>
          <q-btn dense class="sharp" color="secondary">
            <span class="text-small">
              button button
            </span>
          </q-btn>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ComponentHappyChild',

  data () {
    return {
    }
  }
}
</script>
