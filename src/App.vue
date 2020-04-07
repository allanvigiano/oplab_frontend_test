<template>
  <div class="container-fluid">
    <div class="row">
      <div class="bg-phone col-xs-12 col-sm-6 col-md-6 col-lg-6" id="phone"></div>
      <div class="col-xs-12 col-sm-6 col-md-6 col-lg-6" id="content">
        <div class="row">
          <div class="col-xs-12 content-logo">
            <img :src="imgSrc" alt="Logo" class="img-responsive" width="50px" height="50px" />
          </div>
          <div class="col-xs-12 content-text">
            <h4>MESSENGER FOR ANONYMOUS</h4>
            <h1 class="intro-text">Send voice and text message anonymously</h1>
            <p>Aria is a messenger for people who prefer anonymity. Chat, call and hangout with friends anonymously. Aria is a tor for private conversations. None can catch thou.</p>
            <h3>DOWNLOAD ARIA FOR FREE ON</h3>
            <a
              href="#"
              class="wow fadeInDown"
              data-wow-delay=".2s"
              style="visibility: visible; animation-delay: 0.2s; animation-name: fadeInDown;"
            >
              <img class="img-responsive anchor-icon" src="./assets/appstore.png" alt="Icon" />
            </a>
            <a
              href="#"
              class="wow fadeInDown"
              data-wow-delay=".2s"
              style="visibility: visible; animation-delay: 0.2s; animation-name: fadeInDown;"
            >
              <img class="img-responsive anchor-icon" src="./assets/playstore.png" alt="Icon" />
            </a>
          </div>
          <div class="col-xs-12 footer">
            <span class="footer-credits">© Aria Messenger 2016</span>
            <ul class="nav nav-pills pull-right">
              <li>
                <a href="#">Facebook</a>
              </li>
              <li>
                <a href="#">Twitter</a>
              </li>
              <li>
                <a href="#">Instagram</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import img from "./assets/app_icon.png";
export default {
  name: "app",
  data() {
    return {
      imgSrc: img
    };
  }
};
</script>

<style lang="less">
@import "../../node_modules/bootstrap/less/bootstrap.less";
@import "./less/variables.less";

@main-color: #6603c9;
//General
body::-webkit-scrollbar {
  display: none;
}
body {
  -ms-overflow-style: none;
}
::selection {
  color: #1106cc;
  background: #ffff99;
}
h4 {
  margin-top: 0px;
  display: block;
  //margin-block-start: 1.33em;
  margin-block-end: 1.33em;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  color: #a1a1a1;
  font-size: 14px;
  font-weight: 600;
  letter-spacing: 2px;
  text-transform: uppercase;
  line-height: 1.2;
}
/*****/

#content {
  padding-left: 50px;
  padding-right: 50px;
  > div {
    padding-top: 50px;
  }
}
#phone {
  min-height: 100vh;
  height: 100%;
  overflow-y: hidden;
  @media only screen and (min-width: 801px) {
    position: sticky;
    left: 0;
    top: 0;
  }
}
.anchor-icon {
  display: inline-block;
  margin-right: 15px;
}
/*.content > .row {
  div {
    @media only screen and (max-width: 801px) {
      //padding-top: 50px;
    }
    //padding-top: 100px;
  }
}*/
.content-logo {
  @media only screen and (max-width: 801px) {
    padding-bottom: 50px;
  }
  @media only screen and (min-width: 801px) {
    padding-bottom: 100px;
  }
}
.content-text {
  p {
    font-family: Poppins;
    font-size: 16px;
    font-weight: 400;
    color: #a1a1a1;
    letter-spacing: 0px;
    line-height: 1.5;
    margin: 0 0 20px 0;
  }
  h3 {
    font-family: Poppins;
    font-size: 16px;
    font-weight: 600;
    color: #434343;
    text-transform: uppercase;
    letter-spacing: 0;
    line-height: 1.2;
    margin: 50px 0 30px 0;
  }
  a img {
    width: 150px;
  }
}
.footer-credits {
  display: inline;
  font-family: Poppins;
  font-size: 12px;
  font-weight: 400;
  line-height: 1.5;
  color: #111111;
  text-align: right;
  text-decoration: none;
}
.footer {
  margin-top: 50px;
  margin-bottom: 20px;
}
.footer ul {
  display: inline-block;
  list-style-type: none;
  float: right !important;
}
.footer ul li a {
  display: inline;
  font-family: Poppins;
  font-size: 12px;
  font-weight: 400;
  //padding-right: 20px;
  color: #072def;
  text-decoration: none;
  &:hover {
    color: #6603c9;
    text-decoration: line-through;
    background: inherit;
  }
}
.bg-phone {
  background: url("./assets/bg1.png") no-repeat center center;
  background-size: cover;
}
.intro-text {
  color: @main-color;
  font-weight: 600;
  //font-family: Poppins;
  font-size: 42px;
  letter-spacing: -2px;
  line-height: 1.1;
  margin: 0 0 15px 0;
  letter-spacing: -2px;
}
</style>
