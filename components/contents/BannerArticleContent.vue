<template>
    <div>
        <b-row>
            <b-col md="4">
                <b-img :src="config.img" fluid alt="Responsive image" />
            </b-col>
            <b-col md="8">
                <h6>{{ config.title }}</h6>
                <p>{{ config.description }}</p>
            </b-col>
        </b-row>  
    </div>
</template>

<script>

export default {
    props:['config'],
}
</script>


