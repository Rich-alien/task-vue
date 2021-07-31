<template>
  <button class="button">
    {{text}}
  </button>
</template>

<script>
export default {
  name: 'button',
  props: {
    text: String
  },

}
</script>

<style scoped lang="sass">
  .button
    padding: 13px 64px
    color: #FFFFFF
    border: none
    background: linear-gradient(91.6deg, #8F00FF 0%, #1638FF 93.79%, #093FFF 104.14%)
    opacity: 0.29
    box-shadow: 0 0 30px rgba(97, 0, 255, 0.8), inset 0 10px 10px rgba(255, 255, 255, 0.25)
</style>
