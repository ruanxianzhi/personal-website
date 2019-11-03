<template>
  <v-toolbar dark>
    <v-toolbar-title v-html="msg" />
    <v-spacer />

    <v-btn icon href="https://www.linkedin.com/in/xianzhi-olivia-ruan" right>
      <v-icon color="grey darken-4">mdi-linkedin</v-icon>
    </v-btn>

    <v-btn icon href="https://github.com/ruanxianzhi" right>
      <v-icon color="grey darken-4">mdi-github-circle</v-icon>
    </v-btn>
  </v-toolbar>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>
