<template>
  <div id="app">
    <Slider
      animation="fade"
      v-model="sliderValue"
      :duration="5000"
      :speed="1000"
    >
      <SliderItem
        v-for="item  in list"
        :key="item.imageId"
        @click="changeIndex(1);"
        :style="i"
      >
      <img :src="item.myImage">
        <!-- <p style="line-height: 280px; font-size: 5rem; text-align: center;">
          Page{{ index + 1 }}
        </p> -->
      </SliderItem>
    </Slider>
  </div>
</template>

<script>
import { Slider, SliderItem } from "vue-easy-slider";

export default {
  name: "App",
  components: {
    Slider,
    SliderItem
  },
  data() {
    return {
      list: [
          {imgId:7, myImage:'/pawpaw.jpg'},
          {imgId:8, myImage:'/kolanut.jpg'},
          {imgId:9, myImage:'/guava.jpg'},
          {imgId:10, myImage:'/strawberry.jpg'},
          {imgId:1, myImage:'/apple.jpg'},
          {imgId:2, myImage:'pineapple.jpg'},
          {imgId:3, myImage:'/cucumber.jpg'},
          {imgId:4, myImage:'/greenBeans.jpg'},
          {imgId:5, myImage:'/watermelon.jpg'},
          {imgId:6, myImage:'/cocoyam.jpg'}
      ],
      sliderValue: 2
    };
  },
  methods: {
    changeIndex(index) {
      this.sliderValue = index;
    }
  }/* ,
  mounted() {
    setTimeout(
      () =>
        (this.list = [
          {
            backgroundColor: "green",
            width: "100%",
            height: "100%"
          },
          {
            backgroundColor: "#eee",
            width: "100%",
            height: "100%"
          },
          {
            backgroundColor: "#f44336",
            width: "100%",
            height: "100%"
          },
          {
            backgroundColor: "#eee",
            width: "100%",
            height: "100%"
          }
        ]),
      1000
    );
  } */
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

p {
  margin: 0;
}
</style>
