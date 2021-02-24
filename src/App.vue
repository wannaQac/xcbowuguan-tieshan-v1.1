<template>
  <div>
    <el-row>
      <el-col :span="5"><img :src="imgIcon" style="width: 100%"></el-col>
      <el-col :span="19" >
        <el-menu router
              :default-active="this.$route.path"
              class="el-menu-demo"
              mode="horizontal"
              @select="handleSelect">
       <!-- <el-menu-item index="1" style="margin-top: 3%">处理中心</el-menu-item>-->
        <el-menu-item id="navv" v-for="(item,i) in navList" :key="i" :index="item.name" >
          <template slot="title">
            <!--<i class="el-icon-s-platform"></i>-->
            <span>{{item.navItem}}</span>
          </template>
        </el-menu-item>

      </el-menu></el-col>
    </el-row>
    <el-main>
      <router-view>

      </router-view>
    </el-main>
    <div class="mainbox-ld bottominfo">
      <p class="crcn">版权所有：乡旅国际数字博物馆</p>
      <p class="cren">Copyright 2020 © All rights reserved by XCGJ.</p>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        navList:[
          {name:'/Cunluo',navItem:'铁山街道'},
          {name:'/Quanjing',navItem:'全景展示'},
          {name:'/Lishi',navItem:'历史文化'},
          {name:'/Huanjing',navItem:'环境格局'},
          {name:'/Chuantong',navItem:'传统建筑'},
          {name:'/Minsu',navItem:'民俗文化'},
          {name:'/Meishi',navItem:'美食物产'},
          {name:'/Lvyou',navItem:'旅游导览'},
          {name:'/Zhaoshang',navItem:'招商信息'},
        ],
        imgIcon: require("../static/logo.png"),
      };
    },
    methods: {
    }
  }
</script>

<style>
  #navv{
    margin-top: 2.5%;
    margin-left: 1%;
    margin-right: 1%;
  }
</style>