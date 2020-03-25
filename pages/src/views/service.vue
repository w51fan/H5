<template>
  <div class="servicePage">
    <mt-navbar v-model="active">
      <mt-tab-item id="1">9.9</mt-tab-item>
      <mt-tab-item id="2">99</mt-tab-item>
    </mt-navbar>
    <mt-tab-container v-model="active">
      <mt-tab-container-item id="1">
        <div class="itemContent">9.9</div>
      </mt-tab-container-item>
      <mt-tab-container-item id="2">
        <div class="itemContent">99</div>
      </mt-tab-container-item>
    </mt-tab-container>
  </div>
</template>

<script>
// import btn from "./btn.vue";
export default {
  name: "service",
  components: {
    // btn
  },
  data() {
    return {
      selected: "1",
      active: "1",
      title1: "tab-container 1",
      title2: "tab-container 2",
      title3: "tab-container 3"
    };
  },
  methods: {}
};
</script>


<style lang="less" scoped>
.servicePage {
  // display: flex;
  .itemContent{
    margin: 10px;
  }
}
</style> 
