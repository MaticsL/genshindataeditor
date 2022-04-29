<template>
  <div id="app">
    <el-container>
      <el-aside width="300px">
        <el-menu default-active="1" class="el-menu-vertical-demo">
          <router-link to='/drop'>
            <el-menu-item index="1">
              <i class="el-icon-menu"></i>
              <span slot="title">掉落物</span>
            </el-menu-item>
          </router-link>
          <el-menu-item index="2" disabled>
            <i class="el-icon-document"></i>
            <span slot="title">卡池</span>
          </el-menu-item>
          <el-menu-item index="3" disabled>
            <i class="el-icon-setting"></i>
            <span slot="title">生成物</span>
          </el-menu-item>
        </el-menu>
      </el-aside>
      <el-main><router-view/></el-main>
    </el-container>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
.el-menu-vertical-demo {
  width: 200px;
  min-height: 400px;
  text-align: left;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
