<template>
    <el-main>
        <el-card class="box-card">
            <template #header>
                <div class="card-header">
                    <b>你可能需要 iqBoost</b>
                    <el-button tag="a" href="//b8y.shop" target="_blank">求赞助</el-button>
                </div>
            </template>
            <div>
                <!--主要内容-->
                <el-image src="./index.webp" lazy/>
                <h3>什么是 iqBoost？</h3>
                <p>你是否感到你的智商一直在阻碍你的发展？你是否期望自己能变得更聪明、更有创造力、更成功？</p>
                <p>现在，我们推出了 iqBoost 这款革命性的新产品可以帮助你释放全部潜力。我们的专有配方基于尖端研究，并已被证明在提高大脑功能方面非常有效。</p>
                <p>最棒的是， iqBoost 非常容易使用。只需服用一粒胶囊，您就会很快感受到效果。无论是在备考考试、进行项目工作还是只是想提高认知能力， iqBoost 都是适合您的产品。</p>
                <p>还在等什么？立即购买 iqBoost，释放您的全部潜力！</p>
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
                <el-text>Create by <el-icon><ElementPlus/></el-icon> <el-link :underline="false" href="//b8y.top" target="_blank">Xzai</el-link>&boxv;纯属恶搞&boxv;<el-link type="primary" :underline="false" href="//beian.miit.gov.cn" target="_blank">蜀ICP备2022010825号-1</el-link></el-text>
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