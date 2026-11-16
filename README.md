<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
  <meta name="theme-color" content="#101421">
  <meta name="description" content="A personal letter for Liora Angelin, written with sincerity and care.">
  <title>A Letter For Liora ♡</title>
  <style>
    :root {
      color-scheme: dark;
      --night: #101421;
      --rose: #df9bad;
      --rose-light: #f2c7d1;
      --gold: #d8bd8c;
      --paper: #f4e9e4;
      --muted: #c2b8bd;
      --line: rgba(230,198,189,.2);
      --serif: Georgia, 'Times New Roman', serif;
      --sans: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
      --safe-top: env(safe-area-inset-top, 0px);
      --safe-bottom: env(safe-area-inset-bottom, 0px);
    }
    * { box-sizing: border-box; }
    html, body { width: 100%; height: 100%; margin: 0; overflow: hidden; }
    body { min-width: 320px; min-height: 100%; background: var(--night); color: var(--paper); font-family: var(--sans); line-height: 1.7; -webkit-font-smoothing: antialiased; }
    button { font: inherit; }
    button:focus-visible { outline: 2px solid var(--gold); outline-offset: 4px; }
    .ambient { position: fixed; inset: 0; z-index: 0; overflow: hidden; pointer-events: none; background: radial-gradient(ellipse at 50% 0%,rgba(106,56,78,.28),transparent 49%),radial-gradient(ellipse at 95% 74%,rgba(55,58,91,.24),transparent 42%),linear-gradient(145deg,#101421,#171421 56%,#101421); }
    .ambient::after { content: ''; position: absolute; inset: 0; opacity: .17; background-image: linear-gradient(rgba(255,255,255,.018) 1px,transparent 1px),linear-gradient(90deg,rgba(255,255,255,.018) 1px,transparent 1px); background-size: 54px 54px; mask-image: linear-gradient(to bottom,black,transparent 80%); }
    .glow { position: absolute; width: 22rem; height: 22rem; border-radius: 50%; filter: blur(95px); opacity: .13; background: #ca7790; animation: drift 22s ease-in-out infinite alternate; }
    .glow.one { top: 10%; left: -12rem; }.glow.two { right: -13rem; bottom: 8%; background: #b99a67; animation-delay: -8s; }
    @keyframes drift { to { transform: translate(5rem,3rem) scale(1.08); } }
    .specks,.petals { position:absolute; inset:0; }
    .speck { position:absolute; width:2px; height:2px; border-radius:50%; background:#f5d9c9; opacity:.4; animation:twinkle 5s ease-in-out infinite alternate; }
    @keyframes twinkle { to { opacity:.1; transform:scale(.65); } }
    .petal { position:absolute; top:-10vh; color:#dc9bae; opacity:.28; animation:fall linear infinite; }
    @keyframes fall { to { transform:translate3d(28px,115vh,0) rotate(280deg); } }
    .progress-track { position:fixed; z-index:20; inset:0 0 auto; height:3px; background:rgba(255,255,255,.08); }
    .progress-bar { width:0; height:100%; background:linear-gradient(90deg,var(--rose),var(--gold)); transition:width .55s ease; box-shadow:0 0 12px rgba(223,155,173,.4); }
    .topbar { position:fixed; z-index:15; inset:3px 0 auto; height:64px; display:flex; justify-content:space-between; align-items:center; gap:14px; padding:0 max(28px,calc((100vw - 1120px)/2)); padding-top:var(--safe-top); background:rgba(16,20,33,.53); border-bottom:1px solid rgba(255,255,255,.055); backdrop-filter:blur(18px); }
    .brand { color:var(--rose-light); font:18px var(--serif); letter-spacing:.015em; }
    .top-actions { display:flex; align-items:center; gap:8px; }
    .music-controls { display:flex; align-items:center; gap:7px; }
    .icon-button,.volume-wrap { min-width:40px; min-height:40px; display:inline-flex; justify-content:center; align-items:center; gap:7px; padding:8px 11px; border:1px solid var(--line); border-radius:999px; color:var(--paper); background:rgba(255,255,255,.045); backdrop-filter:blur(12px); cursor:pointer; transition:background .2s,border-color .2s,transform .2s; }
    .icon-button:hover { background:rgba(223,155,173,.13); border-color:rgba(223,155,173,.5); transform:translateY(-1px); }
    .icon-button[aria-pressed="true"] { color:var(--rose-light); border-color:rgba(223,155,173,.45); }
    .music-word { font-size:11px; }
    .volume-wrap { min-height:38px; cursor:default; font-size:11px; color:var(--muted); }
    input[type="range"] { width:64px; accent-color:var(--rose); }
    main { position:fixed; z-index:1; inset:67px 0 78px; overflow:hidden; }
    .page { position:absolute; inset:0; display:grid; place-items:center; padding:clamp(18px,3.4vh,38px) clamp(20px,6vw,90px); opacity:0; visibility:hidden; transform:translate3d(28px,0,0) scale(.985); filter:blur(5px); transition:opacity .48s ease,transform .62s cubic-bezier(.2,.72,.2,1),filter .48s ease,visibility .48s; overflow:hidden; }
    .page.active { opacity:1; visibility:visible; transform:none; filter:blur(0); z-index:2; }
    .page.exit-left { opacity:0; transform:translate3d(-24px,0,0) scale(.985); filter:blur(4px); }
    .page-content { width:min(100%,830px); max-height:100%; overflow:auto; scrollbar-width:thin; scrollbar-color:rgba(216,189,140,.35) transparent; padding:clamp(20px,4vh,42px) clamp(18px,4vw,48px); border:1px solid rgba(216,189,140,.19); border-radius:8px; background:linear-gradient(145deg,rgba(255,255,255,.055),rgba(255,255,255,.018)); box-shadow:0 24px 80px rgba(0,0,0,.2),inset 0 1px rgba(255,255,255,.045); backdrop-filter:blur(12px); }
    .page-content::-webkit-scrollbar { width:4px; }.page-content::-webkit-scrollbar-thumb { background:rgba(216,189,140,.3); border-radius:9px; }
    .opening-page { text-align:center; }
    .opening-page .page-content { width:min(100%,720px); display:flex; flex-direction:column; align-items:center; padding:clamp(20px,3.5vh,36px) 24px; border:0; background:transparent; box-shadow:none; overflow:visible; }
    .opening-page .eyebrow,.opening-page h1,.opening-page .opening-name,.opening-page .opening-tagline,.opening-page .hint { width:100%; text-align:center; }
    .opening-page h1 { max-width:100%; }
    #typedIntro { display:flex; align-items:center; justify-content:center; min-height:3em; max-width:480px; }
    .eyebrow,.section-number { color:var(--gold); font-size:10px; letter-spacing:.25em; text-transform:uppercase; }
    h1,h2 { font-family:var(--serif); font-weight:400; line-height:1.17; }
    .opening-page h1 { margin:12px 0 6px; color:var(--rose-light); font-size:clamp(34px,6vw,62px); }
    .opening-name { margin:0; color:var(--gold); font:italic clamp(16px,2vw,21px) var(--serif); letter-spacing:.06em; }
    .opening-tagline { margin:9px auto 0; max-width:480px; color:var(--muted); font:italic clamp(14px,1.8vw,18px)/1.5 var(--serif); }
    .envelope-wrap { width:min(270px,66vw); margin:clamp(15px,3vh,28px) auto 15px; perspective:900px; }
    .envelope { position:relative; height:clamp(112px,19vh,158px); border:1px solid rgba(232,193,178,.42); border-radius:5px; background:linear-gradient(145deg,#704958,#493447 75%); box-shadow:0 22px 65px rgba(0,0,0,.34),0 0 50px rgba(213,143,164,.12); overflow:hidden; transition:transform .8s ease,opacity .7s ease; }
    .envelope::before { content:''; position:absolute; inset:0; background:linear-gradient(34deg,transparent 49.5%,rgba(241,207,192,.23) 50%,transparent 50.5%),linear-gradient(-34deg,transparent 49.5%,rgba(241,207,192,.19) 50%,transparent 50.5%); }
    .flap { position:absolute; z-index:2; top:-1px; left:0; width:100%; height:58%; transform-origin:top; background:#815466; clip-path:polygon(0 0,100% 0,50% 100%); transition:transform .85s ease; }
    .seal { position:absolute; z-index:3; left:50%; top:51%; transform:translate(-50%,-50%); display:grid; place-items:center; width:39px; height:39px; border-radius:50%; color:#f6d9c8; background:#b27583; box-shadow:0 3px 16px #392533; font-size:19px; transition:opacity .3s; }
    .envelope.open { transform:translateY(15px) scale(.9); opacity:0; }.envelope.open .flap { transform:rotateX(180deg); }.envelope.open .seal { opacity:0; }
    .open-button,.nav-button,.read-again { min-height:46px; display:inline-flex; justify-content:center; align-items:center; gap:9px; padding:10px 21px; border:1px solid rgba(223,155,173,.58); border-radius:999px; color:#fff3ed; background:linear-gradient(120deg,rgba(173,99,122,.28),rgba(176,143,101,.16)); cursor:pointer; transition:transform .2s,background .2s,border-color .2s,opacity .2s; }
    .open-button:hover,.nav-button:hover,.read-again:hover { transform:translateY(-2px); background-color:rgba(223,155,173,.12); border-color:var(--rose); }
    .hint { margin:10px 0 0; color:#9c929d; font-size:11px; }
    .section-number { display:block; margin-bottom:12px; }
    .page h2 { max-width:700px; margin:0 0 20px; color:var(--rose-light); font-size:clamp(27px,4vw,43px); }
    .page p { margin:0 0 12px; color:#ded3d1; font-size:clamp(14px,1.55vw,17px); line-height:1.78; }
    .page p:last-child { margin-bottom:0; }
    .page p em { color:#e9c7cd; }
    .promise-page .page-content { border-color:rgba(216,189,140,.28); background:radial-gradient(ellipse at 50% 45%,rgba(114,67,82,.28),transparent 72%),rgba(255,255,255,.025); padding-inline:clamp(24px,6vw,66px); }
    .promise-page .page-content::after { content:'♡'; display:block; margin-top:17px; color:rgba(216,189,140,.65); text-align:center; font:21px var(--serif); }
    .question-page .page-content { width:min(100%,900px); border-color:rgba(223,155,173,.31); background:radial-gradient(ellipse at 50% 25%,rgba(120,69,89,.32),transparent 67%),linear-gradient(145deg,rgba(255,255,255,.055),rgba(255,255,255,.02)); box-shadow:0 25px 90px rgba(0,0,0,.24),0 0 60px rgba(202,119,144,.07); }
    .question-page h2 { text-shadow:0 0 25px rgba(223,155,173,.12); }
    .question-lead { color:var(--gold)!important; font-family:var(--serif); font-style:italic; }
    .heart-question { margin:19px 0!important; padding:17px 19px; border:1px solid rgba(216,189,140,.35); border-radius:5px; background:rgba(20,20,32,.45); color:#ffe1dc!important; font:clamp(17px,2.4vw,22px)/1.6 var(--serif)!important; box-shadow:0 0 40px rgba(202,119,144,.08); }
    .typed-questions { display:grid; gap:9px; margin-top:20px; }
    .typed-line { padding:11px 14px; border-left:2px solid var(--rose); background:rgba(255,255,255,.035); color:#f2d4d7; font:italic clamp(15px,2vw,19px)/1.5 var(--serif); opacity:0; transform:translateY(8px); transition:opacity .75s ease,transform .75s ease; }
    .question-page.active .typed-line { opacity:1; transform:none; }.question-page.active .typed-line:nth-child(2) { transition-delay:.16s; }.question-page.active .typed-line:nth-child(3) { transition-delay:.32s; }
    .signature { margin-top:20px!important; color:var(--rose-light)!important; font:italic clamp(17px,2.2vw,20px)/1.6 var(--serif)!important; }
    .signoff { margin-top:16px!important; color:var(--gold)!important; font-family:var(--serif); font-style:italic; }
    .footer-note { margin-top:16px; color:#958a95; font-size:11px; }
    .bottom-bar { position:fixed; z-index:15; inset:auto 0 0; min-height:74px; display:grid; grid-template-columns:1fr auto 1fr; align-items:center; gap:15px; padding:10px max(28px,calc((100vw - 1120px)/2)); padding-bottom:calc(10px + var(--safe-bottom)); background:rgba(16,20,33,.69); border-top:1px solid rgba(255,255,255,.07); backdrop-filter:blur(18px); }
    .page-count { color:var(--muted); font:12px var(--serif); letter-spacing:.12em; white-space:nowrap; }
    .page-count strong { color:var(--gold); font-weight:400; }
    .bottom-progress { width:min(32vw,310px); height:2px; background:rgba(255,255,255,.1); overflow:hidden; }
    .bottom-progress span { display:block; width:0; height:100%; background:linear-gradient(90deg,var(--rose),var(--gold)); transition:width .55s ease; }
    .page-controls { display:flex; justify-content:flex-end; gap:8px; }
    .nav-button { min-height:40px; padding:7px 15px; font-size:12px; }
    .nav-button:disabled { opacity:.34; cursor:default; transform:none; }
    .nav-button.next { color:#fff4ed; border-color:rgba(216,189,140,.45); }
    .read-again { min-height:40px; padding:7px 14px; font-size:12px; }
    .read-again[hidden] { display:none; }
    @media (max-height:700px) and (min-width:601px) {
      main { inset:62px 0 65px; }.topbar { height:59px; }.bottom-bar { min-height:61px; }.page { padding-block:10px; }.page-content { padding-block:18px; }.page p { margin-bottom:8px; line-height:1.6; }.page h2 { margin-bottom:13px; }.section-number { margin-bottom:8px; }.heart-question { margin:12px 0!important; padding:12px 15px; }.typed-questions { gap:6px; margin-top:13px; }.typed-line { padding:8px 11px; }
    }
    @media (max-width:600px) {
      .topbar { height:calc(55px + var(--safe-top)); padding:var(--safe-top) 13px 0; gap:5px; }
      .brand { font-size:15px; white-space:nowrap; }
      .top-actions { gap:4px; }.music-controls { gap:5px; }
      .icon-button { min-width:40px; min-height:40px; padding:8px 10px; }
      .music-word { display:none; }
      .volume-wrap { display:inline-flex; min-width:0; padding:5px; gap:0; font-size:0; }
      .volume-wrap input[type="range"] { width:46px; }
      main { inset:calc(58px + var(--safe-top)) 0 calc(76px + var(--safe-bottom)); }
      .page { padding:10px 14px; }
      .page-content { width:100%; padding:clamp(17px,3vh,27px) clamp(16px,5vw,24px); border-radius:7px; }
      .opening-page .page-content { padding:10px 12px; }
      .opening-page h1 { font-size:clamp(34px,9vw,49px); }
      .opening-name { font-size:17px; }
      .opening-tagline { max-width:320px; font-size:15px; }
      .envelope-wrap { width:min(250px,70vw); margin:clamp(16px,3vh,26px) auto 14px; }
      .envelope { height:clamp(118px,19vh,148px); }
      .open-button { min-height:48px; padding-inline:22px; }
      .page h2 { font-size:clamp(27px,7.6vw,36px); margin-bottom:15px; }
      .page p { font-size:clamp(14px,3.8vw,16px); line-height:1.65; margin-bottom:10px; }
      .section-number { font-size:9px; letter-spacing:.19em; margin-bottom:9px; }
      .promise-page .page-content { padding-inline:20px; }
      .question-page .page-content { padding:16px clamp(14px,4.5vw,21px); }
      .question-page .page h2 { margin-bottom:12px; }
      .question-page p { margin-bottom:8px; line-height:1.57; }
      .heart-question { padding:12px 14px; margin:12px 0!important; font-size:17px!important; }
      .typed-questions { gap:6px; margin-top:12px; }.typed-line { padding:8px 10px; font-size:15px; }
      .bottom-bar { min-height:calc(70px + var(--safe-bottom)); grid-template-columns:auto 1fr auto; gap:9px; padding:8px 12px calc(8px + var(--safe-bottom)); }
      .page-count { font-size:10px; letter-spacing:.05em; }.bottom-progress { width:100%; }
      .page-controls { gap:6px; }.nav-button { min-height:44px; min-width:44px; padding:7px 12px; font-size:11px; }.read-again { min-height:42px; padding:6px 10px; font-size:11px; }
    }
    @media (max-width:380px) {
      .brand { font-size:13px; }.topbar { padding-left:10px; padding-right:10px; }.page { padding-inline:9px; }.page-content { padding-inline:14px; }
      .page p { font-size:13px; line-height:1.55; margin-bottom:8px; }.page h2 { font-size:26px; }
      .bottom-bar { padding-inline:8px; gap:6px; }.nav-button { min-width:40px; padding-inline:9px; }.page-count { font-size:9px; }
    }
    @media (max-height:700px) and (max-width:600px) {
      main { inset:calc(54px + var(--safe-top)) 0 calc(66px + var(--safe-bottom)); }
      .page { padding-block:6px; }.page-content { padding-block:13px; }.page h2 { margin-bottom:9px; font-size:clamp(24px,6.7vw,31px); }.page p { font-size:13px; line-height:1.48; margin-bottom:6px; }.section-number { margin-bottom:6px; }.question-page .page-content { padding-block:11px; }.question-page p { margin-bottom:5px; }.heart-question { margin:8px 0!important; padding:8px 10px; font-size:15px!important; }.typed-questions { margin-top:8px; gap:4px; }.typed-line { padding:6px 9px; font-size:13px; }
      .opening-page .page-content { padding-block:5px; }.opening-page h1 { font-size:34px; }.envelope-wrap { margin-block:10px; }.envelope { height:100px; }
    }
    @media (prefers-reduced-motion:reduce) {
      *,*::before,*::after { scroll-behavior:auto!important; animation-duration:.01ms!important; animation-iteration-count:1!important; transition-duration:.01ms!important; }
      .specks,.petals { display:none; }.page { filter:none; }
    }

    /* Cinematic closing sequence */
    .cinematic-ending { position:fixed; z-index:40; inset:0; display:grid; place-items:center; overflow:hidden; visibility:hidden; opacity:0; pointer-events:none; isolation:isolate; background:radial-gradient(ellipse at 50% 58%,rgba(90,48,57,.22),transparent 43%),linear-gradient(145deg,#101421,#080b14 72%,#130d18); transition:opacity 1.8s ease,visibility 1.8s; }
    .cinematic-ending.active { visibility:visible; opacity:1; pointer-events:auto; }
    .cinematic-ending::before { content:''; position:absolute; inset:-20%; z-index:-1; opacity:0; transform:scale(1.12); background:radial-gradient(ellipse at 50% 52%,rgba(207,164,105,.24),transparent 18%),radial-gradient(ellipse at 50% 58%,rgba(163,91,111,.14),transparent 46%); transition:opacity 3s ease,transform 8s ease; }
    .cinematic-ending.active::before { opacity:1; transform:scale(1); }
    body.cinematic-active .topbar,body.cinematic-active .bottom-bar,body.cinematic-active .progress-track,body.cinematic-active main { opacity:0; filter:blur(7px); transform:scale(.975); transition:opacity 1.8s ease,filter 1.8s ease,transform 2.6s ease; pointer-events:none; }
    .ending-stars,.ending-motes,.ending-petals { position:absolute; inset:0; overflow:hidden; pointer-events:none; }
    .ending-star { position:absolute; width:2px; height:2px; border-radius:50%; background:#fff1d8; box-shadow:0 0 9px 2px rgba(233,198,137,.58); opacity:0; animation:endingTwinkle var(--dur,4s) ease-in-out var(--delay,0s) infinite alternate; }
    @keyframes endingTwinkle { 0%{opacity:.08;transform:scale(.6)} 100%{opacity:.9;transform:scale(1.45)} }
    .ending-mote { position:absolute; left:var(--left); top:var(--top); width:var(--size); height:var(--size); border-radius:50%; background:#f4d7a5; box-shadow:0 0 8px 2px rgba(232,184,112,.42); opacity:0; animation:moteDrift var(--dur) ease-in-out var(--delay) infinite; }
    @keyframes moteDrift { 0%{opacity:0;transform:translate3d(0,18px,0) scale(.45)} 35%{opacity:.68} 100%{opacity:0;transform:translate3d(var(--drift),-55px,0) scale(1.2)} }
    .ending-petal { position:absolute; top:-8vh; left:var(--left); color:#d89aa4; opacity:0; font-size:var(--size); animation:roseFall var(--dur) linear var(--delay) infinite; }
    @keyframes roseFall { 0%{opacity:0;transform:translate3d(0,-4vh,0) rotate(0)} 12%{opacity:.5} 85%{opacity:.38} 100%{opacity:0;transform:translate3d(34px,112vh,0) rotate(330deg)} }
    .ending-orbit-glow { position:absolute; left:50%; top:50%; width:min(72vw,650px); aspect-ratio:1; border-radius:50%; background:radial-gradient(circle,rgba(218,174,111,.16),rgba(172,100,117,.08) 29%,transparent 68%); filter:blur(20px); opacity:0; transform:translate(-50%,-50%) scale(.55); transition:opacity 2.2s ease,transform 4s ease; }
    .cinematic-ending.active .ending-orbit-glow { opacity:1; transform:translate(-50%,-50%) scale(1); }
    .ending-stage { position:relative; z-index:2; display:grid; place-items:center; width:min(100%,900px); min-height:100%; padding:calc(28px + var(--safe-top)) 24px calc(28px + var(--safe-bottom)); text-align:center; }
    .ending-reveal,.ending-final-copy,.ending-signature,.final-screen { position:absolute; inset:0; display:flex; flex-direction:column; align-items:center; justify-content:center; padding:clamp(20px,4vh,36px) clamp(18px,5vw,44px); opacity:0; visibility:hidden; transform:translate3d(0,12px,0) scale(.985); transition:opacity .85s ease,transform 1s cubic-bezier(.2,.72,.2,1),visibility 0s linear .85s; }
    .ending-reveal.visible,.ending-final-copy.visible,.ending-signature.visible,.final-screen.visible { opacity:1; visibility:visible; transform:none; transition-delay:0s; }
    .ending-reveal.is-leaving,.ending-final-copy.is-leaving,.ending-signature.is-leaving,.final-screen.is-leaving { opacity:0; visibility:hidden; transform:translate3d(0,-8px,0) scale(.99); transition:opacity .65s ease,transform .65s ease,visibility 0s linear .65s; }
    .ending-reveal p { max-width:100%; margin:9px 0; color:#f4e6d9; font-family:var(--serif); font-size:clamp(25px,5vw,50px); line-height:1.25; letter-spacing:.015em; text-shadow:0 0 30px rgba(233,192,129,.3); opacity:0; filter:blur(8px); transform:translateY(10px); transition:opacity 1.2s ease,filter 1.4s ease,transform 1.4s ease; }
    .ending-reveal.visible p { opacity:1; filter:blur(0); transform:none; }
    .ending-reveal p + p { color:#f0cad0; }
    .ending-reveal.visible p + p { transition-delay:1.8s; }
    .ending-reveal:not(.visible) p + p { transition-delay:0s; }
    .heart-formation { position:absolute; left:50%; top:50%; width:1px; height:1px; opacity:0; transition:opacity 1s ease; }
    .heart-formation.visible { opacity:1; }
    .heart-particle { position:absolute; left:0; top:0; width:4px; height:4px; border-radius:50%; background:#f5d9a8; box-shadow:0 0 9px 2px rgba(233,170,139,.74); opacity:0; transform:translate(var(--x),var(--y)) scale(.1); transition:transform 1.5s cubic-bezier(.2,.8,.2,1),opacity 1.4s ease; }
    .heart-formation.visible .heart-particle { opacity:.9; transform:translate(var(--x),var(--y)) scale(1); transition-delay:var(--delay); }
    .heart-formation.pulse { animation:heartPulse 1.6s ease-in-out infinite; }
    @keyframes heartPulse { 0%,100%{filter:drop-shadow(0 0 8px rgba(226,160,133,.3))} 50%{filter:drop-shadow(0 0 25px rgba(238,182,137,.82))} }
    .heart-formation.scattered .heart-particle { opacity:0; transform:translate(calc(var(--x) + var(--dx)),calc(var(--y) + var(--dy))) scale(.15); transition:transform 2.8s cubic-bezier(.15,.7,.25,1),opacity 2.3s ease; }
    .ending-final-copy { gap:clamp(9px,2vh,18px); }
    .ending-final-copy p,.ending-signature p { max-width:720px; margin:0; color:#e6d6d0; font:clamp(15px,2vw,19px)/1.5 var(--sans); text-shadow:0 0 20px rgba(222,172,122,.12); }
    .ending-final-copy > p { opacity:0; transform:translateY(8px); transition:opacity .8s ease,transform .9s ease; }
    .ending-final-copy.visible > p { opacity:1; transform:none; }
    .ending-final-copy.visible > p:nth-child(2) { transition-delay:.15s; }
    .ending-final-copy.visible > p:nth-child(3) { transition-delay:.35s; }
    .ending-final-copy.visible > p:nth-child(4) { transition-delay:.6s; }
    .ending-final-copy .for-you { margin-bottom:8px; color:var(--gold); font:italic clamp(23px,4vw,38px)/1.2 var(--serif); }
    .ending-final-copy .heart-piece { max-width:690px; margin:10px 0; color:#f5d9d8; font:italic clamp(22px,3.7vw,36px)/1.45 var(--serif); }
    .ending-signature { gap:10px; }
    .ending-signature > p { opacity:0; transform:translateY(7px); transition:opacity .8s ease,transform .8s ease; }
    .ending-signature.visible > p { opacity:1; transform:none; }
    .ending-signature.visible > p:nth-of-type(2) { transition-delay:.2s; }
    .ending-signature.visible > p:nth-of-type(3) { transition-delay:.55s; }
    .ending-signature .signoff-line { color:#f2d5d0; font:italic clamp(19px,3vw,27px)/1.4 var(--serif); }
    .ending-signature .forever-line { margin-top:12px; color:var(--gold); font:italic clamp(17px,2.5vw,24px)/1.4 var(--serif); }
    .signature-art { width:min(280px,60vw); height:78px; overflow:visible; margin:5px 0 0; }
    .signature-art path { fill:none; stroke:#e5bd8e; stroke-width:1.6; stroke-linecap:round; stroke-linejoin:round; stroke-dasharray:1; stroke-dashoffset:1; filter:drop-shadow(0 0 5px rgba(226,179,128,.55)); }
    .ending-signature.visible .signature-art path { animation:drawSignature 2.7s ease forwards .35s; }
    @keyframes drawSignature { to{stroke-dashoffset:0} }
    .final-screen { gap:13px; background:radial-gradient(ellipse at 50% 48%,rgba(116,54,71,.22),transparent 53%); }
    .final-screen::before { content:''; position:absolute; inset:12%; z-index:-1; background:radial-gradient(ellipse at 50% 45%,rgba(218,176,116,.2),transparent 57%); filter:blur(18px); animation:finalGlow 5s ease-in-out infinite alternate; }
    @keyframes finalGlow { to{opacity:.48;transform:scale(.88)} }
    .final-rose { width:clamp(55px,9vw,86px); height:clamp(55px,9vw,86px); color:#dba6a4; filter:drop-shadow(0 0 18px rgba(226,157,143,.4)); animation:roseBloom 3.8s ease-in-out infinite alternate; }
    @keyframes roseBloom { to{transform:scale(1.08) rotate(-4deg);filter:drop-shadow(0 0 28px rgba(232,174,132,.62))} }
    .final-name { margin:0; color:#f3d9c7; font:clamp(32px,7vw,68px)/1.08 var(--serif); letter-spacing:.16em; text-shadow:0 0 35px rgba(225,178,125,.34); }
    .final-caption { margin:0; color:#bfaeb0; font:italic clamp(13px,1.8vw,17px) var(--serif); letter-spacing:.06em; }
    .ending-read-again { min-height:44px; margin-top:13px; padding:9px 22px; border:1px solid rgba(216,189,140,.52); border-radius:999px; color:#f6e9dc; background:rgba(255,255,255,.045); cursor:pointer; backdrop-filter:blur(12px); transition:background .25s,transform .25s,border-color .25s; }
    .ending-read-again:hover { transform:translateY(-2px); border-color:var(--gold); background:rgba(216,189,140,.12); }
    body.ending-finale .ending-reveal,body.ending-finale .ending-final-copy,body.ending-finale .ending-signature { opacity:0; visibility:hidden; }
    @media (max-width:600px) {
      .ending-stage { padding-inline:18px; }
      .ending-reveal,.ending-final-copy,.ending-signature,.final-screen { padding:20px 17px; }
      .ending-final-copy { gap:clamp(8px,1.8vh,14px); }
      .ending-final-copy .heart-piece { font-size:clamp(21px,6vw,29px); }
      .final-name { letter-spacing:.1em; }
      .heart-particle { width:3px; height:3px; }
    }
    @media (prefers-reduced-motion:reduce) {
      .ending-star,.ending-mote,.ending-petal,.heart-formation.pulse,.final-rose,.final-screen::before { animation:none!important; }
      .heart-particle { transition:none!important; }
    }
  </style>
</head>
<body>
  <div class="ambient" aria-hidden="true"><div class="glow one"></div><div class="glow two"></div><div class="specks" id="specks"></div><div class="petals" id="petals"></div></div>
  <div class="progress-track" role="progressbar" aria-label="Progress membaca surat" aria-valuemin="0" aria-valuemax="100" aria-valuenow="0"><div class="progress-bar" id="progressBar"></div></div>
  <header class="topbar">
    <div class="brand">A Letter For Liora ♡</div>
    <div class="top-actions" aria-label="Kontrol musik">
      <div class="music-controls">
        <button class="icon-button" id="musicToggle" type="button" aria-pressed="false" aria-label="Putar musik ambient">♫ <span class="music-word" id="musicLabel">Play</span></button>
        <button class="icon-button" id="muteToggle" type="button" aria-pressed="false" aria-label="Matikan suara">◖</button>
        <label class="volume-wrap" for="volume">Vol <input id="volume" type="range" min="0" max="100" value="24" aria-label="Volume musik"></label>
      </div>
    </div>
  </header>

  <main id="presentation" aria-live="polite">
    <section class="page opening-page active" data-page="0" aria-label="Pembuka surat">
      <div class="page-content">
        <span class="eyebrow">A letter, written with care</span>
        <h1>For Someone Special...</h1>
        <p class="opening-name">Liora Angelin</p>
        <p class="opening-tagline">A Letter Written From My Heart</p>
        <p class="opening-tagline" id="typedIntro" aria-label="There's something I've been wanting to tell you, Liora.">There's something I've been wanting to tell you, Liora.</p>
        <p class="opening-tagline">Some feelings are difficult to say, so I made a little place for them.</p>
        <div class="envelope-wrap" aria-hidden="true"><div class="envelope" id="envelope"><div class="flap"></div><div class="seal">♡</div></div></div>
        <button class="open-button" id="openLetter" type="button">Open My Letter ♡</button>
        <p class="hint">A little place for the things that are hard to say.</p>
      </div>
    </section>

    <section class="page" data-page="1" aria-label="01 — A little story">
      <div class="page-content"><span class="section-number">01 — A LITTLE STORY</span>
        <h2>Before You, There Was a Part of Me That Learned to Be Careful.</h2>
        <p>Ada sesuatu tentang diriku yang mungkin belum sepenuhnya kamu ketahui.</p>
        <p>Aku pernah mengalami sesuatu yang membuatku memahami bahwa mencintai seseorang bukan hanya tentang memberikan perasaan, tetapi juga tentang kepercayaan.</p>
        <p>Aku pernah menaruh kepercayaan kepada seseorang, tetapi pada akhirnya aku merasakan bagaimana rasanya ketika kepercayaan itu tidak dijaga.</p>
        <p>Sejak saat itu, membuka hati tidak selalu terasa mudah bagiku.</p>
      </div>
    </section>

    <section class="page" aria-label="01 — A little story, continued">
      <div class="page-content"><span class="section-number">01 — A LITTLE STORY · CONTINUED</span>
        <h2>Learning to Trust Again.</h2>
        <p>Terkadang, hal-hal kecil bisa membuatku berpikir terlalu jauh. Bahkan ketika seseorang yang aku sayangi hanya sedang sibuk atau belum sempat membalas pesanku, pikiranku terkadang mulai dipenuhi berbagai pertanyaan.</p>
        <p>Aku tahu tidak semua orang sama. Aku juga tidak ingin menjadikan pengalaman sebelumnya sebagai alasan untuk meragukanmu.</p>
        <p>Aku hanya ingin kamu memahami bahwa di balik caraku mencintai, ada seseorang yang sedang belajar untuk kembali percaya.</p>
      </div>
    </section>

    <section class="page" data-page="2" aria-label="02 — What you mean to me">
      <div class="page-content"><span class="section-number">02 — WHAT YOU MEAN TO ME</span>
        <h2>Why You Matter to Me.</h2>
        <p>Liora, aku tidak tahu bagaimana perjalanan kita akan berjalan nantinya.</p>
        <p>Namun, aku ingin kamu tahu bahwa kehadiranmu memiliki arti tersendiri bagiku.</p>
        <p>Aku menyukai percakapan sederhana kita, cerita tentang hari-harimu, hal-hal kecil yang kamu ceritakan, bahkan percakapan biasa yang mungkin terlihat tidak istimewa.</p>
        <p>Bagiku, mencintai bukan hanya tentang mengatakan <em>love you</em> setiap hari.</p>
        <p>Tetapi juga tentang mendengarkan, memahami, menghargai kesibukan, menjaga kepercayaan, dan tetap berusaha ketika ada sesuatu yang perlu diperbaiki.</p>
        <p>Aku tidak ingin menjadi seseorang yang hanya pandai mengucapkan janji. Aku ingin belajar membuktikan perasaanku melalui sikapku.</p>
      </div>
    </section>

    <section class="page promise-page" data-page="3" aria-label="03 — A promise I don't say lightly">
      <div class="page-content"><span class="section-number">03 — A PROMISE I DON'T SAY LIGHTLY</span>
        <h2>One Promise, From the Bottom of My Heart.</h2>
        <p>Ada satu hal yang ingin aku sampaikan kepadamu.</p>
        <p>Aku pernah berjanji kepada diriku sendiri bahwa mungkin ini akan menjadi kali terakhir aku berani mencintai seseorang sedalam ini.</p>
        <p>Aku bahkan tidak tahu kapan lagi aku akan mampu membuka hati dengan perasaan yang sama.</p>
        <p>Bukan karena aku ingin membuatmu merasa terbebani, dan bukan pula karena aku ingin meminta sesuatu sebagai balasannya.</p>
      </div>
    </section>

    <section class="page promise-page" aria-label="03 — A promise, continued">
      <div class="page-content"><span class="section-number">03 — A PROMISE I DON'T SAY LIGHTLY · CONTINUED</span>
        <h2>A Promise Meant to Be Lived.</h2>
        <p>Aku hanya ingin menjalani perasaan ini dengan sungguh-sungguh.</p>
        <p>Aku tidak tahu sampai kapan perjalanan kita akan berlangsung, tetapi selama kita memilih untuk bersama, aku ingin menjaga hubungan ini dengan kejujuran, kesetiaan, dan rasa saling menghargai.</p>
        <p>Aku tidak menjanjikan bahwa aku akan selalu sempurna.</p>
        <p>Namun, aku ingin terus belajar menjadi seseorang yang bisa kamu percaya.</p>
      </div>
    </section>

    <section class="page question-page" data-page="4" aria-label="04 — The question I keep in my heart">
      <div class="page-content"><span class="section-number">04 — THE QUESTION I KEEP IN MY HEART</span>
        <h2>Can I Ask You Something, Liora?</h2>
        <p class="question-lead">Sometimes, there are questions I keep inside because I don't always know how to ask them.</p>
        <p>Aku terkadang penasaran, apakah apa yang aku rasakan selama ini juga kamu rasakan?</p>
        <p>Ketika kamu mengatakan bahwa kamu menyayangiku, apakah kamu juga melihat hubungan ini sebagai sesuatu yang ingin kamu jaga dengan sungguh-sungguh?</p>
        <p>Apakah kamu juga ingin kita saling setia, saling jujur, dan saling menjaga kepercayaan?</p>
        <p>Dan ada satu hal yang sebenarnya paling ingin aku ketahui...</p>
        <p class="heart-question"><strong>Menurutmu, apakah kita berdua benar-benar ingin menjaga hubungan ini dengan kesetiaan, kejujuran, dan kesungguhan yang sama?</strong></p>
      </div>
    </section>

    <section class="page question-page" aria-label="04 — The question, continued">
      <div class="page-content"><span class="section-number">04 — THE QUESTION I KEEP IN MY HEART · CONTINUED</span>
        <h2>What I Hope We Can Choose Together.</h2>
        <p>Bukan hanya ketika semuanya terasa menyenangkan, tetapi juga ketika kita sedang sibuk, menghadapi jarak, mengalami kesalahpahaman, atau melewati hari-hari yang tidak selalu mudah.</p>
        <p>Apakah kita sama-sama ingin mempertahankan hubungan ini bukan hanya melalui kata-kata, tetapi juga melalui tindakan?</p>
        <p>Apakah kamu juga ingin menjadi seseorang yang saling menjaga, bukan hanya seseorang yang saling mengatakan cinta?</p>
        <p>Aku tidak ingin menjadi satu-satunya orang yang berusaha menjaga hubungan ini. Aku ingin kita berdua memiliki keinginan yang sama untuk merawat apa yang sedang kita bangun.</p>
        <p>Aku tidak sedang menuduhmu, meragukanmu, atau memintamu membuktikan sesuatu secara berlebihan.</p>
      </div>
    </section>

    <section class="page question-page" aria-label="04 — The question, one last thought">
      <div class="page-content"><span class="section-number">04 — THE QUESTION I KEEP IN MY HEART · CONTINUED</span>
        <h2>What I Hope We Can Understand.</h2>
        <p>Aku hanya ingin memahami isi hatimu.</p>
        <p>Karena bagiku, kesetiaan bukan sekadar tidak berpaling, kejujuran bukan sekadar berkata benar, dan kesungguhan bukan sekadar berjanji.</p>
        <p>Semuanya perlu terlihat dalam cara kita memperlakukan satu sama lain.</p>
        <div class="typed-questions" aria-label="Pertanyaan untuk direnungkan"><div class="typed-line">Do you feel the same way?</div><div class="typed-line">Do you want to remain faithful to each other?</div><div class="typed-line">Are we both willing to protect this relationship with the same honesty and sincerity?</div></div>
      </div>
    </section>

    <section class="page" data-page="5" aria-label="05 — What I hope we can build together">
      <div class="page-content"><span class="section-number">05 — WHAT I HOPE WE CAN BUILD TOGETHER</span>
        <h2>Not a Perfect Relationship, Just an Honest One.</h2>
        <p>Aku tidak meminta hubungan yang sempurna.</p>
        <p>Aku tahu kita memiliki kesibukan, kehidupan, dan tanggung jawab masing-masing.</p>
        <p>Mungkin akan ada hari ketika kita tidak bisa berbicara sebanyak biasanya. Mungkin ada saat ketika kita salah memahami perkataan satu sama lain.</p>
        <p>Namun, aku berharap ketika hal-hal seperti itu terjadi, kita tidak langsung menyerah atau saling menjauh.</p>
      </div>
    </section>

    <section class="page" aria-label="05 — What I hope we can build, continued">
      <div class="page-content"><span class="section-number">05 — WHAT I HOPE WE CAN BUILD TOGETHER · CONTINUED</span>
        <h2>Choosing to Keep Showing Up.</h2>
        <p>Aku ingin kita bisa membicarakan masalah dengan jujur, mengakui kesalahan, saling meminta maaf, dan belajar memperbaikinya.</p>
        <p>Aku ingin kesetiaan datang dari kesadaran, bukan keterpaksaan.</p>
        <p>Aku ingin kejujuran menjadi kebiasaan, bukan hanya sesuatu yang kita lakukan ketika ditanya.</p>
        <p>Dan aku ingin kesungguhan datang dari kedua hati, bukan hanya dari salah satu pihak.</p>
        <p>Aku ingin kita sama-sama memilih untuk menjaga hubungan ini.</p>
      </div>
    </section>

    <section class="page" data-page="6" aria-label="06 — No pressure, just honesty">
      <div class="page-content"><span class="section-number">06 — NO PRESSURE, JUST HONESTY</span>
        <h2>You Don't Have to Give Me a Perfect Answer.</h2>
        <p>Aku tidak mengharapkan jawaban yang sempurna.</p>
        <p>Aku juga tidak ingin kamu mengatakan sesuatu hanya karena takut membuatku kecewa.</p>
        <p>Aku lebih menghargai jawaban yang jujur, meskipun sederhana.</p>
        <p>Kalau ada sesuatu yang kamu rasakan, katakanlah.</p>
        <p>Kalau ada sesuatu yang menurutmu perlu kita perbaiki, aku ingin mendengarnya.</p>
        <p>Aku ingin kita bisa saling berbicara tanpa merasa terpaksa, saling memahami tanpa harus menebak-nebak, dan saling menyayangi tanpa kehilangan diri kita masing-masing.</p>
        <p>Aku ingin jawaban yang benar-benar berasal dari hatimu.</p>
      </div>
    </section>

    <section class="page" data-page="7" aria-label="07 — The final letter">
      <div class="page-content"><span class="section-number">07 — THE FINAL LETTER</span>
        <h2>To Liora Angelin ♡</h2>
        <p>Terima kasih sudah menjadi bagian dari cerita yang sedang aku jalani sekarang.</p>
        <p>Aku tidak tahu apa yang akan terjadi besok, beberapa bulan lagi, atau tahun-tahun mendatang.</p>
        <p>Aku juga tidak tahu sampai kapan perjalanan ini akan berlangsung.</p>
        <p>Namun, aku berharap selama kita masih memilih untuk berjalan bersama, kita tidak berhenti belajar memahami satu sama lain.</p>
      </div>
    </section>

    <section class="page" data-page="7" aria-label="07 — The final letter, continued">
      <div class="page-content"><span class="section-number">07 — THE FINAL LETTER · CONTINUED</span>
        <h2>To Liora Angelin ♡</h2>
        <p>Aku ingin mencintaimu dengan cara yang tulus, bukan dengan ketakutan.</p>
        <p>Aku ingin kita saling menjaga, bukan saling menyakiti.</p>
        <p>Aku ingin kita saling percaya, bukan terus-menerus mempertanyakan perasaan satu sama lain.</p>
        <p>Dan yang paling penting, aku ingin kesetiaan, kejujuran, serta kesungguhan menjadi sesuatu yang kita jaga bersama.</p>
        <p>Aku tidak tahu apakah kamu merasakan semuanya dengan cara yang sama.</p>
      </div>
    </section>

    <section class="page" aria-label="07 — The final letter, ending">
      <div class="page-content"><span class="section-number">07 — THE FINAL LETTER · CONTINUED</span>
        <h2>With All My Sincerity.</h2>
        <p>Tetapi aku berharap kita bisa menemukan jawabannya melalui percakapan yang jujur.</p>
        <p class="signature">And maybe, this time, I want to believe that love can also feel peaceful.</p>
        <p class="signoff">With all my sincerity.<br><br>Someone who truly cares about you. ♡</p>
        <div class="footer-note">Made with sincerity, for Liora.</div>
      </div>
    </section>
  </main>

  <footer class="bottom-bar" aria-label="Navigasi halaman">
    <div class="page-count" id="pageCount"><strong>00</strong> / 17</div>
    <div class="bottom-progress" aria-hidden="true"><span id="pageProgress"></span></div>
    <div class="page-controls">
      <button class="read-again" id="readAgain" type="button" hidden>Read Again ♡</button>
      <button class="nav-button" id="previousPage" type="button" aria-label="Halaman sebelumnya" disabled>← <span>Previous</span></button>
      <button class="nav-button next" id="nextPage" type="button">Next <span>→</span></button>
    </div>
  </footer>

  <section class="cinematic-ending" id="cinematicEnding" aria-label="A final message for Liora" aria-hidden="true">
    <div class="ending-stars" id="endingStars" aria-hidden="true"></div>
    <div class="ending-motes" id="endingMotes" aria-hidden="true"></div>
    <div class="ending-petals" id="endingPetals" aria-hidden="true"></div>
    <div class="ending-orbit-glow" aria-hidden="true"></div>
    <div class="ending-stage">
      <div class="ending-reveal" id="endingReveal" aria-live="polite">
        <p>Every Letter Has an Ending...</p>
        <p>But Some Feelings Remain.</p>
      </div>
      <div class="heart-formation" id="heartFormation" aria-hidden="true"></div>
      <div class="ending-final-copy" id="endingFinalCopy">
        <p class="for-you">For You, Liora Angelin ♡</p>
        <p>Thank you for being part of my story.</p>
        <p>May we always choose honesty, kindness, and sincerity.</p>
        <p class="heart-piece">Somewhere between all these words, I hope you found a little piece of my heart.</p>
      </div>
      <div class="ending-signature" id="endingSignature">
        <p class="signoff-line">With all my sincerity,</p>
        <p>Someone who truly cares about you.</p>
        <svg class="signature-art" viewBox="0 0 320 90" role="img" aria-label="A handwritten heart signature">
          <path pathLength="1" d="M12 57 C27 24 39 22 37 49 C35 72 49 72 58 48 C64 32 70 31 70 53 C71 70 82 66 91 49 C100 32 105 34 102 53 C99 70 112 68 123 50 C132 35 141 37 133 55 C127 70 145 67 158 49 C169 33 178 37 168 55 C159 73 181 69 197 48 C208 33 217 38 204 58 C196 72 213 68 229 48 C241 33 248 39 237 58 C229 73 247 67 263 47 C276 31 285 39 270 57 C260 70 281 67 306 49 M141 78 C157 70 173 69 190 76 C206 82 225 82 243 75" />
        </svg>
        <p class="forever-line">— Forever Written in This Little Letter ♡</p>
      </div>
      <div class="final-screen" id="finalScreen">
        <svg class="final-rose" viewBox="0 0 100 100" aria-label="A rose for Liora" role="img">
          <path fill="currentColor" d="M50 51C30 48 29 29 44 24c-1-13 17-18 24-5 13-3 22 12 12 22 2 13-13 19-22 10-5 13-9 28-8 39h-4c1-14-1-27-6-38-9 3-19-4-18-13 1-8 9-12 17-10-2 9 2 16 11 22Zm-1-8c-8-2-13-9-12-16-9-1-14 6-12 12 2 7 12 9 24 4Zm5-2c7 4 15 0 16-7 2-8-5-13-12-11 2 7 0 13-4 18Zm-2-8c7-8 2-18-5-18-7 0-10 7-7 12 5-1 9 1 12 6Z"/>
          <path d="M48 75c-8-8-17-10-24-8m27 10c8-9 16-11 23-9" fill="none" stroke="#b99a67" stroke-width="2" stroke-linecap="round"/>
        </svg>
        <h1 class="final-name">LIORA ANGELIN</h1>
        <p class="final-caption">A little piece of my heart, written just for you.</p>
        <button class="ending-read-again" id="endingReadAgain" type="button">Read Again ♡</button>
      </div>
    </div>
  </section>

  <script>
    (() => {
      const reduceMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
      const pages = [...document.querySelectorAll('.page')];
      const envelope = document.getElementById('envelope');
      const openButton = document.getElementById('openLetter');
      const previousButton = document.getElementById('previousPage');
      const nextButton = document.getElementById('nextPage');
      const readAgain = document.getElementById('readAgain');
      const pageCount = document.getElementById('pageCount');
      const pageProgress = document.getElementById('pageProgress');
      const progressBar = document.getElementById('progressBar');
      const progressTrack = document.querySelector('.progress-track');
      const cinematicEnding = document.getElementById('cinematicEnding');
      const endingStars = document.getElementById('endingStars');
      const endingMotes = document.getElementById('endingMotes');
      const endingPetals = document.getElementById('endingPetals');
      const endingReveal = document.getElementById('endingReveal');
      const heartFormation = document.getElementById('heartFormation');
      const endingFinalCopy = document.getElementById('endingFinalCopy');
      const endingSignature = document.getElementById('endingSignature');
      const finalScreen = document.getElementById('finalScreen');
      const endingReadAgain = document.getElementById('endingReadAgain');
      let currentPage = 0;
      let opened = false;
      let endingStarted = false;
      let endingTimers = [];
      let endingParticlesBuilt = false;
      let touchStartX = 0;
      let touchStartY = 0;
      const pad = value => String(value).padStart(2, '0');
      const typedIntro = document.getElementById('typedIntro');
      const introText = "There's something I've been wanting to tell you, Liora.";
      if (!reduceMotion) {
        typedIntro.textContent = '';
        let character = 0;
        const typing = window.setInterval(() => {
          typedIntro.textContent = introText.slice(0, ++character);
          if (character >= introText.length) window.clearInterval(typing);
        }, 38);
      }

      const specks = document.getElementById('specks');
      const petals = document.getElementById('petals');
      if (!reduceMotion) {
        for (let i = 0; i < 26; i++) {
          const dot = document.createElement('i'); dot.className = 'speck';
          dot.style.left = `${Math.random() * 100}%`; dot.style.top = `${Math.random() * 100}%`;
          dot.style.animationDelay = `${Math.random() * 5}s`; specks.appendChild(dot);
        }
        ['✿', '·', '❀', '·', '✿'].forEach((symbol, i) => {
          const petal = document.createElement('i'); petal.className = 'petal'; petal.textContent = symbol;
          petal.style.left = `${8 + Math.random() * 84}%`; petal.style.animationDuration = `${22 + Math.random() * 14}s`;
          petal.style.animationDelay = `${-Math.random() * 28}s`; petal.style.fontSize = `${10 + (i % 3) * 3}px`; petals.appendChild(petal);
        });
      }

      function renderPage(nextIndex, direction = 1) {
        const target = Math.max(0, Math.min(pages.length - 1, nextIndex));
        if (target === currentPage && pages[target].classList.contains('active')) return;
        const oldPage = pages[currentPage];
        const newPage = pages[target];
        oldPage.classList.remove('active', 'exit-left');
        if (direction < 0) oldPage.classList.add('exit-left');
        newPage.classList.remove('exit-left');
        newPage.classList.add('active');
        currentPage = target;
        const progress = currentPage === 0 ? 0 : (currentPage / (pages.length - 1)) * 100;
        pageCount.innerHTML = `<strong>${pad(currentPage)}</strong> / ${pad(pages.length - 1)}`;
        pageProgress.style.width = `${progress}%`;
        progressBar.style.width = `${progress}%`;
        progressTrack.setAttribute('aria-valuenow', String(Math.round(progress)));
        previousButton.disabled = currentPage === 0;
        nextButton.innerHTML = currentPage === pages.length - 1 ? 'Finish Reading <span>♡</span>' : 'Next <span>→</span>';
        readAgain.hidden = currentPage !== pages.length - 1;
        newPage.querySelector('.page-content')?.scrollTo(0, 0);
      }
      function buildEndingParticles() {
        endingStars.replaceChildren(); endingMotes.replaceChildren(); endingPetals.replaceChildren();
        heartFormation.replaceChildren();
        const smallScreen = window.matchMedia('(max-width: 600px)').matches;
        const lowPower = smallScreen || (navigator.deviceMemory && navigator.deviceMemory <= 2);
        const starCount = lowPower ? 40 : 82;
        const moteCount = lowPower ? 58 : 148;
        const petalCount = lowPower ? 7 : 14;
        const heartCount = lowPower ? 48 : 84;
        for (let i = 0; i < starCount; i++) {
          const star = document.createElement('i'); star.className = 'ending-star';
          star.style.left = `${Math.random() * 100}%`; star.style.top = `${Math.random() * 100}%`;
          star.style.setProperty('--dur', `${2.2 + Math.random() * 4}s`);
          star.style.setProperty('--delay', `${Math.random() * 3}s`);
          endingStars.appendChild(star);
        }
        for (let i = 0; i < moteCount; i++) {
          const mote = document.createElement('i'); mote.className = 'ending-mote';
          mote.style.setProperty('--left', `${Math.random() * 100}%`);
          mote.style.setProperty('--top', `${20 + Math.random() * 80}%`);
          mote.style.setProperty('--size', `${1 + Math.random() * 2.5}px`);
          mote.style.setProperty('--dur', `${5 + Math.random() * 7}s`);
          mote.style.setProperty('--delay', `${Math.random() * 8}s`);
          mote.style.setProperty('--drift', `${-35 + Math.random() * 70}px`);
          endingMotes.appendChild(mote);
        }
        for (let i = 0; i < petalCount; i++) {
          const petal = document.createElement('i'); petal.className = 'ending-petal';
          petal.textContent = i % 2 ? '❀' : '✿';
          petal.style.setProperty('--left', `${Math.random() * 100}%`);
          petal.style.setProperty('--size', `${11 + Math.random() * 11}px`);
          petal.style.setProperty('--dur', `${17 + Math.random() * 14}s`);
          petal.style.setProperty('--delay', `${-Math.random() * 20}s`);
          endingPetals.appendChild(petal);
        }
        for (let i = 0; i < heartCount; i++) {
          const t = (i / heartCount) * Math.PI * 2;
          const x = 16 * Math.pow(Math.sin(t), 3);
          const y = 13 * Math.cos(t) - 5 * Math.cos(2 * t) - 2 * Math.cos(3 * t) - Math.cos(4 * t);
          const particle = document.createElement('i'); particle.className = 'heart-particle';
          particle.style.setProperty('--x', `${x * 5}px`);
          particle.style.setProperty('--y', `${-y * 5}px`);
          particle.style.setProperty('--dx', `${(Math.random() - .5) * (smallScreen ? 260 : 520)}px`);
          particle.style.setProperty('--dy', `${(Math.random() - .5) * (smallScreen ? 300 : 540)}px`);
          particle.style.setProperty('--delay', `${Math.random() * .65}s`);
          heartFormation.appendChild(particle);
        }
        endingParticlesBuilt = true;
      }
      function showEndingPanel(panel) {
        panel.classList.remove('is-leaving');
        panel.classList.add('visible');
      }
      function hideEndingPanel(panel) {
        panel.classList.remove('visible');
        panel.classList.add('is-leaving');
      }
      function startCinematicEnding() {
        if (endingStarted) return;
        endingStarted = true;
        if (!endingParticlesBuilt) buildEndingParticles();
        document.body.classList.add('cinematic-active');
        cinematicEnding.classList.add('active');
        cinematicEnding.setAttribute('aria-hidden', 'false');
        const moments = reduceMotion
          ? [[0, () => showEndingPanel(endingReveal)], [1200, () => { hideEndingPanel(endingReveal); heartFormation.classList.add('visible', 'pulse'); }], [3500, () => heartFormation.classList.add('scattered')], [5000, () => showEndingPanel(endingFinalCopy)], [8000, () => { hideEndingPanel(endingFinalCopy); showEndingPanel(endingSignature); }], [11500, () => { hideEndingPanel(endingSignature); showFinalScreen(); }]]
          : [[1000, () => showEndingPanel(endingReveal)], [5200, () => { hideEndingPanel(endingReveal); heartFormation.classList.add('visible', 'pulse'); }], [8000, () => heartFormation.classList.add('scattered')], [10600, () => { heartFormation.classList.remove('pulse'); showEndingPanel(endingFinalCopy); }], [13200, () => { hideEndingPanel(endingFinalCopy); showEndingPanel(endingSignature); }], [17000, () => { hideEndingPanel(endingSignature); showFinalScreen(); }]];
        moments.forEach(([delay, callback]) => endingTimers.push(window.setTimeout(callback, delay)));
      }
      function showFinalScreen() {
        document.body.classList.add('ending-finale');
        showEndingPanel(finalScreen);
      }
      function resetFromEnding() {
        endingTimers.forEach(window.clearTimeout); endingTimers = [];
        endingStarted = false;
        cinematicEnding.classList.remove('active');
        cinematicEnding.setAttribute('aria-hidden', 'true');
        document.body.classList.remove('ending-finale', 'cinematic-active');
        endingReveal.classList.remove('visible', 'is-leaving');
        heartFormation.classList.remove('visible', 'pulse', 'scattered');
        endingFinalCopy.classList.remove('visible', 'is-leaving');
        endingSignature.classList.remove('visible', 'is-leaving');
        finalScreen.classList.remove('visible', 'is-leaving');
        resetToOpening();
      }
      function next() {
        if (endingStarted) return;
        if (currentPage === 0 && !opened) openLetter();
        else if (currentPage === pages.length - 1) startCinematicEnding();
        else renderPage(currentPage + 1, 1);
      }
      function previous() { if (!endingStarted) renderPage(Math.max(currentPage - 1, 0), -1); }
      function resetToOpening() {
        opened = false;
        envelope.classList.remove('open');
        openButton.disabled = false;
        renderPage(0, -1);
      }
      function openLetter() {
        if (opened) { renderPage(1, 1); return; }
        opened = true;
        openButton.disabled = true;
        envelope.classList.add('open');
        window.setTimeout(() => renderPage(1, 1), reduceMotion ? 10 : 470);
      }
      openButton.addEventListener('click', openLetter);
      nextButton.addEventListener('click', next);
      previousButton.addEventListener('click', previous);
      readAgain.addEventListener('click', resetToOpening);
      endingReadAgain.addEventListener('click', resetFromEnding);
      document.addEventListener('keydown', event => {
        if (event.altKey || event.ctrlKey || event.metaKey) return;
        if (event.key === 'ArrowRight' || event.key === 'PageDown') { event.preventDefault(); next(); }
        if (event.key === 'ArrowLeft' || event.key === 'PageUp') { event.preventDefault(); previous(); }
        if (event.key === 'Home') { event.preventDefault(); if (endingStarted) resetFromEnding(); else if (currentPage !== 0) resetToOpening(); }
      });
      const presentation = document.getElementById('presentation');
      presentation.addEventListener('touchstart', event => { touchStartX = event.changedTouches[0].clientX; touchStartY = event.changedTouches[0].clientY; }, { passive: true });
      presentation.addEventListener('touchend', event => {
        const dx = event.changedTouches[0].clientX - touchStartX;
        const dy = event.changedTouches[0].clientY - touchStartY;
        if (Math.abs(dx) > 55 && Math.abs(dx) > Math.abs(dy) * 1.25) dx < 0 ? next() : previous();
      }, { passive: true });

      const musicToggle = document.getElementById('musicToggle');
      const musicLabel = document.getElementById('musicLabel');
      const muteToggle = document.getElementById('muteToggle');
      const volumeControl = document.getElementById('volume');
      let audioContext = null, masterGain = null, musicOn = false, muted = false, noteTimer = null, noteIndex = 0;
      const notes = [220, 261.63, 329.63, 293.66, 196, 246.94, 293.66, 261.63];
      function playNote() {
        if (!musicOn || !audioContext || audioContext.state !== 'running') return;
        const now = audioContext.currentTime, fundamental = notes[noteIndex++ % notes.length];
        [fundamental, fundamental * 1.5].forEach((frequency, index) => {
          const oscillator = audioContext.createOscillator(), gain = audioContext.createGain();
          oscillator.type = 'sine'; oscillator.frequency.value = frequency;
          gain.gain.setValueAtTime(.0001, now); gain.gain.exponentialRampToValueAtTime(index ? .012 : .024, now + 1.2);
          gain.gain.exponentialRampToValueAtTime(.0001, now + 4.1); oscillator.connect(gain).connect(masterGain);
          oscillator.start(now); oscillator.stop(now + 4.2);
        });
      }
      function updateAudioLevel() {
        if (masterGain && audioContext) masterGain.gain.setTargetAtTime(muted ? 0 : Number(volumeControl.value) / 100 * .22, audioContext.currentTime, .12);
        muteToggle.textContent = muted ? '◖̸' : '◖';
        muteToggle.setAttribute('aria-pressed', String(muted));
        muteToggle.setAttribute('aria-label', muted ? 'Nyalakan suara' : 'Matikan suara');
      }
      musicToggle.addEventListener('click', async () => {
        if (musicOn) {
          musicOn = false; window.clearInterval(noteTimer);
          if (audioContext && audioContext.state === 'running') await audioContext.suspend();
        } else {
          const AudioContextClass = window.AudioContext || window.webkitAudioContext;
          if (!AudioContextClass) { musicLabel.textContent = 'Unavailable'; musicToggle.disabled = true; return; }
          if (!audioContext) { audioContext = new AudioContextClass(); masterGain = audioContext.createGain(); masterGain.connect(audioContext.destination); }
          await audioContext.resume(); musicOn = true; updateAudioLevel(); playNote(); noteTimer = window.setInterval(playNote, 3300);
        }
        musicLabel.textContent = musicOn ? 'Pause' : 'Play';
        musicToggle.setAttribute('aria-pressed', String(musicOn));
        musicToggle.setAttribute('aria-label', musicOn ? 'Jeda musik ambient' : 'Putar musik ambient');
      });
      muteToggle.addEventListener('click', () => { muted = !muted; updateAudioLevel(); });
      volumeControl.addEventListener('input', updateAudioLevel);
    })();
  </script>
</body>
</html>
