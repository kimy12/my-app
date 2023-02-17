<template>

<!-- header colour: #145de7 -->
  <div class="nav-container">
    <!-- <v-app-bar-nav-icon @click="drawer = !drawer" />
    <v-navigation-drawer v-model="drawer">
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h6"> Dashboard </v-list-item-title>
          <v-list-item-subtitle> Navigation drawers</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
      <v-divider></v-divider>
      <v-list dense nav>
        <v-list-item v-for="item in items" :key="item.title" link>
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer> -->
    <v-toolbar title="my weather" extended>
      <v-app-bar-title class="title">my weather</v-app-bar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xs-only">
        <v-btn
          flat
          v-for="item in items"
          :key="item.title"
          >
          <v-icon left dark>{{ item.icon }}</v-icon>
          {{ item.title }}
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
  </div>
</template>

<script>
export default {
  data(){
    return {
      drawer : false,
      items: [
        { title: 'dayily note', icon: 'fa-solid fa-book' },
      ],
      rail: true,
    }
  }

}
</script>

<style scoped>
.title {
  color: #145de7;
}
</style>