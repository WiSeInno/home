<template>
  <div class='talk'>
    <el-row>
      <el-col :span='24'>
        <h1 class="title">Let's Talk</h1>
        <p class="text">We are really open to conversation and we love great ideas. So if you have anything to suggest or even if you think we can be of any help do not hesitate to contact as through WiSeInno or in person.</p>
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
