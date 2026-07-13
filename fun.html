<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>THE BUTTON OF ULTIMATE CHAOS™</title>
<style>
  * { box-sizing: border-box; }
  html, body {
    margin: 0; padding: 0; height: 100%; overflow: hidden;
    font-family: 'Comic Sans MS', 'Arial Black', sans-serif;
    background: linear-gradient(270deg, #ff0000, #ff9900, #ffee00, #33ff00, #00fff2, #0033ff, #cc00ff, #ff0000);
    background-size: 1600% 1600%;
    animation: rainbow 8s linear infinite;
    text-align: center;
    user-select: none;
  }
  @keyframes rainbow {
    0% { background-position: 0% 50%; }
    100% { background-position: 100% 50%; }
  }
  h1 {
    color: white;
    -webkit-text-stroke: 2px black;
    font-size: 3em;
    margin-top: 20px;
    animation: wiggle 0.6s infinite alternate;
    text-shadow: 4px 4px 0 #000;
  }
  @keyframes wiggle {
    0% { transform: rotate(-3deg) scale(1); }
    100% { transform: rotate(3deg) scale(1.05); }
  }
  #score {
    font-size: 1.5em;
    color: white;
    -webkit-text-stroke: 1px black;
    margin-bottom: 10px;
  }
  #msg {
    font-size: 1.8em;
    color: #fff;
    -webkit-text-stroke: 1px black;
    min-height: 50px;
    margin-bottom: 10px;
    transition: transform 0.2s;
  }
  #chaosBtn {
    font-size: 2.5em;
    padding: 30px 60px;
    border-radius: 50px;
    border: 8px solid black;
    background: gold;
    cursor: pointer;
    box-shadow: 0 10px 0 #b8860b;
    font-weight: bold;
    transition: transform 0.1s;
    animation: pulse 1s infinite;
  }
  @keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.08); }
  }
  #chaosBtn:active {
    transform: scale(0.9) translateY(10px);
    box-shadow: none;
  }
  .float {
    position: fixed;
    font-size: 40px;
    pointer-events: none;
    top: -50px;
    z-index: 999;
    animation: fall linear forwards;
  }
  @keyframes fall {
    to { transform: translateY(110vh) rotate(720deg); }
  }
  #achievements {
    color: white;
    font-size: 1em;
    margin-top: 10px;
    -webkit-text-stroke: 0.5px black;
  }
  .shake {
    animation: screenshake 0.4s;
  }
  @keyframes screenshake {
    0% { transform: translate(0,0) rotate(0); }
    20% { transform: translate(-15px,10px) rotate(-2deg); }
    40% { transform: translate(15px,-10px) rotate(2deg); }
    60% { transform: translate(-10px,15px) rotate(-1deg); }
    80% { transform: translate(10px,-15px) rotate(1deg); }
    100% { transform: translate(0,0) rotate(0); }
  }
  #flashOverlay {
    position: fixed; top:0; left:0; width:100%; height:100%;
    background: white; opacity: 0; pointer-events: none; z-index: 9999;
  }
</style>
</head>
<body>
<div id="flashOverlay"></div>
<h1>🎪 THE BUTTON OF ULTIMATE CHAOS™ 🎪</h1>
<div id="score">Chaos Points: 0</div>
<div id="msg">Press the button. I dare you.</div>
<button id="chaosBtn">DO NOT PRESS 🚨</button>
<div id="achievements"></div>

<script>
const body = document.body;
const btn = document.getElementById('chaosBtn');
const msg = document.getElementById('msg');
const scoreEl = document.getElementById('score');
const ach = document.getElementById('achievements');
const flash = document.getElementById('flashOverlay');

let score = 0;
let clicks = 0;

const messages = [
  "You absolute legend, you clicked it.",
  "Congratulations, you now own 3 invisible goats.",
  "A wizard somewhere just sneezed because of you.",
  "The button is judging your life choices.",
  "You have unlocked: mild chaos.",
  "Somewhere, a printer is jamming. You did that.",
  "The button says: 'meh, do it again.'",
  "You just gained +1 imaginary friend.",
  "Scientists are baffled. Click again.",
  "A pigeon outside just gained sentience.",
  "You have been legally declared 12% more chaotic.",
  "This click has been reported to the moon.",
  "Achievement unlocked: Button Toucher.",
  "You feel a disturbance in the snack force.",
  "The universe shrugged. Then clapped.",
  "Your left sock is now missing. Coincidence?",
  "You just made a cat somewhere very confused.",
  "This is fine. Everything is fine. Click again.",
  "Warning: excessive awesomeness detected.",
  "A tiny gremlin high-fived your mouse hand."
];

const emojis = ["🎉","🌈","🔥","💥","🐸","🦄","🍕","👽","🎩","💩","🚀","🐙","🍩","👑","🤡","🪩","🧃","🛸"];

const bgFilters = [
  "hue-rotate(90deg)",
  "invert(1)",
  "saturate(5)",
  "contrast(2)",
  "grayscale(1)",
  "blur(2px)",
  "sepia(1)",
  "hue-rotate(200deg) saturate(3)",
  ""
];

const cursors = ["crosshair","grab","zoom-in","help","not-allowed","wait","cell",""];

function randomFloatEmoji() {
  const el = document.createElement('div');
  el.className = 'float';
  el.textContent = emojis[Math.floor(Math.random()*emojis.length)];
  el.style.left = Math.random()*100 + "vw";
  el.style.fontSize = (20 + Math.random()*50) + "px";
  el.style.animationDuration = (1.5 + Math.random()*2) + "s";
  body.appendChild(el);
  setTimeout(() => el.remove(), 4000);
}

function emojiBurst(n) {
  for (let i=0;i<n;i++) {
    setTimeout(randomFloatEmoji, i*40);
  }
}

function doScreenShake() {
  body.classList.remove('shake');
  void body.offsetWidth; // reflow to restart animation
  body.classList.add('shake');
}

function doFlash() {
  flash.style.transition = 'none';
  flash.style.opacity = '0.8';
  requestAnimationFrame(() => {
    flash.style.transition = 'opacity 0.5s';
    flash.style.opacity = '0';
  });
}

function randomFilter() {
  body.style.filter = bgFilters[Math.floor(Math.random()*bgFilters.length)];
}

function randomCursor() {
  body.style.cursor = cursors[Math.floor(Math.random()*cursors.length)];
}

function spinBody() {
  body.style.transition = 'transform 0.8s';
  body.style.transform = 'rotate(' + (Math.random()>0.5?360:-360) + 'deg)';
  setTimeout(() => { body.style.transition='none'; body.style.transform='rotate(0deg)'; }, 850);
}

function growBtn() {
  const scale = 0.7 + Math.random()*1.5;
  btn.style.transform = 'scale(' + scale + ') rotate(' + (Math.random()*40-20) + 'deg)';
  setTimeout(() => { btn.style.transform=''; }, 400);
}

function renameBtn() {
  const names = ["DO NOT PRESS 🚨","PRESS AGAIN 😈","WHY ARE YOU STILL HERE","OK ONE MORE TIME","IT TICKLES","STOP. OR DON'T.","MORE CHAOS PLZ","BUTTON GO BRRR","FINE, AGAIN","🚨 SIREN NOISES 🚨"];
  btn.textContent = names[Math.floor(Math.random()*names.length)];
}

const achievementsList = [
  {n: 1, text: "🏅 Achievement: First Click!"},
  {n: 5, text: "🏅 Achievement: Mildly Concerning."},
  {n: 15, text: "🏅 Achievement: Chaos Enthusiast."},
  {n: 30, text: "🏅 Achievement: The Button Fears You."},
  {n: 50, text: "🏅 Achievement: Certified Menace."},
  {n: 100, text: "🏅 Achievement: You Should Touch Grass."}
];

function checkAchievements() {
  const found = achievementsList.find(a => a.n === clicks);
  if (found) {
    ach.textContent = found.text;
    ach.style.animation = 'none';
    void ach.offsetWidth;
    ach.style.animation = 'wiggle 0.4s ease';
  }
}

const chaosActions = [
  () => { doScreenShake(); },
  () => { emojiBurst(15); },
  () => { randomFilter(); setTimeout(()=>body.style.filter='', 1200); },
  () => { randomCursor(); },
  () => { spinBody(); },
  () => { doFlash(); },
  () => { growBtn(); }
];

btn.addEventListener('click', () => {
  clicks++;
  score += Math.floor(Math.random()*10)+1;
  scoreEl.textContent = "Chaos Points: " + score;
  msg.textContent = messages[Math.floor(Math.random()*messages.length)];
  renameBtn();

  // fire a random 2-3 chaos actions each click
  const shuffled = [...chaosActions].sort(()=>Math.random()-0.5);
  const count = 2 + Math.floor(Math.random()*2);
  for (let i=0;i<count;i++) shuffled[i]();

  checkAchievements();
});

// idle chaos: random emoji drizzle every few seconds just because
setInterval(() => {
  if (Math.random() < 0.5) randomFloatEmoji();
}, 1500);
</script>
</body>
</html>
