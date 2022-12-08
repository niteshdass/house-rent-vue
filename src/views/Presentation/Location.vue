<template>
    <GoogleMap api-key="AIzaSyDFBLiV8Took-03KgKIkP8eYwM66jqTfqI" style="width: 100%; height: 500px" :center="center" :zoom="15">
      <Marker :options="{ position: center }" />
    </GoogleMap>
  </template>
  
  <script>
  import { defineComponent } from "vue";
  import { GoogleMap, Marker } from "vue3-google-map";
  
  export default defineComponent({
    components: { GoogleMap, Marker },
    setup() {
      const center = { lat: 24.8949, lng: 91.8687 };
  
      return { center };
    },
  });
  </script>