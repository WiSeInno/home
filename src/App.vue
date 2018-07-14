<template>
  <div id="app">
    <navbar></navbar>
    <el-container>
      <el-header height='400px'>
          <hero></hero>
      </el-header>
      <el-main>
        <el-row type="flex" justify="center">
          <el-col :span='18'>
            <items></items>
            <router-view/>
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

export default {
  name: 'App',
  components: {
    navbar, card, my_footer, hero, items
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
