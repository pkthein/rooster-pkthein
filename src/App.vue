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
.welcome-background {
  background-image: url('~assets/hero.jpg');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  width: 100%;
  // height: 52vw;
  height: 100vh;
}

.mother-child-background {
  @extend .welcome-background;
  background-image: url('~assets/banner-1.jpg');
  height: 42vw;
}

.happy-child-background {
  @extend .mother-child-background;
  background-image: url('~assets/banner-2.jpg');
}

.helping-hands-background {
  @extend .welcome-background;
  background-image: url('~assets/img-1.jpg');
  height: 37vw;
}

button.sharp {
  border-radius: 0px;
  min-width: 100px;
}

span.text-small {
  font-size: 8px;
  padding: 0px 5px;
}

b.clear-outline {
  color: #000;
  color: rgba(0, 0, 0, 0.0);
  -webkit-text-stroke: 1px white;
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
