<template>
  <div>
    <el-row :gutter="20">
      <el-col :span="6">
        <div class="grid-content bg-purple"></div>
      </el-col>
      <el-col :span="6">
        <div class="grid-content bg-purple"></div>
      </el-col>
      <el-col :span="6">
        <div class="grid-content bg-purple"></div>
      </el-col>
      <el-col :span="6">
        <div class="grid-content bg-purple"></div>
      </el-col>
    </el-row>
    <p>
      Row 组件 提供
      <code>gutter</code>属性来指定每一栏之间的间隔，默认间隔为 0。
    </p>
    <el-collapse>
      <el-collapse-item title="显示代码" name="1">
        <el-input
          type="textarea"
          :autosize="{ minRows: 25, maxRows: 4}"
          readonly
          placeholder="请输入内容"
          v-model="textarea2"
        ></el-input>
      </el-collapse-item>
    </el-collapse>
  </div>
</template>

<script>
export default {
  methods: {
    handleClick(row) {
      console.log(row);
    }
  },
  data() {
    return {
      textarea2: `
                <template>
                    <div>
                       <el-row :gutter="20">
                          <el-col :span="6">
                            <div class="grid-content bg-purple"></div>
                          </el-col>
                          <el-col :span="6">
                            <div class="grid-content bg-purple"></div>
                          </el-col>
                          <el-col :span="6">
                            <div class="grid-content bg-purple"></div>
                          </el-col>
                          <el-col :span="6">
                            <div class="grid-content bg-purple"></div>
                          </el-col>
                        </el-row>
                    </div>
                     <style>
                            .el-row {
                              margin-bottom: 20px;
                              &:last-child {
                                margin-bottom: 0;
                              }
                            }
                            .el-col {
                              border-radius: 4px;
                            }
                            .bg-purple-dark {
                              background: #99a9bf;
                            }
                            .bg-purple {
                              background: #d3dce6;
                            }
                            .bg-purple-light {
                              background: #e5e9f2;
                            }
                            .grid-content {
                              border-radius: 4px;
                              min-height: 36px;
                            }
                            .row-bg {
                              padding: 10px 0;
                              background-color: #f9fafc;
                            }
                          </style>
                </template>
            `
    };
  }
};
</script>
<style scoped>
.el-row {
  margin-bottom: 20px;
  &:last-child {
    margin-bottom: 0;
  }
}
.el-col {
  border-radius: 4px;
}
.bg-purple-dark {
  background: #99a9bf;
}
.bg-purple {
  background: #d3dce6;
}
.bg-purple-light {
  background: #e5e9f2;
}
.grid-content {
  border-radius: 4px;
  min-height: 36px;
}
.row-bg {
  padding: 10px 0;
  background-color: #f9fafc;
}
</style>
