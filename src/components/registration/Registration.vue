<template>
  <section class="hero is-fullheight">
    <div class="hero-body is-paddingless">
     <section class="wrapper is-fullheight">
      <div class="left-half has-bg">
        <article>
          <h1 class="title title-left is-1">This revolution - like any good revolution - is free to join.</h1>
          <div class="socials">
            <h3 class="title is-3 center">You can also sign up with one of your social media accounts.</h3>
          </div>
        </article>
      </div>
      <div class="right-half">
       <article>
         <h1>Right Half</h1>
         <p>If your knees aren't green by the end of the day, you ought to seriously re-examine your life.</p>
        </article>
      </div>
     </section>
    </div>
  </section>
</template>


<script>
    export default {
        name: 'registration'
    }
</script>

<style lang="sass" scoped>
@import "~bulma/sass/utilities/_all";
@import "~bulma/sass/grid/columns";
@import "~bulma/sass/layout/_all";
@import "~bulma/sass/base/_all";
@import "~bulma/sass/custom/mixins";
@import "~bulma/sass/elements/_all";


@import "~bulma/sass/custom/mixins";
@import "~include-media/dist/_include-media"

html, body, section 
  height: 100%

div 
  display: flex
  flex-direction: column
  justify-content: center
  
.wrapper 
  height: 100vh
  width: 100vw
  display: flex

.left-half 
  background-color: #ff9e2c
  flex: 1
  padding: 6rem
  @include media("<desktop")
    display: none

.right-half 
  flex: 1
  padding: 1rem

.title 
  color: white
  text-shadow: 0 4px 6px rgba(0,0,0,0.50)
  
.title.title-left
  text-align: left !important

.has-bg 
    @include cover-background('../../assets/img/registration-background-left.jpg');
    /*min-height: 100%;*/

.socials 
  
</style>