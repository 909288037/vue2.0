<template>
  <div>
    <div class="app-head">
      <div class="app-head-inner">
          <img src="../assets/logo.png">
          <p>Vue电商平台</p>
        <div class="head-nav">
          <ul class="nav-list">
            <li><a href="javascript:void(0);">登录</a></li>
            <li class="nav-pile">|</li>
            <li><a href="javascript:void(0);">注册</a></li>
            <li class="nav-pile">|</li>
            <li><a href="javascript:void(0);">关于</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="app-content">
      <keep-alive>
        <router-view></router-view>
      </keep-alive>
    </div>
    <div class="app-footer">
      <p>© 2017 Vue Study</p>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'app',
    data(){
        return{

        }
    }
  }
</script>

<style>
  /* http://meyerweb.com/eric/tools/css/reset/
   v2.0 | 20110126
   License: none (public domain)
*/

  html, body, div, span, applet, object, iframe,
  h1, h2, h3, h4, h5, h6, p, blockquote, pre,
  a, abbr, acronym, address, big, cite, code,
  del, dfn, em, img, ins, kbd, q, s, samp,
  small, strike, strong, sub, sup, tt, var,
  b, u, i, center,
  dl, dt, dd, ol, ul, li,
  fieldset, form, label, legend,
  table, caption, tbody, tfoot, thead, tr, th, td,
  article, aside, canvas, details, embed,
  figure, figcaption, footer, header, hgroup,
  menu, nav, output, ruby, section, summary,
  time, mark, audio, video {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
  }
  /* HTML5 display-role reset for older browsers */
  article, aside, details, figcaption, figure,
  footer, header, hgroup, menu, nav, section {
    display: block;
  }
  body {
    line-height: 1;
  }
  ol, ul {
    list-style: none;
  }
  blockquote, q {
    quotes: none;
  }
  blockquote:before, blockquote:after,
  q:before, q:after {
    content: '';
    content: none;
  }
  table {
    border-collapse: collapse;
    border-spacing: 0;
  }
  a {
    color: inherit;
    text-decoration: none;
  }
  body {
    background: #f0f2f5;
    font-family: "Helvetica Neue",Helvetica,Arial,"Hiragino Sans GB","Hiragino Sans GB W3","Microsoft YaHei UI","Microsoft YaHei","WenQuanYi Micro Hei",sans-serif;
    font-size: 14px;
    color: #444;
  }

  .app-head {
    background: #363636;
    color: #b2b2b2;
    height: 90px;
    line-height: 90px;
    width: 100%;
  }
  .app-head-inner {
    width: 90%;
    margin: 0 auto;
    overflow: hidden;
  }
  .app-head-inner img {
    width: 50px;
    margin-top: 20px;
    float: left;
  }
  .app-head-inner p{
    float: left;
    font-size: 24px;
    color: #ff6905;
    margin-left: 10px;
    cursor: pointer;
  }
  .head-nav {
    float: right;
  }
  .head-nav ul {
    overflow: hidden;
  }
  .head-nav li {
    /*cursor: pointer;*/
    float: left;
  }
  .head-nav li>a:hover {
    color: #fff9f0;
  }
  .nav-pile {
    padding: 0 10px;
  }
  .app-footer {
    text-align: center;
    height: 80px;
    width: 100%;
    line-height: 80px;
    background: #e3e4e8;
    clear: both;
    margin-top: 30px;
  }
</style>
