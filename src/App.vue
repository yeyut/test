<template>
  <div id="app">
    <div class="left">
      <ul>
        <li><a href="#">我的首页<span></span></a></li>
        <li><a href="#">名人名言<span></span></a></li>
        <li><a href="#">我的相册<span></span></a></li>
        <li><a href="#">我的简介<span></span></a></li>
        <li><a href="#">留下脚印<span></span></a></li>
      </ul>
    </div>
    <div class="right">
      <div class="content">
        <div class="message">
          <p>夜已深，而咖啡的浓香久久不能挥去。</p>
          <p>我已经养成这种喝咖啡的习惯，自觉不自觉地表达着一种优雅的韵味，一种浪漫情调，一种享受生活的写意感。它已经融入我的生活中了。。。。。。</p>
          <p>在这茫茫雾霭中，伴着思绪的纷飞走进冬的怀抱。悄然领悟了雪的晶莹，落叶的飘落，猛然间发觉这已是今年的最后一个季节...</p>
          <p>夜已深，而咖啡的浓香久久不能挥去。我已经养成这种喝咖啡的习惯，自觉不自觉地表达着一种优雅的韵味，一种浪漫情调，一种享受生活的写意感。它已经融入我的生活中了。。。。。。</p>
          <p>在这茫茫雾霭中，伴着思绪的纷飞走进冬的怀抱。悄然领悟了雪的晶莹，落叶的飘落，猛然间发觉这已是今年的最后一个季节...</p>
          <span>圣诞快乐</span>
        </div>
        <div class="comment">
          <div>
            <div>09::12::2009</div>
            <p><strong>春如幽蓝.</strong>当你不了解一个人的时候，你看到的不一定是真的，你心里所想的也不一定是对的 <a href="#">详细<span></span></a></p>
          </div>
          <div>
            <div>09::12::2009</div>
            <p><strong>懂得感悟.</strong>伤心，绝望那一定是有的，承受吧，没有人能替代你，然后把一切交给时间，时间有用！其实一切只是经过而已！ <a href="#">详细<span></span></a></p>
          </div>
        </div>
      </div>
      <div class="pic">
        <div>
          <img src="./images/pic.jpg">
          <img src="./images/pic2.jpg">
        </div>
        <div class="login">
          <div>
            <label>用户名：</label>
            <input type="text" />
          </div>
          <div>
            <label>密码：</label>
            <input type="passage" />
          </div>
          <button type="submit">登录</button>
          <a href="#">忘记密码？</a>
        </div>
      </div>
    </div>
  </div>
    <!-- <ul>
    <tree :model="data"></tree>
    </ul> -->
</template>

<style>
*{
  margin: 0;
  padding: 0;
  font-family: '微软雅黑';
}
a{
  text-decoration: none;
}
ul,li{
  list-style-type: none;
}
body{
  height: 100ch;
}
#app{
  border: 10px solid #c5c5c5;
  background: linear-gradient(#8297a8,#4a6077);
  display: flex;
  padding: 15px;
  height: calc(100% - 50px);
}
.left{
  flex: 0 0 30%;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
}
.left>ul{
  border-top: 1px solid #fff;
  width: 40%;
}
.left>ul>li{
  border-bottom: 1px solid #fff;
  text-align: center;
}
.left>ul>li>a{
  color: #fff;
  font-size: 1.3rem;
  letter-spacing: 5px;
  line-height: 3rem;
}
.left>ul>li>a>span{
  display: inline-block;
  width: 0;
  height: 0;
  border: 8px solid;
  border-color: transparent #44596e transparent transparent;
}
.right{
  background: #fff;
  flex: auto;
  display: flex;
}
.content{
  flex: 0 0 45%;
  padding: 50px 80px 30px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.message{
  border-bottom: 1px dotted #ccc;
  color: #bc412f;
  font-weight: bold;
  padding-bottom: 40px;
}
.message>p{
  text-indent: 2em;
  line-height: 1.5rem;
  margin-bottom: 0.4rem;
}
.message>span{
  display: flex;
  justify-content: flex-end;
  font-size: 1.3rem;
}
.comment{
  line-height: 1.5rem;
}
.comment>div>div{
  color: #8dcbe2;
}
.comment>div>p{
  margin-bottom: 1rem;
}
.comment>div>p>strong{
  letter-spacing: 10px;
}
.comment>div>p>a{
  color: #653147;
  font-weight: bold;
  float: right;
  margin-right: 1rem;
  font-size: 15px;
}
.comment>div>p>a>span{
  display: inline-block;
  width: 0;
  height: 0;
  border: 4px solid;
  border-color: transparent  transparent transparent #653147;
  margin-left: 4px;
}
.pic{
  flex: 0 0 27%;
  background: #ededed;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding-bottom: 40px;
}
.pic img{
  width: 100%;
}
.login{
  text-align: right;
}
.login>div{
  margin-bottom: 15px;
  text-align: center;
}
.login label{
  display: inline-block;
  width: 4rem;
  text-align: left;
}
.login input{
  width: 12rem;
  border: 1px solid #869bac;
  height: 1.8rem;
  border-radius: 5px;
}
.login button{
  width: 4rem;
  height: 1.8rem;
  border-radius: 5px;
  border: none;
  background: #869bac;
  color: #fff;
  margin: 0 3rem 15px 0;
}
.login>a{
  color: #869bac;
  margin-right: 3rem;
  display: block;
}
</style>

<script>
// import tree from './components/tree.vue'

export default {
  name: 'App',
  // components: {
  //   tree
  // },
  data () {
    return {
      // data: data
    }
  }
}

// var data = {
//   name: 'My Tree',
//   children: [
//     { name: 'hello' },
//     { name: 'wat' },
//     {
//       name: 'child folder',
//       children: [
//         {
//           name: 'child folder',
//           children: [
//             { name: 'hello' },
//             { name: 'wat' }
//           ]
//         },
//         { name: 'hello' },
//         { name: 'wat' },
//         {
//           name: 'child folder',
//           children: [
//             { name: 'hello' },
//             { name: 'wat' }
//           ]
//         }
//       ]
//     }
//   ]
// }
</script>
