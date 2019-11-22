<template lang="html">
    <div class="centerx">
        <vs-upload action="https://jsonplaceholder.typicode.com/posts/" @on-success="successUpload" />
    </div>
</template>

<script>
    export default {
        name: 'FileUpload',
        methods:{
            successUpload(){
                this.$vs.notify({color:'success',title:'Upload Success',text:'Lorem ipsum dolor sit amet, consectetur'})
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
