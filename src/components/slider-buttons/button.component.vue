<template>
  <div class="button">
    <div class="button__dot-active">
      <div class="button__dot-active__white">
        <button class="button__dot-purple"></button>
      </div>
    </div>
    <button class="button__dot"></button>
    <button class="button__dot"></button>
    <button class="button__dot"></button>
    <button class="button__dot"></button>
  </div>
</template>

<script>
export default {
  name: 'button',
}
</script>

<style scoped lang="sass">
.button
  display: flex
  align-items: center
  height: 22px
  justify-content: space-between
  width: 122px
  &__dot
    border: none
    width: 10px
    height: 10px
    border-radius: 90%
    background-color: #D9D9D9
    &-purple
      border: none
      width: 10px
      height: 10px
      border-radius: 90%
      background: linear-gradient(91.72deg, #8F00FF 0%, #093FFF 103.3%)
    &-active
      display: flex
      align-items: center
      justify-content: center
      border-radius: 90%
      width: 22px
      height: 22px
      background: linear-gradient(91.72deg, #8F00FF 0%, #093FFF 103.3%)
      &__white
        display: flex
        align-items: center
        justify-content: center
        border-radius: 90%
        background: white
        width: 18px
        height: 18px
</style>
