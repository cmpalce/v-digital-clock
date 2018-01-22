<template>
  <span>
    {{ time }} {{ city }}
  </span>
</template>

<script>

import moment from 'moment-timezone'

export default {
  name: 'VDigitalClock',
  props: {
    city: {
      type: String,
      default: 'UTC'
    },
    timezone: {
      type: String,
      default: 'Etc/Utc'
    }
  },
  data () {
    return {
      time: ''
    }
  },
  created () {
    setInterval(() => {
      this.time = moment().tz(this.timezone).format('MMM DD, YYYY HH:mm:ss')
    }, 1000)
  }
}
</script>

<style>

</style>
