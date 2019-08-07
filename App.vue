<script>
  import { StackNavigator } from "vue-native-router";
  import WelcomeScreen from "./screens/WelcomeScreen.vue";
  import DetailScreen from "./screens/DetailScreen.vue";
  const AppNavigation = StackNavigator(
    {
      Welcome: WelcomeScreen,
      Detail: DetailScreen
    },
    {
      initialRouteName: 'Welcome',
    }
  );
  export default {
    components: { AppNavigation }
  }
</script>

<template>
  <app-navigation></app-navigation>
</template>
