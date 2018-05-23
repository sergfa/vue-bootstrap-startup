<template>
  <div :id="id" class="carousel slide" data-ride="carousel">
    <ul class="carousel-indicators">
      <li :data-target="carouselId" v-for="(item, index) in items" :key="index" :data-slide-to="index" :class="{active: item.active}"></li>
    </ul>
    <div class="carousel-inner">
      <div class="carousel-item" v-for="(item, index) in items" :key="index" :class="{active: item.active}">
        <img :src="item.image" alt="project" width="500px">
      </div>
    </div>
    <a :href="carouselId" class="carousel-control-prev" data-slide="prev">
      <span class="carousel-control-prev-icon"></span>
    </a>
    <a :href="carouselId" class="carousel-control-next" data-slide="next">
      <span class="carousel-control-next-icon"></span>
    </a>

  </div>
</template>
<script>


export default {
    props: ['items'],
    data () {
        return {
            id: null
        }
    },
    computed: {
       carouselId () {
           return '#' + this.id
       } 
    },
    mounted () {
        this.id = 'carousel' + this._uid
    }
}
</script>
