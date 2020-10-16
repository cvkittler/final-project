<template>
  <div class="snake">
    <h1>{{ msg }}</h1>
    <canvas id="canvas" width="800" height="800">
    </canvas>
  </div>
</template>

<script>
export default {
  name: 'Snake',
  data () {
    return {
      msg: 'Snake game'
    }
  },
  mounted () {
    const plugin = document.createElement('script')
    plugin.setAttribute(
      'src',
      '/project.js'
    )
    plugin.async = true
    document.head.appendChild(plugin)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
