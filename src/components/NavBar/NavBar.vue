
<template>
    <nav class="navbar navbar-expand-lg navbar-light navigator">
        <div class="container-fluid">
            <img src="/img/a.svg" alt="icon">
            <a class="navbar-brand title" href="#">2tomatoes前端监控系统</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarText" aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarText">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">    </ul>

                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link"  href="#">首页</a>
                    </li>

                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">错误</a>
                            <ul class="dropdown-menu">
                            <li>
                                <router-link class="dropdown-item" :to="{name: 'errorStat'}">错误统计</router-link>
                            </li>
                            <li><a class="dropdown-item" href="#">Api接口错误统计</a></li>
                            <li><a class="dropdown-item" href="#">静态资源错误统计</a></li>
                            </ul>
                    </li>

                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">性能</a>
                            <ul class="dropdown-menu">
                            <li>
                                <router-link class="dropdown-item" :to="{name: 'jkhsfx'}">接口耗时分析</router-link>
                            </li>
                            <li><router-link class="dropdown-item" :to="{name: 'ymxnfx'}">页面性能分析</router-link></li>
                            </ul>
                    </li>

                    <!-- <li class="nav-item">
                        <a class="nav-link"  href="#">性能</a>

                    </li> -->
                    <li class="nav-item">
                        <a class="nav-link" href="#">实验室</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">设置</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

</template>

<script>
export default {
    name: "NavBar",
}
</script>

<style lang="css" scoped>
.navigator{
    background-color: white;
    box-shadow: 0 0 0 1px rgb(0 0 0 / 3%), 0 2px 5px 1px rgb(0 0 0 / 5%);

    z-index: 10;
}
.title{
    margin-left: 5px;

    font-weight:800;
    font-size: 23px;
    /* color: white; */
}
.nav-link:hover{
    color: #21d48f;
}
</style>