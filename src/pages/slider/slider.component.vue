<template>
  <div class="slider">
    <div class="slider__text">
      <div>
        <div class="slider__upper-text">
          <div class="slider__text-line"></div>
          <h1 class="slider__text-title">Услуги</h1>
        </div>
        <div class="slider__description">
          <div class="slider__number-chapter">
            <img src="../../assets/01.png" alt="01">
            <h3>Редизайн сайта</h3>
          </div>
          <h4 class="slider__text__chapter-description">Редизайн – это разработка нового дизайна, включая в него
            определенные данные с уже существующего сайта.</h4>
          <h4 class="slider__text__question">
            В каком случае стоит задуматься о редизайне сайта:
          </h4>
          <ul class="slider__text__answer">
            <li>существующая версия сайта создавалась достаточно давно</li>
            <li>сайты конкурентов стали современнее и привлекают больше внимания</li>
            <li>появилась необходимость в доработке или добавлении функционала</li>
            <li>упала конверсия и пропали продажи</li>
            <li>нет адаптивной версии сайта</li>
          </ul>
          <h4 class="slider__text-pre-footer">
            Участие в редизайне принимает как дизайнер, так и верстальщик. Происходит адаптация сайта под современные
            реалии, ускоряется его скорость и качество.
          </h4>
          <h4 class="slider__text-footer">Обновление сайта рекомендуется проводить один раз в 3-4 года.</h4>
        </div>
      </div>
      <SliderButton class="slider__dots"/>
    </div>
    <div  class="slider__button">
      <ArrowIcon class="slider__button-arrow-left"/>
      <ArrowIcon class="slider__button-arrow-right"/>
    </div>
    <img src="../../assets/bibord.png"/>
  </div>
</template>
<script>
import SliderButton from "../../components/slider-buttons/button.component"
import ArrowIcon from "../../components/Logo/logo.arrow.component"

export default {
  name: 'slider',
  components: {
    SliderButton,
    ArrowIcon
  }

}
</script>

<style scoped lang="sass">
.slider
  position: relative
  height: 100vh
  color: black
  background: white
  display: flex
  justify-content: space-between

  &__description
    margin-left: 143px

  &__upper-text
    display: flex
    align-items: center
    margin-top: 87px

  &__number-chapter
    width: 306px
    display: flex
    justify-content: space-between
    align-items: center
    margin-top: 20px

  &__text
    display: flex
    flex-direction: column
    justify-content: space-between
    color: black
    height: 100%

    &__chapter-description
      margin-top: 10px
      width: 566px

    &__question
      margin-top: 20px
      width: 464px

    &__answer
      line-height: 27px
      margin-left: 20px
      list-style-type: circle
      padding-top: 20px

    &-line
      width: 108px
      height: 6px
      background: linear-gradient(91.72deg, #8F00FF 0%, #093FFF 103.3%)
      filter: blur(4px)

    &-pre-footer
      margin-top: 20px
      width: 582px

    &-footer
      margin-top: 20px
      width: 582px

    &-title
      margin-left: 30px

  &__dots
    margin-left: 360px
    margin-bottom: 20px

  &__button
    display: flex
    align-items: center
    position: absolute
    cursor: pointer
    bottom: 0
    right: 570px
    width: 237px
    height: 80px
    background-image: url("../../assets/rec.png")
    background-size: 100%
    background-repeat: no-repeat
    &-arrow
      &-left
        transform: rotate(-180deg)
        margin-left: 51px
      &-right
        margin-left: 107px
</style>
