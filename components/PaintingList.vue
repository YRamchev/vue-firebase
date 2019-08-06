<template>
  <div class="listing">
    <div
      v-for="(painting, index) in paintings" 
      :key="index"
      class="listing__item"
    >
      <PaintingListItem :painting="painting"/>
    </div>
  </div>
</template>

<script>
import PaintingListItem from './PaintingListItem'
export default {
  props: {
    paintings: {
      required: true,
      type: Array
    }
  },

  components: {
    PaintingListItem
  }
}
</script>

<style>
  .listing {
    display: flex;
    flex-wrap: wrap;
    margin: -.4rem;
  }

  .listing__item {
    padding: .4rem;
    width: calc(33.33% - .8rem);
  }
</style>
