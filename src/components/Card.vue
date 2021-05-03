<template>
    <a class="card col-sm-12 col-md-6 col-lg-4 py-12" :href="card.link">
        <img :src="card.src" class="w-100">
    <div class="card-title-cont">
        <h2 class="card-title">
            {{ card.title }}
        </h2>
        <p class="card-desc">
            {{ card.desc }}
        </p>
    </div>
    </a>
</template>

<script>
export default {
    title: 'card',
    props: ['card']
}
</script>

<style>
    a {
        color: #000;
        text-decoration: none;
        transition: opacity .15s ease-in-out;
    }
    a:hover {
        color: #000;
        opacity: 0.85;
    }
</style>
