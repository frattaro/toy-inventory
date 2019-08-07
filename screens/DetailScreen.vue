<script>
  export default {
    name: "DetailScreen",
    props: {
      navigation: {
        type: Object
      }
    },
    data: function() {
      return {
        message: "Detail Screen"
      };
    },
    methods: {
      handleLetGoBtnPress: function () {
        this.navigation.navigate("Welcome");
      }
    }
  };
</script>

<template>
  <view class="container">
    <text class="text-color-primary">{{message}}</text>
    <button
      :on-press="handleLetGoBtnPress"
      title="Go To Welcome Screen"
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
