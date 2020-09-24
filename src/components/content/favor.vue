<template>
    <div style="text-align: left">
      <el-tabs tab-position="left" style="height: 100%;" >
        <el-tab-pane label="爱好" >
          <ul v-for="(item,index) in favorArr">
            <li :key="index">{{item}}</li>
          </ul>
        </el-tab-pane>

        <el-tab-pane label="个人评价" >
          <ul v-for="(item,index) in commentArr">
            <li :key="index">{{item}}</li>
          </ul>
        </el-tab-pane>
      </el-tabs>
    </div>
</template>

<script>
    export default {
        name: "favor",
        data:function () {
          return{
            favorArr:[
              "喜欢历史和金融",
              "喜欢绘画和口琴",
              "对电脑的装机和简单修理有一定了解",
              "对新奇的事物充满兴趣"
            ],
            commentArr:[
              "有良好的自学能力和自学体系,有做笔记的良好习惯",
              "积极上进,喜欢做挑战有难度的事",
              "做事精炼,珍惜时间",
              "有对疑问追问和自我寻求解答的能力",
              "做事有计划和安排,也能即时改变计划,适应情况",
              "能吃苦耐劳,能抵抗一定强度的工作",
              "有好奇心,对新事物充满好奇",
            ]
          }
        }
    }
</script>

<style scoped>

</style>
