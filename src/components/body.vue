<template>
    <div id="con">
      <el-tabs type="border-card">
        <el-tab-pane label="能力">
          <Ability/>
        </el-tab-pane>
        <el-tab-pane label="小白级能力">
          <Unfamiliar/>
        </el-tab-pane>
        <el-tab-pane label="爱好&个人评价">
          <Favor/>
        </el-tab-pane>
        <el-tab-pane label="经历">
          <Exp/>
        </el-tab-pane>
        <el-tab-pane label="项目">
          <Project/>
        </el-tab-pane>
        <el-tab-pane label="笔记(只选择部分展示)">
          <Note/>
        </el-tab-pane>
      </el-tabs>
    </div>
</template>
<script>
  import Ability from "./content/ability";
  import Unfamiliar from "./content/novice";
  import Favor from "./content/favor";
  import Exp from "./content/experience";
  import Project from "./content/project";
  import Note from "./content/note";

    export default {
        name: "Con",
        components:{
          Ability,
          Unfamiliar,
          Favor,
          Exp,
          Project,
          Note
        }
    }
</script>

<style scoped>
  #con{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .el-tabs{
    margin-top: 2rem;
    width: 80%;
    border-radius: 0.3rem;
  }
</style>
