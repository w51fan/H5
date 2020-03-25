<template>
  <div class="btnCntent">
    <div class="title">{{option.title}}</div>
    <div class="content">{{option.content}}</div>
    <div class="more">
      <i></i>
      <div class="text">详情</div>
      <div>
        <img src="../assets/more.png" width="12" height="12" alt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "btn",
  props:['option'],
  data() {
    return {};
  },
  methods: {}
};
</script>


<style lang="less" scoped>
.btnCntent {
  display: flex;
  color: #656b79;
  background-color: #f6f8fa;
  box-shadow: 0 0 1px #b8bbbf;
  margin: 5px;
  appearance: none;
  border-radius: 4px;
  border: 0;
  box-sizing: border-box;
  color: inherit;
  font-size: 18px;
  height: 40px;
  outline: 0;
  overflow: hidden;
  position: relative;
  text-align: center;
  line-height: 40px;
  .title {
    width: 40%;
  }
  .content {
    width: 40%;
  }
  .more {
    width: 20%;
    display: flex;
    i {
      display: inline-block;
      height: 20px;
      width: 0;
      border: 1px solid #d9d9d9;
      vertical-align: top;
      margin-top: 10px;
      margin: 10px 0;
    }
    .text{
      margin: 0 0 0 10px;
    }
  }
}
</style> 
