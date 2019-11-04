<template>
  <div class="home">
    <HelloWorld msg="Welcome to Olivia's home page" />
    <Header />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Header from "@/components/Header.vue";

export default {
  name: "home",
  components: { HelloWorld, Header }
};
</script>
