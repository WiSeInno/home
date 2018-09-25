<template>
  <div class='talk'>
    <el-row :gutter="15">
      <el-col type="flex" justify="center" :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <h1 class="title">Let's Talk</h1>
        <p class="text">We love new ideas! So if you want to share your story, article or to make any kind of suggestion we are more than happy to hear from you! You can get in touch with us either via WiSeInno social media accounts or by reaching us on our personal social accounts!</p>
        <el-row type="flex" justify="center" gutter="50">
          <el-col :xs="8" :sm="8" :md="8" :lg="8" :xl="8" v-for="p in content" :key="o">
            <h2 class="name">{{p.name}}</h2>
            <img class='logo' v-bind:src='p.pic'>
            <ul>
              <li>
                <a v-bind:href="'https://twitter.com/'+p.twitter">
                  <i class="fab fa-twitter twitter"></i>
                </a>  
              </li>
              <li>
                <a v-bind:href=" 'mailto:'+p.mail">
                  <i class="fas fa-envelope"></i>
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
    margin: auto;
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
    ul{
      list-style-type: none;
      padding-left: 0;
       li{
        float: left;
        margin-left: 10px;
        a{
          color: inherit;
          font-size: 18px;
          font-size-adjust: inherit;
        }
      }
    }
    .logo{
      width: 50%;
      max-width: 85px;
      margin-left: 7%;
    }
    .twitter{
      color: #1da1f2;
    }
    .talk{
      background-color: #f2f2f2;
      padding: 0px 5% 2% 5%;
      margin-bottom: 20px;
    }
</style>
