<template>
  <el-row>
    <el-col :span='12'>
      <img src="../assets/post.svg" class="svg">
    </el-col>
    <el-col :span='12'>
      <h1 class="title">Blogging</h1>
      <p class="text" type='warning'>
        Bloggin is our passion and we are trying to grow along with it
      </p>
    </el-col>
  </el-row>
</template>

<script>
export default {
  name: 'items',
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Gaegu|Patua+One');
  .svg{
    width: 90%;
  }
  .title{
    font-size: 44px;
    text-align: center;
    text-decoration: underline;
    font-family: 'Gaegu', cursive;
  }
  p.text{
    font-size: 18px;
    text-align: center;
    font-family: 'Patua One', cursive;
    color:  #C89EC4;
  }
</style>
