<template>
  <div class='items'>
    <el-row>
      <el-col :span='12'>
        <h1 class="title">Events</h1>
        <p class="text info">
          Events are what get us started. We organized a lot, all of them supported by <a href="http://ieee-cas.org/">IEEE CAS Society</a> and <a href="http://electronics.physics.auth.gr/">Sector of Electronics of the Physics Dept. AUTh</a>. It was a great experience, you <strong>should</strong> try it! 
          <br>
          <a href='http://wiseinno-events.herokuapp.com'><el-button type="primary" plain class="btn">Past Events</el-button></a>
        </p>
      </el-col>
      <el-col :span='12'>
        <img src="../assets/events.svg" class="svg">
      </el-col>
    </el-row>
    <el-row>
      <el-col :span='12'>
        <img src="../assets/post.svg" class="svg">
      </el-col>
      <el-col :span='12'>
        <h1 class="title">Blogging</h1>
        <p class="text">
          Our blog is a initiative we dreamed a lot time ago and now trying to make it real. We want to be a step for everyone to share their story, their passion, and the way through their persuing their dreams. We believe everything is possible so  If you think you got something to share in order to help us inspire more people to thrive you are more that welcome. Just drop us some words  😀.
          <br>
          <a href='https://blog.wiseinno.tech'><el-button type="warning" plain class="btn">Visit Blog</el-button></a>
        </p>
      </el-col>
    </el-row>
  </div>
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
    color:  #C89EC4;}
  
    p.text.info{
      color: #84B1ED;
      a{
        color: inherit;
        font-weight: 700;
      }
    }
    .btn{
      margin-top: 15px;
    }
</style>
