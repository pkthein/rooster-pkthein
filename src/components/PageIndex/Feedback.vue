<template>
  <div class="row q-mb-xl">
    <div class="col-12 col-md-5 offset-md-1 flex flex-center">
      <div class="q-px-xl q-py-xl q-my-xl" align="left">
        <div class="head-md text-bold">
          {{ 'Lorem Ipsum Dolor Sit Amet'.toUpperCase() }}
        </div>
        <div>
          <q-icon
            v-for="i in 5" :key="i"
            color="secondary" name="grade"
            size="1.5em"
          />
        </div>
      </div>
    </div>

    <div class="col-12 col-md-6">
      <q-carousel
        animated infinite autoplay arrows
        transition-prev="slide-right"
        transition-next="slide-left"
        control-color="accent"
        v-model="slide"
        height="300px"
      >
        <q-carousel-slide
          v-for="val in slides" :key="val.id"
          class="flex flex-center q-px-xl" :name="val.slide"
        >
          <b class="text-bold text-accent">
            {{ val.header }}
          </b><br><br>

          <p class="q-px-md" align="left">
            {{ val.body }}
          </p>
        </q-carousel-slide>
      </q-carousel>

      <div style="text-align:center;">
        <span
          v-for="dot in slides" :key="dot.id"
          class="dot"
          :class="{ active: slide === dot.slide }"
          @click="slide = dot.slide"
        />
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'ComponentFeedback',

  data () {
    return {
      slide: 1,
      slides: [
        {
          header: 'John Doe 08/08/2019',
          body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          slide: 1
        },
        {
          header: 'Jane Doe 01/08/2019',
          body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.',
          slide: 2
        },
        {
          header: 'John Daly 07/08/2019',
          body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          slide: 3
        }
      ]
    }
  }
}
</script>
