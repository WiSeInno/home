<template>
  <div class='talk'>
    <el-row>
      <el-col :span='24'>
        <h1 class="title">Let's Talk</h1>
        <p class="text">Our greatest dream was the creation of a blog and now it's the time to bring this dream into life! We want to be a step for everyone to share their story, their passion, and the way through their persuing their dreams. We believe everything is possible so If you think you got something to share in order to help  more people to thrive you are more than welcome. Just drop us some words</p>
        <el-row type="flex" justify="center">
          <el-col :span='8'>
            <h2 class="name">WiSeInno</h2>
            <img class='logo' v-bind:src='require("@/assets/logo.png")'>
            <ul>
              <li>
                <i class="fab fa-twitter fa-2x twitter"></i>
              </li>
              <li>
                <i class="fas fa-envelope fa-2x "></i>
              </li>
            </ul>
          </el-col>
          <el-col :span='8'>
            <h2 class="name">Markella</h2>
            <img class='logo' v-bind:src='require("@/assets/logo.png")'>
            <ul>
              <li>
                <i class="fab fa-twitter fa-2x twitter"></i>
              </li>
              <li>
                <i class="fas fa-envelope fa-2x"></i>
              </li>
            </ul>
          </el-col>
          <el-col :span='8'>
            <h2 class="name">Dimitris</h2>
            <img class='logo' v-bind:src='require("@/assets/logo.png")'>
            <ul>
              <li>
                <i class="fab fa-twitter fa-2x twitter"></i>
              </li>
              <li>
                <i class="fas fa-envelope fa-2x"></i>
              </li>
            </ul>
          </el-col>
        </el-row>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'letstalk',
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
    ul{
      list-style-type: none;
      li{
        float: left;
        margin-left: 10px;
      }
    }
    .logo{
      width: 20%;
      border-radius: 50%;
      padding: 10px;
      background-color: white;
    }
    .twitter{
      color: #1da1f2;
    }
</style>
