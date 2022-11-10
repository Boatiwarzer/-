<template>
    <div class="flex items-center justify-center spce-x-5 h-screen">
        <div v-for="member in members" :key="member">
            <profileCard v-if="member.img"  
            :img="member.img" 
            :name="member.name" 
            :nickname="member.nickname" 
            :content="member.content" 
            :age="member.age">
            </profileCard>

        </div>
            
    </div>

    
</template>
<script>
import profileCard from "../components/Profile.vue";

export default {
    data(){
        return{
            members: [
                {
                    img:'/assets/images/B.jpg',
                    name: 'Puttita',
                    nickname: 'Bow',
                    content: 'KU81',
                    age:'21',
                    isMember: true
                },{
                    img:'/assets/images/BT.jpg',
                    name: 'Puttipong',
                    nickname: 'Boat',
                    content: 'KU81',
                    age:'19',
                    isMember: true

                },{
                    img:'/assets/images/E.jpg',
                    name: 'Hataichanok',
                    nickname: 'Earth',
                    content: 'KU81',
                    age:'19',
                    isMember: true


                },{
                    img:'',
                    name: 'Hataichanok',
                    nickname: 'Earth',
                    content: 'KU81',
                    age:'19',
                    isMember: false


                },
            ],
            
        };
    },    
    components: {profileCard,},
};


</script>
<style>
</style>
