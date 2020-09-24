<template>
    <div style="text-align: left;">
        <ul v-for="(item,index) in projectArr" style="display: flex;justify-content: space-between">
          <li :key="index">{{item.name}}:
          </li>
          <el-link icon="el-icon-view" :href="item.url">查看github</el-link>
        </ul>
    </div>
</template>

<script>
    export default {
        name: "project",
        data:function () {
          return{
            projectArr:[
              {
                name:"ftp的windows客户端(Swing)",
                url: "https://github.com/jinxiaochi/FTP_Client"
              },
              {
                name:"个人博客(即本网站,vue.js+elementUI)",
                url: "https://github.com/jinxiaochi/jinxiaochi.github.io"
              },
              {
                name:"淘房网(类似链家,vue.js+springBoot+bootstrap,包含vue-router和Vue-resource)",
                url: "https://github.com/jinxiaochi/houseMarket"
              },
            ]
          }
        }
    }
</script>

<style scoped>
  .el-button{
    height: 80%;
  }
  .el-link{
    margin-right: 0px;
  }

</style>
