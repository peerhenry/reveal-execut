<template lang="pug">
section
  img.wyte(src="../assets/devs/a.png")
  img.wyte(src="../assets/devs/p.png")
  img.wyte(src="../assets/devs/n.jpg")
  img.wyte(src="../assets/devs/l.png")
  p
    span 4 devs
  p
    div
      span + {{monthCount}} months
  p
    span = Cool project!
</template>

<script>
export default {
  props: ['monthCount'],
}
</script>

<style lang="scss" scoped>
.wyte {
  background-color: white;
}
</style>