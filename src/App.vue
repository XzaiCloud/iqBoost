<template>
    <el-main>
        <el-card class="box-card">
            <template #header>
                <div class="card-header">
                    <b>iqBoost 公益加速ip</b>
                    <el-button tag="a" href="//b8y.shop" target="_blank">求赞助</el-button>
                </div>
            </template>
            <div>
                <!--主要内容-->
                <el-image src="./index.webp"/>
                <p>节点列表（点击复制ip）</p>
                <div class="btn-group">
                    <el-button tag="a" @click="copyText('cn-01.iqboost.icu')">上海专线-01</el-button>
                    <el-button tag="a" @click="copyText('us-01.iqboost.icu')">美国专线-01</el-button>
                    <el-button tag="a" @click="copyText('us-02.iqboost.icu')">美国专线-02</el-button>
                    <el-button tag="a" @click="copyText('us-03.iqboost.icu')">美国专线-03</el-button>
                </div>
                <el-divider/>
                <p><a id="hitokoto">
                    <el-icon class="is-loading">
                        <Loading/>
                    </el-icon>
                </a></p>
                <el-link type="primary" :underline="false" href="//fuibafuyu.net" target="_blank">冬優ちゃんの小窝</el-link>
                &boxv;
                <el-link type="primary" :underline="false" href="//b8y.top" target="_blank">Xzaiの个人主页</el-link>
                <el-divider/>
                <el-text>Create by <el-icon><ElementPlus/></el-icon> <el-link :underline="false" href="//b8y.top" target="_blank">Pigeon Network</el-link></el-text>
                <!--主要内容-->
            </div>
        </el-card>
    </el-main>
</template>

<script>
import { ElMessage } from 'element-plus'
export default {
  methods: {
    copyText(text) {
      navigator.clipboard.writeText(text)
        .then(() => {
          ElMessage({message: '文本已复制到剪贴板',type: 'success',})
        })
        .catch((error) => {
          ElMessage.error('复制文本失败，请联系网站管理员')
        });
    }
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@300&display=swap');
</style>

<style scoped>
.btn-group {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}
:deep(.el-button){
  margin-left: 0;
}
.card-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.text {
  font-size: 14px;
}
.item {
  margin-bottom: 18px;
}
.box-card {
  width: 800px;
  margin: auto;
}
@media only screen and (max-width: 1000px) {
  .box-card {
    width: 99%;
  }
}
* {
  font-family:"Noto Sans SC";
  text-decoration: none;
  overflow: hidden;
}
.el-link {
  margin-top: -4px;
}
.el-image {
  border-radius: 10px;
}
</style>