<template>
  <div class="app-container">

    <img src="https://img0.baidu.com/it/u=4162443464,2854908495&fm=253&app=138&size=w931&n=0&f=JPEG&fmt=auto?sec=1684342800&t=84d3a38704082e76c2b0485b7037b03a" alt="">
  </div>
</template>

<script>
import Driver from 'driver.js' // import driver.js
import 'driver.js/dist/driver.min.css' // import driver.js css
import steps from './steps'

export default {
  name: 'Guide',
  data() {
    return {
      driver: null
    }
  },
  mounted() {
    // this.driver = new Driver()
  },
  methods: {
    guide() {
      this.driver.defineSteps(steps)
      this.driver.start()
    }
  }
}
</script>
