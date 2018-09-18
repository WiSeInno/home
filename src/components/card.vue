<template>
<div id="team">
  <el-row :gutter="40">
        <el-col :span="8" v-for="(card, index) in content" :key="o">
          <el-card :body-style="{ padding: '0px' }">
            <img v-bind:src="card.pic" height="250" class="image">
            <div style="padding: 14px;">
              <span>{{card.name}}</span>
              <div class="bottom clearfix">
                <time class="time">{{ currentDate }}</time>
                <a v-bind:href="card.link" target="_blank">
                  <el-button type="text" class="button">Check it out</el-button>
                </a>
              </div>
            </div>
          </el-card>
        </el-col>
    </el-row>
    <hr>
</div>
</template>

<script>
export default {
  name: 'card',
  data() {
    return {
      content: [
        {name: 'Success Stories', pic: require('@/assets/success.svg'), link: 'https://blog.wiseinno.tech/success-stories/home'},
        {name: 'Technical Articles', pic: require('@/assets/research.svg'), link: 'https://blog.wiseinno.tech/technical/home'},
        {name: 'Piece of Advice', pic: require('@/assets/help.svg'), link: 'https://blog.wiseinno.tech/advice/home'}
      ]
    };
  }
}
</script>

<style lang="scss" scoped>
hr{
  color: #EE7785;
  border: 2px solid #EE7785;
  border-radius: 10px;
  margin-top: 50px;
  margin-bottom: 50px;
}
</style>
