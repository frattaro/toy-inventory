<script>
  export default {
    name: "WelcomeScreen",
    props: {
      navigation: {
        type: Object
      }
    },
    data: function() {
      return {
        message: "Welcome Screen"
      };
    },
    methods: {
      handleLetGoBtnPress: function () {
        this.navigation.navigate("Detail");
      }
    }
  };
</script>

<template>
  <view class="container">
    <text class="text-color-primary">{{message}}</text>
    <button
      :on-press="handleLetGoBtnPress"
      title="Go To Detail Screen"
      color="#841584"
      accessibility-label="Learn more about this purple button" />
  </view>
</template>

<style>
  .container {
    background-color: white;
    align-items: center;
    justify-content: center;
    flex: 1;
  }

  .text-color-primary {
    color: blue;
  }
</style>
