<template>
  <div id="hero">
    <h1 class="title">WiSeInno</h1>
    <h2 class="subtitle">A Team Devoted to Innovation</h2>
    <div class="icon_bar">
      <a>
        <el-button type='primary' icon='el-icon-search' circle></el-button>
      </a>
      <a>
        <el-button type='primary' icon='el-icon-edit' circle></el-button>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'hero',
}
</script>

<style lang="scss" scoped>
  #hero{
    background-color: #008ed6;
    //height: 100%;
    text-align: center;
    .title{
      padding-top: 50px;
      font-family: Menlo;
      font-size: 52px;
      color: #fffff2;
    }
    .subtitle{
      font-family: Menlo;
      font-size: 22px;
      color: whitesmoke;
    }
    .icon_bar{
      i{
        font-size: 2rem;
      }
      color: #fffff2;
      
      padding-bottom: 50px;
    }
  }
</style>
