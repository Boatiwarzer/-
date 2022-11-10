<template>

    <div class="fontlink">
        <router-link to="/">Home</router-link>
        <slot></slot>

    </div>
</template>
<script>
export default{

}
</script>
<style>
.fontlink{
    @apply text-center text-2xl text-pink-900 bg-rose-400 
}

</style>