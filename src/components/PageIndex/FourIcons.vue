<template>
  <div class="row">
    <div
      class="col-12 col-sm-5 offset-sm-1 flex flex-center q-py-lg"
    >
      <div class="q-px-xl q-my-xl" align="left">
        <div class="text-h5 text-bold">
          {{ 'Lorem Ipsum Dolor Sit Amet'.toUpperCase() }}
        </div>
        <div class="q-mt-sm" style="font-size: 10px;">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        </div>
        <div>
          <q-btn
            no-caps flat dense rounded
            size=".5em" color="accent"
          >
            > Lorem Ipsum
          </q-btn>
        </div>
      </div>
    </div>

    <div class="col-12 col-sm-5 bg-grey-1 q-py-lg" align="center">
      <div
        v-for="val in icons" :key="val.id"
        class="row q-mt-xl q-mb-xl"
      >
        <div v-for="col in val" :key="col.id" class="col">
          <div
            class="q-mb-sm flex flex-center icon-border"
          >
            <q-icon
              :class="col.class"
              size="50px" :name="col.name"
            />
          </div>
          <b>{{ col.label }}</b>
        </div>
      </div>
    </div>

    <div class="col-sm-1 bg-grey-1"></div>
  </div>
</template>

<script>
export default {
  name: 'ComponentFourIcons',
  data () {
    return {
      icons: [
        [
          {
            name: 'img:icons/home-expertise.svg',
            label: 'LOREM',
            class: 'animate__animated animate__pulse animate__slow animate__infinite'
          },
          {
            name: 'img:icons/home-hygiene.svg',
            label: 'LOREM IPSUM',
            class: 'animate__animated animate__tada animate__infinite animate__slow'
          }
        ],
        [
          {
            name: 'img:icons/home-lab.svg',
            label: 'LOREM IPSUM',
            class: 'animate__animated animate__jello animate__infinite animate__slow'
          },
          {
            name: 'img:icons/home-retention.svg',
            label: 'LOREM',
            class: 'animate__animated animate__pulse animate__infinite'
          }
        ]
      ]
    }
  }
}
</script>
