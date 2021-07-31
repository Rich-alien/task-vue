<template>
  <div class="header">
    <h2 class="header__logo">logo</h2>
    <div class="header__nav">
      <span class="header__nav-link">Портфолио</span>
      <span class="header__nav-link">Услуги</span>
      <span class="header__nav-link">Стоимость</span>
      <span class="header__nav-link">Контакты</span>
    </div>
    <div class="header__icons">
      <TelegramIcon/>
      <BeIcon/>
      <InstagramIcon/>
      <div class="header__icons-line"></div>
    </div>
  </div>
</template>

<script>
import TelegramIcon from "../Logo/logo.telegram.component"
import BeIcon from "../Logo/logo.be.component"
import InstagramIcon from "../Logo/logo.instagram.component"
export default {
  name: 'header',
  props: {
    msg: String
  },
  components: {
    TelegramIcon,
    BeIcon,
    InstagramIcon
  }
}
</script>

<style scoped lang="sass">
  .header
    padding:  49px 0 0 134px
    display: flex
    align-items: center
    justify-content: space-between
    &__logo
      cursor: pointer
      text-transform: uppercase
      font-size: 36px
      line-height: 43px
    &__nav
      display: flex
      justify-content: space-between
      width: 501px
      &-link
        cursor: pointer
    &__icons
      display: flex
      width: 315px
      justify-content: space-between
      align-items: center
      &-line
        width: 138px
        height: 2px
        box-shadow: 0 0 20px rgba(66, 0, 255, 0.5), inset 0 10px 10px rgba(255, 255, 255, 0.25)
</style>
