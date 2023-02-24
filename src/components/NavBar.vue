<template>

  <v-card
    color="grey-lighten-4"
    flat
    height="200px"
    rounded="0"
  >
    <v-toolbar title="my weather" flat outlined>
      <v-toolbar-title class="title">
        my weather :)
      </v-toolbar-title>
      <v-spacer></v-spacer>
        <v-btn
          class="align-center"
          text
          v-for="item in items"
          :key="item.title"
          >
          <v-icon class="align-start">{{ item.icon }}</v-icon>
          <span>{{ item.title }}</span>
        </v-btn>
    </v-toolbar>
  </v-card>
</template>

<script>
export default {
  data(){
    return {
      drawer : false,
      items: [
        { title: 'dayily', icon: 'fa-solid fa-book' },
        { title: 'weather', icon: 'fa-solid fa-cloud' }
      ],
      rail: true,
    }
  }

}
</script>

<style scoped>
.title {
  color: #145de7;
  font-weight: 900;
}
.v-app-bar-title__content {
  width: 200px;
}
</style>