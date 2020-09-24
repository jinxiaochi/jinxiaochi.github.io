<template>
  <div style="text-align: left">
    <ul  v-for="(item,index) in abilityArr">
      <li :key="index">{{item}}</li>
    </ul>
  </div>
</template>

<script>
   import dataAbility from "../data/dataAbility.json";
    export default {
        name: "ability",
        data:function () {
          return{
            abilityArr:[]
          }
        },
      created:function () {
          this.abilityArr = dataAbility;
      }
    }
</script>

<style scoped>

</style>
