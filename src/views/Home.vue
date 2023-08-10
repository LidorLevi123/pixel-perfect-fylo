<template>
    <section class="home main-container">
        <AppHeader />
        <Hero />
        <CardList />
        <Productive />
        <ReviewList />
    </section>
</template>

<script>
import AppHeader from '../cmps/AppHeader.vue'
import Hero from '../cmps/Hero.vue'
import CardList from '../cmps/CardList.vue'
import Productive from '../cmps/Productive.vue'
import ReviewList from '../cmps/ReviewList.vue'

export default {
    components: {
        AppHeader,
        Hero,
        CardList,
        Productive,
        ReviewList
    }
}
</script>