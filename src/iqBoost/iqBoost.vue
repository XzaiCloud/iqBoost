<template>
    <el-main>
        <el-card class="box-card">
            <template #header>
                <div class="card-header">
                    <b>欣赏LowIQ用户</b>
                    <el-button tag="a" href="/">返回主页</el-button>
                </div>
            </template>
            <div>
                <!--主要内容-->
                <h3>apple > android</h3>
                <p/>
                <el-image src="../LowIQ/1.jpg" lazy/>
                <h3>亲妈献祭</h3>
                <p/>
                <el-image src="../LowIQ/2.webp" lazy/>
                <p>如果你有素材，欢迎投稿xzai0313@qq.com</p>
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
                <el-text>Create by <el-icon><ElementPlus/></el-icon> <el-link :underline="false" href="//b8y.top" target="_blank">Xzai</el-link>&boxv;<el-link type="primary" :underline="false" href="//beian.miit.gov.cn" target="_blank">蜀ICP备2022010825号-1</el-link></el-text>
                <!--主要内容-->
            </div>
        </el-card>
    </el-main>
</template>

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