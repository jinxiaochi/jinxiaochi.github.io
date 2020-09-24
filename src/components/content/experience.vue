<template>
  <div style="text-align: left">
    <el-tabs tab-position="left" style="height: 100%;">
      <el-tab-pane label="工作经历">
        <ul v-for="(item,index) in jobArr">
          <li :key="index">{{item}}</li>
        </ul>
      </el-tab-pane>

      <el-tab-pane label="教育经历">
        <ul v-for="(item,index) in eduArr">
          <li :key="index">{{item}}</li>
        </ul>
      </el-tab-pane>
    </el-tabs>
  </div>
</template>

<script>
    export default {
        name: "experience",
        data:function () {
          return{
            jobArr:[
              "大三暑假 在武汉亿信华辰工作和实习过两个月",
              "大一暑假 在汉阳威佳电子厂做流水线工人，组装光猫和路由器",
              "2019年11月-2020年1月,在金证股份实习",
              "2020年7月14-2020年9月23在 金证股份工作"
            ],
            eduArr:[
              "毕业于武汉轻工大学计算机科学与技术专业",
              "大二参加思特沃克训练营校内培训（主要包含nodejs和一些js框架）"
            ]
          }
        }
    }
</script>

<style scoped>

</style>
