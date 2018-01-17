<template>
  <section>
    <header class="flex row">
      <div class="logo"></div>
      <div class="link">Products & Plans</div>
      <div class="link">Get help</div>
      <div class="flex row link--icon">
        <img src="../assets/my_user_small.svg" alt="">
        <div class="link link--dotted">Log in</div>
      </div>
      <div class="spacer"></div>
      <img class="hoverable" src="../assets/my_zoom.svg" alt="">
      <div class="flex row link--icon">
        <div class="link link--no-border">EN</div>
        <img style="margin-left: .5rem; margin-right: 2rem" src="../assets/my_icon_down.svg" alt="">
      </div>
    </header>
    <carousel></carousel>
    <article class="account flex column">
      <div class="account-caption flex row">
        <img src="../assets/my_user.svg" alt="">
        <div class="account-caption--text">My Account</div>
      </div>
      <div class="account-icons flex row">
        <div class="flex column wr">
          <icon-doc></icon-doc>
          <div class="account-icons--text">View & pay your bill</div>
        </div>
        <div class="hr"></div>
        <div class="flex column wr">
          <icon-gauge></icon-gauge>
          <div class="account-icons--text">View your usage</div>
        </div>
        <div class="hr"></div>
        <div class="flex column wr">
          <icon-plus></icon-plus>
          <div class="account-icons--text">Add or change services</div>
        </div>
        <div class="hr"></div>
        <div class="flex column wr">
          <icon-phone></icon-phone>
          <div class="account-icons--text">Upgrade your device</div>
        </div>
      </div>
    </article>
    <div class="frog">
      <div class="frog-top"></div>
      <div class="frog-bot flex row">
        <div class="card">
          <div class="card-header">You're getting a first look at our new Web site.</div>
          <div class="card-text">It's not finished, yet. We want you to see what we've done so far. Tell us what you love, or wish we'd do differently. We're listening to your feedback. It makes us better.</div>
          <div class="card-footers flex row">
            <div class="card-footer">
              <button>Share your feedback</button>
              <div class="card-text">Cant find what you're looking for?</div>
              <div class="linked">Visit our current site.</div>
            </div>
            <div class="card-footer-small flex column">
              <img src="../assets/nc_logo.png" alt="">
              <div class="linked">Follow our blog and join the rebuild.</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <footer class="flex column">
      <article class="flex row">
        <div class="link">About us</div>
        <div class="link">Careers</div>
        <div class="link">Special Needs</div>
        <div class="link">Privacy</div>
        <div class="link">Security</div>
        <div class="link">User Terms</div>
      </article>
      <div class="hr"></div>
      <div class="copyright">© 2013 Communications Company</div>
    </footer>
  </section>
</template>

<script>
import IconGauge from './IconGauge.vue'
import IconDoc from './IconDoc.vue'
import IconPhone from './IconPhone.vue'
import IconPlus from './IconPlus.vue'
import Carousel from './Carousel.vue'
export default {
  name: 'Landing',
  components: {
    IconGauge,
    IconDoc,
    IconPhone,
    IconPlus,
    Carousel
  },
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus">
  $main-blue = #0365a1
  $main-active = #974a00

  section
    overflow hidden
  button
    display: inline-block;
    padding: .5rem .5rem;
    font-size: 1.5rem;
    cursor: pointer;
    text-align: center;
    text-decoration: none;
    outline: none;
    color: #fff;
    background-color: #548cb7;
    border: none;
    border-radius: 5px;
    box-shadow: 0 9px #0053a1;
    margin-top 1rem
    margin-bottom 1rem

  button:hover {background-color: $main-blue}

  button:active {
    background-color: $main-blue;
    box-shadow: 0 5px #0053a1;
    transform: translateY(4px);
  }

  header
    height 10vh
    max-width 100vw
    justify-content space-between
    align-items center
    div.logo
      width 20rem
      margin-left 1rem
      background url('../assets/nc_hd.jpg') no-repeat center center
      background-size contain
      height 100%
      cursor pointer
    div.link
      color: $main-blue
      border-bottom 1px solid $main-blue
      font-size 1.5rem
      cursor pointer
      &:hover
        color: $main-active
        border-bottom 1px solid transparent
      &--icon
        justify-content center
        align-items center
        img
          cursor pointer
        &:hover
          img
            filter: hue-rotate(190deg);
      &--dotted
        border-bottom 1px dotted $main-blue
      &--no-border
        border-bottom 1px solid transparent
    img
      max-width 1.5rem
      max-height  1.5rem

  footer
    background-color: #333333;
    height 35vh
    width 100vw
    justify-content flex-start
    align-items center
    article
      justify-content center
      align-items center
      height 8rem
    div.link
      color: #fff
      font-size 1.5rem
      border-bottom 1px solid #fff
      margin 1rem
      cursor pointer
      &:hover
        border: none
        color: $main-active
    div.hr
      width 90%
      height 0px
      margin-bottom 3rem
      border-top 1px solid rgba(81, 81, 81, 0.64)
    div.copyright
      font-size 1.5rem
      color: rgba(81, 81, 81, 0.64)

  .hoverable
    transition fill .3s linear
    cursor pointer
  img.hoverable
    &:hover
      filter: hue-rotate(190deg);
  .hovered
    fill: $main-active !important
  .flex
    display flex
  .row
    flex-flow row
  .column
    flex-flow column
  .hr
    width 1px
    height 7rem
    background-color rgba(255, 255, 255, 0.42)
  .account
    height: 35vh;
    max-width: 100vw;
    background-color: #333333;
    justify-content space-around
    align-items center
    &-caption
      align-self flex-start
      margin 1rem
      margin-bottom 3rem
      justify-content center
      align-items center
      &--text
        color: #fff
        font-size 3rem
        margin-left 2rem
      img
        width 3rem
    &-icons
      width 90vw
      justify-content space-around
      align-items center
      margin-bottom 3rem
      div.wr
        justify-content center
        align-items center
      div.flex
        cursor pointer
      &--text
        color: #fff
        font-size 1.2rem
        margin-top .5rem
      &-wrapper
        width 5rem
        height 7rem
  .frog
    height 100vh
    max-width 100vw
    &-top
      height 20vh
      background url('../assets/frog_top.png'), #f5f6f7
      background-repeat no-repeat, no-repeat
      background-position 95% 100%
    &-bot
      height 80vh
      justify-content flex-start
      align-items center
      background-image url('../assets/frog_bot.png')
      background-repeat no-repeat
      background-position 95% 0%
  .card
    width 55vw
    margin-left 15rem
    &-header
      font-size: 4rem
      text-align: start;
      color: $main-blue
    &-text
      margin-top 2rem;
      font-size: 2rem;
      text-align: start;
    &-footers
      justify-content space-between
      align-items center
    &-footer
      justify-content center
      align-items center
      text-align left
      button
        width 100%
      &-small
        justify-content center
        align-items center
        width 30%
        text-align right
        margin-left 5rem
        img
          margin 2rem
          width 80%
  .linked
    font-size 2rem
    color: $main-blue
    line-height 3rem
    text-decoration underline
    cursor pointer
    &:hover
      text-decoration none
      color: $main-active
  .spacer
    width 30vw

  @media only screen and (max-width: 1400px)
    .spacer
      width 15vw
    .card
      &-header
        font-size: 4rem
      &-text
        font-size: 1.5rem;
    .linked
      font-size 1.5rem
      line-height 2rem
    .account
      &-caption
        margin-bottom 2rem
      &-icons-wrapper
        width 5rem
        height 7rem

  @media only screen and (max-width: 1000px)
    .spacer
      width 5vw
    header
        div.logo
          width 15rem
        div.link
          font-size 1rem
    footer
      div.link
        font-size 1rem
    .account
      &-caption
        margin-bottom 2rem
      &-icons
        &--text
          font-size .8rem
    .card
      width 100vw
      margin 1rem
      &-header
        max-width 80vw
</style>
