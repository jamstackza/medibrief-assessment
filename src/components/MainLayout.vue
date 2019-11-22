<template>
  <vs-row vs-w="12">
    <!-- start left column -->
    <vs-col vs-type="flex" vs-justify="flex-start" vs-align="flex-start" vs-lg="2" vs-sm="4" vs-xs="12" >
    <div>
      <FileTree />
    </div>
    </vs-col>
    <!-- start middle column -->
    <vs-col vs-type="flex" vs-justify="center" vs-align="flex-start" vs-lg="8" vs-sm="4" vs-xs="12">
      <DocViewerLayout />
    </vs-col>
    <!-- start right column -->
    <vs-col vs-type="flex" vs-justify="center" vs-align="flex-start" vs-lg="2" vs-sm="4" vs-xs="12">
    right column
    </vs-col>
  </vs-row>
</template>

<script>
  import DocViewerLayout from './DocViewerLayout.vue'
  import FileTree from "./FileTree";

export default {
  name: 'MainLayout',
  components: {
    DocViewerLayout,
    FileTree
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
