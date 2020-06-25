<template>
  <div class="row mother-child-background" align="center">
    <div class="col-5 offset-1 flex flex-center">
      <div class="q-px-xl full-width" align="left">
        <div class="text-h5 text-accent text-bold">
          {{ 'Lorem Ipsum'.toUpperCase() }}
        </div>
        <div class="q-mt-sm">
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
  name: 'ComponentMotherAndChild',

  data () {
    return {
    }
  }
}
</script>
