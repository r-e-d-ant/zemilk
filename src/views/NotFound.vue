


<template>
<div class="not-found__container">
    <div class="not-found">
        <h1>404</h1>

        <p>PAGE NOT FOUND.</p>
    </div>
    <p>Go back <router-link :to="{ name: 'Home' }">Home</router-link></p>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
.not-found__container {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
.not-found__container p {
    font-size: 1.1rem;
    text-align: center;
}
.not-found
h1 {
    font-size: 10rem;
    opacity: .85;
}
.not-found
p {
    font-size: 2rem;
}
</style>