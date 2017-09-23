<template>
  <div id="wrapper">
    <el-row class="tac">
      <el-col :span="8">
        <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" theme="dark">
          <el-submenu index="1">
            <template slot="title">Navigator One</template>
            <el-menu-item-group title="Group One">
              <el-menu-item index="1-1">item one</el-menu-item>
              <el-menu-item index="1-2">item two</el-menu-item>
            </el-menu-item-group>
            <el-menu-item-group title="Group Two">
              <el-menu-item index="1-3">item three</el-menu-item>
            </el-menu-item-group>
            <el-submenu index="1-4">
              <template slot="title">item four</template>
              <el-menu-item index="1-4-1">item one</el-menu-item>
            </el-submenu>
          </el-submenu>
          <el-menu-item index="2">Navigator Two</el-menu-item>
          <el-menu-item index="3">Navigator Three</el-menu-item>
        </el-menu>
      </el-col>
      <el-col :span="16">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cupiditate perspiciatis accusantium ullam nam necessitatibus quasi a tempore ipsum illo aspernatur, quo numquam ducimus nulla itaque, perferendis voluptate repellat dolore non.
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cupiditate perspiciatis accusantium ullam nam necessitatibus quasi a tempore ipsum illo aspernatur, quo numquam ducimus nulla itaque, perferendis voluptate repellat dolore non.
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cupiditate perspiciatis accusantium ullam nam necessitatibus quasi a tempore ipsum illo aspernatur, quo numquam ducimus nulla itaque, perferendis voluptate repellat dolore non.
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cupiditate perspiciatis accusantium ullam nam necessitatibus quasi a tempore ipsum illo aspernatur, quo numquam ducimus nulla itaque, perferendis voluptate repellat dolore non.
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cupiditate perspiciatis accusantium ullam nam necessitatibus quasi a tempore ipsum illo aspernatur, quo numquam ducimus nulla itaque, perferendis voluptate repellat dolore non.
      </el-col>
    </el-row>
  </div>
</template>

<script>
  import ChecklistList from './HomePage/ChecklistList'
  import ChecklistContent from './HomePage/ChecklistContent'
  import ChecklistAdd from './HomePage/ChecklistAdd'

  export default {
    name: 'landing-page',
    components: {
      ChecklistList,
      ChecklistContent,
      ChecklistAdd,
    },
    data() {
      return {
        visible: false,
      }
    }
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Source+Sans+Pro');

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body { font-family: 'Source Sans Pro', sans-serif; }
</style>
