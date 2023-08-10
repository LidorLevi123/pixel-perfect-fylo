<template>
    <article class="review-preview">
        <p>{{ review.txt }}</p>
        <div class="user">
            <img :src="review.by.imgUrl" alt="">
            <h4>{{ review.by.name }}</h4>
            <small>{{ review.by.role }}</small>
        </div>
    </article>
</template>

<script>
export default {
    props: {
        review: { type: Object }
    }
}
</script>