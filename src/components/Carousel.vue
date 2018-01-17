<template>
  <section class="flex column">
    <div class="carousel flex row">
      <div class="arrow arrow-left" @click="handleSlide(-1)">
        <img class="hoverable" src="../assets/my_icon_left.svg" alt="">
      </div>
      <img class="carousel-img" :src="data[current].url" alt="">
      <article class="flex column carousel-info">
        <div class="carousel-caption">{{data[current].caption}}</div>
        <div class="carousel-text">{{data[current].text}}</div>
        <button style="max-width: 15rem ">Shop now</button>
      </article>
      <div class="arrow arrow-right" @click="handleSlide(1)">
        <img class="hoverable" src="../assets/my_icon_right.svg" alt="">
      </div>
    </div>
    <div class="carousel-footer flex row">
      <div class="carousel-toggler"
           v-for="(_, index) in 3"
           @click="handleSwitch(index)"
           :class="{'carousel-toggler--active': index === current}"></div>
    </div>
  </section>
</template>

<script>
  //Pure implementation for this task.
  import s4 from '../assets/s4.jpg'
  import s5 from '../assets/s5.jpg'
  import iphone from '../assets/iphone.jpg'
  export default {
    name: 'Carousel',
    data () {
      return {
        current: 0,
        data: [
          {
            'url': s4,
            'caption': 'Perfect Match',
            'text': 'Get the Samsung GALAXY S4™ on Canada\'s most reliable 4G⁶ network and see why we\'re better together.'
          },
          {
            'url': s5,
            'caption': 'Best Choice',
            'text': 'Get the most popular phone in bla if you can paid for it, ofc.'
          },
          {
            'url': iphone,
            'caption': 'Iphoneeee X',
            'text': 'Modern, fast, furious, smart? Can unlock by your face, and costs like a used car.. Best choice, ever!'
          }
        ]
      }
    },
    methods: {
      handleSlide (dir) {
        if (dir === -1 && this.current === 0) {
          this.current = 2
        }
        else if (dir === 1 && this.current === 2) {
          this.current = 0
        }
        else {
          this.current += dir
        }
      },
      handleSwitch (num) {
        this.current = num
      }
    }
  }
</script>
<style scoped lang="stylus">
  $main-blue = #0365a1
  section
    max-width 100vw
    height 55vh
    img
      max-width 40vw
      transition all .3s linear
  .carousel
    justify-content space-between
    align-items center
    &-caption
      font-size 5rem
      color: $main-blue
    &-text
      text-align left
      font-size 3rem
      color: darkgrey
    &-img
      width 25vw
    &-info
      max-width 50vw
    &-footer
      height 2.5rem
      justify-content center
      align-items flex-start
    &-toggler
      cursor pointer
      width .8rem
      height .8rem
      border: .2rem solid $main-blue
      margin-left .5rem
      margin-right .5rem
      transition all .3s linear
      &--active
        background-color $main-blue
  .arrow
    width 3rem
    height 55vh
    display flex
    justify-content center
    align-items center
    img
      max-width 2rem
  img.hoverable
    &:hover
      filter: drop-shadow(0px 0px 2px #974a00);
  @media only screen and (max-width: 1400px)
    .carousel
      &-caption
        font-size 4rem
      &-text
        font-size 2rem
  @media only screen and (max-width: 1000px)
    .carousel
      &-caption
        font-size 3rem
      &-text
        font-size 1.5rem
</style>
