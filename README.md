<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Para mis personitas favoritas 💚</title>
<style>
:root{
  --lime:#b7ff3c;
  --lime2:#d9ff8b;
  --deep:#183b20;
  --ink:#25442b;
  --cream:#fbfff3;
}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{
  margin:0; min-height:100vh; overflow-x:hidden;
  font-family:Georgia,'Times New Roman',serif; color:var(--ink);
  background:radial-gradient(circle at 15% 15%,#efffc8 0,transparent 28%),
             radial-gradient(circle at 85% 80%,#c9ff72 0,transparent 30%),
             linear-gradient(135deg,#f7ffe8,#dfff9d 55%,#f4ffd9);
}
button{font:inherit}
.star{position:fixed;z-index:0;pointer-events:none;color:#7dbd25;opacity:.5;animation:twinkle 3s ease-in-out infinite alternate}
@keyframes twinkle{from{transform:scale(.7) rotate(0);opacity:.2}to{transform:scale(1.25) rotate(18deg);opacity:.85}}
.heart{position:fixed;bottom:-40px;z-index:0;pointer-events:none;animation:floatUp linear forwards;opacity:.7}
@keyframes floatUp{to{transform:translateY(-115vh) rotate(360deg);opacity:0}}
main{position:relative;z-index:1;width:min(920px,94%);margin:auto;padding:38px 0 28px;text-align:center}
.tag{display:inline-block;border:1px solid #a4d94e;background:#f7ffdfb8;border-radius:999px;padding:8px 15px;font:700 12px Arial,sans-serif;letter-spacing:2px;text-transform:uppercase;color:#537d20}
h1{font-size:clamp(2.25rem,7vw,4.5rem);line-height:1.04;margin:20px auto 14px;color:var(--deep)}
h1 span{color:#72a91b}
.intro{max-width:610px;margin:0 auto 24px;line-height:1.7;font-size:1.05rem}
.panel{background:#ffffffb8;border:1px solid #c8ed8b;box-shadow:0 20px 55px #527e2220;border-radius:28px;padding:clamp(20px,5vw,42px);backdrop-filter:blur(8px)}
.gift-wrap{height:220px;display:grid;place-items:center;margin:4px auto 12px}
.gift{width:150px;height:115px;position:relative;cursor:pointer;filter:drop-shadow(0 12px 10px #5a811f28);transition:transform .25s}
.gift:hover{transform:translateY(-5px) rotate(-2deg)}
.box{position:absolute;bottom:0;left:10px;width:130px;height:88px;border-radius:7px;background:linear-gradient(135deg,#a5ef31,#79c91b);border:2px solid #5f9d17}
.box:before{content:"";position:absolute;left:47px;top:0;width:28px;height:100%;background:#f8ffe9}
.lid{position:absolute;top:18px;left:0;width:150px;height:27px;border-radius:6px;background:#caff67;border:2px solid #6eab1d;z-index:2;transition:transform .6s}
.ribbon{position:absolute;z-index:3;top:-3px;left:56px;width:38px;height:25px;border:7px solid #f8ffe9;border-radius:50%;transform:rotate(-15deg)}
.ribbon:after{content:"";position:absolute;left:10px;top:-5px;width:38px;height:25px;border:7px solid #f8ffe9;border-radius:50%;transform:rotate(35deg)}
.gift.open .lid{transform:translate(-12px,-45px) rotate(-18deg)}
.gift.open{animation:bounce .55s ease}
@keyframes bounce{50%{transform:scale(1.08)}}
.gift-note{font-size:.95rem;color:#577b30;margin:0 0 12px}
.btn{border:0;border-radius:999px;padding:13px 22px;background:var(--deep);color:#f5ffd9;cursor:pointer;font-weight:bold;box-shadow:0 8px 20px #1c4a2222;transition:.2s;margin:6px}
.btn:hover{transform:translateY(-2px);background:#2f612b}
.btn.alt{background:#e9ffc2;color:#294d1b;border:1px solid #b5df71}
.hidden{display:none!important}
.reveal{animation:reveal .8s ease both}
@keyframes reveal{from{opacity:0;transform:translateY(18px)}to{opacity:1;transform:translateY(0)}}
.letter{margin-top:26px;text-align:left;background:var(--cream);border:1px solid #d4efad;border-radius:18px;padding:clamp(22px,5vw,42px);line-height:1.9;box-shadow:inset 0 0 0 6px #f2ffdf}
.letter h2{text-align:center;color:#477a1c;font-size:clamp(1.7rem,5vw,2.4rem);margin:0 0 24px}
.letter p{margin:0 0 16px}
.letter .sign{text-align:right;color:#4d811d;font-size:1.2rem;font-style:italic;margin-top:25px}
.divider{text-align:center;color:#8abf3d;letter-spacing:9px;margin:22px 0}
footer{font:13px Arial,sans-serif;color:#52742c;margin:28px 0 4px}
.music-note{font-size:.86rem;color:#5b7939;margin-top:8px}
@media(max-width:500px){main{padding-top:24px}.gift-wrap{height:190px}.panel{border-radius:22px}.letter{line-height:1.8}}
</style>
</head>
<body>
<main>
  <div class="tag">hecho con cariño · para mis kps</div>
  <h1>Una cosita para<br><span>mis personas favoritas 💚</span></h1>
  <p class="intro">Hay cosas que a veces no digo en voz alta, así que preparé este pequeño rincón para ustedes. Tienen que abrir el regalo… 👀</p>

  <section class="panel">
    <div class="gift-wrap">
      <div class="gift" id="gift" role="button" tabindex="0" aria-label="Abrir regalo" onclick="openGift()">
        <div class="lid"></div><div class="ribbon"></div><div class="box"></div>
      </div>
    </div>
    <p class="gift-note" id="giftNote">🎁 Un regalito para ustedes. Toca la cajita.</p>
    <button class="btn" id="openBtn" onclick="openGift()">Abrir mi regalo ✨</button>
    <div id="afterGift" class="hidden">
      <div class="divider">✦ ✧ ✦</div>
      <h2 style="color:#315d20">¡Sorpresaaaa! 💚</h2>
      <p style="line-height:1.7">El regalo más lindo es poder compartir momentos con ustedes. Y ahora sí… hay una cartita que quiero que lean.</p>
      <button class="btn" onclick="showLetter()">Leer la cartita 💌</button>
    </div>
    <article class="letter hidden" id="letter">
      <h2>Para los mejor, con todo mi cariño 💌</h2>
      <p>Weno dia. 💚</p>
      <p>Hice esta cartita porque quería recordarles algo que quizá no digo tan seguido: <strong>ustedes son muy importantes para mí</strong>, y me alegra muchísimo que formen parte de mi vida.</p>
      <p>Gracias por cada risa, cada conversación, cada tontería que termina convirtiéndose en un recuerdo y cada momento en el que, sin darse cuenta, hacen que un día normal sea mucho más lindo. A veces las cosas más pequeñas son las que más se quedan en el corazón.</p>
      <p>Quiero que sepan que los aprecio tal y como son. Cada uno tiene algo especial, una forma única de ser y de aportar algo bonito al grupo. No hace falta que todo sea perfecto ni que siempre estemos de acuerdo; para mí, también se trata de aprender, entendernos y seguir compartiendo.</p>
      <p>Quizá no siempre encuentre las palabras correctas o no demuestre todo lo que siento, pero eso no significa que no me importe. Me importan sus alegrías, sus sueños, sus días buenos y también esos días en los que las cosas cuestan un poquito más. Espero que entre nosotros siempre haya espacio para escucharnos, apoyarnos y ser nosotros mismos.</p>
      <p>Ojalá nos queden muchísimas anécdotas por vivir, fotos feas que nos den risa después, conversaciones interminables y recuerdos que algún día miremos con una sonrisa. No sé cómo cambiarán las cosas con el tiempo, pero de verdad espero que la vida nos regale muchos momentos más juntos.</p>
      <p>Y si alguna vez se les olvida lo mucho que valen, acuérdense de que son personas únicas y merecen cariño, respeto y cosas bonitas. Me siento afortunado/a de conocerlos y poder llamarlos mis amigos. 🫶</p>
      <p><strong>Los quiero un montón. Gracias por existir, por ser ustedes y por formar parte de mi historia.</strong> Esta página es pequeñita, pero está hecha con muchísimo cariño para todos ustedes. 💚</p>
      <div class="sign">Con mucho cariño,<br> Danithoo ♡</div>
      <div class="divider">☘ ✧ 💚 ✧ ☘</div>
      <p style="text-align:center;margin-bottom:0">Fin de la cartita… ¡pero no del cariño! (no me voy a suicidar gente)✨</p>
    </article>
    <div id="letterControls" class="hidden">
      <button class="btn alt" onclick="showLetter()">Volver a leer 💌</button>
      <button class="btn alt" onclick="window.scrollTo({top:0,behavior:'smooth'})">Volver al inicio ↑</button>
    </div>
    <p class="music-note">♪ Puedes poner tu canción favorita de fondo mientras lees esta carta.</p>
  </section>
  <footer>Hecho con cariño y un poquito de esfuerso ♡</footer>
</main>
<script>
function openGift(){
  const gift=document.getElementById('gift'); 
  gift.classList.add('open');
  document.getElementById('giftNote').textContent='¡Sorpresaaaa! 💚';
  document.getElementById('openBtn').classList.add('hidden');
  setTimeout(()=>{
    document.getElementById('afterGift').classList.remove('hidden');
    document.getElementById('afterGift').classList.add('reveal');
  },350);
}
document.getElementById('gift').addEventListener('keydown',e=>{
  if(e.key==='Enter'||e.key===' '){e.preventDefault();openGift();}
});
function showLetter(){
  const letter=document.getElementById('letter');
  letter.classList.remove('hidden');
  letter.classList.add('reveal');
  document.getElementById('letterControls').classList.remove('hidden');
  setTimeout(()=>letter.scrollIntoView({behavior:'smooth',block:'start'}),80);
}
function floatHeart(){
  const el=document.createElement('div');
  el.className='heart';
  el.textContent=['♡','♥','✧','💚'][Math.floor(Math.random()*4)];
  el.style.left=Math.random()*100+'vw';
  el.style.fontSize=(14+Math.random()*19)+'px';
  el.style.animationDuration=(7+Math.random()*7)+'s';
  document.body.appendChild(el);
  setTimeout(()=>el.remove(),14500);
}
setInterval(floatHeart,650);
for(let i=0;i<15;i++){
  const s=document.createElement('span');
  s.className='star';
  s.textContent=['✦','✧','·'][Math.floor(Math.random()*3)];
  s.style.left=Math.random()*100+'vw';
  s.style.top=Math.random()*100+'vh';
  s.style.fontSize=(12+Math.random()*18)+'px';
  s.style.animationDelay=Math.random()*3+'s';
  document.body.appendChild(s);
}
</script>
</body>
</html>
