<template>

    <div class="fontlinks">
        <router-link to="/" class="bg-sky-300">Home</router-link>
        <slot></slot>

    </div>
</template>
<script>
export default{

}
</script>
<style>
.fontlinks{
    @apply p-2 text-right text-2xl text-pink-900 bg-rose-400 ;
    background-repeat: no-repeat;
    
}

</style>