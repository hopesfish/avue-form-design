<template>
  <div>
    <el-form-item label="图标">
      <avue-icon-select v-model="data.icon"
                        :icon-list="iconList"
                        placeholder="图标"></avue-icon-select>
    </el-form-item>
    <el-form-item label="是否可以追加">
      <el-switch v-model="data.duplicatable"></el-switch>
    </el-form-item>
  </div>
</template>
<script>

export default {
  name: "config-group",
  props: ['data'],
  data () {
    return {
      iconList: [{
        label: 'element-ui',
        list: ['el-icon-info', 'el-icon-error', 'el-icon-success', 'el-icon-warning', 'el-icon-question']
      }]
    }
  }
}
</script>
<style lang="scss" scoped>
</style>
