<script>
export default {
    name: 'ProductCard',
    props: {
        image: String,
        title: String
    }
}
</script>
<template>
    <div class="box">
        <img :src="image" :alt="title">
        <h3>{{ title }}</h3>
    </div>
</template>
<style lang="scss" scoped></style>