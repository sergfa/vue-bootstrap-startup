<template>
    <section id="price" class="bg-light py-5">
        
        <div class="container">
            <app-title title-value="Price" subtitle-value="Lorem ipsum dolor sit amet." color="dark"></app-title>
           
            <div class="row mt-5">
                <div class="col-md-4 mb-3" v-for="item in items" :key="item.name">
                    <div class="card">
                        <div class="card-header bg-warning text-uppercase text-center py-4" v-once>{{item.name}}</div>
                         <div class="card-title text-center my-4">
                            <h4 v-once><sup>$</sup>{{item.price}}<sub>/month</sub></h4>
                         </div>   
                           <ul class="list-group list-group-flush">
                               <li class="list-group-item text-muted" v-for="(line, index) in item.text" :key="index">
                                   {{line}}
                               </li>
                           </ul> 
                        <div class="card-footer">
                            <a href="#" class="btn btn-outline-warning btn-block btn-lg">Sign up</a>
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
            items: [{name: 'standard', text: ['Lorem ipsum dolor', 'Lorem ipsum dolor', 'Lorem ipsum dolor'], price: 5},
            {name: 'basic', text: ['Lorem ipsum dolor', 'Lorem ipsum dolor', 'Lorem ipsum dolor'], price: 15},
            {name: 'pro', text: ['Lorem ipsum dolor', 'Lorem ipsum dolor', 'Lorem ipsum dolor'], price: 100}]
        }
    }
}
</script>
