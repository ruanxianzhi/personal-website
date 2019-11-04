<template>
  <v-toolbar class="ma-0 pa-0">
    <v-toolbar-title v-html="msg" />
    <v-spacer />

    <v-btn icon href="https://www.linkedin.com/in/xianzhi-olivia-ruan">
      <v-icon color="grey darken-4">mdi-linkedin</v-icon>
    </v-btn>

    <v-btn icon href="https://github.com/ruanxianzhi">
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
