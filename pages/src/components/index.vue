<template>
  <div class="content">
    <img src alt />
    <div class="btn">
      <div v-for="(option,index) in options" :key="index">
        <btn :option="option" />
      </div>
      <mt-button type="primary" @click="go(3)">加入会议</mt-button>
    </div>
  </div>
</template>

<script>
import btn from "./btn.vue";
export default {
  name: "index",
  components: {
    btn
  },
  data() {
    return {
      options: [{title:'9.9',content:'家庭清洁1次'},{title:'99',content:'家庭清洁10次'}]
    };
  },
  methods: {
    go() {}
  }
};
</script>


<style lang="less" scoped>
.btn {
  display: flex;
  flex-direction: column;
  button {
    margin: 5px;
  }
}
</style> 
