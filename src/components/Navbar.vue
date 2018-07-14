<template>
<div id="navbar">
  <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
  <el-menu-item index="1">
    <a href="/">
      <img src="../assets/logo.png" width="10%">
    </a>
  </el-menu-item>
  
  <el-menu-item index="2">
    <a href='#team'>
      About
    </a>
  </el-menu-item>
  <el-menu-item index="3">
    <a href="#team">
     Team
    </a>
  </el-menu-item>
</el-menu>
</div>
</template>

<script>
export default {
  name: 'navbar',
  data () {
    return {
      activeIndex: '1',
      activeIndex2: '1'
    }
  },
  methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss' scoped>
#navbar{
  margin: -10px -20px 0 -20px;
}

</style>
