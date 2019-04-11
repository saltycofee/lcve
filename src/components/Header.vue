<template>
    <div id="Header">
      <header>
        <div class="container">
          <div class="logo_title" data-scroll-reveal="enter right and move 20px over 1s">走在海边，走在月下</div>
        </div>
        <nav class="navbar navbar-static-top" role="navigation">
          <div class="container">
            <div class="navbar-header">
              <button type="button" data-scroll-reveal="enter bottom and move 20px over 1s after 1s" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#index_menu" aria-expanded="false">
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
              </button>
            </div>
            <div class="collapse navbar-collapse" id="index_menu">
              <ul class="nav navbar-nav" data-scroll-reveal="enter bottom and move 20px over 0.7s after 0.3s">
                <li><a href="/"><span>首页</span><span>Home</span></a></li>
                <li><a href="/about/"><span>关于我</span><span>About</span></a></li>
                <li><a href="/learn/0/1"><span>学无止境</span><span>Learn</span></a></li>
                <li><a href="/slowlife/"><span>慢生活</span><span>Life</span></a></li>
                <li><a href="/liuyan/"><span>留言</span><span>Saying</span></a></li>
                <li><a href="/admin" target="_blank"><span>管理</span><span>Admin</span></a></li>
              </ul>
              <form class="navbar-form navbar-right" method='get' action="/search/" id="search">
                <div class="form-group">
                  <input type="text" name="q" class="form-control" placeholder="搜索文章">
                </div>
                <button type="submit" class="btn btn-default">Search</button>
              </form>
            </div>
          </div>
        </nav>
      </header>

  </div>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>

</style>
