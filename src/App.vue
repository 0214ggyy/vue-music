<template>
  <div id="app">
  <div class="app-g">
    <Menu mode="horizontal" :theme="theme1" active-name="1">
        <Icon type="md-reorder" class="ico-active"/>
         <MenuItem name="2">
            <Icon type="ios-at" />
        </MenuItem>
        <MenuItem name="3">
            <Icon type="md-musical-notes" />
        </MenuItem>
        
        <MenuItem name="4">
            <Icon type="logo-youtube" />
        </MenuItem>
       <Icon type="ios-search-outline" class="ico-active" />
    </Menu>
  </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
            return {
                theme1: 'dark'
            }
        }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.ivu-menu-dark{
  background-color: red;
}
.ivu-menu{
  display: flex;
  justify-content: space-around;
}
.ivu-icon{
 font-size:30px;
}
.ivu-icon.ico-active{
  color:#fff;
  
  line-height: 60px;
}
</style>
