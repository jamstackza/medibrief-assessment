<template lang="html">
    <div style="text-align: left; padding-left: 10px;">
        <sui-accordion exclusive>
            <sui-accordion-title active>
                <sui-icon name="dropdown" />
                My Documents
            </sui-accordion-title>
            <sui-accordion-content active>
                <p>Document</p>
            </sui-accordion-content>
            <sui-accordion-title>
                <sui-icon name="dropdown" />
                Shared Documents
            </sui-accordion-title>
            <sui-accordion-content>
                <p>Document</p>
            </sui-accordion-content>
        </sui-accordion>
    </div>
</template>

<script>
    export default {
        name: 'FileTree'
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
