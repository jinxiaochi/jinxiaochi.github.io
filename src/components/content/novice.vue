<template>
  <div style="text-align: left">
    <p>注: 以下能力有段时间没有使用,遗忘了许多</p>
    <ul v-for="(item, index) in unfamiliarArr">
      <li :key="index">{{item}}</li>
    </ul>
  </div>
</template>

<script>
    export default {
        name: "novice",
        data:function () {
          return{
            unfamiliarArr:[
              "能独立编写小型微信小程序(曾获得微信小程序高校小程序大赛三等奖)",
              "了解nodejs和express前端框架",
              "了解Python",
              "了解并会使用AE PR PS这些编辑软件",
              "了解完整的计算机体系结构和相关硬件",
              "了解web安全相关知识(如XSS,CSRF等)",
              "Unity3D入门小白"
            ]
          }
        }
    }
</script>

<style scoped>

</style>
