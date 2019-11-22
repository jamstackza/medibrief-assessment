<template>
    <div class="fullWidth">
        <sui-tab
                :menu="{ secondary: true }"
        >
            <sui-tab-pane title="View Document" :attached="false">
                <iframe class="pdfViewer" src="https://rossta.net/vue-pdfjs-demo" frameborder="0" allowfullscreen></iframe>
            </sui-tab-pane>
            <sui-tab-pane title="Comments" :attached="false" style="text-align: left;">
                <FileComment />
            </sui-tab-pane>
            <sui-tab-pane title="Upload New Document" :attached="false">
                <FileUpload />
            </sui-tab-pane>
        </sui-tab>
    </div>
</template>

<script>
    import FileUpload from "./FileUpload";
    import FileComment from "./FileComment";
    export default {
        name: "DocViewerLayout",
        components: {
            FileUpload,
            FileComment
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.fullWidth {
    width: 100%;
    display: flex;
}
    .pdfViewer {
        display: flex;
        height: 70vh;
        width: 60vw;
        flex-direction: column;
        align-items: center;
    }
</style>
