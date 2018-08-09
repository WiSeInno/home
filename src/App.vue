<template>
  <div id="app">
    <navbar></navbar>
    <el-container>
      <el-header height='400px'>
          <hero></hero>
      </el-header>
      <el-main>
        <el-row type="flex" justify="center">
          <el-col :span='14'>
            <items></items>
            <router-view/>
          </el-col>
        </el-row>
        <el-row type="flex" class="row-bg" justify="center">
          <el-col :span='18'>
            <card></card>
          </el-col>
        </el-row>
        <el-row type="flex" justify="center">
          <el-col :span='18'>
            <letstalk></letstalk>
          </el-col>
        </el-row>
      </el-main>
    </el-container>
    <my_footer></my_footer>
  </div>
</template>

<script>
import navbar from '@/components/Navbar';
import card  from '@/components/card';
import my_footer from '@/components/footer';
import hero from'@/components/hero';
import items from '@/components/items';
import letstalk from '@/components/letstalk'

export default {
  name: 'App',
  components: {
    navbar, card, my_footer, hero, items, card, letstalk
  }
}
</script>

<style @lang='scss'>
body{
  background-color: #fffff2;
  height: 100%;
  width: 100%;
  padding: 0;
}
</style>
