<template>
    <section id="blog" class="bg-light p-5">
        <div class="container">
            <app-title title-value="Blog" subtitle-value="Lorem ipsum dolor sit amet." color="dark"></app-title>
            <div class="row">
                <div v-for="(blog, index) in blogs" :key="index" class="col-md-6 col-lg-4 mb-3">
                    <div class="card">
                        <img :src="blog.image" alt="blog" class="card-img-top img-thumbnail">
                        <div class="card-body">
                            <h2 class="text-capitalize text-dark" v-once>{{blog.name}}</h2>
                            <p class="text-dark mt-3" v-once>{{blog.text}}</p>
                            <a href="#" class="btn btn-lg btn-outline-warning btn-block mt-2">Show more</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import blogImage1 from '../assets/projects/project2.jpg'
export default {
    data () {
        return {
            blogs: [{image: blogImage1, name: 'Project 1', text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat totam sed quasi consequatur, quaerat et accusamus eligendi. Accusantium, recusandae numquam!'}, 
            {image: blogImage1, name: 'Project 2', text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat totam sed quasi consequatur, quaerat et accusamus eligendi. Accusantium, recusandae numquam!'}, 
            {image: blogImage1, name: 'Project 2', text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat totam sed quasi consequatur, quaerat et accusamus eligendi. Accusantium, recusandae numquam!'}]
        }
    }
}
</script>
