<template>
    <div style="text-align: left">
      <el-tabs tab-position="left" style="height: 100%;" >
        <el-tab-pane label="JAVA(节选)" >
          <ul v-for="(item,index) in JavaArr"  style="display: flex;justify-content: space-between">
            <li :key="index">{{item.name}}</li>
             <el-link icon="el-icon-view" :href="item.url">查看笔记</el-link>
          </ul>
        </el-tab-pane>

        <el-tab-pane label="前端(节选)" >
          <ul v-for="(item,index) in jsArr"  style="display: flex;justify-content: space-between">
           <li :key="index">{{item.name}}</li>
             <el-link icon="el-icon-view" :href="item.url">查看笔记</el-link>
          </ul>
        </el-tab-pane>

      <el-tab-pane label="数据库(节选)" >
          <ul v-for="(item,index) in DbArr"  style="display: flex;justify-content: space-between">
           <li :key="index">{{item.name}}</li>
             <el-link icon="el-icon-view" :href="item.url">查看笔记</el-link>
          </ul>
        </el-tab-pane>

        
     </el-tabs> 
    </div>
</template>

<script>
    export default {
        name: "note",
        data:function () {
          return{
            JavaArr:[
                {name:"二维码 加密 发送邮件 xml解析等常用功能",url:"https://shimo.im/docs/PV3XWcXJKQY8TT38/"},
                {name:"监听器 过滤器和拦截器",url:"https://shimo.im/docs/kq9pQChpRpJPpgr3/"},
                {name:"文件上传 下载和zip压缩 解压",url:"https://shimo.im/docs/TGdR6tygKJ3qdDDd/"},
                {name:"JavaSE Socket的编程 多线程 和IO及NIO AIO",url:"https://shimo.im/docs/TPtCdkyRkVvDgqRx/"}
            ],
            jsArr:[
                {name:"js及前端要点小记",url:"https://shimo.im/docs/t83rRRJWhrvpGyy3/"}
            ],
            DbArr:[
                {name:"数据库小结",url:"https://shimo.im/docs/gvr6r36Ptp9JGxYj/"}
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
