<template>
    <section id="team" class="bg-primary p-5">
        <div class="container">
            <app-title title-value="Team" subtitle-value="Lorem ipsum dolor sit amet." color="light"></app-title>
            <div class="row mt-5">
                    <div v-for="(member, index) in members" :key="index" class="col-md-6 col-lg-4 my-3">
                        <div class="card">
                            <img :src="member.image" alt="member" class="card-img-top">
                            <div class="card-body">
                                <h2 class="text-dark text-capitalize" v-once>{{member.name}}</h2>
                                <p class="text-dark" v-once>{{member.desc}}</p>
                            </div>
                            <div class="card-footer d-flex justify-content-around bg-primary">
                                <a class="text-secondary" href="#"><i class="fab fa-facebook fa-2x"></i></a>
                                <a class="text-secondary" href="#"><i class="fab fa-twitter fa-2x"></i></a>
                                <a class="text-secondary" href="#"><i class="fab fa-youtube fa-2x"></i></a>
                                <a class="text-secondary" href="#"><i class="fab fa-google fa-2x"></i></a>
                                
                            </div>
                        </div>
                    </div>
            </div>
        </div>
    </section>
</template>
<script>
import imgTeam1 from '../assets/team/team1.jpg'
export default {
    data () {
        return {
            members: [{image: imgTeam1, name: 'Team Member', desc:'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos ex pariatur excepturi veniam ducimus nisi aperiam voluptatem maiores illum mollitia.'},
            {image: imgTeam1, name: 'Team Member', desc:'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos ex pariatur excepturi veniam ducimus nisi aperiam voluptatem maiores illum mollitia.'},
            {image: imgTeam1, name: 'Team Member', desc:'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quos ex pariatur excepturi veniam ducimus nisi aperiam voluptatem maiores illum mollitia.'}]
        }
    }
}
</script>
