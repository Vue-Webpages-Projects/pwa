<template>
    <div>
         

        poig
    
    
    </div>
</template>

<script>
export default {
    name: 'Movie',
    props: {
        movie: Object
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
