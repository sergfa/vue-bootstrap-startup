<template>
    <section id="projects" class="bg-light p-5">
        <div class="container">
            <app-title title-value="last projects" subtitle-value="Lorem ipsum dolor sit amet." color="dark"></app-title>
            <div class="row py-3">
                <div v-for="(project, index) in projects" :key="index" class="col-sm-6 col-md-4">
                    <img :src="project.image" alt="project" class="img-fluid img-thumbnail bg-primary my-3">
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import imgProject1 from '../assets/projects/project1.jpg'
import imgProject2 from '../assets/projects/project2.jpg'
import imgProject3 from '../assets/projects/project3.jpg'

export default {
    data () {
        return {
            projects: [{image:imgProject1},
                        {image:imgProject2},
                        {image: imgProject3}
                        ]
        }
    }
}
</script>
