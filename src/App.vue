<template>
    <div id="app">
        <h1>PupFest 2020</h1>
        <ul class="dogs">
            <li v-for="dog in dogs" :key="dog.id">
                <DogCard :dog="dog" />
            </li>
        </ul>
    </div>
</template>

<script>
import DogCard from "@/components/DogCard"

export default {
    components: {
        DogCard,
    },
    data(){
        return {
            dogs: [{
                id: 1,
                name: "Spud",
                description: "A real good buddy",
                imageUrl: "https://hips.hearstapps.com/ghk.h-cdn.co/assets/17/30/2560x1280/landscape-1500925839-golden-retriever-puppy.jpg?resize=480:*"
            },{
                id: 2,
                name: "McKenzie",
                description: "A great gal",
                imageUrl: "https://hips.hearstapps.com/ghk.h-cdn.co/assets/17/30/2560x1280/landscape-1500925839-golden-retriever-puppy.jpg?resize=480:*"
            },{
                id: 3,
                name: "Rocket",
                description: "A scamp!",
                imageUrl: "https://hips.hearstapps.com/ghk.h-cdn.co/assets/17/30/2560x1280/landscape-1500925839-golden-retriever-puppy.jpg?resize=480:*"
            }]
        }
    }
}
</script>

<style lang="scss">
ul {
    list-style: none;
}
</style>
