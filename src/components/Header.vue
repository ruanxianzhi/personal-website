<template>
  <div id="header">
    <v-container pa-0 fluid fill-height grid-list-xl>
      <v-row no-gutters>
        <v-col cols="12" md="4">
          <transition>
            <v-avatar
              class="grey lighten-4"
              v-if="isAvatarVisible"
              :size="avatarSize"
            >
              <img src="@/assets/olivia.png" />
            </v-avatar>
          </transition>
        </v-col>
        <v-col cols="12" md="8">
          <v-card id="jumbo-card" flat dark>
            <h1 class="display-1 mb-3">Xianzhi Olivia Ruan</h1>
            <h1 class="display-2 mb-3">Full Stack Software Engineer</h1>
            <h2>
              A Technology Enthusiast
              <em style="display:block;font-size:1rem;"
                >- React.js, Vue.js, Vuetify, Bootstrap, Typescript, GraphQL,
                MongoDB, ElasticSearch, etc.</em
              >
            </h2>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Header extends Vue {
  avatarSize = 300;
  isAvatarVisible = false;

  mounted() {
    this.isAvatarVisible = true;
  }
}
</script>

<style scoped>
#header {
  height: auto;
  color: white;
  background-color: black;
}

#jumbo-card {
  background-color: rgba(0, 0, 0, 0);
}

.v-enter-active,
.v-leave-active {
  transition: opacity 0.5s;
}

.v-enter,
.v-leave-to {
  opacity: 0;
}
</style>
