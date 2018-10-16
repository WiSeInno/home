<template>
  <div class='items'>
    <el-row :gutter="100">
      <el-col :xs="24" :sm="24" :md="12" :lg="12" :xl="12">
        <h1 class="title">Events</h1>
        <p id="txt1"class="text info">
          WiseInno was founded in 2016 in order to help organize a variety of workshops and schools held by the <a href="http://electronics.physics.auth.gr/">Sector of Electronics of the Physics Dept. AUTh</a>  and sponsored by <a href="http://ieee-cas.org/">IEEE CAS Society</a>. WiSe School 2016 has brought us, WiSeInno team, together and our passion motivated us to organise WiSeIoT, IoT-BB School 2017 and Biolelectronics! It was a great experience and we recommend that you <strong>should </strong>, definitely, try it!
          <br>
          <a href='http://wiseinno-events.herokuapp.com'><el-button type="primary" plain class="btn">Past Events</el-button></a>
        </p>
      </el-col>
      <el-col class="hidden-sm-and-down" :md="12" :lg="12" :xl="12">
        <img src="../assets/events.svg" class="svg">
      </el-col>
    </el-row>
    <el-row :gutter="100">
      <el-col id="block2" class="hidden-sm-and-down" :md="12" :lg="12" :xl="12">
        <img src="../assets/post.svg" class="svg">
      </el-col>
      <el-col :xs="24" :sm="24" :md="12" :lg="12" :xl="12">
        <h1 class="title">Blogging</h1>
        <p id="txt2" class="text">
          Our greatest dream was the creation of a blog and now it's time to bring this dream into life! We would love this blog to be a place for each and everyone to share their stories, their passion and to be a step on persuing their dreams. We believe everything is possible, so... If you think you got something to share in order to help  other people thrive , just drop us some words!
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
.items{
  margin-bottom: 40px;
}
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
