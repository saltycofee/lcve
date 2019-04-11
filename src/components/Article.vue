<template>
    <div id="Home">
      <article>
        <div class="container center_content">
          <div class="row" data-scroll-reveal="enter left and move 20px over 1s">
            <div class="col-xs-4">
              <a href="#"><img src="../../static/images/anPic1.jpg" class="img-responsive" alt="Responsive image"></a>
              <p>不管前方的路有多苦，只要走的方向正确，不管多么崎岖不平，都比站在原地更接近幸福。</p>
              <h3 class="text-right">——宫崎骏《千与千寻》</h3>
            </div>
            <div class="col-xs-4">
              <a href="#"><img src="../../static/images/anPic2.jpg" class="img-responsive" alt="Responsive image"></a>
              <div class="center_animition">
                <div class="panghu_moving"><img src="../../static/images/zz.gif" class="img-responsive"></div>
                <ul class="controlbox">
                  <li class="glyphicon glyphicon-play"></li>
                  <li class="glyphicon glyphicon-pause"></li>
                </ul>
              </div>
            </div>
            <div class="col-xs-4">
              <a href="#"><img src="../../static/images/anPic3.jpg" class="img-responsive" alt="Responsive image"></a>
              <p>我不知道离别的滋味是这样凄凉，我不知道说声再见要这么坚强。</p>
              <h3 class="text-right">——宫崎骏《千与千寻》</h3>
            </div>
          </div>

          <ul class="tmtimeline">
            <div id="changeBox">
              <span class="glyphicon glyphicon-indent-left"></span>
            </div>
            <div class="container col-xs-12" id="pie"></div>
          </ul>

          <div class="pages">
            <a href="javascript:;">&lt;</a>
            <a href="javascript:;">&gt;</a>
          </div>
        </div>
      </article>

      <span id="sitetime"></span>     <!--网站运行时间统计-->
    </div>
</template>

<script>

    export default {
        name: "Home",
      data(){
          return{
            msg:'454545'
          }
      },
    }
</script>

<style scoped>

</style>
