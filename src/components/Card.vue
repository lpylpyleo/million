<template>
    <div class="card">
        <img :src="img" class="card-img-top" alt="">
        <div class="card-body">
            <div class="card-title">{{title}}</div>
            <div class="card-text">{{text}}</div>
        </div>
        <div class="card-footer">{{footer}}</div>
    </div>
</template>

<script>
    export default {
        name: 'HelloWorld',
        props: ['img','title','text','footer']
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card{
    margin-left: 50px;
    margin-right: 50px;
}
</style>
