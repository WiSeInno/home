<template>
  <div class='items'>
    <el-row :gutter="100">
      <el-col :span='12'>
        <h1 class="title">Events</h1>
        <p id="txt1"class="text info">
          WiseInno has been found back at 2016 in order to help the organisation of various workshops and schools organised by the <a href="http://electronics.physics.auth.gr/">Sector of Electronics of the Physics Dept. AUTh</a> and sponsored by <a href="http://ieee-cas.org/">IEEE CAS Society</a>. WiSe School 2016 brought us ( <i>Dimitris, Markella, Kosmas, Despina </i>) together and our passion motivated us to organise WiSeIoT, IoT-BB School 2017 and Biolelectronics! It was a great experience and you <strong>should </strong>, definitely, try it!
          <br>
          <a href='http://wiseinno-events.herokuapp.com'><el-button type="primary" plain class="btn">Past Events</el-button></a>
        </p>
      </el-col>
      <el-col :span='12'>
        <img src="../assets/events.svg" class="svg">
      </el-col>
    </el-row>
    <el-row :gutter="100">
      <el-col id="block2" :span='12'>
        <img src="../assets/post.svg" class="svg">
      </el-col>
      <el-col :span='12'>
        <h1 class="title">Blogging</h1>
        <p id="txt2" class="text">
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
    margin-top: 100px;
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
    text-align: justify;
    }
  
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
