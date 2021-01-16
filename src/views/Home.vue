<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" height="100" style="margin-top: 50px;"/>
    <HelloWorld />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src

@Options({
  components: {
    HelloWorld
  }
})
export default class Home extends Vue {}
</script>
