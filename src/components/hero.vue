<template>
  <div id="hero">
    <h1 class="title">WiSeInno</h1>
    <h2 class="subtitle">Innovation is fun</h2>
    <div class="icon_bar">
      <a href="https://twitter.com/wise_inno">
        <i class="fab fa-twitter fa-2x"></i>
      </a>
      <a href="https://facebook.com/wiseinno.tech">
        <i class="fab fa-facebook fa-2x"></i>
      </a>
      <a href="mailto:info@wiseinno.tech">
        <i class="fas fa-envelope fa-2x"></i>
      </a>
      <a href="https://wiseinno-events.herokuapp.com">
        <i class="fas fa-calendar-alt fa-2x"></i>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'hero',
}
</script>

<style lang="scss" scoped>
  #hero{
    background-color: #008ed6;
    //height: 100%;
    text-align: center;
    .title{
      padding-top: 50px;
      font-family: Menlo;
      font-size: 52px;
      color: #fffff2;
    }
    .subtitle{
      font-family: Menlo;
      font-size: 22px;
      color: whitesmoke;
    }
    .icon_bar{
      * {
        margin-right: 5px;
      }
      a{
        color: #fffff2;
      }
      i{
        font-size: 2rem;
      }
      color: #fffff2;
      
      padding-bottom: 50px;
    }
  }
</style>
