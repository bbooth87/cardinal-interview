<template>
  <div id="app">

    <header id="header">

      <div class="bg-header"></div>
      <div class="cd-wrapper">
        <div class = "cd-row-1">
          <div class ="cd-logo">
          <span><img src="./assets/logos/logo-cardinal.png"></span>
          </div>
        </div>

        <div class ="cd-row-2">
        <h1>Enjoy the proven success<br>
           of our experience.</h1>
      </div>

      </div>
    </header>

    <div class ="client-service-wrapper">
      <div class="cs-row-1">
        <div class ="cs-icon">
        <span><img src="./assets/icons/icon-bi.svg"></span>
        </div>
        <div class="cs-service-content">
          <h1> Business Intelligence</h1>
          <h3>
            We use technology to turn data into
            knowledge that can help you manage and
            monitor your business.
          </h3>
        </div>
        <div class ="cs-icon">
        <span><img src="./assets/icons/icon-appdev.svg"></span>
        </div>
        <div class="cs-service-content">
          <h1> App Development</h1>
          <h3>
            Our mobile specialists work to create rich,
            easy-to-use consumer or enterprise
            experiences for IOS or Android.
          </h3>
        </div><div class ="cs-icon">
        <span><img src="./assets/icons/icon-ba.svg"></span>
        </div>
        <div class="cs-service-content">
          <h1> Business Analysis</h1>
          <h3>
            Great strategy begins with listening. We
            learn about businesses from the inside out,
            and then propose improvements.
          </h3>
        </div>

      </div>
      <div class="cs-row-2">
        <div class="cs-row-2-top">


        <div class ="client-box">
          <h1> Our Clients</h1>
          <h3>
            Over the years, our team has had the distinction
             of working with a variety of brands in different industries.
             Here is a short list of some of the names we have worked with.
          </h3>
        </div>

        <div class ="cs-logo">
        <span><img src="./assets/logos/logo-fifththird.png"></span>
        </div>

        <div class ="cs-logo">
        <span><img src="./assets/logos/logo-chhn.png"></span>
        </div>
        </div>
        <div class="cs-row-2-bottom">

        <div class ="cs-logo">
        <span><img src="./assets/logos/logo-chs.png"></span>
        </div>

        <div class ="cs-logo">
        <span><img src="./assets/logos/logo-skanska.png"></span>
        </div>

        <div class ="cs-logo">
        <span><img src="./assets/logos/logo-pg.png"></span>
        </div>

        <div class ="cs-logo">
        <span><img src="./assets/logos/logo-rackroom.png"></span>
        </div>
        </div>

      </div>


    </div>
    <div class="purell-section">


    <div class="purell-bg"></div>
    <div class="purell-wrapper">



      <div class = "purell-pic">
        <img src= "./assets/images/pic-gojo.png">

      </div>

      <div>

      </div>



    </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {

    }
  }
}
</script>

<style lang="scss">
@font-face {
	font-family: 'Effra Std Bd';
	src: url('./assets/fonts/Effra_Std_Bd.ttf');
}
@font-face {
	font-family: 'Effra Std Lt';
	src: url('./assets/fonts/Effra_Std_Lt.ttf');
}
@font-face {
	font-family: 'Effra Std Md';
	src: url('./assets/fonts/Effra_Std_Md.ttf');
}
@font-face {
	font-family: 'Effra Std Rg';
	src: url('./assets/fonts/Effra_Std_Rg.ttf');
}
#app {

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

body {
  margin: 0;
  font-size: 1.1em;
  text-align: center;
}


// Header/Top Section
#header{
  display: grid;
  min-height: 450px;
  color: #fff;
  text-align: center;
  line-height: 3em;
}
.cd-logo span > img {
  width: 10em;
  padding-top: 15%;
  margin: auto;
}
.cd-wrapper{
  display:grid;
  grid-row-gap:.5em;
}
.cd-wrapper h1{
  font-family: 'Effra Std Rg';
  font-size: 2.2em;
  color: #fff;
}
.cd-logo{
  align-self: start;
}
#header .cd-wrapper{
  padding: 0 1.5em;
}
#header .bg-header {
  position: absolute;
  background:
    url("./assets/images/cardinal-bg.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
  height: 450px;
  z-index: -1;
  &:before {
   content: '';
   position: absolute;
   top: 0;
   right: 0;
   bottom: 0;
   left: 0;
   background: linear-gradient(to bottom right, #0D588D, #057CC4);
   opacity: .93;
}
}
// Client and Services Section
.client-service-wrapper{
  display: grid;
}

// .client-service-wrapper h1, .client-service-wrapper h3{
//   padding: 1.5em;
// }
.cs-row-1{
  display: grid;
  background-color: #f0f0f0;
  padding-top: 1em;
  text-align: center;
  padding-bottom: 10em;
}

.cs-service-content{
  font-family: 'Effra Std Rg';
  font-size: 75%;
  line-height: 1.5em;
}
.cs-service-content h3{
  margin-top: -1px;
  font-size: 1.25em;
}
.cs-icon span > img{
  width: 2.5em;
  margin: auto;
}

.cs-row-2{
  display: grid;
  text-align: center;
  grid-gap:1em;
  width: auto;
}
.cs-row-2-top{
  display: grid;
  margin-top: -5em;
  grid-gap:1em;
}
.cs-row-2-bottom{
  display: grid;
  grid-gap:1em;
}
div.client-box{
  background-color: #383d49;
  color: #FFF;
  font-family: 'Effra Std Rg';
  font-size: 75%;
  line-height: 1.5em;
  margin: auto;
  width: 80%;
}
// .logo-div{
//   display: grid;
// }
// .cs-logo{
//
// }
.cs-logo span > img{
  margin: auto;
  width: 70%;
  background-color:white;
  font-size: .75em;
  border: 2px solid #eaeaea;
  justify-content: center;
  padding: 1.5em;
  height: 4em;
}
// purell div

.purell-bg{
  position: absolute;
  background:
    url("./assets/images/pic-gojo-bg.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
  height: 450px;
  z-index: -1;
}
.purell-wrapper{
  display: grid;
  grid-template-columns:repeat(2, 1fr);
}
.purell-pic > img{
  width: 100%;
  height: 100%;
  padding-top: 4em;
  padding-left: 2em;
}
.purell-section{
  height: 450px;
}

// desktop styles
@media only screen and (min-width: 768px) {
  .cd-logo span > img {
    width: 8em;
    margin: auto;
  }
  .cd-wrapper h1{
    font-size: 3em;
  }

  .cd-row-1{
    display: grid;
    grid-template-areas:
    "lg . . . "
    ". . . .";
  }
  .cs-row-1{
    grid-template-columns:repeat(3, 1fr 3fr);
    padding-right: 1.5em;
  }
  .cs-row-2-top{
    grid-template-columns: 2fr 1fr 1fr;
    margin-top: -1em;
  }
  .cs-row-2-bottom{
    grid-template-columns:repeat(4, 1fr);
  }
  .cs-logo{
    border: 2px solid #eaeaea;
    background-color:white;
  }
  .cs-logo span > img{
    margin: auto;
    height: 80%;
    width: 80%;
    border: hidden;
    justify-content: center;
    padding: 1.5em;
    // justify-self: center;
    // align-self: center;
    height: 4em;
  }
  div.client-box{
    width: 100%;
    margin-left: 1em;
    margin-right:1em;
  }
}

img {
  display: block;
  width: 100%;
  height: auto;
}

h1, h2, h3 {
  margin: 0;
  padding: 1em 0;
}

a {
  color: #42b983;
}
</style>
