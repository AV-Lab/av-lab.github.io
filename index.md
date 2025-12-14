---
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

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
<span class="avlab-badge">SAFETY-CRITICAL AUTONOMY</span>
    At <a href="https://ku.ac.ae">Khalifa University</a>, we study safe autonomy under realistic uncertainty and deployment constraints, combining formal methods and real-world validation for safety-critical systems.
  </p>
  <div class="questions">
  <span class="section-label">Research Focus</span>
  <ul>
    <li><strong>Decision-making safety:</strong> Formal analysis of autonomous decision pipelines, including failure modes, safety guarantees, and verification under uncertainty.</li>
    <li><strong>Multi-agent coordination:</strong> Coordination and information sharing under uncertainty, including communication constraints and trust assumptions.</li>
    <li><strong>Risk-bounded planning:</strong> Planning and control methods that explicitly encode risk, enabling safety guarantees rather than empirical tuning.</li>
  </ul>
<!--.	 <a href="https://mindshield.ai"><img width="220" style="float: right; margin-top:-35px; margin-right:-18px" src="assets/img/mindshield-logo.gif"/></a> -->
  </div>
  
</div>
  <div class="right-column">

    <a href="3-research"><img src="/assets/banner-anim.gif"/></a>

  </div>
</div>
</div>


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
