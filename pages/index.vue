<template>
  <HelloWorld />
</template>

<script lang="ts">
import { Component, Vue } from "nuxt-property-decorator";
import HelloWorld from "~/components/HelloWorld.vue";

@Component({
  components: {
    HelloWorld
  }
})
export default class Home extends Vue {
  created() {
    console.log("created");
  }

  asyncData() {
    console.log("asyncData");
  }

  fetch() {
    console.log("fetch");
  }
}
</script>
