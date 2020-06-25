<template>
  <q-page align="center">
    <Welcome />

    <HelpingHands />

    <MotherAndChild />

    <FourIcons />

    <HappyChild />

    <Feedback />
  </q-page>
</template>

<script>
import Welcome from '../components/PageIndex/Welcome'
import HelpingHands from '../components/PageIndex/HelpingHands'
import MotherAndChild from '../components/PageIndex/MotherAndChild'
import FourIcons from '../components/PageIndex/FourIcons'
import HappyChild from '../components/PageIndex/HappyChild'
import Feedback from '../components/PageIndex/Feedback'

export default {
  name: 'PageIndex',
  components: {
    Welcome,
    HelpingHands,
    MotherAndChild,
    FourIcons,
    HappyChild,
    Feedback
  },
  data () {
    return {
    }
  }
}
</script>
