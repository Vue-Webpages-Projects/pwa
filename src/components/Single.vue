<template>
    <b-col sm="12" md="4" lg="4">
        <router-link to="/movie" v-on:click="movieSearch">
            <b-card no-body class="overflow-hidden" style="padding-top: 50px; border: none; padding-bottom: 20px; border-bottom: 3px dotted #fd8b3c">
                <b-row no-gutters align-v="center">
                    <b-col md="3">
                        <b-card-img v-bind:src="new_info.image" class="rounded-0 imagem"></b-card-img>
                    </b-col>
                    <b-col md="9">
                        <b-card-body style="padding-top: 0; text-align: left">
                            <small style="padding:0; margin: 0;font-weight: bold; color: darkblue; font-size: 15px"> {{new_info.date}} </small>
                            <h4 class="title"> {{new_info.title}} </h4>
                            <b-card-text class="content">
                                {{new_info.content}}
                            </b-card-text>
                        </b-card-body>
                    </b-col>
                </b-row>
            </b-card>
        </router-link>
    </b-col>
</template>

<script>
export default {
    name: 'Single',
    props: {
        new_info: Object
    },
    data () {
        return {
            movies: [
                {
                    id: 1,
                    description: '' 
                }  
            ]
        }
    },
    methods: {
        movieSearch () {
            this.movieId = this.new_info.id;
            alert(JSON.stringify(this.movie.id))
        }
    }
}
</script>








<style scoped>
.content {
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 4;  /* Number of lines displayed before it truncate */
    overflow: hidden;
    text-align: justify;
    line-height: 1rem;
    font-size: 14px;
}

.title {
    font-size: 15px!important;
    color: #fd8b3c;
    font-weight: bold;
}
.imagem {
    width: 35%;
}

a:hover {
    text-decoration-line: none;
}

@media (min-width: 576px) { 
    .imagem {
        width: 100%;
    } 
    
 }
</style>
