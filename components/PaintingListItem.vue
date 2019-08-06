<template>
  <nuxt-link :to="{name: 'home'}" tag="figure" class="painting" v-if="painting">
    <img class="painting__image" :src="painting.images[0]" alt="">
    <figcaption class="painting__title">
      {{ painting.title }}
    </figcaption>
  </nuxt-link>
</template>

<script>
export default {
  props: {
    painting:{
      required: true,
      type: Object
    }
  }
}
</script>

<style scoped>
  .painting {
    margin: 0;
    position: relative;
    padding-bottom: 50%;
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
    transition: all 0.3s cubic-bezier(.25,.8,.25,1);
    cursor: pointer;
  }

  .painting:hover {
    box-shadow: 0 7px 15px rgba(0,0,0,0.12), 0 5px 5px rgba(0,0,0,0.11);
  }

  .painting:before {
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    display: block;
    width: 100%;
    height: 100%;
    z-index: 1;
    transition: all .2s ease-in-out;
    pointer-events: none;
    opacity: 0;
  }

  .painting:hover:before {
    background: rgba(255, 255, 255);
    opacity: .5;
  }

  .painting__title {
    position: absolute;
    top: 55%;
    left: 1rem;
    right: 1rem;
    width: 100%;
    transform: translateY(-50%);
    opacity: 0;
    transition: all .2s ease-in-out;
    text-align: center;
    text-transform: uppercase;
    color: rgba(0, 0, 0, .87);
    z-index: 2;
  }

  .painting:hover .painting__title{
    top: 50%;
    opacity: 1;
  }

  .painting__image {
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
</style>
