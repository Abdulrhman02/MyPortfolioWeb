<div class="container">
  <div class="box">
    <span />
    <div class="content">
      <h3>Abdulrhman Ali Al-Ghamdi</h3>
    </div>
  </div>
</div>

<div class="content2">
  <div class="content__container">
    <p class="content__container__text">Coming Soon</p>

    <!-- <ul class="content__container__list">
		<li class="content__container__list__item">FrontEnd Developer</li>
		<li class="content__container__list__item">Mobile Developer</li>
		<li class="content__container__list__item">Software Engineer</li>
		<li class="content__container__list__item">FullStack Developer</li>
	  </ul> -->
  </div>
</div>

<!-- <h4>Technical Skills</h4>
  <div class=" test">
	<h1>Web framework</h1>
  
	<span class="content v2"><p>Svelte</p></span>
	<span class="content v2"><p>Vue.js</p></span>
	<span class="content v2"><p>Vanilla</p></span>
  </div>
  <div class=" test">
	<h1>Mobile framework</h1>
  
	<span class="content v2"><p>Flutter</p></span>
	<span class="content v2"><p>Android</p></span>
  </div>
  <div class=" test">
	<h1>Programming languages</h1>
  
	<span class="content v2"><p>Dart</p></span>
	<span class="content v2"><p>Java</p></span>
	<span class="content v2"><p>C++</p></span>
	<span class="content v2"><p>HTML</p></span>
	<span class="content v2"><p>CSS</p></span>
	<span class="content v2"><p>JavaScript</p></span>
  </div>
  <div class=" test">
	<h1>Back End framework</h1>
  
	<span class="content v2"><p>FireBase</p></span>
	<span class="content v2"><p>SQL</p></span>
	<span class="content v2"><p>REST API</p></span>
  </div>
  <div class=" test">
	<h1>Other</h1>
  
	<span class="content v2"><p>Wordepress</p></span>
  </div> -->

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: consolas;
  }
  h1 {
    color: #00d0ff;
    margin-bottom: 10px;
  }
  h4 {
    color: #00d0ff;
    font-size: 2vw;
    margin-left: 10%;
  }

  /* :global(body) {
	   display: flex;
		  justify-content: center;
		  align-items: center; 
	  min-height: 100vh;
	  background: #060d1d;
	} */

  .container {
    display: flex;
    justify-content: left;
    align-items: center;
    padding: 40px 0;
  }

  .container .box {
    position: relative;
    width: 32vw;
    height: 10vw;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 4vw 3vw;
    transition: 0.5s;
  }

  .container .box::before {
    content: " ";
    position: absolute;
    top: 0;
    left: 50px;
    width: 50%;
    height: 100%;
    text-decoration: none;
    background: #fff;
    border-radius: 8px;
    transform: skewX(15deg);
    transition: 0.5s;
  }

  .container .box::after {
    content: "";
    position: absolute;
    top: 0;
    left: 50;
    width: 50%;
    height: 100%;
    background: #fff;
    border-radius: 8px;
    transform: skewX(15deg);
    transition: 0.5s;
    filter: blur(30px);
  }

  .container .box:hover:before,
  .container .box:hover:after {
    transform: skewX(0deg);
    left: 20px;
    width: calc(100% - 90px);
  }

  .container .box:nth-child(1):before,
  .container .box:nth-child(1):after {
    background: linear-gradient(315deg, #4bd8a2, #7f3fac);
  }

  .container .box:nth-child(3):before,
  .container .box:nth-child(3):after {
    background: linear-gradient(315deg, #4dff03, #00d0ff);
  }

  .container .box span {
    display: block;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: 5;
    pointer-events: none;
  }

  .container .box span::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 0;
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(10px);
    opacity: 0;
    transition: 0.1s;
    animation: animate 2s ease-in-out infinite;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
  }

  .container .box:hover span::before {
    top: -50px;
    left: 20px;
    width: 50px;
    height: 50px;
    opacity: 1;
  }

  .container .box span::after {
    content: "";
    position: absolute;
    bottom: 0;
    right: 0;
    width: 100%;
    height: 100%;
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(10px);
    opacity: 0;
    transition: 0.5s;
    animation: animate 2s ease-in-out infinite;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
    animation-delay: -1s;
  }

  .container .box:hover span:after {
    bottom: -20px;
    right: 50px;
    width: 50px;
    height: 50px;
    opacity: 1;
  }

  @keyframes animate {
    0%,
    100% {
      transform: translateY(10px);
    }

    50% {
      transform: translate(-10px);
    }
  }

  .container .box .content {
    position: relative;
    left: 0;
    padding: 2vw 3.5vw;
    background: rgba(255, 255, 255, 0.05);
    backdrop-filter: blur(10px);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    z-index: 1;
    transform: 0.5s;
    color: #fff;
  }

  .container .box .content h3 {
    font-size: 2vw;
    color: #fff;
    /* margin-bottom: 10px; */
  }

  .container .box .content p {
    font-size: 1.1em;
    margin-bottom: 10px;
    line-height: 1.4em;
  }

  /* .container .box .content a {
		  display: inline-block;
		  font-size: 1.1em;
		  color: #111;
		  background: #fff;
		  padding: 10px;
		  border-radius: 4px;
		  text-decoration: none;
		  font-weight: 700;
		  margin-top: 5px;
	  } */

  /* .container .box .content a:hover {
		  background: #ffcf4d;
		  border: 1px solid rgba(255, 0, 88, 0.4);
		  box-shadow: 0 1px 15px rgba(1, 1, 1, 0.2);
	  } */

  .content p {
    font-size: 2em;
    display: inline;
    background-repeat: no-repeat;
    transition: all 300ms ease-in-out;
  }
  .v2 p {
    color: #00d0ff;
    background-position: left;
    background-size: 0% 100%;
    border-radius: 8px;
    padding: 5px 15px;
    background-image: linear-gradient(
      315deg,
      rgba(75, 216, 162, 0.2),
      rgba(127, 63, 172, 0.2)
    );
  }
  .v2:hover p {
    background-size: 100% 100%;
  }
  .test {
    margin: 2% 10%;
    font-size: 0.8vw;
  }

  .content2 {
    height: 20vw;
    margin-top: 10%;
    display: flex;
    justify-content: center;
    /* font-family: 'Lato', sans-serif; */
    font-size: 3vw;
    /* line-height: 4vw; */
    /* color: #ffffff; */
  }
  .content__container {
    font-weight: 600;
    overflow: hidden;
    height: 4vw;
    padding: 0 4vw;
  }
  .content__container__text {
    display: inline;
    float: left;
    margin: 0;
  }
  .content__container__list {
    margin-top: 0;
    padding-left: 10vw;
    text-align: left;
    list-style: none;
    -webkit-animation-name: change;
    -webkit-animation-duration: 10s;
    -webkit-animation-iteration-count: infinite;
    animation-name: change;
    animation-duration: 10s;
    animation-iteration-count: infinite;
  }
  @-webkit-keyframes change {
    0%,
    12.66%,
    100% {
      transform: translate3d(0, 0, 0);
    }
    16.66%,
    29.32% {
      transform: translate3d(0, -25%, 0);
    }
    33.32%,
    45.98% {
      transform: translate3d(0, -50%, 0);
    }
    49.98%,
    62.64% {
      transform: translate3d(0, -75%, 0);
    }
    66.64%,
    79.3% {
      transform: translate3d(0, -50%, 0);
    }
    83.3%,
    95.96% {
      transform: translate3d(0, -25%, 0);
    }
  }
</style>
