<template>
<div id="header">
  <div>
    <el-avatar :size="avatar_size" :src="imgUrl"></el-avatar>
  </div>

  <div class="motto">
    <h2>
      求知若渴,虚心若愚
    </h2>
  </div>

  <div class="date">
    <p>当前日期:<el-input
      v-model="date"  :disabled="true"
       style="color: red"/>
    </p>
  </div>
</div>
</template>

<script>
    export default {
        name: "Header",
        data:function () {
          return{
            avatar_size:130,
            imgUrl: require("../assets/headPortrait.jpg"),
            date:'',
            timer:null
          }
        },
      created() {
          var current = new Date();
          this.date = //修改数据date
            current.getFullYear() +
            "-" +
            (current.getMonth() + 1) +
            "-" +
            current.getDate() ;

      }

    }
</script>

<style scoped>
  #header{
    display: flex;
    height: 10rem;
    justify-content: space-around;
    align-items: center;

  }

  h2{
    font-family: 华文隶书;
  }


  .motto, .date{
    height: 90%;
    display: flex;
    align-items: flex-end;
    color: white;
  }
</style>
