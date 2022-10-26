<template>
  <v-app>
    <v-main>
      <FileBrowser
          :axiosConfig="myhost"
          :maxUploadFileSize="5242880"
          :maxUploadFilesCount="20000"
      />
    </v-main>
  </v-app>
</template>
<script type="text/javascript">
export default {
  name: 'App'
}
</script>

<script setup>
// import HelloWorld from './components/HelloWorld.vue'
import FileBrowser from "vuetify-file-browser";

const myhost = {baseURL:'http://localhost:8070'};

</script>

