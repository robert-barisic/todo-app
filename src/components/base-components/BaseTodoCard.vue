<template>
    <div class="card">
        {{ title }}
    </div>
</template>

<script>
export default ({
    props: ['title']
})
</script>

<style scoped>
.card {
    color: lightblue;
    background-color: bisque;
    width: 400px;
    height: 50px;
    font-size: 20pt;
}
</style>