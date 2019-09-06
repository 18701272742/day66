<template>
  <div class="shou">
      <div class="swiper-container">
        <div class="swiper-wrapper">
          <div class="swiper-slide">slider1</div>
          <div class="swiper-slide">slider2</div>
          <div class="swiper-slide">slider3</div>
        </div>
      </div>
      <div class="lie">
        <dl v-for="(item,ind) in list" :key=(ind)>
          <dt>{{item.title}}</dt>
          <dd>{{item.con}}</dd>
        </dl>
      </div>
  </div>
</template>
<script>
import Swiper from "swiper";
import "../../node_modules/swiper/dist/css/swiper.min.css";

var mySwiper = new Swiper('.swiper-container', {
	autoplay: true,//可选选项，自动滑动
})

export default {
  props: {},
  components: {
    
  },
  data() {
    return {
      list:[{
        id:0,
        title:"第1图",
        con:"第1"
      },{
        id:1,
        title:"第2图",
        con:"第2"
      },{
        id:2,
        title:"第3图",
        con:"第3"
      },{
        id:3,
        title:"第4图",
        con:"第4"
      },{
        id:4,
        title:"第5图",
        con:"第5"
      },{
        id:5,
        title:"第6图",
        con:"第6"
      },{
        id:6,
        title:"第7图",
        con:"第7"
      },{
        id:7,
        title:"第8图",
        con:"第8"
      }]
    };
  },
  computed: {},
  methods: {
   swiper(){
     console.log("1");
   }
  },
  created() {},
  mounted() {},
};
</script>
<style scoped lang="">
</style>
