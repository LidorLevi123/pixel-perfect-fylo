<template>
    <ul v-if="reviews.length" class="review-list clean-list">
        <li>
            <img class="quotes" src="src/assets/bg-quotes.png" alt="">
            <ReviewPreview :review="reviews[0]" />
        </li>
        <li><ReviewPreview :review="reviews[1]" /></li>
        <li><ReviewPreview :review="reviews[2]" /></li>
    </ul>
</template>

<script>
import ReviewPreview from './ReviewPreview.vue';

export default {

    data() {
        return {
            reviews: []
        }
    },

    created() {
        this.loadReviews()
    },

    methods: {
        loadReviews() {
            const names = ['Satish Patel', 'Bruce McKenzie', 'Iva Boyd']
            const images = ['src/assets/001.png', 'src/assets/002.png', 'src/assets/003.png']

            for (let i = 0; i < 3; i++) {
                this.reviews.push({
                    txt: `Fylo has improved our team productivity by an order of magnitude. 
                        Since making the switch our team has become a well-oiled collaboration machine.`,
                    by: {
                        name: names[i],
                        imgUrl: images[i],
                        role: 'Founder & CEO, Huddle',
                    }
                })
            }
        }
    },

    components: {
        ReviewPreview
    }
}
</script>