<template>
  <div id="app" class="container">
    <Card />
    <Card title="flamingo" font_size=5 image_url="https://bipbap.ru/wp-content/uploads/2019/05/1-flamingo-drawing-step-by-step-136.jpg" />
  </div>
</template>

<script>
import Card from './components/Card.vue'

export default {
  name: 'App',
  components: {
    Card
  },
}
</script>

<style>

</style>
