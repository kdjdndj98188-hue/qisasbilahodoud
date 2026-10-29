<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>قصص بلا حدود</title>
<meta name="description" content="صفحة متخصصة في تقديم القصص الخيالية والمغامرات المشوقة باستخدام الذكاء الاصطناعي. كل قصة عالم جديد.">
<meta name="theme-color" content="#07050d">
<meta property="og:type" content="website">
<meta property="og:locale" content="ar_AR">
<meta property="og:title" content="قصص بلا حدود">
<meta property="og:description" content="كل قصة عالم جديد 🌍 — قصص خيالية ومغامرات مشوقة باستخدام الذكاء الاصطناعي.">
<meta name="twitter:card" content="summary">
<link rel="icon" href="logo.png">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Reem+Kufi:wght@600;700&family=Cairo:wght@400;600;700&display=swap" rel="stylesheet">
<style>
:root{
  color-scheme:dark;
  --black:#07050d;
  --ink:#120a22;
  --violet:#7b3fe4;
  --violet-soft:#b392ff;
  --gold:#e8b84a;
  --gold-soft:#f6dc92;
  --text:#efe9fb;
  --muted:#b9aed3;
  box-sizing:border-box;
  padding-top:env(safe-area-inset-top,0px);
  padding-bottom:env(safe-area-inset-bottom,0px);
}
*,*::before,*::after{box-sizing:inherit}
html{height:100%;scroll-padding-top:env(safe-area-inset-top,0px)}
body{
  margin:0;min-height:100%;
  background:var(--black);
  color:var(--text);
  font-family:"Cairo",system-ui,"Segoe UI",Tahoma,Arial,sans-serif;
  line-height:1.9;
  overflow-x:hidden;
}
.sky{
  position:fixed;inset:0;z-index:0;pointer-events:none;
  background:
    radial-gradient(60% 45% at 80% 8%,rgba(123,63,228,.45),transparent 70%),
    radial-gradient(50% 40% at 10% 95%,rgba(232,184,74,.22),transparent 70%),
    radial-gradient(70% 60% at 50% 50%,var(--ink),var(--black) 80%);
}
.sky .star{
  position:absolute;border-radius:50%;background:var(--gold-soft);
  opacity:.7;animation:twinkle var(--d,4s) ease-in-out infinite;
}
.sky .moon{
  position:absolute;top:7%;left:9%;width:clamp(70px,14vw,130px);aspect-ratio:1;border-radius:50%;
  background:radial-gradient(circle at 35% 35%,#fff3cf,var(--gold) 60%,#a9791c);
  box-shadow:0 0 60px 14px rgba(232,184,74,.35);
  animation:float 9s ease-in-out infinite;
}
.sky .castle{
  position:absolute;bottom:0;left:0;width:100%;height:30vh;min-height:150px;
  color:#0b0716;
}
main{
  position:relative;z-index:1;min-height:100vh;min-height:100dvh;
  display:flex;flex-direction:column;align-items:center;justify-content:center;
  text-align:center;padding:48px 22px 120px;
}
.card{width:100%;max-width:760px;padding:clamp(28px,6vw,56px) clamp(18px,5vw,48px);border-radius:28px;border:1px solid rgba(232,184,74,.35);background:linear-gradient(160deg,rgba(26,15,51,.72),rgba(7,5,13,.6));backdrop-filter:blur(10px);-webkit-backdrop-filter:blur(10px);box-shadow:0 0 0 1px rgba(123,63,228,.25),0 30px 80px rgba(0,0,0,.55),0 0 90px rgba(123,63,228,.2)}
.tagline{margin:0 0 14px;font-size:clamp(1.15rem,4.2vw,1.6rem);font-weight:600;color:var(--gold-soft)}
.logo{display:block;width:clamp(150px,38vw,220px);height:auto;margin:0 auto 6px;border-radius:50%;filter:drop-shadow(0 0 34px rgba(232,184,74,.4))}
h1{
  font-family:"Reem Kufi","Cairo",Tahoma,Arial,sans-serif;
  font-weight:700;margin:6px 0 8px;
  font-size:clamp(2.8rem,10vw,5.6rem);line-height:1.25;
  background:linear-gradient(100deg,var(--gold-soft),var(--gold) 30%,var(--violet-soft) 60%,var(--gold-soft));background-size:200% auto;animation:shimmer 8s linear infinite;
  -webkit-background-clip:text;background-clip:text;color:transparent;
  text-shadow:0 0 40px rgba(123,63,228,.35);
}
.line{width:min(220px,50%);height:2px;margin:0 auto 22px;background:linear-gradient(90deg,transparent,var(--gold),transparent)}
.lead{max-width:640px;margin:0 auto 38px;font-size:clamp(1.02rem,3.6vw,1.28rem);color:var(--text)}
.actions{display:flex;flex-wrap:wrap;gap:16px;justify-content:center;width:100%;max-width:640px;margin:0 auto}
.btn{
  position:relative;overflow:hidden;
  flex:1 1 260px;display:inline-flex;align-items:center;justify-content:center;gap:12px;
  padding:15px 24px;border-radius:999px;text-decoration:none;
  font-weight:700;font-size:1.08rem;color:var(--text);
  border:1.5px solid var(--gold);
  background:rgba(18,10,34,.7);
  backdrop-filter:blur(6px);-webkit-backdrop-filter:blur(6px);
  transition:transform .2s ease,box-shadow .25s ease,background .25s ease,color .25s ease;
}
.btn::after{content:"";position:absolute;inset:0;background:linear-gradient(100deg,transparent 30%,rgba(255,255,255,.22) 50%,transparent 70%);transform:translateX(110%);transition:transform .7s ease}
.btn:hover::after{transform:translateX(-110%)}
.btn svg{width:26px;height:26px;flex:none}
.btn:hover{transform:translateY(-3px);box-shadow:0 10px 30px rgba(123,63,228,.45)}
.btn:active{transform:scale(.95)}
.btn:focus-visible{outline:3px solid var(--violet-soft);outline-offset:3px}
.btn.tt:hover{background:var(--gold);color:#1a1100}
.btn.ig:hover{background:linear-gradient(120deg,var(--violet),#c2468f);border-color:var(--violet-soft)}
footer{
  position:fixed;left:0;right:0;bottom:0;z-index:2;
  padding:14px 16px calc(14px + env(safe-area-inset-bottom,0px));
  text-align:center;color:var(--muted);font-size:.95rem;
  background:linear-gradient(0deg,rgba(7,5,13,.92),rgba(7,5,13,0));
}
.rise{opacity:0;transform:translateY(22px);animation:rise .9s cubic-bezier(.2,.7,.2,1) forwards}
.d1{animation-delay:.1s}.d2{animation-delay:.3s}.d3{animation-delay:.5s}.d4{animation-delay:.7s}.d5{animation-delay:.9s}
@keyframes rise{to{opacity:1;transform:none}}
@keyframes shimmer{to{background-position:-200% center}}
@keyframes twinkle{0%,100%{opacity:.15}50%{opacity:.9}}
@keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-12px)}}
@media (prefers-reduced-motion:reduce){
  *{animation-duration:.01ms!important;animation-iteration-count:1!important;transition:none!important}
  .rise{opacity:1;transform:none}
}
</style>
</head>
<body>
<div class="sky" aria-hidden="true" id="sky">
  <div class="moon"></div>
  <svg class="castle" viewBox="0 0 800 200" preserveAspectRatio="xMidYMax slice" fill="currentColor">
    <path d="M0 200V150l60-30 60 30 70-50 70 50 60-40V200zM330 200v-90h20V70l20-30 20 30v40h20V200zM480 200v-60l30-20 30 20 40-30 40 30v60zM680 200v-70l40-30 40 30 40-20v90z"/>
  </svg>
</div>

<main><section class="card">
  <img class="logo rise d1" src="logo.png" alt="شعار قصص بلا حدود" width="220" height="220" decoding="async">
  <h1 class="rise d2">قصص بلا حدود</h1>
  <p class="tagline rise d3">كل قصة عالم جديد 🌍</p>
  <div class="line rise d3"></div>
  <p class="lead rise d4">نحن «قصص بلا حدود»، صفحة متخصصة في تقديم القصص الخيالية والمغامرات المشوقة باستخدام الذكاء الاصطناعي. نصنع عوالم مليئة بالشخصيات المميزة والأحداث المثيرة، من قصص الفواكه الكرتونية إلى الحكايات الدرامية والخيالية. هدفنا هو تقديم محتوى ممتع ومبتكر يأخذكم إلى عوالم جديدة مع كل قصة.</p>
  <div class="actions">
    <a class="btn tt rise d4" href="https://www.tiktok.com/@qisasbilahodoud3?_r=1&amp;_t=ZS-9AxaIDiBXsq" target="_blank" rel="noopener noreferrer">
      <svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M19.6 6.7a5.4 5.4 0 0 1-3.3-1.9A5.3 5.3 0 0 1 15 2h-3.4v13.3a2.9 2.9 0 1 1-2-2.8V9a6.3 6.3 0 1 0 5.4 6.2V9.1a8.7 8.7 0 0 0 5 1.6z"/></svg>
      <span>تابعنا على تيك توك</span>
    </a>
    <a class="btn ig rise d5" href="https://www.instagram.com/qisasbilahodoud3?psln=NzhlNTI4cWNhdWhs&amp;utm_source=qr" target="_blank" rel="noopener noreferrer">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" aria-hidden="true"><rect x="3" y="3" width="18" height="18" rx="5"/><circle cx="12" cy="12" r="4.2"/><circle cx="17.4" cy="6.6" r="1.1" fill="currentColor" stroke="none"/></svg>
      <span>تابعنا على إنستغرام</span>
    </a>
  </div>
</section></main>

<footer class="rise d5">قصص بلا حدود © 2026 — كل قصة عالم جديد</footer>

<script>
(function(){
  var sky=document.getElementById('sky'),f=document.createDocumentFragment();
  for(var i=0;i<60;i++){
    var s=document.createElement('span');s.className='star';
    var z=Math.random()*2.4+.8;
    s.style.cssText='width:'+z+'px;height:'+z+'px;top:'+(Math.random()*85)+'%;left:'+(Math.random()*100)+'%;--d:'+(2.5+Math.random()*4)+'s;animation-delay:'+(Math.random()*4)+'s';
    f.appendChild(s);
  }
  sky.appendChild(f);
})();
</script>
</body>
</html>
