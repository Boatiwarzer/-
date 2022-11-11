<template>
    <div class="fontlink">

        
        <div class="block p-4 bg-slate-300  border-red-200 shadow-md hover:bg-red-100 dark:bg-red-800 dark:border-red-700 dark:hover:bg-red-700r">
        <router-link to="/" class="bg-slate-400">Home</router-link>
            <div class="fontsmain">
                <div class="container">
                    <div class="box">
                        <strong class="text-5xl">Group Teletubbie</strong>
                        <img src="../assets/images/te.jpg" alt="teletubbie" >
                        If you want to know my member go to this link
                        <strong><router-link to="/profile">Profile</router-link></strong>
                        <div>
                            <strong><router-link to="/form">Form</router-link></strong>

                        </div>


                    </div>
                
                </div>
                
            
             
            </div>
    </div>



    </div>
    
</template>
<script>

export default{
    // components: {RouterLink}

}
</script>
<style>
.fontlink{
    @apply block text-right text-2xl text-pink-900;

}
.container{
    width: 100%;
    padding: 20px;
    margin: 20px auto;
    display: block;
}
.box{
    width: 35%;
    margin: auto;
    
    
}
.box img{
    display: block;
    width: 300%;
    border-radius: 20px;
}
.fontsmain{
    @apply  text-sky-700 text-center text-3xl ;
    font-family: 'Poor Story', cursive;

}
</style>