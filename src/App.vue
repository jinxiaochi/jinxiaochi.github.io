<template>
  <div id="app">
    <el-container>
      <el-header height="100%">
        <Header/>
      </el-header>
      <el-main>
        <Con/>
      </el-main>


      <el-footer>
        <hr/>
        <Footer/>
      </el-footer>
    </el-container>
  </div>
</template>

<script>
  import Header from "./components/Header";
  import Footer from "./components/Footer";
  import Con from "./components/body";

export default {
  name: 'App',
  components:{
    Header,
    Footer,
    Con
  }
}
</script>

<style>
  #app{
    width: 100%;
    height: 100%;
    margin-top: 0px;
  }
  .el-header {
    color:#303133;
    text-align: center;
    height:100%;
    border-radius: 0.3rem 0.3rem 0rem 0rem;
    background-color: #303133;
  }

  .el-footer {
    color:#303133;
    text-align: center;
    height:100%;
    border-radius: 0rem 0rem 0.3rem 0.3rem;
    background-color: #909399;
  }

  .el-main {
    /*background-color: #E9EEF3;*/
    background-color: #909399;
    color: #333;
    text-align: center;
  }

  body > .el-container {
    margin-bottom: 40px;
  }
</style>
