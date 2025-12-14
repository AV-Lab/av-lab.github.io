---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<head>
  <meta charset="UTF-8">
  <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;1,100;1,200;1,300;1,400;1,500;1,600;1,700&display=swap" rel="stylesheet">
</head>

<div class="container">
<div class="header-container"> 
    <h1 class='av-title typewriter'>
      <span class="typewriter-text"></span>
    </h1> 
    <div class="devops-icon" > 
      <a href="2-devops" >
      <img src="assets/img/devops icon.gif"/>
      </a>
    </div> 
    <div class="knowledge-base-icon"> 
      <a href="https://kb.avlab.io" target="_blank">
      <video autoplay muted loop >
        <source src="assets/kb-video.mp4" type="video/mp4">
      </video>
      </a>
    </div> 
</div>
<img class="small-banner"/> 
<div class="columns">
<div class="left-column">
  <p class="sum">
    At <a href="https://ku.ac.ae">Khalifa University's</a> Autonomous Vehicles Lab, our research focuses on advancing autonomous vehicle technology, prioritizing safety, seamless integration into smart urban environments, and ensuring AI systems are aligned with passenger needs.
  </p>
  <div class="questions">
  <p>Our key research areas include:</p>
  <ul>
    <li>Developing strategies to enhance the safety of key components in AV decision-making.</li>
    <li>Enabling multi-agent vehicles to safely and efficiently share perception and decision-making data, including epistemic and aleatoric uncertainties, through V2X industry standards.</li>
    <li>Designing decision-making frameworks that deliver strong safety assurances, grounded in rigorous theoretical validation.</li>
  </ul>
<!--.	 <a href="https://mindshield.ai"><img width="220" style="float: right; margin-top:-35px; margin-right:-18px" src="assets/img/mindshield-logo.gif"/></a> -->
  </div>
  
</div>
  <div class="right-column">
    <a href="3-research"><img src="/assets/banner-anim.gif"/></a>
  </div>
</div>
</div>


<style>

@font-face {
  font-family: 'Titr';
  src: url('/assets/fonts/titr-bold.ttf') format('truetype');
  font-weight: bold;
}

@font-face {
  font-family: 'Cairo';
  src: url('/assets/fonts/static/Cairo-Regular.ttf') format('truetype');
  font-weight: normal;
}

.container {
  display:flex;
  flex-direction: column; /* Ensure the container stacks its children vertically */
  position: relative;
  top:-28px;
}
.header-container {
  display: flex;
  align-items: center;
  height: 100%; /* Set height to 100% of the parent element */
  margin-bottom: -2px;
}
.knowledge-base-icon {
  cursor: pointer; /* Changes cursor to indicate the icon is clickable */
  border: solid 1.5px white;
}
.devops-icon{
  cursor: pointer; /* Changes cursor to indicate the icon is clickable */
}
.devops-icon img {
  width: 92px;
}
.knowledge-base-icon video {
  width: 200px;
  margin-bottom: -8px;
}

.devops-icon:hover{
  animation: moveL .5s forwards; /* Initial animation */
  transition: transform 1s ease-in-out; /* Smooth transition for transform property */
  opacity:.8;
}
.knowledge-base-icon:hover{
  animation: moveU .3s forwards; /* Initial animation */
  opacity:.8;
}

@keyframes moveL {
  0% { transform: translateX(0); }
  100% { transform: translateX(-10px); }
}
@keyframes moveU {
  0% { transform: translateZ(0px); }
  100% { transform: scale(1.05); }
}


.columns {
  display: flex;
}


.left-column,
.right-column {
  display: flex;
  flex-direction: column;
  height: 100%; /* Add this line */
  hyphens: auto;
  text-align: justify;
}

.left-column {
  flex: 60%;
  margin-right:1px;
}

.right-column {
  flex: 40%;
  min-width: 295.5px;
}
.right-column img {
  width: 100%;
}

.left-column ul {
  list-style-type: "‣ ";
  margin-top: -10px;
  margin-bottom: -10px;
}
.left-column li {
  padding-bottom: 10px;
}
.sum{
    margin-top: 3px;
    margin-bottom: 0px;
    color:#838996;
    background-color:#f5f5f5;
    /*background-color: #101357;*/
	padding-top: 20px;
	padding-bottom: 20px;
    padding-left: 20px;
    padding-right: 25px;
}
.right-column:hover{
    opacity:0.8;
  animation: moveU .3s forwards; /* Initial animation */
}

.sum:hover{
    background-color:#f8f8ff;
}
.questions{
  background-color:#a28089; /* #f9fbff ;*/
  /*color:#566968 ;*/
  color:#f9fbff;
  padding-top: 20px;
  padding-bottom:32px;
  padding-right:10px;
  padding-left:10px;
  padding-right: 25px;
  margin:0px;
}
.questions:hover{
  opacity: 80%;
    background-color: #566968 ;
    color:#f9fbff;
}




.small-banner{
  display: none;
  z-index: -1;
  margin: 0;
}


a{
    color: black;
}

.typewriter{
  overflow: hidden;
  white-space: nowrap;
  margin-bottom: 0px;
  display: block;
  font-size: clamp(1.5rem, 2vw, 1.9rem);
  font-family: "IBM Plex Mono", "Cairo", "Titr", monospace;
  min-height: 1.5em;
  flex: 1;
}

.typewriter-text {
  display: inline-block;
  animation: blink-caret .75s step-end infinite;
}

/* RTL-specific cursor positioning */
.typewriter.ltr {
  direction: ltr;
  text-align: left;
}

.typewriter.rtl {
  direction: rtl;
  text-align: right;
  padding-right: 10px;
}

.typewriter-text.ltr {
  border-right: .15em solid black;
  border-left: none;
  padding-right: 2px;
  padding-left: 0;
}

.typewriter-text.rtl {
  border-left: .15em solid black;
  border-right: none;
  padding-left: 2px;
  padding-right: 0;
  direction: rtl;
  unicode-bidi: bidi-override;
}

/* The typewriter cursor effect */
@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: black; }
}

@media (max-width: 650px) {
  .columns {
    display: flex;
  }

  .right-column {
    width: 100%;
    display: none;
  }

  .small-banner{
      display: block;
      content: url("assets/img/banner-small.png");
      z-index: -1;
  }
  .knowledge-base-icon{
    display: none;
  } 
  .devops-icon {
    display: none;
  }
  .type-writer{
    display: none;
  }
  .container{
    z-index: -1;
  }
}




</style>

<script>
const texts = [
  { text: "Autonomous Vehicles Lab", dir: "ltr" },
  { text: "مختبر المركبات ذاتية القيادة", dir: "rtl" }
];

const element = document.querySelector('.typewriter-text');
const container = document.querySelector('.typewriter');
let textIndex = 0;

function sleep(ms) {
  return new Promise(resolve => setTimeout(resolve, ms));
}

async function typeText(text, dir) {
  // Set direction classes on both container and text element
  container.className = 'av-title typewriter ' + dir;
  element.className = 'typewriter-text ' + dir;
  
  // Type in
  for (let i = 0; i <= text.length; i++) {
    element.textContent = text.substring(0, i);
    await sleep(80);
  }
  
  await sleep(2000); // Pause before erasing
  
  // Erase
  for (let i = text.length; i >= 0; i--) {
    element.textContent = text.substring(0, i);
    await sleep(50);
  }
  
  await sleep(500);
}

async function loop() {
  while (true) {
    await typeText(texts[textIndex].text, texts[textIndex].dir);
    textIndex = (textIndex + 1) % texts.length;
  }
}

loop();
</script>
