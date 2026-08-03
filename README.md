<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Частная клиника общей практики «Пульс» в Москве: терапевты, кардиологи, неврологи, УЗИ и анализы. Приём в день обращения, без очередей.">
<meta name="theme-color" content="#0E5A4A">
<title>Клиника «Пульс» — частная клиника общей практики в Москве</title>
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 32 32'%3E%3Cpath d='M16 28C9 22 3 17 3 11a7 7 0 0 1 13-3.6A7 7 0 0 1 29 11c0 6-6 11-13 17z' fill='%230E5A4A'/%3E%3Cpath d='M6 15h5l2-4 3 8 2-4h6' stroke='%23F5F2EA' stroke-width='2' fill='none' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E">
<script>document.documentElement.classList.add('js');</script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Prata&family=Golos+Text:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;500;700&display=swap" rel="stylesheet">
<style>
/* ============ 1. БАЗА ============ */
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box}
:root{
  --bg:#F5F2EA; --bg2:#FBF9F3; --card:#FFFEFA;
  --ink:#14312C; --ink-soft:#51685F; --line:#E2DBC9; --line-soft:#ECE6D6;
  --green:#0E5A4A; --green-deep:#0A3F34; --green-dark:#082B24;
  --coral:#E4573D; --coral-soft:#FBE9E3; --mint:#DCEBE2; --cream:#F3EFE2;
  --display:'Prata',Georgia,serif;
  --body:'Golos Text',system-ui,-apple-system,sans-serif;
  --mono:'JetBrains Mono',ui-monospace,monospace;
  --ease:cubic-bezier(.22,.75,.25,1);
  --shadow:0 14px 40px -18px rgba(20,49,44,.28);
  --shadow-sm:0 6px 20px -10px rgba(20,49,44,.18);
  --header-h:74px;
  color-scheme:light;
}
html{scroll-behavior:smooth;scroll-padding-top:calc(var(--header-h) + 16px)}
body{font-family:var(--body);background:var(--bg);color:var(--ink);font-size:16.5px;line-height:1.6;-webkit-font-smoothing:antialiased;overflow-x:hidden}
body.lock{overflow:hidden}
img{display:block;max-width:100%}
a{color:inherit;text-decoration:none}
button{font-family:inherit;cursor:pointer;background:none;border:none;color:inherit}
input,select,textarea{font-family:inherit;font-size:1rem;color:inherit}
::selection{background:var(--coral);color:#fff}
:focus-visible{outline:2.5px solid var(--coral);outline-offset:3px;border-radius:4px}
.container{width:min(1180px,92%);margin-inline:auto}
section{position:relative}

/* типографика */
.h2{font-family:var(--display);font-weight:400;font-size:clamp(1.85rem,3.6vw,2.9rem);line-height:1.16;letter-spacing:.005em}
.lead{color:var(--ink-soft);max-width:56ch}
.label{display:inline-flex;align-items:center;gap:.7em;font-family:var(--mono);font-size:.72rem;font-weight:500;letter-spacing:.22em;text-transform:uppercase;color:var(--green)}
.label::before{content:"";width:8px;height:8px;border-radius:50%;background:var(--coral);animation:pulseDot 2.2s infinite}
.label.light{color:#BCD8CC}
@keyframes pulseDot{0%,100%{box-shadow:0 0 0 0 rgba(228,87,61,.45)}55%{box-shadow:0 0 0 7px rgba(228,87,61,0)}}

/* кнопки */
.btn{display:inline-flex;align-items:center;justify-content:center;gap:.65em;padding:.95em 1.6em;border-radius:999px;font-weight:600;font-size:.98rem;line-height:1;letter-spacing:.01em;border:1.5px solid transparent;transition:transform .35s var(--ease),background .35s,color .35s,border-color .35s,box-shadow .35s;white-space:nowrap}
.btn svg{width:17px;height:17px;transition:transform .35s var(--ease)}
.btn:hover svg{transform:translateX(4px)}
.btn:active{transform:scale(.97)}
.btn-primary{background:var(--green);color:var(--cream)}
.btn-primary:hover{background:var(--green-deep);transform:translateY(-2px);box-shadow:var(--shadow)}
.btn-coral{background:var(--coral);color:#fff}
.btn-coral:hover{background:#c9432b;transform:translateY(-2px);box-shadow:var(--shadow)}
.btn-ghost{border-color:rgba(20,49,44,.28);color:var(--ink)}
.btn-ghost:hover{border-color:var(--green);background:var(--card);transform:translateY(-2px)}
.btn-sm{padding:.62em 1.15em;font-size:.86rem}
.btn-block{width:100%}

/* зерно плёнки */
.noise{position:fixed;inset:0;z-index:60;pointer-events:none;opacity:.045;background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='140' height='140'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='.9' numOctaves='2'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E")}

/* прогресс-бар */
#progressBar{position:fixed;top:0;left:0;height:3px;width:0;background:linear-gradient(90deg,var(--coral),#f08a63);z-index:200;transition:width .1s linear}

/* ============ 2. ПРЕЛОАДЕР ============ */
#preloader{position:fixed;inset:0;z-index:300;background:var(--bg);display:flex;flex-direction:column;gap:22px;align-items:center;justify-content:center;transition:opacity .6s var(--ease),visibility .6s}
#preloader.hide{opacity:0;visibility:hidden}
#preloader .pl-logo{font-family:var(--display);font-size:1.7rem;letter-spacing:.06em}
#preloader .pl-logo b{color:var(--coral);font-weight:400}
#preloader svg{width:min(280px,60vw);overflow:visible}
#preloader .pl-line{stroke:var(--green);stroke-width:2.4;fill:none;stroke-linecap:round;stroke-dasharray:1000;stroke-dashoffset:1000;animation:draw 1.1s var(--ease) forwards}
#preloader .pl-dot{fill:var(--coral)}
@keyframes draw{to{stroke-dashoffset:0}}

/* ============ 3. ШАПКА ============ */
.topbar{background:var(--green-dark);color:#CBDDD4;font-size:.82rem}
.topbar .container{display:flex;align-items:center;gap:1.6rem;height:40px}
.topbar a{transition:color .25s}
.topbar a:hover{color:#fff}
.topbar .sep{opacity:.35}
.topbar .grow{flex:1}
.open-badge{display:inline-flex;align-items:center;gap:.5em;font-weight:600}
.open-badge i{width:8px;height:8px;border-radius:50%;background:#7ED09B;box-shadow:0 0 0 0 rgba(126,208,155,.5);animation:pulseDot 2s infinite}
.open-badge.closed i{background:#E7B04A}
header.site{position:sticky;top:0;z-index:150;background:rgba(245,242,234,.9);backdrop-filter:blur(8px);border-bottom:1px solid transparent;transition:border-color .35s,box-shadow .35s}
header.site.scrolled{border-color:var(--line);box-shadow:0 8px 30px -18px rgba(20,49,44,.25)}
.nav-row{display:flex;align-items:center;gap:2rem;height:var(--header-h)}
.logo{display:flex;align-items:center;gap:.7rem;font-family:var(--display);font-size:1.45rem;letter-spacing:.04em}
.logo .lg-mark{width:42px;height:42px;border-radius:13px;background:var(--green);display:grid;place-items:center;transition:transform .4s var(--ease)}
.logo:hover .lg-mark{transform:rotate(-8deg) scale(1.05)}
.logo .lg-mark svg{width:24px;height:24px;stroke:var(--cream);fill:none;stroke-width:2;stroke-linecap:round;stroke-linejoin:round}
.logo small{display:block;font-family:var(--mono);font-size:.58rem;letter-spacing:.28em;color:var(--ink-soft);text-transform:uppercase}
.nav-links{display:flex;gap:.35rem;margin-inline:auto}
.nav-links a{position:relative;padding:.55em .85em;font-size:.94rem;font-weight:500;color:var(--ink-soft);border-radius:999px;transition:color .3s,background .3s}
.nav-links a:hover{color:var(--ink);background:rgba(14,90,74,.07)}
.nav-links a.active{color:var(--green);background:rgba(14,90,74,.1);font-weight:600}
.head-phone{display:flex;flex-direction:column;align-items:flex-end;line-height:1.2;margin-right:.4rem}
.head-phone b{font-family:var(--mono);font-size:1rem;letter-spacing:-.01em}
.head-phone span{font-size:.7rem;color:var(--ink-soft)}
#burgerBtn{display:none;width:46px;height:46px;border-radius:14px;border:1.5px solid var(--line);position:relative;z-index:210}
#burgerBtn span{position:absolute;left:12px;right:12px;height:2px;background:var(--ink);border-radius:2px;transition:transform .4s var(--ease),opacity .3s,top .4s var(--ease)}
#burgerBtn span:nth-child(1){top:16px}#burgerBtn span:nth-child(2){top:22px}#burgerBtn span:nth-child(3){top:28px}
body.menu-open #burgerBtn span:nth-child(1){top:22px;transform:rotate(45deg)}
body.menu-open #burgerBtn span:nth-child(2){opacity:0}
body.menu-open #burgerBtn span:nth-child(3){top:22px;transform:rotate(-45deg)}

/* мобильное меню */
#mobileMenu{position:fixed;inset:0;z-index:205;background:var(--green-dark);color:var(--cream);padding:110px 8% 40px;clip-path:circle(0 at calc(100% - 60px) 40px);transition:clip-path .65s var(--ease);display:flex;flex-direction:column}
body.menu-open #mobileMenu{clip-path:circle(150% at calc(100% - 60px) 40px)}
#mobileMenu .mm-link{display:flex;align-items:baseline;gap:1rem;font-family:var(--display);font-size:clamp(1.6rem,5.5vw,2.4rem);padding:.42em 0;border-bottom:1px solid rgba(243,239,226,.12);opacity:0;transform:translateY(18px);transition:opacity .5s var(--ease),transform .5s var(--ease),color .3s}
#mobileMenu .mm-link:hover{color:#f0a48e}
#mobileMenu .mm-link em{font-family:var(--mono);font-style:normal;font-size:.7rem;color:#7fa79a;letter-spacing:.15em}
body.menu-open #mobileMenu .mm-link{opacity:1;transform:none}
body.menu-open #mobileMenu .mm-link:nth-child(1){transition-delay:.1s}body.menu-open #mobileMenu .mm-link:nth-child(2){transition-delay:.16s}body.menu-open #mobileMenu .mm-link:nth-child(3){transition-delay:.22s}body.menu-open #mobileMenu .mm-link:nth-child(4){transition-delay:.28s}body.menu-open #mobileMenu .mm-link:nth-child(5){transition-delay:.34s}body.menu-open #mobileMenu .mm-link:nth-child(6){transition-delay:.4s}
#mobileMenu .mm-foot{margin-top:auto;display:flex;flex-wrap:wrap;gap:1rem;align-items:center;justify-content:space-between;font-size:.9rem;color:#A9C6BB}
#mobileMenu .mm-foot a.tel{font-family:var(--mono);font-size:1.25rem;color:var(--cream)}

/* ============ 4. ГЕРОЙ ============ */
.hero{padding:calc(var(--header-h) + 26px) 0 0;overflow:hidden;background:
  url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='52' height='52'%3E%3Cpath d='M26 20v12M20 26h12' stroke='%230E5A4A' stroke-opacity='.07' stroke-width='2' stroke-linecap='round'/%3E%3C/svg%3E")}
.hero-grid{display:grid;grid-template-columns:1.08fr .92fr;gap:3.5rem;align-items:center;min-height:min(620px,72vh)}
.hero-over{margin-bottom:1.4rem}
.hero h1{font-family:var(--display);font-weight:400;font-size:clamp(2.5rem,5.4vw,4.35rem);line-height:1.08;letter-spacing:.002em}
.hero h1 .accent{color:var(--coral)}
.line{display:block;overflow:hidden;padding-bottom:.08em;margin-bottom:-.08em}
.line-in{display:block;transform:translateY(112%)}
body.is-loaded .line-in{animation:rise 1s var(--ease) forwards}
body.is-loaded .hero .line:nth-child(1) .line-in{animation-delay:.05s}
body.is-loaded .hero .line:nth-child(2) .line-in{animation-delay:.16s}
body.is-loaded .hero .line:nth-child(3) .line-in{animation-delay:.27s}
@keyframes rise{to{transform:none}}
.hero-sub{margin:1.6rem 0 2.1rem;max-width:46ch;color:var(--ink-soft);font-size:1.08rem;opacity:0;transform:translateY(14px)}
body.is-loaded .hero-sub{animation:fadeUp .8s var(--ease) .45s forwards}
.hero-cta{display:flex;flex-wrap:wrap;gap:.9rem;opacity:0;transform:translateY(14px)}
body.is-loaded .hero-cta{animation:fadeUp .8s var(--ease) .6s forwards}
@keyframes fadeUp{to{opacity:1;transform:none}}
.hero-trust{display:flex;flex-wrap:wrap;gap:1.4rem;margin-top:2.1rem;font-size:.88rem;color:var(--ink-soft);opacity:0}
body.is-loaded .hero-trust{animation:fadeUp .8s ease .8s forwards}
.hero-trust b{color:var(--ink)}
.stars{color:var(--coral);letter-spacing:2px;font-size:.95rem}

.hero-visual{position:relative;opacity:0;transform:translateY(24px)}
body.is-loaded .hero-visual{animation:fadeUp 1s var(--ease) .5s forwards}
.hero-photo{border-radius:26px 26px 26px 90px;overflow:hidden;box-shadow:var(--shadow);border:1px solid var(--line);aspect-ratio:4/4.6;max-height:540px}
.hero-photo img{width:100%;height:100%;object-fit:cover;filter:saturate(.88) contrast(1.03);animation:breathe 14s ease-in-out infinite alternate}
@keyframes breathe{from{transform:scale(1)}to{transform:scale(1.07)}}
.float-chip{position:absolute;background:var(--card);border:1px solid var(--line);border-radius:16px;padding:.75rem 1.05rem;box-shadow:var(--shadow-sm);font-size:.85rem;font-weight:600;display:flex;align-items:center;gap:.6rem;animation:floaty 5.5s ease-in-out infinite alternate}
.float-chip .fc-ico{width:34px;height:34px;border-radius:10px;display:grid;place-items:center;background:var(--mint);color:var(--green);font-size:1rem}
.float-chip small{display:block;font-weight:400;color:var(--ink-soft);font-size:.74rem}
.chip-1{top:9%;left:-9%}
.chip-2{bottom:12%;right:-6%;animation-delay:1.4s}
.chip-2 .fc-ico{background:var(--coral-soft);color:var(--coral)}
@keyframes floaty{from{transform:translateY(-6px)}to{transform:translateY(8px)}}

/* кардиограмма */
.ecg-wrap{margin-top:2.6rem}
.ecg-wrap svg{width:100%;height:74px;display:block;overflow:visible}
.ecg-base{stroke:rgba(14,90,74,.22);stroke-width:2;fill:none;stroke-linecap:round;stroke-linejoin:round}
.ecg-run{stroke:var(--coral);stroke-width:2.6;fill:none;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:70 930;animation:ecgRun 4.2s linear infinite;filter:drop-shadow(0 0 6px rgba(228,87,61,.5))}
@keyframes ecgRun{from{stroke-dashoffset:1000}to{stroke-dashoffset:0}}

/* быстрые ссылки */
.quick-links{display:grid;grid-template-columns:repeat(4,1fr);gap:1rem;margin:3.2rem 0 0}
.ql-card{display:flex;flex-direction:column;gap:.55rem;text-align:left;background:var(--card);border:1px solid var(--line);border-radius:18px;padding:1.15rem 1.25rem;transition:transform .4s var(--ease),border-color .35s,box-shadow .4s}
.ql-card:hover{transform:translateY(-5px);border-color:rgba(14,90,74,.45);box-shadow:var(--shadow-sm)}
.ql-card .ql-ico{width:40px;height:40px;border-radius:12px;background:var(--mint);color:var(--green);display:grid;place-items:center;transition:transform .4s var(--ease)}
.ql-card:hover .ql-ico{transform:rotate(-8deg) scale(1.08)}
.ql-ico svg{width:20px;height:20px;stroke:currentColor;fill:none;stroke-width:1.8;stroke-linecap:round;stroke-linejoin:round}
.ql-card b{font-size:.98rem}
.ql-card small{color:var(--ink-soft);font-size:.8rem;line-height:1.4}
.ql-card .ql-go{margin-top:auto;font-weight:600;font-size:.82rem;color:var(--green);display:flex;align-items:center;gap:.4em}
.ql-card:hover .ql-go{color:var(--coral)}

/* ============ 5. ЦИФРЫ ============ */
.stats{background:var(--green-dark);color:var(--cream);margin-top:4.5rem}
.stats-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:1rem;padding:3.4rem 0}
.stat{padding:0 1.6rem;border-left:1px solid rgba(243,239,226,.14)}
.stat:first-child{border-left:none;padding-left:0}
.stat .num{font-family:var(--display);font-size:clamp(2.1rem,3.6vw,3.1rem);line-height:1.1;color:#fff}
.stat .num sup{font-size:.5em;color:var(--coral)}
.stat p{font-size:.86rem;color:#9DBFB2;margin-top:.35rem}

/* ============ 6. БЕГУЩАЯ СТРОКА ============ */
.marquee{border-bottom:1px solid var(--line);background:var(--bg2);overflow:hidden;padding:1.05rem 0}
.marquee-track{display:flex;gap:2.6rem;width:max-content;animation:mar 30s linear infinite;font-family:var(--display);font-size:1.15rem;color:var(--green);white-space:nowrap}
.marquee:hover .marquee-track{animation-play-state:paused}
.marquee-track .plus{color:var(--coral);font-family:var(--body);font-weight:700}
@keyframes mar{to{transform:translateX(-50%)}}

/* ============ 7. ОБЩИЕ СЕКЦИИ ============ */
.section{padding:clamp(4.5rem,8vw,7.5rem) 0}
.sec-head{display:flex;flex-wrap:wrap;align-items:flex-end;justify-content:space-between;gap:1.5rem;margin-bottom:clamp(2.2rem,4vw,3.4rem)}
.sec-head .h2{max-width:20ch}

/* О клинике */
.about-grid{display:grid;grid-template-columns:1.05fr .95fr;gap:4rem;align-items:start}
.about-sticky{position:sticky;top:calc(var(--header-h) + 30px)}
.about-sticky .h2{margin:1rem 0 1.2rem}
.about-sticky .lead{margin-bottom:1.8rem}
.values{display:grid;gap:.9rem;margin-bottom:2rem}
.value{display:flex;gap:.9rem;align-items:flex-start}
.value .v-ico{flex:none;width:38px;height:38px;border-radius:12px;background:var(--mint);color:var(--green);display:grid;place-items:center;margin-top:2px}
.value .v-ico svg{width:19px;height:19px;stroke:currentColor;fill:none;stroke-width:2;stroke-linecap:round;stroke-linejoin:round}
.value b{display:block;font-size:.99rem}
.value p{font-size:.88rem;color:var(--ink-soft)}
.dms{display:flex;flex-wrap:wrap;gap:.55rem;align-items:center;font-size:.8rem;color:var(--ink-soft)}
.dms span{border:1px solid var(--line);background:var(--card);border-radius:999px;padding:.4em .95em;font-weight:600;color:var(--ink);transition:border-color .3s,transform .3s}
.dms span:hover{border-color:var(--green);transform:translateY(-2px)}
.about-pics{display:grid;grid-template-columns:1fr 1fr;gap:1rem}
.about-pics figure{border-radius:20px;overflow:hidden;border:1px solid var(--line);box-shadow:var(--shadow-sm)}
.about-pics figure:first-child{grid-column:1/-1;aspect-ratio:16/9}
.about-pics figure:nth-child(2){aspect-ratio:4/4.6}
.about-pics figure:nth-child(3){aspect-ratio:4/4.6;transform:translateY(1.6rem)}
.about-pics img{width:100%;height:100%;object-fit:cover;filter:saturate(.85);transition:transform 1.2s var(--ease)}
.about-pics figure:hover img{transform:scale(1.06)}
.exp-badge{position:absolute;right:-10px;top:-16px;background:var(--coral);color:#fff;border-radius:16px;padding:.8rem 1.1rem;font-weight:700;text-align:center;box-shadow:var(--shadow);transform:rotate(4deg)}
.exp-badge b{font-family:var(--display);font-size:1.9rem;display:block;line-height:1}
.about-pics{position:relative}

/* ============ 8. ОТДЕЛЕНИЯ ============ */
.services{background:var(--bg2);border-block:1px solid var(--line-soft)}
.srv-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1.15rem}
.srv-card{position:relative;background:var(--card);border:1px solid var(--line);border-radius:20px;padding:1.7rem 1.6rem 1.5rem;display:flex;flex-direction:column;gap:.8rem;transition:transform .45s var(--ease),border-color .35s,box-shadow .45s;overflow:hidden}
.srv-card::after{content:"";position:absolute;inset:auto 0 0 0;height:3px;background:linear-gradient(90deg,var(--coral),#f2a184);transform:scaleX(0);transform-origin:left;transition:transform .5s var(--ease)}
.srv-card:hover{transform:translateY(-7px);border-color:rgba(14,90,74,.4);box-shadow:var(--shadow)}
.srv-card:hover::after{transform:scaleX(1)}
.srv-ico{width:52px;height:52px;border-radius:16px;background:var(--mint);color:var(--green);display:grid;place-items:center;transition:transform .45s var(--ease),background .35s,color .35s}
.srv-card:hover .srv-ico{transform:rotate(-9deg) scale(1.07);background:var(--green);color:var(--cream)}
.srv-ico svg{width:26px;height:26px;stroke:currentColor;fill:none;stroke-width:1.7;stroke-linecap:round;stroke-linejoin:round}
.srv-card h3{font-size:1.18rem;font-weight:700}
.srv-card p{font-size:.9rem;color:var(--ink-soft);flex:1}
.srv-foot{display:flex;align-items:center;justify-content:space-between;gap:1rem;padding-top:.9rem;border-top:1px dashed var(--line)}
.srv-price{font-family:var(--mono);font-size:.92rem;font-weight:700}
.srv-price small{display:block;font-weight:400;font-size:.68rem;color:var(--ink-soft);font-family:var(--body)}
.srv-book{font-weight:600;font-size:.88rem;color:var(--green);display:inline-flex;gap:.4em;align-items:center;transition:color .3s}
.srv-book:hover{color:var(--coral)}
.srv-book svg{width:15px;height:15px;stroke:currentColor;fill:none;stroke-width:2;stroke-linecap:round;stroke-linejoin:round;transition:transform .3s var(--ease)}
.srv-book:hover svg{transform:translateX(4px)}

/* ============ 9. КАК ПРОХОДИТ ПРИЁМ ============ */
.steps-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:1.2rem;position:relative}
.steps-grid::before{content:"";position:absolute;top:34px;left:7%;right:7%;border-top:2px dashed rgba(14,90,74,.25)}
.step{position:relative;background:var(--card);border:1px solid var(--line);border-radius:20px;padding:2.6rem 1.5rem 1.6rem;transition:transform .4s var(--ease),box-shadow .4s}
.step:hover{transform:translateY(-6px);box-shadow:var(--shadow-sm)}
.step .st-num{position:absolute;top:-22px;left:1.4rem;width:56px;height:56px;border-radius:50%;background:var(--green);color:var(--cream);font-family:var(--mono);font-weight:700;display:grid;place-items:center;font-size:1.05rem;box-shadow:var(--shadow-sm)}
.step:nth-child(even) .st-num{background:var(--coral)}
.step h3{font-size:1.06rem;margin-bottom:.45rem}
.step p{font-size:.87rem;color:var(--ink-soft)}

/* ============ 10. ЦЕНЫ ============ */
.prices{background:var(--bg2);border-block:1px solid var(--line-soft)}
.prices-tools{display:flex;flex-wrap:wrap;gap:1rem;align-items:center;margin-bottom:1.6rem}
.price-tabs{display:flex;flex-wrap:wrap;gap:.5rem;background:var(--card);border:1px solid var(--line);padding:.35rem;border-radius:999px}
.price-tab{padding:.6em 1.25em;border-radius:999px;font-weight:600;font-size:.9rem;color:var(--ink-soft);transition:background .3s,color .3s}
.price-tab:hover{color:var(--ink)}
.price-tab[aria-selected="true"]{background:var(--green);color:var(--cream)}
.price-search{position:relative;flex:1;min-width:230px;max-width:360px;margin-left:auto}
.price-search input{width:100%;padding:.8em 1.1em .8em 2.7em;border-radius:999px;border:1.5px solid var(--line);background:var(--card);transition:border-color .3s,box-shadow .3s}
.price-search input:focus{outline:none;border-color:var(--green);box-shadow:0 0 0 4px rgba(14,90,74,.12)}
.price-search svg{position:absolute;left:1em;top:50%;transform:translateY(-50%);width:17px;height:17px;stroke:var(--ink-soft);fill:none;stroke-width:2;stroke-linecap:round}
.price-list{background:var(--card);border:1px solid var(--line);border-radius:22px;overflow:hidden;box-shadow:var(--shadow-sm)}
.pl-row{display:grid;grid-template-columns:1fr auto auto auto;gap:1.2rem;align-items:center;padding:1.05rem 1.6rem;border-bottom:1px solid var(--line-soft);transition:background .25s;animation:rowIn .45s var(--ease) both}
.pl-row:last-child{border-bottom:none}
.pl-row:hover{background:rgba(14,90,74,.045)}
@keyframes rowIn{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}
.pl-name{font-weight:600;font-size:.98rem;display:flex;align-items:center;gap:.7rem;flex-wrap:wrap}
.pl-name small{display:block;width:100%;font-weight:400;font-size:.78rem;color:var(--ink-soft)}
.pl-hot{font-family:var(--mono);font-size:.62rem;letter-spacing:.08em;text-transform:uppercase;background:var(--coral-soft);color:var(--coral);padding:.3em .8em;border-radius:999px;font-weight:700}
.pl-price{font-family:var(--mono);font-weight:700;font-size:1.02rem;white-space:nowrap}
.pl-empty{padding:3rem 1.5rem;text-align:center;color:var(--ink-soft)}
.pl-empty b{color:var(--ink)}
.price-note{display:flex;flex-wrap:wrap;gap:1rem;align-items:center;justify-content:space-between;margin-top:1.3rem;font-size:.83rem;color:var(--ink-soft)}

/* ============ 11. ВРАЧИ ============ */
.doc-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1.3rem}
.doc-card{background:var(--card);border:1px solid var(--line);border-radius:22px;overflow:hidden;transition:transform .45s var(--ease),box-shadow .45s,border-color .35s;display:flex;flex-direction:column}
.doc-card:hover{transform:translateY(-7px);box-shadow:var(--shadow);border-color:rgba(14,90,74,.35)}
.doc-ph{aspect-ratio:4/4.2;overflow:hidden;position:relative}
.doc-ph img{width:100%;height:100%;object-fit:cover;filter:saturate(.82) contrast(1.02);transition:transform 1s var(--ease)}
.doc-card:hover .doc-ph img{transform:scale(1.06)}
.doc-exp{position:absolute;left:1rem;bottom:1rem;background:rgba(8,43,36,.82);color:var(--cream);backdrop-filter:blur(4px);font-size:.74rem;font-weight:600;padding:.45em 1em;border-radius:999px}
.doc-body{padding:1.4rem 1.5rem 1.5rem;display:flex;flex-direction:column;gap:.4rem;flex:1}
.doc-body h3{font-size:1.2rem;font-weight:700}
.doc-spec{color:var(--green);font-weight:600;font-size:.9rem}
.doc-meta{font-size:.82rem;color:var(--ink-soft)}
.doc-foot{margin-top:auto;display:flex;align-items:center;justify-content:space-between;gap:1rem;padding-top:1rem}
.doc-price{font-family:var(--mono);font-weight:700}
.doc-price small{font-family:var(--body);font-weight:400;color:var(--ink-soft);font-size:.72rem;display:block}

/* ============ 12. ОТЗЫВЫ (тёмная) ============ */
.reviews{background:var(--green-dark);color:var(--cream);overflow:hidden}
.reviews::before{content:"";position:absolute;inset:0;background:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='52' height='52'%3E%3Cpath d='M26 20v12M20 26h12' stroke='%23F3EFE2' stroke-opacity='.05' stroke-width='2' stroke-linecap='round'/%3E%3C/svg%3E");pointer-events:none}
.reviews .lead{color:#9DBFB2}
.rating-big{display:flex;align-items:center;gap:1.1rem;background:rgba(243,239,226,.07);border:1px solid rgba(243,239,226,.15);border-radius:18px;padding:.9rem 1.4rem}
.rating-big .rb-num{font-family:var(--display);font-size:2.3rem;color:#fff}
.rating-big .stars{font-size:1.05rem}
.rating-big small{display:block;color:#9DBFB2;font-size:.78rem}
.slider{position:relative}
.slider-viewport{overflow:hidden;touch-action:pan-y;cursor:grab}
.slider-viewport:active{cursor:grabbing}
.slider-track{display:flex;list-style:none;transition:transform .65s var(--ease)}
.slider-track li{flex:0 0 100%;padding-right:1.2rem;min-width:0}
.rev-card{background:var(--cream);color:var(--ink);border-radius:20px;padding:1.8rem 1.7rem;height:100%;display:flex;flex-direction:column;gap:1rem;position:relative}
.rev-card::before{content:"“";position:absolute;top:.2rem;right:1.3rem;font-family:var(--display);font-size:4.5rem;color:var(--coral);opacity:.25;line-height:1}
.rev-top{display:flex;gap:.9rem;align-items:center}
.rev-ava{width:46px;height:46px;border-radius:50%;background:var(--green);color:var(--cream);display:grid;place-items:center;font-weight:700;flex:none}
.rev-top b{display:block;font-size:.98rem}
.rev-top small{color:var(--ink-soft);font-size:.78rem}
.rev-card p{font-size:.92rem;line-height:1.65;color:#2c4a43}
.rev-src{margin-top:auto;display:flex;justify-content:space-between;align-items:center;font-size:.76rem;color:var(--ink-soft)}
.slider-ctrl{display:flex;align-items:center;gap:1.1rem;margin-top:2rem}
.sl-btn{width:52px;height:52px;border-radius:50%;border:1.5px solid rgba(243,239,226,.3);color:var(--cream);display:grid;place-items:center;transition:background .3s,border-color .3s,transform .3s}
.sl-btn:hover{background:var(--coral);border-color:var(--coral);transform:scale(1.06)}
.sl-btn svg{width:19px;height:19px;stroke:currentColor;fill:none;stroke-width:2.2;stroke-linecap:round;stroke-linejoin:round}
.sl-dots{display:flex;gap:.5rem}
.sl-dot{width:9px;height:9px;border-radius:999px;background:rgba(243,239,226,.28);transition:width .35s var(--ease),background .3s;padding:0}
.sl-dot.active{width:26px;background:var(--coral)}

/* ============ 13. FAQ ============ */
.faq-wrap{max-width:820px;margin-inline:auto}
.acc-item{background:var(--card);border:1px solid var(--line);border-radius:18px;margin-bottom:.85rem;overflow:hidden;transition:border-color .3s,box-shadow .3s}
.acc-item.open{border-color:rgba(14,90,74,.45);box-shadow:var(--shadow-sm)}
.acc-btn{width:100%;display:flex;align-items:center;justify-content:space-between;gap:1.2rem;text-align:left;padding:1.25rem 1.5rem;font-weight:600;font-size:1.02rem}
.acc-ico{flex:none;width:34px;height:34px;border-radius:50%;background:var(--mint);color:var(--green);display:grid;place-items:center;transition:transform .45s var(--ease),background .3s,color .3s}
.acc-item.open .acc-ico{transform:rotate(45deg);background:var(--coral);color:#fff}
.acc-ico svg{width:15px;height:15px;stroke:currentColor;fill:none;stroke-width:2.4;stroke-linecap:round}
.acc-panel{max-height:0;overflow:hidden;transition:max-height .5s var(--ease)}
.acc-body{padding:0 1.5rem 1.4rem;color:var(--ink-soft);font-size:.93rem;max-width:64ch}

/* ============ 14. ЗАПИСЬ ============ */
.appt{background:var(--bg2);border-block:1px solid var(--line-soft)}
.appt-card{display:grid;grid-template-columns:.9fr 1.1fr;background:var(--card);border:1px solid var(--line);border-radius:28px;overflow:hidden;box-shadow:var(--shadow)}
.appt-info{background:var(--green);color:var(--cream);padding:clamp(2rem,4vw,3.2rem);display:flex;flex-direction:column;gap:1.6rem}
.appt-info h3{font-family:var(--display);font-weight:400;font-size:clamp(1.5rem,2.4vw,2rem);line-height:1.25}
.appt-phone{display:block;font-family:var(--mono);font-size:clamp(1.3rem,2.4vw,1.7rem);font-weight:700;color:#fff;transition:color .3s}
.appt-phone:hover{color:#f2a184}
.appt-info ul{list-style:none;display:grid;gap:.85rem;font-size:.9rem;color:#C6DCD3}
.appt-info li{display:flex;gap:.7rem;align-items:flex-start}
.appt-info li svg{flex:none;width:18px;height:18px;stroke:#8fd0b6;fill:none;stroke-width:2.2;stroke-linecap:round;stroke-linejoin:round;margin-top:2px}
.form-wrap{padding:clamp(2rem,4vw,3.2rem);position:relative}
.form-wrap h3{font-size:1.3rem;margin-bottom:.4rem}
.form-wrap .fw-sub{font-size:.9rem;color:var(--ink-soft);margin-bottom:1.6rem}
.f-grid{display:grid;grid-template-columns:1fr 1fr;gap:1rem}
.field{display:flex;flex-direction:column;gap:.35rem}
.field.full{grid-column:1/-1}
.field label{font-size:.8rem;font-weight:600;color:var(--ink-soft)}
.field input,.field select,.field textarea{padding:.85em 1.05em;border-radius:13px;border:1.5px solid var(--line);background:var(--bg2);transition:border-color .3s,box-shadow .3s,background .3s;width:100%}
.field textarea{resize:vertical;min-height:84px}
.field input:focus,.field select:focus,.field textarea:focus{outline:none;border-color:var(--green);background:#fff;box-shadow:0 0 0 4px rgba(14,90,74,.12)}
.field.invalid input,.field.invalid select{border-color:var(--coral);background:var(--coral-soft)}
.f-err{font-size:.74rem;color:var(--coral);display:none}
.field.invalid .f-err{display:block}
.consent{display:flex;gap:.7rem;align-items:flex-start;font-size:.8rem;color:var(--ink-soft);grid-column:1/-1;cursor:pointer}
.consent input{width:19px;height:19px;accent-color:var(--green);margin-top:2px;flex:none}
.consent.invalid{color:var(--coral)}
.form-success{position:absolute;inset:0;background:var(--card);display:flex;flex-direction:column;align-items:center;justify-content:center;gap:.9rem;text-align:center;padding:2rem;opacity:0;visibility:hidden;transform:scale(.97);transition:opacity .5s var(--ease),transform .5s var(--ease)}
.form-wrap.sent .form-success{opacity:1;visibility:visible;transform:none}
.form-wrap.sent form{opacity:0;pointer-events:none}
.fs-check{width:84px;height:84px}
.fs-check circle{stroke:var(--green);stroke-width:2.5;fill:var(--mint);stroke-dasharray:260;stroke-dashoffset:260}
.fs-check path{stroke:var(--green);stroke-width:4;fill:none;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:60;stroke-dashoffset:60}
.form-wrap.sent .fs-check circle{animation:draw .8s var(--ease) .1s forwards}
.form-wrap.sent .fs-check path{animation:draw .5s var(--ease) .7s forwards}
.fs-code{font-family:var(--mono);background:var(--mint);color:var(--green);padding:.4em 1em;border-radius:999px;font-weight:700;font-size:.9rem}

/* ============ 15. КОНТАКТЫ ============ */
.contacts-grid{display:grid;grid-template-columns:1fr 1.15fr;gap:1.4rem;align-items:stretch}
.c-cards{display:grid;gap:1rem;align-content:start}
.c-card{display:flex;gap:1rem;align-items:flex-start;background:var(--card);border:1px solid var(--line);border-radius:18px;padding:1.25rem 1.4rem;transition:transform .35s var(--ease),border-color .3s}
.c-card:hover{transform:translateX(6px);border-color:rgba(14,90,74,.4)}
.c-ico{flex:none;width:44px;height:44px;border-radius:13px;background:var(--mint);color:var(--green);display:grid;place-items:center}
.c-ico svg{width:21px;height:21px;stroke:currentColor;fill:none;stroke-width:1.9;stroke-linecap:round;stroke-linejoin:round}
.c-card small{display:block;font-size:.76rem;color:var(--ink-soft);text-transform:uppercase;letter-spacing:.08em;font-weight:600;margin-bottom:.2rem}
.c-card b{font-size:1.02rem;line-height:1.4}
.c-card a:hover{color:var(--coral)}
.map-box{position:relative;border-radius:22px;overflow:hidden;border:1px solid var(--line);min-height:380px;background:#EDE8DA;box-shadow:var(--shadow-sm)}
.map-box svg{width:100%;height:100%;display:block;position:absolute;inset:0}
.map-pin-ring{transform-origin:center;transform-box:fill-box;animation:ring 2.4s ease-out infinite}
@keyframes ring{0%{transform:scale(.4);opacity:.9}100%{transform:scale(2.4);opacity:0}}
.map-cta{position:absolute;left:1.2rem;bottom:1.2rem;display:flex;gap:.7rem;flex-wrap:wrap}
.map-tag{position:absolute;top:1.2rem;left:1.2rem;background:var(--card);border:1px solid var(--line);border-radius:999px;padding:.5em 1.1em;font-size:.82rem;font-weight:600;box-shadow:var(--shadow-sm)}

/* ============ 16. ФУТЕР ============ */
footer{background:var(--green-dark);color:#9DBFB2;font-size:.9rem}
.foot-top{display:grid;grid-template-columns:1.3fr 1fr 1fr 1.2fr;gap:2.5rem;padding:4rem 0 3rem}
.foot-top .logo{color:var(--cream);margin-bottom:1rem}
.foot-top .lg-mark{background:var(--coral)}
.foot-desc{font-size:.86rem;line-height:1.65;max-width:34ch}
.socials{display:flex;gap:.6rem;margin-top:1.3rem}
.socials a{width:42px;height:42px;border-radius:13px;border:1px solid rgba(243,239,226,.2);display:grid;place-items:center;transition:background .3s,border-color .3s,transform .3s}
.socials a:hover{background:var(--coral);border-color:var(--coral);transform:translateY(-3px)}
.socials svg{width:18px;height:18px;fill:var(--cream)}
.foot-top h4{color:var(--cream);font-size:.82rem;text-transform:uppercase;letter-spacing:.16em;font-family:var(--mono);font-weight:500;margin-bottom:1.1rem}
.foot-links{list-style:none;display:grid;gap:.55rem}
.foot-links a{transition:color .25s,padding-left .3s var(--ease)}
.foot-links a:hover{color:#fff;padding-left:6px}
.foot-contact li{display:flex;gap:.6rem;margin-bottom:.8rem;align-items:flex-start}
.foot-contact b{color:var(--cream);font-weight:600}
.disclaimer{border-top:1px solid rgba(243,239,226,.12);padding:1.1rem 0;text-align:center;font-family:var(--mono);font-size:.68rem;letter-spacing:.14em;color:#6f9386;text-transform:uppercase}
.foot-bottom{border-top:1px solid rgba(243,239,226,.12);padding:1.4rem 0;display:flex;flex-wrap:wrap;gap:.8rem 2rem;justify-content:space-between;font-size:.78rem;color:#6f9386}
.foot-bottom a:hover{color:#fff}

/* ============ 17. МОДАЛКИ / ТОСТЫ / СЛУЖЕБНОЕ ============ */
.modal-backdrop{position:fixed;inset:0;z-index:250;background:rgba(8,32,27,.62);display:grid;place-items:center;padding:1.2rem;opacity:0;visibility:hidden;transition:opacity .4s var(--ease),visibility .4s}
.modal-backdrop.show{opacity:1;visibility:visible}
.modal{width:min(520px,100%);max-height:92vh;overflow:auto;background:var(--card);border-radius:24px;padding:2.2rem;position:relative;transform:translateY(28px) scale(.97);transition:transform .45s var(--ease);box-shadow:0 30px 80px -20px rgba(0,0,0,.4)}
.modal-backdrop.show .modal{transform:none}
.modal-close{position:absolute;top:1.1rem;right:1.1rem;width:40px;height:40px;border-radius:12px;border:1px solid var(--line);display:grid;place-items:center;transition:background .3s,transform .3s}
.modal-close:hover{background:var(--coral-soft);transform:rotate(90deg)}
.modal-close svg{width:16px;height:16px;stroke:var(--ink);stroke-width:2.4;stroke-linecap:round}
.modal .label{margin-bottom:.8rem}
.modal h3{font-family:var(--display);font-weight:400;font-size:1.6rem;margin-bottom:.3rem}
.modal .m-sub{font-size:.88rem;color:var(--ink-soft);margin-bottom:1.5rem}
.modal .f-grid{grid-template-columns:1fr}
#toastBox{position:fixed;right:1.2rem;bottom:1.2rem;z-index:280;display:flex;flex-direction:column;gap:.7rem}
.toast{display:flex;gap:.8rem;align-items:center;background:var(--green-dark);color:var(--cream);padding:.95rem 1.3rem;border-radius:15px;box-shadow:var(--shadow);font-size:.9rem;max-width:360px;transform:translateX(120%);opacity:0;transition:transform .5s var(--ease),opacity .5s}
.toast.show{transform:none;opacity:1}
.toast .t-dot{flex:none;width:10px;height:10px;border-radius:50%;background:var(--coral)}
#backTop{position:fixed;right:1.2rem;bottom:1.2rem;z-index:140;width:50px;height:50px;border-radius:50%;background:var(--green);color:var(--cream);display:grid;place-items:center;box-shadow:var(--shadow);opacity:0;visibility:hidden;transform:translateY(14px);transition:opacity .4s,transform .4s,visibility .4s,background .3s}
#backTop.show{opacity:1;visibility:visible;transform:none}
#backTop:hover{background:var(--coral)}
#backTop svg{width:19px;height:19px;stroke:currentColor;fill:none;stroke-width:2.4;stroke-linecap:round;stroke-linejoin:round}

/* мобильная панель действий */
#mobileBar{position:fixed;left:0;right:0;bottom:0;z-index:145;display:none;grid-template-columns:1fr 1fr;gap:.6rem;padding:.7rem .9rem calc(.7rem + env(safe-area-inset-bottom));background:rgba(8,43,36,.96);backdrop-filter:blur(8px);border-top:1px solid rgba(243,239,226,.14)}
#mobileBar .btn{padding:.9em}

/* ============ 18. REVEAL ============ */
.js [data-reveal]{opacity:0;transform:translateY(28px);transition:opacity .8s var(--ease),transform .8s var(--ease)}
.js [data-reveal].revealed{opacity:1;transform:none}

/* ============ 19. АДАПТИВ ============ */
@media (max-width:1100px){
  .srv-grid,.doc-grid{grid-template-columns:repeat(2,1fr)}
  .steps-grid{grid-template-columns:repeat(2,1fr)}
  .steps-grid::before{display:none}
  .foot-top{grid-template-columns:1fr 1fr}
  .chip-1{left:0}.chip-2{right:0}
}
@media (max-width:960px){
  .nav-links,.head-phone{display:none}
  #burgerBtn{display:block}
  .hero-grid{grid-template-columns:1fr;gap:2.6rem;min-height:0}
  .hero-visual{max-width:480px}
  .about-grid{grid-template-columns:1fr;gap:2.6rem}
  .about-sticky{position:static}
  .contacts-grid{grid-template-columns:1fr}
  .map-box{min-height:320px}
  .appt-card{grid-template-columns:1fr}
  .quick-links{grid-template-columns:repeat(2,1fr)}
}
@media (max-width:760px){
  .topbar .hide-m{display:none}
  .stats-grid{grid-template-columns:repeat(2,1fr);gap:2rem 0}
  .stat:nth-child(3){border-left:none;padding-left:0}
  .srv-grid,.doc-grid{grid-template-columns:1fr}
  .f-grid{grid-template-columns:1fr}
  .pl-row{grid-template-columns:1fr auto;padding:1rem 1.2rem;row-gap:.5rem}
  .pl-row .pl-note-cell{display:none}
  .pl-row .btn-sm{grid-column:1/-1}
}
@media (max-width:640px){
  body{padding-bottom:74px}
  #mobileBar{display:grid}
  #backTop{bottom:88px}
  #toastBox{bottom:88px;left:1rem;right:1rem;align-items:stretch}
  .toast{max-width:none}
  .head-cta{display:none}
  .quick-links{grid-template-columns:1fr}
  .hero{padding-top:1.6rem}
  .modal{padding:1.7rem 1.4rem}
  .steps-grid{grid-template-columns:1fr}
  .step{padding-top:2.2rem}
  .foot-top{grid-template-columns:1fr;gap:2rem}
}

/* ============ 20. REDUCED MOTION ============ */
@media (prefers-reduced-motion:reduce){
  html{scroll-behavior:auto}
  *,*::before,*::after{animation-duration:.001s!important;animation-iteration-count:1!important;transition-duration:.001s!important}
  .line-in,.hero-sub,.hero-cta,.hero-trust,.hero-visual{opacity:1!important;transform:none!important}
  .js [data-reveal]{opacity:1;transform:none}
  .ecg-run{display:none}
  .marquee-track{animation:none;flex-wrap:wrap;width:auto}
  #preloader{display:none}
}
</style>
</head>
<body>

<!-- прелоадер -->
<div id="preloader" aria-hidden="true">
  <div class="pl-logo">ПУЛЬС<b>·</b></div>
  <svg viewBox="0 0 300 60" aria-hidden="true">
    <path class="pl-line" pathLength="1000" d="M0 30 h60 q8 -14 16 0 h26 l6 -22 l8 40 l7 -18 h30 q9 -13 18 0 h129"/>
    <circle class="pl-dot" cx="292" cy="30" r="4"/>
  </svg>
</div>

<div id="progressBar" aria-hidden="true"></div>
<div class="noise" aria-hidden="true"></div>

<!-- ======= ШАПКА ======= -->
<header class="site" id="siteHeader">
  <div class="topbar">
    <div class="container">
      <span class="open-badge" id="openStatus"><i></i>Проверяем часы…</span>
      <span class="sep hide-m">·</span>
      <a href="#contacts" class="hide-m">Москва, ул. Лесная, 7 · м. Белорусская</a>
      <span class="grow"></span>
      <a href="mailto:info@puls-clinic.ru" class="hide-m">info@puls-clinic.ru</a>
      <span class="sep hide-m">·</span>
      <a href="tel:+74951234567"><b style="font-family:var(--mono)">+7 (495) 123-45-67</b></a>
    </div>
  </div>
  <div class="container nav-row">
    <a href="#home" class="logo" aria-label="Клиника Пульс — на главную">
      <span class="lg-mark"><svg viewBox="0 0 24 24"><path d="M3 12h4l2-5 3 10 2-5h7"/></svg></span>
      <span>Пульс<small>клиника общей практики</small></span>
    </a>
    <nav class="nav-links" aria-label="Основная навигация">
      <a href="#about" data-spy="about">О клинике</a>
      <a href="#services" data-spy="services">Отделения</a>
      <a href="#prices" data-spy="prices">Цены</a>
      <a href="#doctors" data-spy="doctors">Врачи</a>
      <a href="#reviews" data-spy="reviews">Отзывы</a>
      <a href="#contacts" data-spy="contacts">Контакты</a>
    </nav>
    <a class="head-phone" href="tel:+74951234567"><b>+7 (495) 123-45-67</b><span>ежедневно 8:00–21:00</span></a>
    <button class="btn btn-coral head-cta" data-modal-open="#appointmentModal">Записаться</button>
    <button id="burgerBtn" aria-label="Открыть меню" aria-expanded="false"><span></span><span></span><span></span></button>
  </div>
</header>

<!-- мобильное меню -->
<nav id="mobileMenu" aria-label="Мобильное меню">
  <a class="mm-link js-menu-link" href="#about"><em>01</em>О клинике</a>
  <a class="mm-link js-menu-link" href="#services"><em>02</em>Отделения</a>
  <a class="mm-link js-menu-link" href="#prices"><em>03</em>Цены</a>
  <a class="mm-link js-menu-link" href="#doctors"><em>04</em>Врачи</a>
  <a class="mm-link js-menu-link" href="#reviews"><em>05</em>Отзывы</a>
  <a class="mm-link js-menu-link" href="#contacts"><em>06</em>Контакты</a>
  <div class="mm-foot">
    <a class="tel" href="tel:+74951234567">+7 (495) 123-45-67</a>
    <button class="btn btn-coral js-menu-link" data-modal-open="#appointmentModal">Записаться на приём</button>
  </div>
</nav>

<main>
<!-- ======= ГЕРОЙ ======= -->
<section class="hero" id="home">
  <div class="container">
    <div class="hero-grid">
      <div>
        <p class="label hero-over" id="scrambleLine" data-text="Частная клиника общей практики · Москва">Частная клиника общей практики · Москва</p>
        <h1>
          <span class="line"><span class="line-in">Здоровье начинается</span></span>
          <span class="line"><span class="line-in">с <span class="accent">внимательного</span></span></span>
          <span class="line"><span class="line-in">врача</span></span>
        </h1>
        <p class="hero-sub">Приём специалистов, диагностика и анализы в одном месте — строго по записи, без очередей и спешки. Запись в день обращения.</p>
        <div class="hero-cta">
          <button class="btn btn-primary" data-modal-open="#appointmentModal">Записаться на приём
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
          </button>
          <a class="btn btn-ghost" href="#prices">Смотреть цены</a>
        </div>
        <div class="hero-trust">
          <span><span class="stars" aria-hidden="true">★★★★★</span> <b>4,9</b> — 3 214 отзывов</span>
          <span>🩺 <b>Приём в день</b> обращения</span>
          <span>👨‍⚕️ <b>12</b> кандидатов наук</span>
        </div>
      </div>
      <div class="hero-visual">
        <div class="hero-photo">
          <img src="https://picsum.photos/seed/clinic-doctor-reception/640/740" alt="Приём врача в клинике «Пульс»" fetchpriority="high">
        </div>
        <div class="float-chip chip-1"><span class="fc-ico">✚</span><span>18 лет заботы<small>работаем с 2008 года</small></span></div>
        <div class="float-chip chip-2"><span class="fc-ico">♥</span><span>96 000+ пациентов<small>доверяют нам здоровье</small></span></div>
      </div>
    </div>

    <div class="ecg-wrap" aria-hidden="true">
      <svg viewBox="0 0 1440 120" preserveAspectRatio="none">
        <path class="ecg-base" d="M0 70 h110 q14 -20 28 0 h44 l9 -38 l13 70 l11 -32 h50 q16 -22 32 0 h96 h110 q14 -20 28 0 h44 l9 -38 l13 70 l11 -32 h50 q16 -22 32 0 h96 h110 q14 -20 28 0 h44 l9 -38 l13 70 l11 -32 h50 q16 -22 32 0 h96 h260"/>
        <path class="ecg-run" pathLength="1000" d="M0 70 h110 q14 -20 28 0 h44 l9 -38 l13 70 l11 -32 h50 q16 -22 32 0 h96 h110 q14 -20 28 0 h44 l9 -38 l13 70 l11 -32 h50 q16 -22 32 0 h96 h110 q14 -20 28 0 h44 l9 -38 l13 70 l11 -32 h50 q16 -22 32 0 h96 h260"/>
      </svg>
    </div>

    <div class="quick-links">
      <button class="ql-card" data-modal-open="#appointmentModal" data-service="Вызов врача на дом">
        <span class="ql-ico"><svg viewBox="0 0 24 24"><path d="M3 11l9-8 9 8M5 9.5V21h14V9.5M9 21v-6h6v6"/></svg></span>
        <b>Вызвать врача на дом</b><small>Приедем в течение 2 часов в пределах МКАД</small>
        <span class="ql-go">Вызвать <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg></span>
      </button>
      <button class="ql-card js-goto-price" data-tab="Анализы">
        <span class="ql-ico"><svg viewBox="0 0 24 24"><path d="M9 3h6M10 3v6l-5.2 8.7A3 3 0 0 0 7.4 22h9.2a3 3 0 0 0 2.6-4.3L14 9V3M8 15h8"/></svg></span>
        <b>Сдать анализы</b><small>Без записи до 12:00, результаты на e-mail</small>
        <span class="ql-go">Смотреть цены <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg></span>
      </button>
      <button class="ql-card js-goto-price" data-tab="Диагностика">
        <span class="ql-ico"><svg viewBox="0 0 24 24"><path d="M4 12a8 8 0 0 1 16 0M7 12a5 5 0 0 1 10 0M10 12a2 2 0 0 1 4 0M12 12v8"/></svg></span>
        <b>УЗИ-диагностика</b><small>Экспертные аппараты, результат в день приёма</small>
        <span class="ql-go">Смотреть цены <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg></span>
      </button>
      <button class="ql-card" data-modal-open="#appointmentModal" data-service="Онлайн-консультация">
        <span class="ql-ico"><svg viewBox="0 0 24 24"><rect x="2" y="6" width="14" height="12" rx="2.5"/><path d="M16 10.5l6-3.5v10l-6-3.5"/></svg></span>
        <b>Онлайн-консультация</b><small>Видеосвязь с врачом из любой точки мира</small>
        <span class="ql-go">Записаться <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg></span>
      </button>
    </div>
  </div>

  <!-- цифры -->
  <div class="stats">
    <div class="container stats-grid">
      <div class="stat" data-reveal><div class="num"><span data-count="18">0</span></div><p>лет врачебной практики</p></div>
      <div class="stat" data-reveal data-delay="90"><div class="num"><span data-count="42">0</span></div><p>врача, из них 12 кандидатов наук</p></div>
      <div class="stat" data-reveal data-delay="180"><div class="num"><span data-count="96000">0</span><sup>+</sup></div><p>пациентов доверяют нам здоровье</p></div>
      <div class="stat" data-reveal data-delay="270"><div class="num"><span data-count="4.9" data-dec="1">0</span></div><p>средняя оценка на независимых площадках</p></div>
    </div>
  </div>

  <div class="marquee" aria-hidden="true">
    <div class="marquee-track" id="marqueeTrack">
      <span>Терапия <span class="plus">✚</span></span><span>Кардиология <span class="plus">✚</span></span><span>Неврология <span class="plus">✚</span></span><span>Эндокринология <span class="plus">✚</span></span><span>Оториноларингология <span class="plus">✚</span></span><span>Педиатрия <span class="plus">✚</span></span><span>УЗИ-диагностика <span class="plus">✚</span></span><span>Лаборатория <span class="plus">✚</span></span><span>Вакцинация <span class="plus">✚</span></span>
    </div>
  </div>
</section>

<!-- ======= О КЛИНИКЕ ======= -->
<section class="section" id="about">
  <div class="container about-grid">
    <div class="about-sticky">
      <p class="label" data-reveal>01 · О клинике</p>
      <h2 class="h2" data-reveal data-delay="80">Медицина, в которой вас слышат</h2>
      <p class="lead" data-reveal data-delay="150">«Пульс» — клиника общей практики для всей семьи. Мы объединили терапевтов, узких специалистов и диагностику под одной крышей, чтобы путь от жалобы до диагноза занимал дни, а не недели.</p>
      <div class="values">
        <div class="value" data-reveal><span class="v-ico"><svg viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg></span><span><b>Доказательная медицина</b><p>Назначения строго по клиническим рекомендациям — без лишних процедур.</p></span></div>
        <div class="value" data-reveal data-delay="80"><span class="v-ico"><svg viewBox="0 0 24 24"><circle cx="12" cy="8" r="4"/><path d="M4 21c0-4 3.6-6.5 8-6.5s8 2.5 8 6.5"/></svg></span><span><b>Врачи с именем</b><p>Высшая категория, учёные степени, постоянное обучение.</p></span></div>
        <div class="value" data-reveal data-delay="160"><span class="v-ico"><svg viewBox="0 0 24 24"><path d="M12 2l8 4v6c0 5-3.5 8.5-8 10-4.5-1.5-8-5-8-10V6l8-4z"/></svg></span><span><b>Прозрачные цены</b><p>Стоимость известна до начала лечения. Никаких скрытых доплат.</p></span></div>
        <div class="value" data-reveal data-delay="240"><span class="v-ico"><svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3.5 2.5"/></svg></span><span><b>Без очередей</b><p>Приём строго по записи, интервал между пациентами — 30 минут.</p></span></div>
      </div>
      <div class="dms" data-reveal>
        <em style="font-style:normal">Работаем по ДМС:</em>
        <span>Ингосстрах</span><span>СОГАЗ</span><span>РЕСО-Гарантия</span><span>АльфаСтрахование</span><span>ВСК</span>
      </div>
    </div>
    <div class="about-pics" data-reveal data-delay="120">
      <figure><img src="https://picsum.photos/seed/clinic-lobby-interior/900/520" alt="Интерьер холла клиники" loading="lazy"></figure>
      <figure><img src="https://picsum.photos/seed/clinic-ultrasound-room/460/540" alt="Кабинет УЗИ-диагностики" loading="lazy"></figure>
      <figure><img src="https://picsum.photos/seed/clinic-laboratory/460/540" alt="Лаборатория клиники" loading="lazy"></figure>
      <div class="exp-badge"><b>18</b>лет с вами</div>
    </div>
  </div>
</section>

<!-- ======= ОТДЕЛЕНИЯ ======= -->
<section class="section services" id="services">
  <div class="container">
    <div class="sec-head">
      <div>
        <p class="label" data-reveal>02 · Отделения</p>
        <h2 class="h2" data-reveal data-delay="80" style="margin-top:1rem">Все направления — в одном месте</h2>
      </div>
      <p class="lead" data-reveal data-delay="150" style="max-width:38ch">От планового осмотра до узкой диагностики. Не знаете, к кому записатьсясь? Начните с терапевта — он составит маршрут.</p>
    </div>
    <div class="srv-grid">
      <article class="srv-card" data-reveal>
        <span class="srv-ico"><svg viewBox="0 0 24 24"><path d="M5 3v5a5 5 0 0 0 10 0V3M10 13v3a5 5 0 0 0 10 0v-2"/><circle cx="20" cy="11" r="2.4"/></svg></span>
        <h3>Терапия</h3>
        <p>Первичная диагностика, лечение ОРВИ и хронических заболеваний, больничные листы, справки и чек-апы.</p>
        <div class="srv-foot"><span class="srv-price">от 2 400 ₽<small>приём 60 минут</small></span><button class="srv-book js-book" data-service="Терапия" data-label="Приём терапевта">Записаться <svg viewBox="0 0 24 24"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div>
      </article>
      <article class="srv-card" data-reveal data-delay="80">
        <span class="srv-ico"><svg viewBox="0 0 24 24"><path d="M12 20.5C6.5 16 3 12.7 3 8.9A4.6 4.6 0 0 1 12 6.4a4.6 4.6 0 0 1 9 2.5c0 3.8-3.5 7.1-9 11.6z"/><path d="M6 12h3l1.5-3 2.5 6 1.5-3h3.5"/></svg></span>
        <h3>Кардиология</h3>
        <p>Давление, аритмия, боли в груди. ЭКГ, ЭхоКГ и холтер — на месте, расшифровка в день приёма.</p>
        <div class="srv-foot"><span class="srv-price">от 2 900 ₽<small>приём к.м.н.</small></span><button class="srv-book js-book" data-service="Кардиология" data-label="Приём кардиолога">Записаться <svg viewBox="0 0 24 24"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div>
      </article>
      <article class="srv-card" data-reveal data-delay="160">
        <span class="srv-ico"><svg viewBox="0 0 24 24"><path d="M13 2L4.5 13.5H11L9.5 22 19 9.5h-6.5L13 2z"/></svg></span>
        <h3>Неврология</h3>
        <p>Головные боли, головокружения, боли в спине, нарушения сна. Осмотр и план обследования за один визит.</p>
        <div class="srv-foot"><span class="srv-price">от 2 700 ₽<small>приём 45 минут</small></span><button class="srv-book js-book" data-service="Неврология" data-label="Приём невролога">Записаться <svg viewBox="0 0 24 24"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div>
      </article>
      <article class="srv-card" data-reveal>
        <span class="srv-ico"><svg viewBox="0 0 24 24"><path d="M12 3c3.5 4.2 6 7.6 6 10.6a6 6 0 1 1-12 0C6 10.6 8.5 7.2 12 3z"/></svg></span>
        <h3>Эндокринология</h3>
        <p>Щитовидная железа, диабет, лишний вес, усталость. Гормоны — в своей лаборатории за 1 день.</p>
        <div class="srv-foot"><span class="srv-price">от 2 700 ₽<small>приём 45 минут</small></span><button class="srv-book js-book" data-service="Эндокринология" data-label="Приём эндокринолога">Записаться <svg viewBox="0 0 24 24"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div>
      </article>
      <article class="srv-card" data-reveal data-delay="80">
        <span class="srv-ico"><svg viewBox="0 0 24 24"><path d="M4 12a8 8 0 0 1 16 0M7.5 12a4.5 4.5 0 0 1 9 0M10.5 12a1.5 1.5 0 0 1 3 0M12 13.5V21"/></svg></span>
        <h3>УЗИ и функциональная диагностика</h3>
        <p>УЗИ всех органов, ЭКГ, ЭхоКГ, холтер, спирометрия. Аппараты экспертного класса.</p>
        <div class="srv-foot"><span class="srv-price">от 1 600 ₽<small>результат сразу</small></span><button class="srv-book js-book" data-service="УЗИ и функциональная диагностика" data-label="УЗИ-диагностика">Записаться <svg viewBox="0 0 24 24"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div>
      </article>
      <article class="srv-card" data-reveal data-delay="160">
        <span class="srv-ico"><svg viewBox="0 0 24 24"><path d="M9 3h6M10 3v6l-5.2 8.7A3 3 0 0 0 7.4 22h9.2a3 3 0 0 0 2.6-4.3L14 9V3M8 15h8"/></svg></span>
        <h3>Лаборатория</h3>
        <p>Более 1 200 видов анализов. Без записи до 12:00, результаты на e-mail уже на следующий день.</p>
        <div class="srv-foot"><span class="srv-price">от 350 ₽<small>забор крови 250 ₽</small></span><button class="srv-book js-book" data-service="Анализы" data-label="Лабораторные анализы">Записаться <svg viewBox="0 0 24 24"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div>
      </article>
    </div>
  </div>
</section>

<!-- ======= КАК ПРОХОДИТ ПРИЁМ ======= -->
<section class="section">
  <div class="container">
    <div class="sec-head" style="justify-content:center;text-align:center">
      <div>
        <p class="label" data-reveal>03 · Как это работает</p>
        <h2 class="h2" data-reveal data-delay="80" style="margin-top:1rem">Четыре шага до выздоровления</h2>
      </div>
    </div>
    <div class="steps-grid">
      <div class="step" data-reveal><span class="st-num">01</span><h3>Оставьте заявку</h3><p>На сайте или по телефону. Администратор подберёт врача и удобное время за 5 минут.</p></div>
      <div class="step" data-reveal data-delay="100"><span class="st-num">02</span><h3>Подтверждение</h3><p>Пришлём SMS с адресом и памяткой. За день до визита напомним о приёме.</p></div>
      <div class="step" data-reveal data-delay="200"><span class="st-num">03</span><h3>Приём врача</h3><p>30–60 минут без спешки: врач выслушает, проведёт осмотр и при необходимости назначит обследование.</p></div>
      <div class="step" data-reveal data-delay="300"><span class="st-num">04</span><h3>План лечения</h3><p>Понятная схема лечения, результаты анализов в электронном виде, связь с врачом в мессенджере.</p></div>
    </div>
  </div>
</section>

<!-- ======= ЦЕНЫ ======= -->
<section class="section prices" id="prices">
  <div class="container">
    <div class="sec-head">
      <div>
        <p class="label" data-reveal>04 · Прайс-лист</p>
        <h2 class="h2" data-reveal data-delay="80" style="margin-top:1rem">Честные цены без звёздочек</h2>
      </div>
      <p class="lead" data-reveal data-delay="150" style="max-width:36ch">Стоимость известна до начала лечения. Цены действуют с 1 июля 2026 года.</p>
    </div>

    <div class="prices-tools" data-reveal>
      <div class="price-tabs" role="tablist" aria-label="Категории прайс-листа" id="priceTabs">
        <button class="price-tab" role="tab" aria-selected="true" data-tab="Приём специалистов">Приём</button>
        <button class="price-tab" role="tab" aria-selected="false" data-tab="Диагностика">Диагностика</button>
        <button class="price-tab" role="tab" aria-selected="false" data-tab="Анализы">Анализы</button>
        <button class="price-tab" role="tab" aria-selected="false" data-tab="Процедуры">Процедуры</button>
      </div>
      <div class="price-search">
        <svg viewBox="0 0 24 24"><circle cx="11" cy="11" r="7"/><path d="M20 20l-3.5-3.5"/></svg>
        <input type="search" id="priceSearch" placeholder="Поиск: УЗИ, ЭКГ, анализ…" aria-label="Поиск по прайс-листу">
      </div>
    </div>

    <div class="price-list" id="priceList" data-reveal data-delay="120" aria-live="polite"></div>
    <div class="price-note">
      <span id="priceCount">Загрузка…</span>
      <button class="btn btn-ghost btn-sm" id="priceDownload">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 3v12m0 0l-4-4m4 4l4-4M4 19h16"/></svg>
        Скачать полный прайс
      </button>
    </div>
  </div>
</section>

<!-- ======= ВРАЧИ ======= -->
<section class="section" id="doctors">
  <div class="container">
    <div class="sec-head">
      <div>
        <p class="label" data-reveal>05 · Команда</p>
        <h2 class="h2" data-reveal data-delay="80" style="margin-top:1rem">Врачи, к которым возвращаются</h2>
      </div>
      <p class="lead" data-reveal data-delay="150" style="max-width:36ch">Каждый врач проходит внутреннюю аттестацию раз в два года и ведёт приём строго по расписанию.</p>
    </div>
    <div class="doc-grid">
      <article class="doc-card" data-reveal>
        <div class="doc-ph"><img src="https://picsum.photos/seed/doctor-anna-vetrova/460/490" alt="Анна Ветрова, терапевт-кардиолог" loading="lazy"><span class="doc-exp">стаж 16 лет</span></div>
        <div class="doc-body"><h3>Анна Ветрова</h3><span class="doc-spec">Терапевт · Кардиолог</span><p class="doc-meta">к.м.н., доцент. Ведёт пациентов с гипертонией, аритмией, хронической усталостью.</p>
        <div class="doc-foot"><span class="doc-price">2 900 ₽<small>приём 60 минут</small></span><button class="btn btn-ghost btn-sm js-book-doc" data-doctor="Анна Ветрова" data-service="Кардиология">Записаться</button></div></div>
      </article>
      <article class="doc-card" data-reveal data-delay="80">
        <div class="doc-ph"><img src="https://picsum.photos/seed/doctor-dmitry-sokolov/460/490" alt="Дмитрий Соколов, невролог" loading="lazy"><span class="doc-exp">стаж 14 лет</span></div>
        <div class="doc-body"><h3>Дмитрий Соколов</h3><span class="doc-spec">Невролог</span><p class="doc-meta">Специалист по головной боли и боли в спине. Автор 20+ публикаций.</p>
        <div class="doc-foot"><span class="doc-price">2 700 ₽<small>приём 45 минут</small></span><button class="btn btn-ghost btn-sm js-book-doc" data-doctor="Дмитрий Соколов" data-service="Неврология">Записаться</button></div></div>
      </article>
      <article class="doc-card" data-reveal data-delay="160">
        <div class="doc-ph"><img src="https://picsum.photos/seed/doctor-maria-lanskaya/460/490" alt="Мария Ланская, эндокринолог" loading="lazy"><span class="doc-exp">стаж 11 лет</span></div>
        <div class="doc-body"><h3>Мария Ланская</h3><span class="doc-spec">Эндокринолог</span><p class="doc-meta">Щитовидная железа, диабет, коррекция веса. Член Российской ассоциации эндокринологов.</p>
        <div class="doc-foot"><span class="doc-price">2 700 ₽<small>приём 45 минут</small></span><button class="btn btn-ghost btn-sm js-book-doc" data-doctor="Мария Ланская" data-service="Эндокринология">Записаться</button></div></div>
      </article>
      <article class="doc-card" data-reveal>
        <div class="doc-ph"><img src="https://picsum.photos/seed/doctor-igor-melnik/460/490" alt="Игорь Мельник, врач УЗД" loading="lazy"><span class="doc-exp">стаж 12 лет</span></div>
        <div class="doc-body"><h3>Игорь Мельник</h3><span class="doc-spec">Врач УЗ-диагностики</span><p class="doc-meta">УЗИ органов, сосудов и сердца. Расшифровка и заключение сразу после исследования.</p>
        <div class="doc-foot"><span class="doc-price">2 400 ₽<small>исследование</small></span><button class="btn btn-ghost btn-sm js-book-doc" data-doctor="Игорь Мельник" data-service="УЗИ и функциональная диагностика">Записаться</button></div></div>
      </article>
      <article class="doc-card" data-reveal data-delay="80">
        <div class="doc-ph"><img src="https://picsum.photos/seed/doctor-polina-ageeva/460/490" alt="Полина Агеева, педиатр" loading="lazy"><span class="doc-exp">стаж 9 лет</span></div>
        <div class="doc-body"><h3>Полина Агеева</h3><span class="doc-spec">Педиатр</span><p class="doc-meta">Дети с рождения. Вакцинация, наблюдение первого года жизни, справки в сад и школу.</p>
        <div class="doc-foot"><span class="doc-price">2 400 ₽<small>приём 45 минут</small></span><button class="btn btn-ghost btn-sm js-book-doc" data-doctor="Полина Агеева" data-service="Педиатрия">Записаться</button></div></div>
      </article>
      <article class="doc-card" data-reveal data-delay="160">
        <div class="doc-ph"><img src="https://picsum.photos/seed/doctor-sergey-kovalev/460/490" alt="Сергей Ковалёв, оториноларинголог" loading="lazy"><span class="doc-exp">стаж 17 лет</span></div>
        <div class="doc-body"><h3>Сергей Ковалёв</h3><span class="doc-spec">Оториноларинголог</span><p class="doc-meta">ЛОР-хирург. Лечение sinusitis, промывания, малые амбулаторные операции.</p>
        <div class="doc-foot"><span class="doc-price">2 800 ₽<small>приём 45 минут</small></span><button class="btn btn-ghost btn-sm js-book-doc" data-doctor="Сергей Ковалёв" data-service="ЛОР">Записаться</button></div></div>
      </article>
    </div>
  </div>
</section>

<!-- ======= ОТЗЫВЫ ======= -->
<section class="section reviews" id="reviews">
  <div class="container">
    <div class="sec-head">
      <div>
        <p class="label light" data-reveal>06 · Отзывы</p>
        <h2 class="h2" data-reveal data-delay="80" style="margin-top:1rem">Что говорят пациенты</h2>
      </div>
      <div class="rating-big" data-reveal data-delay="150">
        <span class="rb-num">4,9</span>
        <span><span class="stars" aria-hidden="true">★★★★★</span><small>3 214 отзывов на ПроДокторов,<br>Яндекс Картах и 2ГИС</small></span>
      </div>
    </div>
    <div class="slider" id="reviewsSlider" data-reveal tabindex="0" aria-roledescription="карусель" aria-label="Отзывы пациентов">
      <div class="slider-viewport">
        <ul class="slider-track" id="revTrack">
          <li><div class="rev-card"><div class="rev-top"><span class="rev-ava">МК</span><span><b>Марина К.</b><small>28 июля 2026</small></span><span class="stars" style="margin-left:auto" aria-label="Оценка 5 из 5">★★★★★</span></div><p>Наблюдаюсь у Анны Сергеевны третий год. Впервые встречаю врача, который объясняет анализы человеческим языком и не назначает ничего лишнего. Отдельное спасибо администраторам — всегда напомнят о приёме.</p><div class="rev-src"><span>ПроДокторов</span><span>Подтверждённый визит</span></div></div></li>
          <li><div class="rev-card"><div class="rev-top"><span class="rev-ava">ИТ</span><span><b>Игорь Т.</b><small>12 июля 2026</small></span><span class="stars" style="margin-left:auto" aria-label="Оценка 5 из 5">★★★★★</span></div><p>Пришёл с болью в спине, которую терпел полгода. Дмитрий Владимирович за один приём разобрался, назначил только нужные обследования. Через две недели живу нормальной жизнью. Рекомендую.</p><div class="rev-src"><span>Яндекс Карты</span><span>Подтверждённый визит</span></div></div></li>
          <li><div class="rev-card"><div class="rev-top"><span class="rev-ava">СД</span><span><b>Светлана Д.</b><small>30 июня 2026</small></span><span class="stars" style="margin-left:auto" aria-label="Оценка 5 из 5">★★★★★</span></div><p>Сдавали анализы всей семьёй — пришли без записи утром, взяли кровь за 10 минут, детям даже подарили наклейки. Результаты пришли на почту на следующий день, как и обещали.</p><div class="rev-src"><span>2ГИС</span><span>Подтверждённый визит</span></div></div></li>
          <li><div class="rev-card"><div class="rev-top"><span class="rev-ava">АП</span><span><b>Алексей П.</b><small>18 июня 2026</small></span><span class="stars" style="margin-left:auto" aria-label="Оценка 5 из 5">★★★★★</span></div><p>Панически боялся идти к врачу после неудачного опыта. Здесь всё иначе: никто никуда не торопит, всё объясняют, цены озвучили заранее до рубля. Теперь вся семья ходит только сюда.</p><div class="rev-src"><span>ПроДокторов</span><span>Подтверждённый визит</span></div></div></li>
          <li><div class="rev-card"><div class="rev-top"><span class="rev-ava">НВ</span><span><b>Наталья В.</b><small>2 июня 2026</small></span><span class="stars" style="margin-left:auto" aria-label="Оценка 5 из 5">★★★★★</span></div><p>Вызывали терапевта на дом для бабушки — врач приехал через полтора часа, внимательно осмотрел, скорректировал лечение и оставил свой номер для вопросов. Очень человеческое отношение.</p><div class="rev-src"><span>Яндекс Карты</span><span>Подтверждённый визит</span></div></div></li>
          <li><div class="rev-card"><div class="rev-top"><span class="rev-ava">ДР</span><span><b>Дмитрий Р.</b><small>21 мая 2026</small></span><span class="stars" style="margin-left:auto" aria-label="Оценка 4 из 5">★★★★☆</span></div><p>Делал ЭхоКГ у Игоря Петровича — всё чётко и по делу, заключение выдали сразу с подробным объяснением. Минус одна звезда за то, что сложно дозвониться вечером — лучше записываться через сайт.</p><div class="rev-src"><span>Отзовик</span><span>Подтверждённый визит</span></div></div></li>
        </ul>
      </div>
      <div class="slider-ctrl">
        <button class="sl-btn" id="revPrev" aria-label="Предыдущие отзывы"><svg viewBox="0 0 24 24"><path d="M15 5l-7 7 7 7"/></svg></button>
        <button class="sl-btn" id="revNext" aria-label="Следующие отзывы"><svg viewBox="0 0 24 24"><path d="M9 5l7 7-7 7"/></svg></button>
        <div class="sl-dots" id="revDots"></div>
      </div>
    </div>
  </div>
</section>

<!-- ======= FAQ ======= -->
<section class="section" id="faq">
  <div class="container">
    <div class="sec-head" style="justify-content:center;text-align:center">
      <div>
        <p class="label" data-reveal>07 · Вопросы и ответы</p>
        <h2 class="h2" data-reveal data-delay="80" style="margin-top:1rem">Спрашивали? Отвечаем</h2>
      </div>
    </div>
    <div class="faq-wrap">
      <div class="acc-item open" data-reveal>
        <button class="acc-btn" aria-expanded="true">Как записаться на приём?<span class="acc-ico"><svg viewBox="0 0 24 24"><path d="M12 5v14M5 12h14"/></svg></span></button>
        <div class="acc-panel"><div class="acc-body">Тремя способами: кнопкой «Записаться» на сайте, по телефону +7 (495) 123-45-67 или в мессенджерах (Telegram, WhatsApp). Администратор подберёт врача и время, подтверждение придёт в SMS. Обычно есть слоты на сегодня-завтра.</div></div>
      </div>
      <div class="acc-item" data-reveal data-delay="60">
        <button class="acc-btn" aria-expanded="false">Что взять с собой на первый приём?<span class="acc-ico"><svg viewBox="0 0 24 24"><path d="M12 5v14M5 12h14"/></svg></span></button>
        <div class="acc-panel"><div class="acc-body">Паспорт и, если есть, результаты предыдущих обследований и выписки — это сэкономит время и поможет врачу. Приходите за 10 минут до приёма, чтобы спокойно оформить карту.</div></div>
      </div>
      <div class="acc-item" data-reveal data-delay="120">
        <button class="acc-btn" aria-expanded="false">Работаете ли вы по ДМС?<span class="acc-ico"><svg viewBox="0 0 24 24"><path d="M12 5v14M5 12h14"/></svg></span></button>
        <div class="acc-panel"><div class="acc-body">Да, мы работаем с пятью страховыми компаниями: Ингосстрах, СОГАЗ, РЕСО-Гарантия, АльфаСтрахование и ВСК. Перечень услуг по вашему полису уточнит администратор — достаточно назвать страховую и номер полиса.</div></div>
      </div>
      <div class="acc-item" data-reveal data-delay="180">
        <button class="acc-btn" aria-expanded="false">Как подготовиться к сдаче анализов?<span class="acc-ico"><svg viewBox="0 0 24 24"><path d="M12 5v14M5 12h14"/></svg></span></button>
        <div class="acc-panel"><div class="acc-body">Кровь сдаётся натощак после 8–14 часов голодания, воду пить можно. За сутки исключите алкоголь и интенсивные тренировки. Для отдельных исследований есть особые правила — администратор пришлёт памятку при записи.</div></div>
      </div>
      <div class="acc-item" data-reveal data-delay="240">
        <button class="acc-btn" aria-expanded="false">Выезжаете ли вы на дом?<span class="acc-ico"><svg viewBox="0 0 24 24"><path d="M12 5v14M5 12h14"/></svg></span></button>
        <div class="acc-panel"><div class="acc-body">Да, терапевт и педиатр выезжают по Москве в пределах МКАД и до 15 км за МКАД. При заказе до 18:00 врач приедет в тот же день, обычно в течение двух часов. Также на дому можно сдать анализы и сделать ЭКГ.</div></div>
      </div>
      <div class="acc-item" data-reveal data-delay="300">
        <button class="acc-btn" aria-expanded="false">Есть ли парковка и доступная среда?<span class="acc-ico"><svg viewBox="0 0 24 24"><path d="M12 5v14M5 12h14"/></svg></span></button>
        <div class="acc-panel"><div class="acc-body">Бесплатная парковка для пациентов во дворе клиники (въезд со стороны 2-го Лесного переулка). Вход оборудован пандусом, внутри — лифт и широкие дверные проёмы. Маломобильных пациентов сопровождаем.</div></div>
      </div>
    </div>
  </div>
</section>

<!-- ======= ЗАПИСЬ ======= -->
<section class="section appt" id="appointment">
  <div class="container">
    <div class="appt-card" data-reveal>
      <div class="appt-info">
        <p class="label light">08 · Запись на приём</p>
        <h3>Оставьте заявку — перезвоним в течение 15 минут</h3>
        <a class="appt-phone" href="tel:+74951234567">+7 (495) 123-45-67</a>
        <ul>
          <li><svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3.5 2.5"/></svg>Пн–Пт 8:00–21:00 · Сб–Вс 9:00–20:00</li>
          <li><svg viewBox="0 0 24 24"><path d="M12 21C7 16.5 4 13.4 4 9.9A5 5 0 0 1 12 6a5 5 0 0 1 8 3.9c0 3.5-3 6.6-8 11.1z"/></svg>Москва, ул. Лесная, 7 · м. Белорусская</li>
          <li><svg viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg>Не дозвонились? Мы перезвоним сами</li>
          <li><svg viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg>Отмена и перенос — бесплатно, в любой момент</li>
        </ul>
      </div>
      <div class="form-wrap" id="mainWrap">
        <form id="mainForm" novalidate>
          <h3>Записаться на приём</h3>
          <p class="fw-sub">Заполните форму — администратор свяжется с вами и подберёт время.</p>
          <div class="f-grid">
            <div class="field"><label for="fName">Ваше имя *</label><input id="fName" name="name" type="text" autocomplete="name" placeholder="Анна"><span class="f-err">Укажите имя (от 2 букв)</span></div>
            <div class="field"><label for="fPhone">Телефон *</label><input id="fPhone" name="phone" type="tel" autocomplete="tel" inputmode="tel" placeholder="+7 (___) ___-__-__" class="js-phone"><span class="f-err">Введите номер полностью</span></div>
            <div class="field"><label for="fService">Направление</label>
              <select id="fService" name="service">
                <option value="">Подберите мне врача</option>
                <option>Терапия</option><option>Кардиология</option><option>Неврология</option><option>Эндокринология</option><option>ЛОР</option><option>Педиатрия</option><option>УЗИ и функциональная диагностика</option><option>Анализы</option><option>Процедурный кабинет</option><option>Вызов врача на дом</option><option>Онлайн-консультация</option><option>Другое</option>
              </select>
            </div>
            <div class="field"><label for="fDate">Желаемая дата</label><input id="fDate" name="date" type="date"><span class="f-err">Дата не может быть в прошлом</span></div>
            <div class="field full"><label for="fComment">Комментарий</label><textarea id="fComment" name="comment" placeholder="Например: болит голова уже неделю, нужен невролог…"></textarea></div>
            <label class="consent" id="fConsentWrap"><input type="checkbox" id="fConsent"><span>Соглашаюсь на обработку персональных данных и принимаю условия политики конфиденциальности *</span></label>
            <div class="field full"><button type="submit" class="btn btn-primary btn-block">Отправить заявку
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div>
          </div>
        </form>
        <div class="form-success" aria-live="polite">
          <svg class="fs-check" viewBox="0 0 84 84"><circle cx="42" cy="42" r="39"/><path d="M26 43l11 11 21-24"/></svg>
          <h3 style="font-family:var(--display);font-weight:400;font-size:1.5rem">Заявка отправлена!</h3>
          <p style="color:var(--ink-soft);font-size:.92rem;max-width:34ch">Администратор перезвонит в течение 15 минут в часы работы клиники.</p>
          <span class="fs-code" id="mainCode"></span>
          <button class="btn btn-ghost btn-sm" type="button" data-reset-form>Отправить ещё одну заявку</button>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ======= КОНТАКТЫ ======= -->
<section class="section" id="contacts">
  <div class="container">
    <div class="sec-head">
      <div>
        <p class="label" data-reveal>09 · Контакты</p>
        <h2 class="h2" data-reveal data-delay="80" style="margin-top:1rem">Мы в самом центре, но тихо</h2>
      </div>
    </div>
    <div class="contacts-grid">
      <div class="c-cards">
        <div class="c-card" data-reveal><span class="c-ico"><svg viewBox="0 0 24 24"><path d="M12 21C7 16.5 4 13.4 4 9.9A5 5 0 0 1 12 6a5 5 0 0 1 8 3.9c0 3.5-3 6.6-8 11.1z"/><circle cx="12" cy="10" r="2"/></svg></span><span><small>Адрес</small><b>Москва, ул. Лесная, 7, стр. 2<br>м. Белорусская — 4 минуты пешком</b></span></div>
        <div class="c-card" data-reveal data-delay="70"><span class="c-ico"><svg viewBox="0 0 24 24"><path d="M5 4h4l2 5-2.5 1.5a12 12 0 0 0 5 5L15 13l5 2v4a2 2 0 0 1-2.2 2A17 17 0 0 1 3 6.2 2 2 0 0 1 5 4z"/></svg></span><span><small>Телефон и почта</small><b><a href="tel:+74951234567">+7 (495) 123-45-67</a><br><a href="mailto:info@puls-clinic.ru" style="font-weight:500;font-size:.9rem">info@puls-clinic.ru</a></b></span></div>
        <div class="c-card" data-reveal data-delay="140"><span class="c-ico"><svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3.5 2.5"/></svg></span><span><small>Часы работы</small><b>Пн–Пт: 8:00–21:00<br>Сб–Вс: 9:00–20:00 · Лаборатория без записи до 12:00</b></span></div>
        <div class="c-card" data-reveal data-delay="210"><span class="c-ico"><svg viewBox="0 0 24 24"><rect x="3" y="5" width="18" height="14" rx="2"/><path d="M3 9h18M8 3v4M16 3v4"/></svg></span><span><small>Запись</small><b>Онлайн, по телефону и в Telegram<br><a href="https://t.me/" target="_blank" rel="noopener" style="font-weight:500;font-size:.9rem">@puls_clinic</a></b></span></div>
      </div>
      <div class="map-box" data-reveal data-delay="120">
        <svg viewBox="0 0 640 460" preserveAspectRatio="xMidYMid slice" aria-hidden="true">
          <rect width="640" height="460" fill="#EDE8DA"/>
          <path d="M-20 380 C140 330 200 420 360 380 S600 300 700 340" stroke="#BFD9CE" stroke-width="46" fill="none"/>
          <rect x="60" y="60" width="150" height="120" rx="14" fill="#E2DCC9"/>
          <rect x="250" y="40" width="120" height="90" rx="14" fill="#E2DCC9"/>
          <rect x="430" y="70" width="150" height="140" rx="14" fill="#D9E6DC"/>
          <rect x="70" y="230" width="130" height="100" rx="14" fill="#E2DCC9"/>
          <rect x="420" y="250" width="160" height="110" rx="14" fill="#E2DCC9"/>
          <path d="M0 205 H640" stroke="#FBF8F0" stroke-width="20"/>
          <path d="M310 0 V460" stroke="#FBF8F0" stroke-width="20"/>
          <path d="M0 205 H640" stroke="#D8D2C0" stroke-width="1.5" stroke-dasharray="8 10"/>
          <path d="M310 0 V460" stroke="#D8D2C0" stroke-width="1.5" stroke-dasharray="8 10"/>
          <text x="330" y="196" font-family="monospace" font-size="12" fill="#8d8574">ул. Лесная</text>
          <text x="288" y="440" font-family="monospace" font-size="12" fill="#8d8574" transform="rotate(-90 288 440)">2-й Лесной пер.</text>
          <circle cx="310" cy="205" r="26" fill="rgba(228,87,61,.28)" class="map-pin-ring"/>
          <circle cx="310" cy="205" r="13" fill="#E4573D" stroke="#fff" stroke-width="4"/>
          <circle cx="112" cy="205" r="12" fill="#0E5A4A"/><text x="112" y="210" text-anchor="middle" font-size="12" font-weight="bold" fill="#F3EFE2" font-family="sans-serif">М</text>
          <text x="112" y="238" text-anchor="middle" font-size="11" fill="#5d6f67" font-family="sans-serif">Белорусская</text>
        </svg>
        <span class="map-tag">📍 ул. Лесная, 7, стр. 2</span>
        <div class="map-cta">
          <a class="btn btn-primary btn-sm" href="https://yandex.ru/maps/?text=%D0%9C%D0%BE%D1%81%D0%BA%D0%B2%D0%B0%2C%20%D1%83%D0%BB.%20%D0%9B%D0%B5%D1%81%D0%BD%D0%B0%D1%8F%207" target="_blank" rel="noopener">Открыть в Яндекс Картах</a>
          <a class="btn btn-ghost btn-sm" href="https://maps.google.com/?q=Moscow,+Lesnaya+street+7" target="_blank" rel="noopener">Google Maps</a>
        </div>
      </div>
    </div>
  </div>
</section>
</main>

<!-- ======= ФУТЕР ======= -->
<footer>
  <div class="disclaimer">Имеются противопоказания. Необходима консультация специалиста</div>
  <div class="container foot-top">
    <div>
      <a href="#home" class="logo"><span class="lg-mark"><svg viewBox="0 0 24 24"><path d="M3 12h4l2-5 3 10 2-5h7"/></svg></span><span>Пульс<small style="color:#7fa79a">клиника общей практики</small></span></a>
      <p class="foot-desc">Частная клиника общей практики для всей семьи. Работаем с 2008 года: терапия, узкие специалисты, УЗИ и собственная лаборатория.</p>
      <div class="socials">
        <a href="https://t.me/" target="_blank" rel="noopener" aria-label="Telegram"><svg viewBox="0 0 24 24"><path d="M21.9 4.3L2.9 11.6c-.9.4-.9 1.5.1 1.8l4.7 1.5 1.8 5.6c.3.9 1.3 1 1.9.3l2.6-2.6 4.9 3.6c.8.6 1.9.1 2.1-.9l2.7-15c.2-1-.8-1.9-1.8-1.6zM8.5 14.4l9.3-6.9-7.4 7.7-.3 3-1.6-3.8z"/></svg></a>
        <a href="https://wa.me/74951234567" target="_blank" rel="noopener" aria-label="WhatsApp"><svg viewBox="0 0 24 24"><path d="M12 2a10 10 0 0 0-8.6 15L2 22l5.2-1.4A10 10 0 1 0 12 2zm0 18.2a8.2 8.2 0 0 1-4.2-1.1l-.3-.2-3.1.8.8-3-.2-.3A8.2 8.2 0 1 1 12 20.2zm4.6-6.1c-.3-.1-1.5-.7-1.7-.8-.2-.1-.4-.1-.6.1-.2.3-.7.8-.8 1-.1.2-.3.2-.6.1a6.7 6.7 0 0 1-3.3-2.9c-.2-.4.2-.4.7-1.3.1-.2 0-.4 0-.5l-.8-1.9c-.2-.5-.4-.4-.6-.4h-.5c-.2 0-.5.1-.8.4-.3.3-1 1-1 2.5s1.1 2.9 1.2 3.1c.1.2 2.1 3.2 5.1 4.5.7.3 1.3.5 1.7.6.7.2 1.4.2 1.9.1.6-.1 1.5-.6 1.7-1.2.2-.6.2-1.1.2-1.2-.1-.1-.3-.2-.6-.3z"/></svg></a>
        <a href="https://vk.com/" target="_blank" rel="noopener" aria-label="ВКонтакте"><svg viewBox="0 0 24 24"><path d="M13.2 18.5c-6 0-9.9-4.2-10-11.2h3.1c.1 5.1 2.5 7.3 4.3 7.8V7.3h3v4.5c1.8-.2 3.6-2.3 4.2-4.5h3c-.5 2.7-2.4 4.8-3.8 5.7 1.7.7 4 2.5 4.9 5.5h-3.3c-.7-2.2-2.4-3.9-4.9-4.2v4.2h-.5z"/></svg></a>
      </div>
    </div>
    <div>
      <h4>Клиника</h4>
      <ul class="foot-links">
        <li><a href="#about">О клинике</a></li>
        <li><a href="#doctors">Наши врачи</a></li>
        <li><a href="#reviews">Отзывы пациентов</a></li>
        <li><a href="#faq">Вопросы и ответы</a></li>
        <li><a href="#contacts">Контакты</a></li>
      </ul>
    </div>
    <div>
      <h4>Пациентам</h4>
      <ul class="foot-links">
        <li><a href="#prices">Прайс-лист</a></li>
        <li><a href="#services">Отделения</a></li>
        <li><button class="js-goto-price" data-tab="Анализы" style="padding:0;font:inherit">Подготовка к анализам</button></li>
        <li><button data-modal-open="#appointmentModal" data-service="Вызов врача на дом" style="padding:0;font:inherit">Вызов врача на дом</button></li>
        <li><button data-info="privacy" style="padding:0;font:inherit">Политика конфиденциальности</button></li>
      </ul>
    </div>
    <div>
      <h4>Контакты</h4>
      <ul class="foot-links foot-contact">
        <li><b>+7 (495) 123-45-67</b></li>
        <li>Москва, ул. Лесная, 7, стр. 2<br>м. Белорусская</li>
        <li>Пн–Пт 8:00–21:00 · Сб–Вс 9:00–20:00</li>
        <li><a href="mailto:info@puls-clinic.ru">info@puls-clinic.ru</a></li>
      </ul>
    </div>
  </div>
  <div class="container foot-bottom">
    <span>© <span id="yearNow">2026</span> ООО «Пульс Медикал». Лицензия № ЛО-77-01-021253</span>
    <span>Сайт носит информационный характер и не является публичной офертой</span>
  </div>
</footer>

<!-- мобильная панель -->
<div id="mobileBar">
  <a class="btn btn-ghost" style="border-color:rgba(243,239,226,.35);color:var(--cream)" href="tel:+74951234567">📞 Позвонить</a>
  <button class="btn btn-coral" data-modal-open="#appointmentModal">Записаться</button>
</div>

<!-- модалка записи -->
<div class="modal-backdrop" id="appointmentModal" role="dialog" aria-modal="true" aria-labelledby="apTitle" data-modal>
  <div class="modal">
    <button class="modal-close" data-modal-close aria-label="Закрыть окно"><svg viewBox="0 0 24 24"><path d="M6 6l12 12M18 6L6 18"/></svg></button>
    <p class="label">Запись в клинику</p>
    <h3 id="apTitle">Оставьте контакты</h3>
    <p class="m-sub" id="apSubtitle">Администратор перезвонит в течение 15 минут и подберёт время.</p>
    <div class="form-wrap" id="modalWrap" style="padding:0">
      <form id="modalForm" novalidate>
        <div class="f-grid">
          <div class="field"><label for="aName">Ваше имя *</label><input id="aName" type="text" autocomplete="name" placeholder="Анна"><span class="f-err">Укажите имя (от 2 букв)</span></div>
          <div class="field"><label for="aPhone">Телефон *</label><input id="aPhone" type="tel" inputmode="tel" autocomplete="tel" placeholder="+7 (___) ___-__-__" class="js-phone"><span class="f-err">Введите номер полностью</span></div>
          <div class="field"><label for="apService">Направление</label><select id="apService"><option value="">Подберите мне врача</option><option>Терапия</option><option>Кардиология</option><option>Неврология</option><option>Эндокринология</option><option>ЛОР</option><option>Педиатрия</option><option>УЗИ и функциональная диагностика</option><option>Анализы</option><option>Процедурный кабинет</option><option>Вызов врача на дом</option><option>Онлайн-консультация</option><option>Другое</option></select></div>
          <div class="field"><label for="aDate">Желаемая дата</label><input id="aDate" type="date"><span class="f-err">Дата не может быть в прошлом</span></div>
          <label class="consent" id="aConsentWrap"><input type="checkbox" id="aConsent"><span>Соглашаюсь на обработку персональных данных *</span></label>
          <div class="field"><button type="submit" class="btn btn-primary btn-block">Жду звонка</button></div>
        </div>
      </form>
      <div class="form-success" aria-live="polite">
        <svg class="fs-check" viewBox="0 0 84 84"><circle cx="42" cy="42" r="39"/><path d="M26 43l11 11 21-24"/></svg>
        <h3 style="font-family:var(--display);font-weight:400;font-size:1.4rem">Принято!</h3>
        <p style="color:var(--ink-soft);font-size:.9rem">Перезвоним в течение 15 минут в часы работы клиники.</p>
        <span class="fs-code" id="modalCode"></span>
        <button class="btn btn-ghost btn-sm" type="button" data-reset-form>Новая заявка</button>
      </div>
    </div>
  </div>
</div>

<!-- модалка инфо -->
<div class="modal-backdrop" id="infoModal" role="dialog" aria-modal="true" aria-labelledby="infoTitle" data-modal>
  <div class="modal">
    <button class="modal-close" data-modal-close aria-label="Закрыть окно"><svg viewBox="0 0 24 24"><path d="M6 6l12 12M18 6L6 18"/></svg></button>
    <h3 id="infoTitle" style="margin-bottom:1rem"></h3>
    <div id="infoBody" style="color:var(--ink-soft);font-size:.92rem;line-height:1.7"></div>
  </div>
</div>

<button id="backTop" aria-label="Наверх"><svg viewBox="0 0 24 24"><path d="M12 19V5M6 11l6-6 6 6"/></svg></button>
<div id="toastBox" aria-live="polite"></div>

<script>
(function(){
"use strict";
const $=(s,c=document)=>c.querySelector(s), $$=(s,c=document)=>[...c.querySelectorAll(s)];
const RM=window.matchMedia('(prefers-reduced-motion: reduce)').matches;

/* ---------- прелоадер и старт ---------- */
const pre=$('#preloader');
function boot(){
  document.body.classList.add('is-loaded');
  if(pre){pre.classList.add('hide');setTimeout(()=>pre.remove(),700);}
  runScramble();
}
if(RM){document.addEventListener('DOMContentLoaded',boot);}
else{setTimeout(boot,950);}
$('#yearNow').textContent=new Date().getFullYear();

/* ---------- прогресс, шапка, наверх ---------- */
const bar=$('#progressBar'),header=$('#siteHeader'),backTop=$('#backTop');
let ticking=false;
function onScroll(){
  const st=window.scrollY,h=document.documentElement.scrollHeight-innerHeight;
  bar.style.width=(h>0?st/h*100:0)+'%';
  header.classList.toggle('scrolled',st>10);
  backTop.classList.toggle('show',st>600);
  ticking=false;
}
addEventListener('scroll',()=>{if(!ticking){requestAnimationFrame(onScroll);ticking=true;}},{passive:true});
onScroll();
backTop.addEventListener('click',()=>window.scrollTo({top:0,behavior:RM?'auto':'smooth'}));

/* ---------- «открыто сейчас» ---------- */
(function(){
  const el=$('#openStatus');if(!el)return;
  const d=new Date(),day=d.getDay(),h=d.getHours()+d.getMinutes()/60;
  const wk=(day===0||day===6)?{o:9,c:20}:{o:8,c:21};
  if(h>=wk.o&&h<wk.c){el.innerHTML='<i></i>Открыто сейчас · до '+wk.c+':00';}
  else{el.classList.add('closed');el.innerHTML='<i></i>Закрыто · откроемся в '+wk.o+':00';}
})();

/* ---------- бургер-меню ---------- */
const burger=$('#burgerBtn');
function setMenu(open){
  document.body.classList.toggle('menu-open',open);
  document.body.classList.toggle('lock',open);
  burger.setAttribute('aria-expanded',open);
}
burger.addEventListener('click',()=>setMenu(!document.body.classList.contains('menu-open')));
$$('.js-menu-link').forEach(a=>a.addEventListener('click',()=>setMenu(false)));
addEventListener('keydown',e=>{if(e.key==='Escape'){setMenu(false);closeAllModals();}});

/* ---------- scrollspy ---------- */
const spyLinks=$$('[data-spy]');
const spyIO=new IntersectionObserver(es=>{
  es.forEach(e=>{if(e.isIntersecting){
    spyLinks.forEach(l=>l.classList.toggle('active',l.dataset.spy===e.target.id));
  }});
},{rootMargin:'-35% 0px -55% 0px'});
spyLinks.forEach(l=>{const sec=document.getElementById(l.dataset.spy);if(sec)spyIO.observe(sec);});

/* ---------- reveal ---------- */
const revIO=new IntersectionObserver(es=>{
  es.forEach(e=>{if(e.isIntersecting){
    const el=e.target;
    el.style.transitionDelay=(el.dataset.delay||0)+'ms';
    el.classList.add('revealed');
    revIO.unobserve(el);
  }});
},{threshold:.12});
$$('[data-reveal]').forEach(el=>revIO.observe(el));

/* ---------- scramble ---------- */
function runScramble(){
  const el=$('#scrambleLine');if(!el)return;
  const text=el.dataset.text||el.textContent;
  if(RM){el.textContent=text;return;}
  const chars='АБВГДЕЖЗИКЛМНОПРСТУФХЦЧШЩЭЮЯ+·0123456789';
  let frame=0;const total=Math.max(28,text.length+10);
  const iv=setInterval(()=>{
    frame++;
    const done=Math.floor((frame/total)*text.length);
    let out='';
    for(let i=0;i<text.length;i++){
      out+= i<done?text[i] : (text[i]===' '?' ':chars[Math.random()*chars.length|0]);
    }
    el.textContent=out;
    if(done>=text.length){clearInterval(iv);el.textContent=text;}
  },34);
}

/* ---------- счётчики ---------- */
const cntIO=new IntersectionObserver(es=>{
  es.forEach(e=>{if(!e.isIntersecting)return;
    const el=e.target,target=parseFloat(el.dataset.count),dec=parseInt(el.dataset.dec||0);
    cntIO.unobserve(el);
    if(RM){el.textContent=dec?target.toFixed(dec).replace('.',','):target.toLocaleString('ru-RU');return;}
    const t0=performance.now(),dur=1600;
    (function tick(t){
      const p=Math.min(1,(t-t0)/dur),v=target*(1-Math.pow(1-p,3));
      el.textContent=dec?v.toFixed(dec).replace('.',','):Math.round(v).toLocaleString('ru-RU');
      if(p<1)requestAnimationFrame(tick);
    })(t0);
  });
},{threshold:.5});
$$('[data-count]').forEach(el=>cntIO.observe(el));

/* ---------- бегущая строка: дублируем контент ---------- */
const mt=$('#marqueeTrack');
if(mt)mt.innerHTML+=mt.innerHTML;

/* ---------- прайс-лист ---------- */
const PRICES={
 'Приём специалистов':[
  {n:'Первичный приём терапевта',note:'60 минут',p:2400,hot:1},
  {n:'Повторный приём терапевта',note:'30 минут',p:1900},
  {n:'Приём кардиолога',note:'60 минут, ведёт к.м.н.',p:2900},
  {n:'Приём невролога',note:'45 минут',p:2700},
  {n:'Приём эндокринолога',note:'45 минут',p:2700},
  {n:'Приём оториноларинголога',note:'45 минут',p:2800},
  {n:'Приём педиатра',note:'дети с 0 лет',p:2400},
  {n:'Онлайн-консультация врача',note:'видеосвязь, 30 минут',p:1900},
  {n:'Вызов терапевта на дом',note:'в пределах МКАД',p:4500},
  {n:'Санаторно-курортная карта',note:'оформление за 1 день',p:2200}
 ],
 'Диагностика':[
  {n:'УЗИ брюшной полости',note:'комплексное исследование',p:2600},
  {n:'УЗИ щитовидной железы',note:'с допплером',p:1800,hot:1},
  {n:'ЭхоКГ (УЗИ сердца)',note:'с допплерографией',p:3400},
  {n:'ЭКГ с расшифровкой',note:'15 минут',p:1600,hot:1},
  {n:'Холтеровское мониторирование',note:'24 часа, аппарат выдаём',p:4200},
  {n:'Дуплекс сосудов шеи и головы',note:'заключение сразу',p:2900},
  {n:'Спирометрия',note:'оценка функции дыхания',p:1900},
  {n:'УЗИ почек и мочевого пузыря',p:2200}
 ],
 'Анализы':[
  {n:'Общий анализ крови с лейкоформулой',p:650,hot:1},
  {n:'Общий анализ мочи',p:450},
  {n:'Биохимия крови, базовый профиль',note:'12 показателей',p:2100},
  {n:'Липидный профиль',note:'5 показателей',p:1450},
  {n:'Гликированный гемоглобин HbA1c',p:780},
  {n:'Тиреотропный гормон (ТТГ)',p:590},
  {n:'Ферритин',p:820},
  {n:'Витамин D (25-OH)',p:1950},
  {n:'Коагулограмма',note:'4 показателя',p:1350}
 ],
 'Процедуры':[
  {n:'Внутримышечная инъекция',note:'без стоимости препарата',p:350},
  {n:'Внутривенная инъекция',p:450},
  {n:'Внутривенное капельное введение',note:'без стоимости препарата',p:900},
  {n:'Вакцинация от гриппа',note:'с препаратом',p:1800,hot:1},
  {n:'Вакцинация от клещевого энцефалита',note:'с препаратом',p:2400},
  {n:'Перевязка, обработка раны',p:800},
  {n:'Удаление клеща с исследованием',p:1200}
 ]
};
const listEl=$('#priceList'),countEl=$('#priceCount'),searchEl=$('#priceSearch');
let curTab='Приём специалистов';
function serviceFromName(n){
  if(/терапевт/i.test(n))return 'Терапия';
  if(/кардиолог/i.test(n))return 'Кардиология';
  if(/невролог/i.test(n))return 'Неврология';
  if(/эндокринолог/i.test(n))return 'Эндокринология';
  if(/оториноларинголог/i.test(n))return 'ЛОР';
  if(/педиатр/i.test(n))return 'Педиатрия';
  if(/онлайн/i.test(n))return 'Онлайн-консультация';
  if(/дом/i.test(n))return 'Вызов врача на дом';
  if(/УЗИ|ЭКГ|ЭхоКГ|Холтер|Дуплекс|Спирометрия/i.test(n))return 'УЗИ и функциональная диагностика';
  if(/анализ|гемоглобин|ТТГ|ферритин|витамин|коагулограмма|липидный/i.test(n))return 'Анализы';
  if(curTab==='Процедуры')return 'Процедурный кабинет';
  return 'Другое';
}
function renderPrices(){
  const q=(searchEl.value||'').trim().toLowerCase();
  const items=PRICES[curTab].filter(it=>!q||it.n.toLowerCase().includes(q));
  if(!items.length){
    listEl.innerHTML='<div class="pl-empty">По запросу «'+(searchEl.value||'')+'» ничего не нашлось.<br>Позвоните — подскажем: <b><a href="tel:+74951234567">+7 (495) 123-45-67</a></b></div>';
  }else{
    listEl.innerHTML=items.map((it,i)=>{
      const svc=serviceFromName(it.n);
      return '<div class="pl-row" style="animation-delay:'+Math.min(i*45,400)+'ms">'+
        '<div class="pl-name">'+it.n+(it.hot?'<span class="pl-hot">популярно</span>':'')+(it.note?'<small>'+it.note+'</small>':'')+'</div>'+
        '<span class="pl-note-cell"></span>'+
        '<span class="pl-price">'+it.p.toLocaleString('ru-RU')+' ₽</span>'+
        '<button class="btn btn-ghost btn-sm" data-modal-open="#appointmentModal" data-service="'+svc+'" data-label="'+it.n+'">Записаться</button></div>';
    }).join('');
  }
  countEl.textContent='Раздел «'+curTab+'» · показано позиций: '+items.length+' из '+PRICES[curTab].length+(curTab==='Анализы'?' · взятие крови +250 ₽':'');
  bindModalOpeners(listEl);
}
$$('#priceTabs .price-tab').forEach(b=>{
  b.addEventListener('click',()=>{
    $$('#priceTabs .price-tab').forEach(x=>x.setAttribute('aria-selected',x===b));
    curTab=b.dataset.tab;renderPrices();
  });
});
searchEl.addEventListener('input',renderPrices);
renderPrices();

/* скачивание прайса */
$('#priceDownload').addEventListener('click',()=>{
  const d=new Date();
  let txt='МЦ «Пульс» — прайс-лист от '+d.toLocaleDateString('ru-RU')+'\nМосква, ул. Лесная, 7 · +7 (495) 123-45-67\n\n';
  for(const cat in PRICES){
    txt+='=== '+cat.toUpperCase()+' ===\n';
    PRICES[cat].forEach(it=>{txt+='• '+it.n+(it.note?' ('+it.note+')':'')+' — '+it.p.toLocaleString('ru-RU')+' ₽\n';});
    txt+='\n';
  }
  txt+='Цены не являются публичной офертой. Уточняйте по телефону.';
  const a=document.createElement('a');
  a.href=URL.createObjectURL(new Blob([txt],{type:'text/plain;charset=utf-8'}));
  a.download='price-puls.txt';a.click();
  setTimeout(()=>URL.revokeObjectURL(a.href),2000);
  toast('Прайс-лист скачивается 📄');
});

/* быстрый переход к разделу прайса */
$$('.js-goto-price').forEach(b=>b.addEventListener('click',()=>{
  const tab=b.dataset.tab;
  if(tab){const btn=$('#priceTabs .price-tab[data-tab="'+tab+'"]');if(btn)btn.click();}
  document.getElementById('prices').scrollIntoView({behavior:RM?'auto':'smooth'});
}));

/* ---------- тосты ---------- */
function toast(msg){
  const box=$('#toastBox'),t=document.createElement('div');
  t.className='toast';t.innerHTML='<span class="t-dot"></span><span>'+msg+'</span>';
  box.appendChild(t);
  requestAnimationFrame(()=>t.classList.add('show'));
  setTimeout(()=>{t.classList.remove('show');setTimeout(()=>t.remove(),500);},3800);
}

/* ---------- модалки ---------- */
let lastFocus=null;
function openModal(sel,preset){
  const m=$(sel);if(!m)return;
  lastFocus=document.activeElement;
  if(sel==='#appointmentModal')applyPreset(preset||{});
  m.classList.add('show');document.body.classList.add('lock');
  const first=m.querySelector('input,select,textarea,button.modal-close');
  setTimeout(()=>{const f=m.querySelector('input:not([type=checkbox]),select');(f||first).focus();},150);
}
function closeAllModals(){
  $$('[data-modal].show').forEach(m=>m.classList.remove('show'));
  document.body.classList.remove('lock');
  if(lastFocus)lastFocus.focus();
}
$$('[data-modal]').forEach(m=>{
  m.addEventListener('click',e=>{if(e.target===m)closeAllModals();});
});
$$('[data-modal-close]').forEach(b=>b.addEventListener('click',closeAllModals));

function applyPreset({service,doctor,label}){
  const sub=$('#apSubtitle'),sel=$('#apService');
  if(doctor){sub.textContent='Запись к врачу: '+doctor+(service?' · '+service.toLowerCase():'');}
  else if(label){sub.textContent='Заявка: '+label+'. Администратор перезвонит в течение 15 минут.';}
  else{sub.textContent='Администратор перезвонит в течение 15 минут и подберёт время.';}
  if(service&&sel){
    const opt=[...sel.options].find(o=>o.value===service||o.text===service);
    sel.value=opt?opt.value:(service==='Другое'?'Другое':'');
  }
}
function bindModalOpeners(scope){
  $$('[data-modal-open]',scope||document).forEach(b=>{
    if(b.dataset.bound)return;b.dataset.bound='1';
    b.addEventListener('click',e=>{
      e.preventDefault();
      if(b.dataset.info){openInfo(b.dataset.info);return;}
      openModal(b.dataset.modalOpen,{service:b.dataset.service,doctor:b.dataset.doctor,label:b.dataset.label});
    });
  });
}
bindModalOpeners(document);
$$('.js-book-doc').forEach(b=>b.addEventListener('click',()=>openModal('#appointmentModal',{doctor:b.dataset.doctor,service:b.dataset.service})));

/* инфо-модалка (политика конфиденциальности) */
const INFO={privacy:{t:'Политика конфиденциальности',b:'ООО «Пульс Медикал» обрабатывает персональные данные (имя, телефон) исключительно для связи с вами по вопросам записи и оказания медицинских услуг в соответствии с 152-ФЗ. Данные не передаются третьим лицам и хранятся не дольше необходимого. Вы можете отозвать согласие, написав на info@puls-clinic.ru.'}};
function openInfo(key){
  const d=INFO[key];if(!d)return;
  $('#infoTitle').textContent=d.t;$('#infoBody').textContent=d.b;
  openModal('#infoModal');
}
$$('[data-info]').forEach(b=>b.addEventListener('click',()=>openInfo(b.dataset.info)));

/* ---------- формы ---------- */
function maskPhone(input){
  input.addEventListener('input',()=>{
    let d=input.value.replace(/\D/g,'');
    if(d.startsWith('8'))d='7'+d.slice(1);
    if(d.startsWith('9'))d='7'+d;
    d=d.slice(0,11);
    let r='+7';
    if(d.length>1)r+=' ('+d.slice(1,4);
    if(d.length>=5)r+=') '+d.slice(4,7);
    if(d.length>=8)r+='-'+d.slice(7,9);
    if(d.length>=10)r+='-'+d.slice(9,11);
    input.value=d?r:'';
  });
}
$$('.js-phone').forEach(maskPhone);

/* минимальная дата — сегодня */
const today=new Date().toISOString().slice(0,10);
$$('input[type="date"]').forEach(i=>i.min=today);

function setupForm(formId,wrapId,codeId,consentId,consentWrapId){
  const form=$(formId);if(!form)return;
  form.addEventListener('submit',e=>{
    e.preventDefault();
    let ok=true;
    const name=form.querySelector('input[type="text"]'),
          phone=form.querySelector('.js-phone'),
          date=form.querySelector('input[type="date"]'),
          consent=$(consentId);
    const setErr=(el,bad)=>{const f=el.closest('.field');if(f)f.classList.toggle('invalid',bad);if(bad)ok=false;};
    setErr(name,(name.value.trim().length<2));
    setErr(phone,(phone.value.replace(/\D/g,'').length!==11));
    if(date)setErr(date,!!date.value&&date.value<today);
    $(consentWrapId).classList.toggle('invalid',!consent.checked);
    if(!consent.checked)ok=false;
    if(!ok){toast('Проверьте выделенные поля формы');return;}
    const code='П-'+today.slice(2).replace(/-/g,'')+'-'+String(Math.floor(Math.random()*900)+100);
    $('#'+codeId).textContent='Заявка '+code;
    $('#'+wrapId).classList.add('sent');
    toast('Заявка отправлена! Перезвоним в течение 15 минут 💚');
  });
  form.addEventListener('input',e=>{
    const f=e.target.closest('.field');if(f)f.classList.remove('invalid');
    if(e.target.type==='checkbox')$(consentWrapId).classList.remove('invalid');
  });
}
$$('[data-reset-form]').forEach(b=>b.addEventListener('click',()=>{
  const wrap=b.closest('.form-wrap');
  wrap.classList.remove('sent');
  const form=wrap.querySelector('form');
  form.reset();
  setTimeout(()=>form.querySelector('input').focus(),300);
}));
setupForm('#mainForm','mainWrap','mainCode','#fConsent','#fConsentWrap');
setupForm('#modalForm','modalWrap','modalCode','#aConsent','#aConsentWrap');

/* ---------- аккордеон ---------- */
const accItems=$$('.acc-item');
function accSet(item,open){
  const btn=item.querySelector('.acc-btn'),panel=item.querySelector('.acc-panel');
  item.classList.toggle('open',open);
  btn.setAttribute('aria-expanded',open);
  panel.style.maxHeight=open?panel.scrollHeight+'px':'0px';
}
accItems.forEach(item=>{
  item.querySelector('.acc-btn').addEventListener('click',()=>{
    const willOpen=!item.classList.contains('open');
    accItems.forEach(i=>accSet(i,false));
    if(willOpen)accSet(item,true);
  });
});
accSet(accItems[0],true);
addEventListener('resize',()=>{const o=$('.acc-item.open .acc-panel');if(o)o.style.maxHeight=o.scrollHeight+'px';});

/* ---------- слайдер отзывов ---------- */
const sliderEl=$('#reviewsSlider'),track=$('#revTrack'),items=$$('li',track),
      prevBtn=$('#revPrev'),nextBtn=$('#revNext'),dotsBox=$('#revDots');
let idx=0,pv=1,maxIdx=0,autoTimer=null;
function sliderMetrics(){
  const w=sliderEl.getBoundingClientRect().width;
  pv=w>=1000?3:w>=620?2:1;
  maxIdx=Math.max(0,items.length-pv);
  idx=Math.min(idx,maxIdx);
  items.forEach(li=>li.style.flex='0 0 '+(100/pv)+'%');
  dotsBox.innerHTML='';
  for(let i=0;i<=maxIdx;i++){
    const d=document.createElement('button');
    d.className='sl-dot'+(i===idx?' active':'');
    d.setAttribute('aria-label','Слайд '+(i+1));
    d.addEventListener('click',()=>{idx=i;sliderUpdate();restartAuto();});
    dotsBox.appendChild(d);
  }
  sliderUpdate();
}
function sliderUpdate(){
  track.style.transform='translateX('+(-idx*(100/pv))+'%)';
  $$('.sl-dot',dotsBox).forEach((d,i)=>d.classList.toggle('active',i===idx));
}
function slideNext(){idx=idx>=maxIdx?0:idx+1;sliderUpdate();}
function slidePrev(){idx=idx<=0?maxIdx:idx-1;sliderUpdate();}
prevBtn.addEventListener('click',()=>{slidePrev();restartAuto();});
nextBtn.addEventListener('click',()=>{slideNext();restartAuto();});
sliderEl.addEventListener('keydown',e=>{
  if(e.key==='ArrowRight'){slideNext();restartAuto();}
  if(e.key==='ArrowLeft'){slidePrev();restartAuto();}
});
/* свайп */
let sx=null;
const vp=$('.slider-viewport',sliderEl);
vp.addEventListener('pointerdown',e=>{sx=e.clientX;vp.setPointerCapture(e.pointerId);});
vp.addEventListener('pointerup',e=>{
  if(sx===null)return;
  const dx=e.clientX-sx;sx=null;
  if(Math.abs(dx)>45){dx<0?slideNext():slidePrev();restartAuto();}
});
function restartAuto(){
  if(autoTimer)clearInterval(autoTimer);
  if(!RM)autoTimer=setInterval(slideNext,5600);
}
['mouseenter','focusin','touchstart'].forEach(ev=>sliderEl.addEventListener(ev,()=>autoTimer&&clearInterval(autoTimer),{passive:true}));
['mouseleave','focusout'].forEach(ev=>sliderEl.addEventListener(ev,restartAuto));
let rT;addEventListener('resize',()=>{clearTimeout(rT);rT=setTimeout(sliderMetrics,150);});
sliderMetrics();restartAuto();

})();
</script>
</body>
</html>