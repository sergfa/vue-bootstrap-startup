<template>
    <nav class="navbar navbar-expand-md navbar-dark bg-secondary py-3">
        <a href="#" class="navbar-brand text-uppercase">TrueCode</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarBrand">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div id="navbarBrand" class="collapse navbar-collapse">
            <ul class="navbar-nav">
                <li  class="nav-item active" ><a href="#header" class="nav-link text-uppercase">Header</a></li>
                <li  v-for="(item, index) in items" :key="index" class="nav-item" ><a :href="item.id" class="nav-link text-uppercase">{{item.title}}</a></li>
            </ul>
        </div>
    </nav>
</template>
<script>
export default {
    data () {
        return {
            items: [{id: '#skills', title: 'Skills' },
                    {id: '#blog', title: 'Blog' },
                    {id: '#contact', title: 'Contact' },
                    {id: '#review', title: 'review' },
                    {id: '#progress', title: 'progress' },
                    {id: '#price', title: 'price' }]
        }
    }
}
</script>

