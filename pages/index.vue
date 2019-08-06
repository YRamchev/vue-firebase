<template>
  <div class="container">
    <PaintingList :paintings="paintings"/>
  </div>
</template>

<script>
import PaintingList from '../components/PaintingList'

export default {
  components: {
    PaintingList
  },

  data () {
    return {
      paintings: [
        {
          title: 'Some Title',
          images: ['https://dvqlxo2m2q99q.cloudfront.net/000_clients/400941/page/h800-400941MtGIKL9Z.jpg', '', '', ''],
          description: 'lorem',
          isInstock: true
        },
        {
          title: 'Some Title',
          images: ['https://dvqlxo2m2q99q.cloudfront.net/000_clients/400941/page/h800-400941MtGIKL9Z.jpg', '', '', ''],
          description: 'lorem',
          isInstock: true
        },
        {
          title: 'Some Title',
          images: ['https://dvqlxo2m2q99q.cloudfront.net/000_clients/400941/page/h800-400941MtGIKL9Z.jpg', '', '', ''],
          description: 'lorem',
          isInstock: true
        },
        {
          title: 'Some Title',
          images: ['https://dvqlxo2m2q99q.cloudfront.net/000_clients/400941/page/h800-400941MtGIKL9Z.jpg', '', '', ''],
          description: 'lorem',
          isInstock: true
        },
        {
          title: 'Some Title',
          images: ['https://dvqlxo2m2q99q.cloudfront.net/000_clients/400941/page/h800-400941MtGIKL9Z.jpg', '', '', ''],
          description: 'lorem',
          isInstock: true
        },
        {
          title: 'Some Title',
          images: ['https://dvqlxo2m2q99q.cloudfront.net/000_clients/400941/page/h800-400941MtGIKL9Z.jpg', '', '', ''],
          description: 'lorem',
          isInstock: true
        },
        {
          title: 'Some Title',
          images: ['https://dvqlxo2m2q99q.cloudfront.net/000_clients/400941/page/h800-400941MtGIKL9Z.jpg', '', '', ''],
          description: 'lorem',
          isInstock: true
        },
        {
          title: 'Some Title',
          images: ['https://dvqlxo2m2q99q.cloudfront.net/000_clients/400941/page/h800-400941MtGIKL9Z.jpg', '', '', ''],
          description: 'lorem',
          isInstock: true
        },
        {
          title: 'Some Title',
          images: ['https://dvqlxo2m2q99q.cloudfront.net/000_clients/400941/page/h800-400941MtGIKL9Z.jpg', '', '', ''],
          description: 'lorem',
          isInstock: true
        }
      ]
    }
  }
}
</script>