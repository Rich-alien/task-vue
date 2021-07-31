<template>
  <div class="main">
    <HeaderComponent/>
    <div class="main__border">
      <div class="main__text">
        <h1 class="main__text-title">Создание современных сайтов</h1>
        <h4 class="main__text-description">Разработка сайта с продающим дизайном, продуманной структурой и удобным для
          вашей целевой аудитории интерфейсом </h4>
        <div class="main__text-button">
          <div class="main__line"></div>
          <ButtonComponent text="Обсудить проект"/>
        </div>
      </div>
      <PlanetIcon class="main__icon"/>
    </div>
    <button class="main__button">
      Портфолио
      <div >
        <ArrowBlock class="main__button-arrow"/>
      </div>
    </button>
  </div>
</template>
<script>
import HeaderComponent from "../../components/header/header.component"
import ButtonComponent from "../../components/button/button.component"
import PlanetIcon from "../../components/Logo/logo.planet.component"
import ArrowBlock from "../../components/Logo/logo.arrow-block.component"

export default {
  name: 'main',
  props: {
    msg: String
  },
  components: {
    HeaderComponent,
    ButtonComponent,
    PlanetIcon,
    ArrowBlock
  }
}
</script>

<style scoped lang="sass">
.main
  position: relative
  width: 100%
  height: 100vh
  background-image: url("../../assets/bg.png")
  background-size: 100%
  background-repeat: no-repeat

  &__border
    display: flex
    width: 100%
    justify-content: space-between

  &__text
    &-button
      display: flex
      align-items: center

    &-title
      margin-left: 142px
      margin-top: 162px
      font-weight: 600
      font-size: 42px
      line-height: 51px

    &-description
      margin-left: 142px
      margin-top: 40px
      margin-bottom: 60px
      width: 513px
      font-size: 20px
      line-height: 150%
  &__button
    display: flex
    border: none
    color: white
    background: none
    position: absolute
    top: 592px
    right: 479px
    &-arrow
      margin-left: -8px
      width: 37px
      height: 20px
      background: linear-gradient(91.72deg, #8F00FF 0%, #093FFF 103.3%)
      filter: blur(4px)
  &__line
    width: 138px
    height: 2px
    box-shadow: 0 0 20px rgba(66, 0, 255, 0.5), inset 0 10px 10px rgba(255, 255, 255, 0.25)
</style>
