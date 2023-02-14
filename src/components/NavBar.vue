<template>
  <div class="nav-container">
    <!-- <v-toolbar title="Application">
      <v-btn variant="plain">
        Button
      </v-btn>
    </v-toolbar> -->
    <v-navigation-drawer
        v-model="drawer"
        :rail="rail"
        permanent
        @click="rail = false"
      >
    <v-app-bar-nav-icon></v-app-bar-nav-icon>
    <v-app-bar-title>Application</v-app-bar-title>
    <v-list density="compact" nav>
      <v-list-item prepend-icon="fa-solid fa-house" title="Home" value="home"></v-list-item>
      <!-- <v-list-item prepend-icon="mdi-home-city" title="Home" value="home"></v-list-item> -->
      <v-list-item prepend-icon="mdi-account" title="My Account" value="account"></v-list-item>
      <v-list-item prepend-icon="mdi-account-group-outline" title="Users" value="users"></v-list-item>
    </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data(){
    return {
      drawer : true,
      items: [
        { title: 'Home', icon: 'mdi-home-city' },
        { title: 'My Account', icon: 'mdi-account' },
        { title: 'Users', icon: 'mdi-account-group-outline' },
      ],
      rail: true,
    }
  }

}
</script>

<style>

</style>