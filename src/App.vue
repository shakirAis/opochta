<template>
  <div id="app">
    <div class="menu">
      <div class="header_logo_wrapper">
        <a class="header_logo" href="#"></a>
      </div>
      <ul>
        <li>
          <a href="">О сервисе</a>
        </li>
        <li>
          <a href="">Документация</a>
        </li>
        <li>
          <a href="">Стоимость</a>
        </li>
        <li>
          <a href="">Контакты</a>
        </li>
      </ul>
    </div>
    <router-view/>
  </div>
</template>
<script>
export default {
  name: 'App',
};
</script>
<style>
@font-face {
  font-family: Raleway-Regular;
  src: url(./assets/fonts/Raleway-Regular/Raleway-Regular.ttf);
  src: url(./assets/fonts/Raleway-Regular/Raleway-Regular.eot);
  src: url(./assets/fonts/Raleway-Regular/Raleway-Regular.eot?#iefix) format('embedded-opentype'),
      url(./assets/fonts/Raleway-Regular/Raleway-Regular.svg#Raleway-Regular) format('svg'),
      url(./assets/fonts/Raleway-Regular/Raleway-Regular.woff) format('woff'),
      url(./assets/fonts/Raleway-Regular/Raleway-Regular.woff2) format('woff2');
  font-weight: normal;
  font-style: normal;
}
@font-face {
  font-family: Raleway-Medium;
  src: url(./assets/fonts/Raleway-Medium/Raleway-Medium.ttf);
  src: url(./assets/fonts/Raleway-Medium/Raleway-Medium.eot);
  src: url(./assets/fonts/Raleway-Medium/Raleway-Medium.eot?#iefix) format('embedded-opentype'),
      url(./assets/fonts/Raleway-Medium/Raleway-Medium.svg#Raleway-Medium) format('svg'),
      url(./assets/fonts/Raleway-Medium/Raleway-Medium.woff) format('woff'),
      url(./assets/fonts/Raleway-Medium/Raleway-Medium.woff2) format('woff2');
  font-weight: normal;
  font-style: normal;
}
@font-face {
  font-family: Raleway-SemiBold;
  src: url(./assets/fonts/Raleway-SemiBold/Raleway-SemiBold.ttf);
  src: url(./assets/fonts/Raleway-SemiBold/Raleway-SemiBold.eot);
  src: url(./assets/fonts/Raleway-SemiBold/Raleway-SemiBold.eot?#iefix) format('embedded-opentype'),
      url(./assets/fonts/Raleway-SemiBold/Raleway-SemiBold.svg#Raleway-SemiBold) format('svg'),
      url(./assets/fonts/Raleway-SemiBold/Raleway-SemiBold.woff) format('woff'),
      url(./assets/fonts/Raleway-SemiBold/Raleway-SemiBold.woff2) format('woff2');
  font-weight: normal;
  font-style: normal;
}
@font-face {
  font-family: Raleway-SemiBoldItalic;
  src: url(./assets/fonts/Raleway-SemiBoldItalic/Raleway-SemiBoldItalic.ttf);
  src: url(./assets/fonts/Raleway-SemiBoldItalic/Raleway-SemiBoldItalic.eot);
  src: url(./assets/fonts/Raleway-SemiBoldItalic/Raleway-SemiBoldItalic.woff) format('woff'),
    url(./assets/fonts/Raleway-SemiBoldItalic/Raleway-SemiBoldItalic.woff2) format('woff2');
  font-weight: normal;
  font-style: normal;
}
body {
  background-color: rgba(19,13,68, 97);
  margin: 0;
  padding: 0;
  font-variant-numeric: lining-nums;
}
#app {
  color: #FFF3F3;
  position: relative;
  margin: 0;
}
.menu {
  margin: 0;
  display: block;
  height: 90px;
  margin-top: 20px;
}
.menu ul {
  list-style-type: none;
  padding-left: 0;
  margin: 0;
  height: 90px;
  display: block;
  position: absolute;
  right: 0;
  top: 0;
}
.menu ul li a {
  font-family: 'Open Sans';
  font-size: 28px;
  color: #FFF3F3;
  text-decoration: none;
  display: table-cell;
  height: 30px;
  vertical-align: middle;
  letter-spacing: -2px;
}
.menu ul li a:after {
  content: '';
  width: 0px;
  height: 1px;
  display: block;
  background: #13BEBB;
  transition: 300ms;
}
.menu ul li a:hover:after {
  width: 100%;
}
.menu ul li a:hover {
  color: #13BEBB;
}
.menu ul li {
  width: auto;
  height: 90px;
  display: inline-table;
  margin-right: 50px;
}
a.header_logo {
  background-image: url(./assets/img/OPochta.svg);
  width: 300px;
  height: 90px;
  background-repeat: no-repeat;
  background-position: center center;
  display: inline-block;
}
.header_logo_wrapper {
  height: 90px;
  display: block;
  position: absolute;
  left: 0;
  top: 0;
}
</style>
