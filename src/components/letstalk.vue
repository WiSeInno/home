<template>
  <div class='talk'>
    <el-row :gutter="150">
      <el-col :span='24'>
        <h1 class="title">Let's Talk</h1>
        <p class="text">We love new ideas! So if you want to share your story, article or make any kind of suggestion we are more than open to have a conversation! You can get in touch with us either via WiSeInno or in person!</p>
        <el-row type="flex" justify="center" gutter="50">
          <el-col :span='5' v-for="p in content" :key="o">
            <h2 class="name">{{p.name}}</h2>
            <img class='logo' v-bind:src='p.pic'>
            <ul>
              <li>
                <a v-bind:href="'https://twitter.com/'+p.twitter">
                  <i class="fab fa-twitter fa-2x twitter"></i>
                </a>  
              </li>
              <li>
                <a v-bind:href=" 'mailto:'+p.mail">
                  <i class="fas fa-envelope fa-2x "></i>
                </a>
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
  data () {
    return {
      content: [
        {name: 'WiSeInno', pic: require("@/assets/logo.png"), mail: 'info@wiseinno.tech', twitter: 'wise_inno'},
        {name: 'Markella', pic: require("@/assets/avatar-female.jpg"), mail: 'markella@wiseinno.tech', twitter: 'frmarliakou'},
        {name: 'Dimitris', pic: require("@/assets/av-male.jpg"), mail: 'dstrants@wiseinno.tech', twitter: 'dstrants'},
      ]
    }
  },
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
    color:  #C89EC4;
    width: 50%;
    margin: auto;}
  
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
      padding-left: 0;
       li{
        float: left;
        margin-left: 10px;
        a{
          color: inherit;
        }
      }
    }
    .logo{
      width: 25%;
      margin-left: 7%;
    }
    .twitter{
      color: #1da1f2;
    }
    .talk{
      background-color: #f2f2f2;
      padding: 0px 100px 50px 100px;
      margin-bottom: 20px;
    }
</style>
