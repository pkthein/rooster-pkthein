<template>
  <div id="q-app">
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="stylus">
* {
  font-size: 16px;
}

.welcome-background {
  background-image: url('~assets/hero.jpg');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  width: 100%;
  height: 100vh;
  min-height: 250px;
}

.mother-child-background {
  @extend .welcome-background;
  background-image: url('~assets/banner-1.jpg');
  height: 42vw;
  min-height: 100px;
}

.happy-child-background {
  @extend .mother-child-background;
  background-image: url('~assets/banner-2.jpg');
  vertical-align: middle;
}

.helping-hands-background {
  @extend .welcome-background;
  background-image: url('~assets/img-1.jpg');
  height: 37vw;
}

button.sharp {
  border-radius: 0px;
  min-width: 150px;
  height: 55px;
}

button.sharp-resize {
  @extend button.sharp;
  min-width: clamp(100px, 20vw, 150px);
  height: clamp(35px, 7vw, 55px);
}

.head-md {
  font-size: clamp(26px, 7vw, 40px);
  text-transform: uppercase;
}

.head-lg {
  font-size: clamp(32px, 7vw, 64px);
}

.head-xl {
  @extend .head-md;
  font-weight: 800;
  font-size: clamp(36px, 7vw, 72px);
}

span.text-sm {
  font-size: clamp(10px, 1.5vw, 15px);
  padding: 0px 5px;
}

b.clear-outline {
  color: #000;
  color: rgba(0, 0, 0, 0.0);
  -webkit-text-stroke: 2px white;
}

img.logo {
  height: clamp(15px, 3vw, 30px);
}

.icon-border {
  border: solid purple 1px;
  border-radius: 50%;
  width: 75px;
  height: 75px;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 10px;
  width: 10px;
  margin: 0 2px;
  background-color: $yellow-4;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .dot:hover {
  background-color: $yellow-8;
}

.fade-in {
  animation: fadeIn ease 10s;
  -webkit-animation: fadeIn ease 10s;
  -moz-animation: fadeIn ease 10s;
  -o-animation: fadeIn ease 10s;
  -ms-animation: fadeIn ease 10s;
}

@keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
  }
}

@-moz-keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
  }
}

@-webkit-keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
  }
}

@-o-keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
  }
}

@-ms-keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
  }
}
</style>
