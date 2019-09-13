<template>
    <b-container>
        <b-row>
            <b-col class="text-center" cols="12">
                <!-- <h2>Participantes</h2> -->
            </b-col>
        </b-row>

        <b-row align-v="center" > 
            <Single v-for="new_info in news"
            v-bind:key="new_info.id"
            v-bind:new_info="new_info"
            ></Single>
        </b-row>

        <b-row align-h="end" style="padding-top: 20px">
            <b-col sm="12" md="2">
                <router-link to="/" class="btn btn-block btn-color">
                    Ver todas >>
                </router-link>
            </b-col>
        </b-row>

    </b-container>
</template>

<script>
import Single from './Single.vue' 

export default {
    name: 'Group',
    components: {Single},
    data() {
        return {
            news: [
                {
                    id: 1,
                    image: require('../assets/logo.png'),
                    date: '00/00/0000',
                    title: 'Lorem ipsum',
                    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus, architecto voluptate? Reiciendis corporis officia esse nesciunt aliquam ullam sed cupiditate magni voluptas laborum, sapiente quidem cumque fugiat numquam repellat asperiores nobis eaque aliquid, adipisci architecto in et fugit? Itaque, id!”.'
                },
                {
                    id: 2,
                    image: require('../assets/logo.png'),                    
                    date: '00/00/0000',
                    title: 'Lorem ipsum',
                    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus, architecto voluptate? Reiciendis corporis officia esse nesciunt aliquam ullam sed cupiditate magni voluptas laborum, sapiente quidem cumque fugiat numquam repellat asperiores nobis eaque aliquid, adipisci architecto in et fugit? Itaque, id!'
                },
                {
                    id: 3,
                    image: require('../assets/logo.png'),                    
                    date: '00/00/0000',
                    title: 'Lorem ipsum',
                    content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus, architecto voluptate? Reiciendis corporis officia esse nesciunt aliquam ullam sed cupiditate magni voluptas laborum, sapiente quidem cumque fugiat numquam repellat asperiores nobis eaque aliquid, adipisci architecto in et fugit? Itaque, id!'
                }
            ]
        }
    }
}
</script>

<style scoped>
    .btn-color {
        background-color: #fd8b3c;
        border-color: #fd8b3c;
        transition: .5s;
        color: aliceblue;
    }
    .btn-color:hover {
        background-color: #fd885c;
        transition: .5s;
        color: darkblue;
    }
</style>