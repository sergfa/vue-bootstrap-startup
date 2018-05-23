<template>
    <section id="header">
        <div class="container">
            <div class="row height-100 align-items-center">
                <div class="col text-left p-5">
                    <h1 class="text-uppercase text-warning font-weight-bold font-italic"><strong v-once>{{title1}}</strong> <small class="text-dark" v-once>{{title2}}</small></h1>
                    <p class="lead text-light py-2 w-75" v-once>{{description}}</p>
                    <a href="" class="btn btn-warning btn-lg text-uppercase" v-once>{{buttonSecondaryCaption}}</a>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    data () {
        return {
            title1: 'Design & Code',
            title2: '',
            buttonPrimaryCaption : 'Contact',
            buttonSecondaryCaption : 'Contact',
            description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores, corporis!'
        }
    }
}
</script>
<style scoped>
#header {
    background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.5)), url('../assets/header/background.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: fixed;
}
</style>

