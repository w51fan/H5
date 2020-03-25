<template>
  <div class="equityListPage">
    <div>尊敬的：{{userName}}</div>
    <div>您的权益如下：</div>
    <div class="equityList">
      <div v-for="(option,index) in options" :key="index">
        <equityBtn :option="option" />
      </div>
    </div>
  </div>
</template>

<script>
import equityBtn from "./equityBtn.vue";
export default {
  name: "equityList",
  components: {
    equityBtn
  },
  data() {
    return {
      userName: "XXX",
      options: [
        { title: "1张", content: "家庭清洁1次" },
        { title: "10张", content: "家庭清洁10次" },
        { title: "10元", content: "家庭清洁1张" }
      ]
    };
  },
  methods: {}
};
</script>


<style lang="less" scoped>
.equityListPage {
  // display: flex;
  .equityList {
  }
}
</style> 
