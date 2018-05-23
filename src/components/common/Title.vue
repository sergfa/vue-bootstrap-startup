<template>
<div class="row">
  <div class="col text-center">
    <h2 class="text-uppercase m-0" :class="titleColor">
      <strong>{{titleValue}}</strong>
    </h2>
    <div class="title-underline bg-warning"></div>
    <p class="text-capitalize text-light mt-3" :class="subtitleColor">{{subtitleValue}}</p>
  </div>
</div>
</template>
<script>
export default {
    props: ['titleValue', 'subtitleValue', 'color'],
    computed: {
        titleColor () {
            console.log(this.color);
            return this.color === 'light' ? 'text-light': 'text-dark' 
        },
        subtitleColor () {
            return this.color === 'light' ? 'text-light': 'text-dark'
        }
    }
}
</script>
