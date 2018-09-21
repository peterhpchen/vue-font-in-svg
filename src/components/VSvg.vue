<template>
  <span
    @mouseover="isHover=true"
    @mouseout="isHover=false"
  >
    <span v-if="type==='Cancel'">
      <img v-if="isDisable" svg-inline src="../assets/img/disable.svg">
      <img v-else-if="isHover" svg-inline src="../assets/img/hover.svg">
      <img v-else svg-inline src="../assets/img/normal.svg">
    </span>
  </span>
</template>

<script>
export default {
  name: 'VSvg',
  props: {
    type: {
      type: String,
      required: true
    },
    isDisable: {
      type: Boolean,
      default: false
    }
  },
  data() {
    return {
      isHover: false
    }
  }
}
</script>
