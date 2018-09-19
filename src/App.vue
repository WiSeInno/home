<template>
  <div id="app">
    <el-container>
      <el-header height='400px'>
          <hero></hero>
      </el-header>
      <el-main>
        <el-row type="flex" justify="center">
          <el-col :xs="20" :sm="18" :md="14" :lg="14" :xl="14">
            <items></items>
          </el-col>
        </el-row>
        <el-row type="flex" class="row-bg" justify="center">
          <el-col :span='18'>
            <card></card>
          </el-col>
        </el-row>
      </el-main>
      <el-footer :xs="24" :sm="18" :md="14" :lg="14" :xl="14">
        <letstalk></letstalk>
      </el-footer>
    </el-container> 
  </div>
</template>

<script>
import navbar from '@/components/Navbar';
import card  from '@/components/card';
import hero from'@/components/hero';
import items from '@/components/items';
import letstalk from '@/components/letstalk'

export default {
  name: 'App',
  components: {
    navbar, card, hero, items, card, letstalk
  }
}
</script>

<style @lang='scss'>
body{
  background-color: #fffff2;
  height: 100%;
  width: 100%;
  padding: 0;
  overflow-x: hidden;
}
</style>
