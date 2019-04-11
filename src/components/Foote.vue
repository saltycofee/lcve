<template>
    <div id="Foote">
      <a href="javascript:;" class="totop" title="回到顶部"></a>
      <div class="container footer_href">
        <div class="row">
          <div class="col-sm-7 col-sm-offset-3 col-xs-10 col-xs-offset-1">
            <div class="row">
              <div class="col-sm-3 col-xs-3">
                <h4>关于我</h4>
                <ul>
                  <li><a href="https://github.com/shihao1010" target="_blank">github</a></li>
                  <li><a href="https://blog.csdn.net/duke10" target="_blank">csdn</a></li>
                </ul>
              </div>
              <div class="col-sm-3 col-xs-3">
                <h4>CDN资源库</h4>
                <ul>
                  <li><a href="https://www.bootcdn.cn/" target="_blank">bootcdn</a></li>
                  <li><a href="http://staticfile.org/" target="_blank">Staticfile CDN</a></li>
                </ul>
              </div>
              <div class="col-sm-3 col-xs-3">
                <h4>常用教程</h4>
                <ul>
                  <li><a href="http://www.w3school.com.cn/" target="_blank">w3school</a></li>
                  <li><a href="http://www.runoob.com/" target="_blank">菜鸟教程</a></li>
                </ul>
              </div>
              <div class="col-sm-3 col-xs-3">
                <h4>云服务器</h4>
                <ul>
                  <li><a href="https://www.aliyun.com/product/ecs?spm=5176.10695662.744563.1.4b46700c6yzYOh" target="_blank">阿里云</a></li>
                  <li><a href="https://cloud.tencent.com/product/cvm" target="_blank">腾讯云</a></li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
      <footer class="footer11">
        <a href='http://www.miibeian.gov.cn/' target="_blank">豫ICP备18027620号 | </a>
        <span id="sitetime" >{{time}}</span>     <!--网站运行时间统计-->
        <a href="https://tongji.baidu.com/web/welcome/ico?s=c05eafcbb90cbad1f9950cd57287c2a2" target="_blank"> | 网站统计</a>
      </footer>
    </div>
</template>

<script >
    export default {
        name: "Foote",
      data(){
          return {
           time:'',
          }
      },
      methods:{
     /*
       siteTime(){
       var seconds = 1000;
         var minutes = seconds * 60;
         var hours = minutes * 60;
         var days = hours * 24;
         var years = days * 365;
         var today = new Date();
         var todayYear = today.getFullYear();
         var todayMonth = today.getMonth()+1;
         var todayDate = today.getDate();
         var todayHour = today.getHours();
         var todayMinute = today.getMinutes();
         var todaySecond = today.getSeconds();
          Date.UTC() -- 返回date对象距世界标准时间(UTC)1970年1月1日午夜之间的毫秒数(时间戳)
         year - 作为date对象的年份，为4位年份值
         month - 0-11之间的整数，做为date对象的月份
         day - 1-31之间的整数，做为date对象的天数
         hours - 0(午夜24点)-23之间的整数，做为date对象的小时数
         minutes - 0-59之间的整数，做为date对象的分钟数
         seconds - 0-59之间的整数，做为date对象的秒数
         microseconds - 0-999之间的整数，做为date对象的毫秒数
        var t1 = Date.UTC(2018,7,22,0,0,0); //北京时间2016-12-1 00:00:00
    var t2 = Date.UTC(todayYear,todayMonth,todayDate,todayHour,todayMinute,todaySecond);
    var diff = t2-t1;
    var diffYears = Math.floor(diff/years);
    var diffDays = Math.floor((diff/days)-diffYears*365);
    var diffHours = Math.floor((diff-(diffYears*365+diffDays)*days)/hours);
    var diffMinutes = Math.floor((diff-(diffYears*365+diffDays)*days-diffHours*hours)/minutes);
    var diffSeconds = Math.floor((diff-(diffYears*365+diffDays)*days-diffHours*hours-diffMinutes*minutes)/seconds);
    document.getElementById("sitetime").innerHTML="博客已运行"+diffYears+" 年 "+diffDays+" 天 "+diffHours+" 小时 "+diffMinutes+" 分钟 "+diffSeconds+" 秒";
    }
      */

      },
      mounted() {
        window.setInterval(()=>{var seconds = 1000;
          var minutes = seconds * 60;
          var hours = minutes * 60;
          var days = hours * 24;
          var years = days * 365;
          var today = new Date();
          var todayYear = today.getFullYear();
          var todayMonth = today.getMonth()+1;
          var todayDate = today.getDate();
          var todayHour = today.getHours();
          var todayMinute = today.getMinutes();
          var todaySecond = today.getSeconds();
          /* Date.UTC() -- 返回date对象距世界标准时间(UTC)1970年1月1日午夜之间的毫秒数(时间戳)
          year - 作为date对象的年份，为4位年份值
          month - 0-11之间的整数，做为date对象的月份
          day - 1-31之间的整数，做为date对象的天数
          hours - 0(午夜24点)-23之间的整数，做为date对象的小时数
          minutes - 0-59之间的整数，做为date对象的分钟数
          seconds - 0-59之间的整数，做为date对象的秒数
          microseconds - 0-999之间的整数，做为date对象的毫秒数 */
          var t1 = Date.UTC(2019,4,10,0,0,0); //北京时间2016-12-1 00:00:00
          var t2 = Date.UTC(todayYear,todayMonth,todayDate,todayHour,todayMinute,todaySecond);
          var diff = t2-t1;
          var diffYears = Math.floor(diff/years);
          var diffDays = Math.floor((diff/days)-diffYears*365);
          var diffHours = Math.floor((diff-(diffYears*365+diffDays)*days)/hours);
          var diffMinutes = Math.floor((diff-(diffYears*365+diffDays)*days-diffHours*hours)/minutes);
          var diffSeconds = Math.floor((diff-(diffYears*365+diffDays)*days-diffHours*hours-diffMinutes*minutes)/seconds);
          this.time="博客已运行"+diffYears+" 年 "+diffDays+" 天 "+diffHours+" 小时 "+diffMinutes+" 分钟 "+diffSeconds+" 秒";
        }, 1000);
      }

    }
</script>

<style scoped>

</style>
