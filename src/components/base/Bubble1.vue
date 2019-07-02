<template>
  <v-img
    class="grow hidden-sm-and-down"
    contain
    :max-height="maxHeight"
    width="100%"
    position="top right"
    :src="require('@/assets/bubbles1.png')"
  />
</template>
<script>
export default {
  props:{
    maxHeight:{
      default:200
    }
  }
}
</script>
