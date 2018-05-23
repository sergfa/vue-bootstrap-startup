<template>
    <section id="progress" class="bg-primary py-5">
        <div class="container">
            <app-title title-value="progress" subtitle-value="Lorem ipsum dolor sit amet." color="light"></app-title>
            
            <div class="row mt-5">
                <div class="col-md-8 mx-auto">
                    <div v-for="tech in progressItems" :key="tech.name" class="progress-tech mt-4">
                        <div class="text-light d-flex justify-content-between">
                        <p class="mb-0"  v-once>{{tech.name}}</p>
                        <p class="mb-0" v-once>{{tech.percent}}%</p>
                        </div>
                        <div class="progress">
                            <div class="progress-bar" :class="tech.colorClass" role="progressbar" :style="{width: tech.percent + '%'}" :aria-valuenow="tech.percent" aria-valuemin="0" aria-valuemax="100"></div>
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
            items: [{name:'HTML', percent: 75, colorClass: 'bg-success'},{name:'CSS', percent: 25,colorClass: 'bg-danger'}, {name:'JavaScript', percent: 90, colorClass: 'bg-success'}, {name:'Vue', percent: 50, colorClass: 'bg-warning'}]
        }
    },
    computed: {
        progressItems () {
            return this.items.sort(function(item1, item2){
               return item2.percent - item1.percent     
            });
        }
    }
}
</script>
