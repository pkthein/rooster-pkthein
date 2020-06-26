<template>
  <div class="row happy-child-background" align="center">
    <div class="col-5 offset-6 flex flex-center">
      <div class="q-mx-lg q-px-lg" align="left">
        <div class="head-md text-accent text-bold">
          Lorem Ipsum
        </div>
        <p class="q-mt-sm md">
          Lorem ipsum dolor sit amet, et felis integer. Cras ac, duis nisl magna est sociis, neque in odio vel, sit lobortis erat. Fugit quam, ut pede ut ante, in viverra eros dictum nisl ligula.
        </p>
        <div>
          <q-btn
            dense class="sharp" color="secondary"
            @click="salute"
          >
            <span class="text-sm">
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
  },

  methods: {
    salute: function () {
      this.$q.notify({
        type: 'positive',
        message: 'Good click!',
        timeout: 2000
      })
    }
  }
}
</script>
