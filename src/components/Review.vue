<template>
    <section id="review" class="bg-light py-5">
        <div class="container">
             <app-title title-value="Review" subtitle-value="Lorem ipsum dolor sit amet." color="dark"></app-title>
           
            <div class="row">
                <div class="col-sm-6 text-center">
                    <img :src="reviewImg" alt="reviewer" class="img-fluid rounded-circle d-none d-sm-block">
                </div>
                <div class="col-sm-6 align-self-center">
                    <blockquote class="blockquote text-right">
                    <p>
                       <i class="fas fa-quote-left fa-2x mr-3"></i>
                       Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, optio. 
                    </p>
                    <footer class="text-dark text-left blockquote-footer">Code master</footer>    
                    </blockquote>

                    
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
            reviewImg: imgTeam1
        }
    }
}
</script>
