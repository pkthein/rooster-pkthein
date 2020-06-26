<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container>
      <router-view />
    </q-page-container>

    <div class="q-pb-md q-pt-lg bg-grey-1" align="center">
      <b>Follow Us:</b>
      <div class="q-pa-sm q-gutter-sm">
        <q-icon
          class="cursor-pointer" :size="iconSize"
          name="img:icons/instagram.svg"
          @click="goTo('https://www.instagram.com/')"
        />
        <q-icon
          class="cursor-pointer" :size="iconSize"
          name="img:icons/facebook.svg"
          @click="goTo('https://www.facebook.com/RoosterGrin/')"
        />
      </div>
    </div>
  </q-layout>
</template>

<script>
export default {
  name: 'MainLayout',

  components: {
  },

  data () {
    return {
      iconSize: '35px'
    }
  },

  methods: {
    goTo: function (path) {
      window.open(path, '_self', 'noopener')
    }
  }
}
</script>
