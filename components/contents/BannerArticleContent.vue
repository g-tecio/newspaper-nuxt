<template>
    <div class="rigth-border-wrapper">
        <b-row>
            <b-col md="4">
                <b-link :key="config.id" :to="{ name: 'article-id', params: { id: config.id, title: config.title, content: config.content, img: config.img } }">
                    <b-img :src="config.img_url" fluid alt="Responsive image" />
                </b-link>
            </b-col>
            <b-col md="8">
                <h6>{{ config.title }}</h6>
                <p>{{ config.content }}</p>
            </b-col>
        </b-row>  
    </div>
</template>

<script>

export default {
    props:['config'],
}
</script>

<style>
    @media screen and (max-width: 768px){
    }

    .rigth-border-wrapper {
        padding-top: 10px;
    }
</style>



