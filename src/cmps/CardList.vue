<template>
    <ul class="card-list clean-list">
        <li><CardPreview :type="1"/></li>
        <li><CardPreview :type="2"/></li>
        <li><CardPreview :type="3"/></li>
        <li><CardPreview :type="4"/></li>
    </ul>
</template>

<script>
import CardPreview from './CardPreview.vue';

export default {

    components: {
        CardPreview
    }
}
</script>