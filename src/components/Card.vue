<template>
  <div class="wrap">
    <div class="card" style="width: 18rem;">
      <img class="card-img" :src="image_url" alt="">
      <h3 class="card-title" v-bind:style="{fontSize: font_sizeLocal + 'px'}"> {{titleLocal}} </h3>
    </div>
    <div class="content">
      <div class="form-group">
        <p>title</p>
        <input class="form-control" v-model="titleLocal" type="text">
      </div>
      <div class="form-group">
        <p>font size:</p>
        <input class="form-control" v-model="font_sizeLocal" type="number" min="0">
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    title: {
      type: String,
      default: "MENU"
    },
    font_size: {
      type: String,
      default: "20"
    },
    image_url: {
      type: String,
      default: "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRoaqPDmLsepthNX6Jrc9ptK6JwfQvvk3WuRQ&usqp=CAU"
    }
  },
  data () {
    return {
      titleLocal: this.title,
      font_sizeLocal: this.font_size
    }
  }
}
</script>

<style scoped>
  .card {
    text-align: center;
  }
  .wrap {
    display: flex;
    margin: 10px;
  }
  .content {
    margin-left: 40px;
  }
  .card-img {
    max-width: 300px;
  }
</style>
