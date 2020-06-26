<template>
  <div class="row mother-child-background" align="center">
    <div class="col-5 offset-1 flex flex-center">
      <div class="q-px-xl full-width" align="left">
        <div class="head-md text-accent text-bold">
          Lorem Ipsum
        </div>
        <div class="q-mt-sm">
          <q-btn
            dense class="sharp" color="secondary"
            @click="linkedIn"
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
  name: 'ComponentMotherAndChild',

  data () {
    return {
    }
  },

  methods: {
    linkedIn: function () {
      const path = 'https://www.linkedin.com/in/pkthein'
      window.open(path, '_blank', 'noopener')
    }
  }
}
</script>
