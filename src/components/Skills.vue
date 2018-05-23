<template>
    <section id="skills" class="bg-light p-5">
        <div class="container">
            <app-title title-value="Skills" subtitle-value="Lorem ipsum dolor sit amet." color="dark"></app-title>
            
            <div class="row mt-5">
                <div v-for="skill in skills" :key="skill.title" class="col-md-6 col-lg-3 text-center mb-5">
                    <i class="fab fa-5x text-warning" :class="skill.icon"></i>
                    <h2 class="text-uppercase py-3 text-dark" v-once>{{skill.title}}</h2>
                    <p class="text-dark" v-once>{{skill.text}}</p>
                    <a href="#" class="btn btn-outline-warning w-75 text-uppercase mt-2">Learn more</a>
                </div>
           </div>
        </div>
    </section>
</template>
<script>
export default {
    data () {
        return {
            skills: [{icon: 'fa-vuejs', title: 'Vue', text:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis cum labore illum sed veritatis quidem corporis perferendis aperiam voluptate nihil corrupti, veniam at fugiat deleniti pariatur dolorem libero similique exercitationem?'},

            {icon: 'fa-html5', title: 'HTML', text:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis cum labore illum sed veritatis quidem corporis perferendis aperiam voluptate nihil corrupti, veniam at fugiat deleniti pariatur dolorem libero similique exercitationem?'},

            {icon: 'fa-css3', title: 'bootstrap', text:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis cum labore illum sed veritatis quidem corporis perferendis aperiam voluptate nihil corrupti, veniam at fugiat deleniti pariatur dolorem libero similique exercitationem?'},

            {icon: 'fa-js', title: 'javascript', text:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis cum labore illum sed veritatis quidem corporis perferendis aperiam voluptate nihil corrupti, veniam at fugiat deleniti pariatur dolorem libero similique exercitationem?'}
            ]
        }
    }
}
</script>
<style scoped>
.title-underline {
    width: 100px;
}
</style>

