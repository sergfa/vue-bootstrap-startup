<template>
    <section id="about" class="bg-primary">
        <div class="container-fluid">
            <div class="row">
                <div class="col-md-6 about-picture  height-80">

                </div>
                <div class="col-md-6 about-text d-flex align-items-center justify-content-center  height-80">
                    <div class="about-text-center">
                    <app-title title-value="About" subtitle-value="Lorem ipsum dolor sit amet." color="light"></app-title>
                    <div v-for="(item, index) in aboutItems" :key="index" class="checkbox-item d-flex">
                        <i class="fas fa-check fa-3x align-self-center p-2 mr-3 text-warning"></i>
                        <p class="text-light w-75" v-once>{{item}}</p>   
                    </div>
                   
                   
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    data () {
        return {
            aboutItems: ['Lorem ipsum dolor sit amet consectetur, adipisicing elit. Unde, vitae!', 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Unde, vitae!', 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Unde, vitae!', 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Unde, vitae!']
        }
    }
}
</script>

<style scoped>
.about-picture {
    background: url('../assets/code1.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
}
.title-underline {
    width: 100px;
}
</style>
