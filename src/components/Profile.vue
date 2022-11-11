<template>
    <div class="ml-4 inline-block p-8 max-w-md bg-rose-200 rounded-lg border border-red-200 shadow-md hover:bg-red-100 dark:bg-red-800 dark:border-red-700 dark:hover:bg-red-700r">
        <div class="fonts">
            <div class="imgsize" :style="getUrlImage(img)"></div>
                NAME: {{name}}
            <div>
               NICKNAME: {{nickname}}
            </div>
            <div>
                {{content}}
            </div>
            
            <div>
                {{age}} YEAR
            </div>
        </div>  
        <div class="w-2/3 mx-auto text-right space-x-3 border-t-2 p-2 mt-5">
            <font-awesome-icon icon="fa-brands fa-instagram" class="text-2xl text-pink-400" />
            <font-awesome-icon icon="fa-brands fa-facebook" class="text-2xl text-blue-800" />
            <font-awesome-icon icon="fa-brands fa-github" class="text-2xl text-black" />
        </div>
    </div>
</template>
<script>
export default {
    props: {
        img: {
            type: String,
            default:'/assets/images/BT.jpg'
        },
        name: {
            type:String,
            default:'Puttipong Srina'
        },
        nickname: {
            type:String,
            default: 'Boat'
        },
        content: {
            type:String,
            default: 'KU81'
        },
        age: {
            type:String,
            default:'21'
        },
    },
    methods:{
        getUrlImage(imagePath){
            return {'background-image': 'url("./src' + imagePath + '")'};
        }
    }
};

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poor+Story&display=swap');

.fonts{
    @apply  text-sky-700 text-left text-3xl ;
    font-family: 'Poor Story', cursive;

}
.imgsize{
    @apply border-2 border-red-600 rounded-full shadow-sm bg-contain bg-center scale-90 w-96 h-96;
    /* width: 300px ;
    height: 300px; */
} 
</style>