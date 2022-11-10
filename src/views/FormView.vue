<template>
  <div>
    <div>ihis is onelick dropdown</div>
    <botton @click="dropdown=!dropdown">menu</botton>
    <div class="rounded-lg animate-fadeIn" v-if="dropdown">this is dropdown</div>
    <div>this is onchange</div>
    <input type="text" @change="count++">
    <div>
        count is {{count}}
    </div>
    <div>this is v-model</div>
    <input type="text" v-model="name">
    <div>
        {{name}}
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return{
            count: 0,
            dropdown: false,
            name: ''
        }
    }

};
</script>

<style>

</style>