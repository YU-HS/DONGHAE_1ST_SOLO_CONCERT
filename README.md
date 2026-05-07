<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SUPER JUNIOR D&E 應援口號 ・ FANCHANT GUIDE</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Cormorant+Garamond:ital,wght@0,400;0,600;1,400&family=Noto+Sans+TC:wght@300;400;500;700;900&family=Noto+Serif+TC:wght@400;700&family=Space+Grotesk:wght@400;700&display=swap" rel="stylesheet">
<style>
  :root{
    --sapphire:#1e4ec8;
    --sapphire-deep:#0d1f5c;
    --sapphire-glow:#4d7dff;
    --pearl:#a8c5ff;
    --ink:#05060f;
    --ink-soft:#0c0f25;
    --paper:#f4f1ea;
    --hot:#ff3a82;          /* 跟唱 / vocal echo */
    --gold:#ffcc4d;          /* 應援詞 / fanchant */
    --kor:#e8ecff;
    --muted:#7a86b8;
  }

  *{box-sizing:border-box;margin:0;padding:0}
  html{scroll-behavior:smooth}

  body{
    font-family:'Noto Sans TC',sans-serif;
    background:var(--ink);
    color:#dde3ff;
    line-height:1.85;
    overflow-x:hidden;
    -webkit-font-smoothing:antialiased;
  }

  /* ===== 背景：演唱會星空感 ===== */
  body::before{
    content:'';
    position:fixed;inset:0;
    background:
      radial-gradient(ellipse at 20% 0%, rgba(77,125,255,.18), transparent 50%),
      radial-gradient(ellipse at 80% 100%, rgba(30,78,200,.22), transparent 55%),
      radial-gradient(ellipse at 50% 50%, rgba(255,58,130,.05), transparent 70%);
    pointer-events:none;z-index:0;
  }
  body::after{
    content:'';
    position:fixed;inset:0;
    background-image:
      radial-gradient(1px 1px at 20% 30%, #fff, transparent),
      radial-gradient(1px 1px at 60% 70%, var(--pearl), transparent),
      radial-gradient(1px 1px at 80% 20%, #fff, transparent),
      radial-gradient(2px 2px at 30% 80%, var(--sapphire-glow), transparent),
      radial-gradient(1px 1px at 90% 60%, #fff, transparent),
      radial-gradient(1px 1px at 10% 90%, var(--pearl), transparent);
    background-size:550px 550px;
    opacity:.4;
    pointer-events:none;z-index:0;
    animation:twinkle 8s ease-in-out infinite alternate;
  }
  @keyframes twinkle{
    from{opacity:.25}
    to{opacity:.55}
  }

  /* ===== HERO ===== */
  .hero{
    position:relative;z-index:2;
    min-height:92vh;
    display:flex;flex-direction:column;justify-content:center;align-items:center;
    padding:80px 24px 60px;
    text-align:center;
    border-bottom:1px solid rgba(168,197,255,.15);
  }
  .hero-tag{
    font-family:'Space Grotesk',sans-serif;
    letter-spacing:.4em;
    font-size:11px;
    color:var(--pearl);
    text-transform:uppercase;
    margin-bottom:32px;
    opacity:.8;
  }
  .hero-tag::before,.hero-tag::after{
    content:'◆';margin:0 14px;color:var(--sapphire-glow);
  }
  .hero h1{
    font-family:'Bebas Neue',sans-serif;
    font-size:clamp(58px,12vw,150px);
    line-height:.92;
    letter-spacing:.02em;
    color:#fff;
    margin-bottom:14px;
    text-shadow:0 0 60px rgba(77,125,255,.4);
  }
  .hero h1 .amp{
    color:var(--hot);
    font-style:italic;
    display:inline-block;
    transform:translateY(-4px) rotate(-6deg);
    margin:0 4px;
  }
  .hero-sub{
    font-family:'Cormorant Garamond',serif;
    font-style:italic;
    font-size:clamp(18px,3vw,26px);
    color:var(--pearl);
    margin-bottom:8px;
    letter-spacing:.05em;
  }
  .hero-zh{
    font-family:'Noto Serif TC',serif;
    font-size:clamp(15px,2.2vw,18px);
    color:#dde3ff;
    margin-bottom:48px;
  }

  /* ===== Color Legend ===== */
  .legend{
    display:flex;flex-wrap:wrap;justify-content:center;gap:14px;
    max-width:780px;margin:0 auto 36px;
    padding:24px;
    border:1px solid rgba(168,197,255,.18);
    border-radius:4px;
    background:rgba(13,31,92,.18);
    backdrop-filter:blur(10px);
  }
  .legend-title{
    width:100%;
    font-family:'Space Grotesk',sans-serif;
    font-size:11px;letter-spacing:.3em;
    color:var(--muted);
    text-transform:uppercase;
    margin-bottom:6px;
  }
  .legend-item{
    display:flex;align-items:center;gap:10px;
    font-size:13px;
  }
  .legend-dot{
    width:14px;height:14px;border-radius:50%;
    box-shadow:0 0 12px currentColor;
  }
  .legend-item.vocal .legend-dot{background:var(--hot);color:var(--hot)}
  .legend-item.cheer .legend-dot{background:var(--gold);color:var(--gold)}
  .legend-item.kor .legend-dot{background:var(--kor);color:var(--kor)}

  /* ===== Note ===== */
  .note{
    max-width:680px;
    text-align:left;
    font-size:14px;color:#bcc7f0;
    padding:20px 24px;
    border-left:3px solid var(--gold);
    background:rgba(255,204,77,.06);
    margin:0 auto;
  }
  .note strong{color:var(--gold);font-weight:700}

  /* ===== Sticky Navigation ===== */
  .nav{
    position:sticky;top:0;z-index:50;
    background:rgba(5,6,15,.92);
    backdrop-filter:blur(20px);
    border-bottom:1px solid rgba(168,197,255,.18);
    padding:14px 0;
  }
  .nav-inner{
    display:flex;gap:8px;
    overflow-x:auto;
    padding:0 24px;
    scrollbar-width:none;
    max-width:1100px;margin:0 auto;
  }
  .nav-inner::-webkit-scrollbar{display:none}
  .nav-btn{
    flex:0 0 auto;
    background:transparent;
    border:1px solid rgba(168,197,255,.25);
    color:#dde3ff;
    padding:10px 18px;
    font-family:'Noto Sans TC',sans-serif;
    font-size:13px;font-weight:500;
    letter-spacing:.05em;
    border-radius:999px;
    cursor:pointer;
    transition:all .25s ease;
    white-space:nowrap;
  }
  .nav-btn:hover{
    border-color:var(--sapphire-glow);
    color:#fff;
    background:rgba(77,125,255,.1);
  }
  .nav-btn.active{
    background:var(--sapphire);
    border-color:var(--sapphire-glow);
    color:#fff;
    box-shadow:0 0 20px rgba(77,125,255,.5);
  }

  /* ===== Main Content ===== */
  main{
    position:relative;z-index:2;
    max-width:820px;
    margin:0 auto;
    padding:60px 24px 120px;
  }

  .song{
    display:none;
    animation:fadeIn .5s ease;
  }
  .song.active{display:block}
  @keyframes fadeIn{
    from{opacity:0;transform:translateY(20px)}
    to{opacity:1;transform:translateY(0)}
  }

  .song-header{
    margin-bottom:48px;
    padding-bottom:28px;
    border-bottom:1px solid rgba(168,197,255,.18);
    position:relative;
  }
  .song-num{
    font-family:'Bebas Neue',sans-serif;
    font-size:14px;
    letter-spacing:.4em;
    color:var(--sapphire-glow);
    margin-bottom:12px;
  }
  .song-title{
    font-family:'Bebas Neue',sans-serif;
    font-size:clamp(44px,8vw,82px);
    line-height:1;
    color:#fff;
    margin-bottom:8px;
    letter-spacing:.01em;
  }
  .song-subtitle{
    font-family:'Cormorant Garamond',serif;
    font-style:italic;
    font-size:18px;
    color:var(--pearl);
  }

  /* ===== Lyrics Block ===== */
  .lyrics{
    font-size:16px;
    line-height:2.1;
    letter-spacing:.01em;
  }
  .lyrics p{
    margin-bottom:1.4em;
    color:#cfd6f5;
  }
  .lyrics .stanza{
    padding:18px 22px;
    margin-bottom:24px;
    background:rgba(13,31,92,.25);
    border-left:2px solid rgba(77,125,255,.4);
    border-radius:2px;
    transition:border-color .3s ease;
  }
  .lyrics .stanza:hover{
    border-left-color:var(--sapphire-glow);
    background:rgba(13,31,92,.4);
  }
  .lyrics .kor{color:var(--kor);font-weight:400}
  .lyrics .vocal{
    color:var(--hot);
    font-weight:500;
    background:rgba(255,58,130,.08);
    padding:1px 6px;
    border-radius:3px;
  }
  .lyrics .cheer{
    color:var(--gold);
    font-weight:700;
    background:rgba(255,204,77,.1);
    padding:1px 6px;
    border-radius:3px;
    letter-spacing:.05em;
  }
  .lyrics .pron{
    color:var(--pearl);
    font-size:14px;
    font-style:italic;
    opacity:.8;
  }
  .lyrics .label{
    display:inline-block;
    font-family:'Space Grotesk',sans-serif;
    font-size:10px;
    font-weight:700;
    letter-spacing:.2em;
    text-transform:uppercase;
    padding:3px 9px;
    border-radius:3px;
    margin-right:8px;
    vertical-align:middle;
  }
  .lyrics .label.intro{background:var(--sapphire);color:#fff}
  .lyrics .label.chorus{background:var(--hot);color:#fff}
  .lyrics .label.bridge{background:var(--gold);color:var(--ink)}
  .lyrics .label.outro{background:rgba(168,197,255,.3);color:#fff}

  /* ===== Video Toggle ===== */
  .video-section{
    margin-bottom:40px;
    border:1px solid rgba(168,197,255,.2);
    border-radius:6px;
    background:linear-gradient(180deg, rgba(13,31,92,.3), rgba(13,31,92,.1));
    overflow:hidden;
  }
  .video-toggle{
    width:100%;
    background:transparent;
    border:none;
    color:#fff;
    padding:16px 20px;
    display:flex;align-items:center;justify-content:space-between;
    cursor:pointer;
    font-family:'Noto Sans TC',sans-serif;
    font-size:14px;font-weight:500;
    letter-spacing:.05em;
    transition:background .25s ease;
  }
  .video-toggle:hover{
    background:rgba(77,125,255,.1);
  }
  .video-toggle-left{
    display:flex;align-items:center;gap:12px;
  }
  .video-icon{
    width:32px;height:32px;
    display:flex;align-items:center;justify-content:center;
    background:var(--hot);
    border-radius:50%;
    font-size:11px;
    color:#fff;
    box-shadow:0 0 14px rgba(255,58,130,.5);
  }
  .video-label{
    font-family:'Space Grotesk',sans-serif;
    font-size:11px;
    letter-spacing:.3em;
    text-transform:uppercase;
    color:var(--pearl);
    display:block;
    margin-bottom:2px;
  }
  .video-title{
    font-size:14px;
    color:#fff;
    font-weight:500;
  }
  .video-arrow{
    color:var(--sapphire-glow);
    font-size:18px;
    transition:transform .3s ease;
  }
  .video-section.open .video-arrow{
    transform:rotate(180deg);
  }
  .video-content{
    max-height:0;
    overflow:hidden;
    transition:max-height .4s ease;
  }
  .video-section.open .video-content{
    max-height:3000px;
  }
  .video-grid{
    padding:0 20px 24px;
    display:grid;
    gap:20px;
  }
  .video-item{
    display:flex;flex-direction:column;
  }
  .video-tag{
    display:inline-flex;align-items:center;gap:6px;
    align-self:flex-start;
    font-family:'Space Grotesk',sans-serif;
    font-size:10px;
    letter-spacing:.2em;
    text-transform:uppercase;
    padding:4px 10px;
    border-radius:3px;
    margin-bottom:10px;
    font-weight:700;
  }
  .video-tag.youtube{background:rgba(255,58,130,.15);color:var(--hot);border:1px solid rgba(255,58,130,.3)}
  .video-tag.instagram{
    background:linear-gradient(45deg, rgba(255,58,130,.15), rgba(255,204,77,.15));
    color:#ff8db5;
    border:1px solid rgba(255,58,130,.3);
  }
  .video-iframe-wrap{
    position:relative;
    width:100%;
    padding-bottom:56.25%;
    background:#000;
    border-radius:4px;
    overflow:hidden;
  }
  .video-iframe-wrap iframe{
    position:absolute;
    top:0;left:0;
    width:100%;height:100%;
    border:none;
  }
  /* IG 卡片 */
  .ig-card{
    display:flex;align-items:center;gap:16px;
    padding:18px;
    background:linear-gradient(135deg, rgba(255,58,130,.1), rgba(77,125,255,.08));
    border:1px solid rgba(255,58,130,.25);
    border-radius:6px;
    text-decoration:none;
    color:#fff;
    transition:all .3s ease;
  }
  .ig-card:hover{
    transform:translateY(-2px);
    border-color:var(--hot);
    box-shadow:0 8px 24px rgba(255,58,130,.2);
  }
  .ig-icon-wrap{
    width:48px;height:48px;
    flex-shrink:0;
    display:flex;align-items:center;justify-content:center;
    background:linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888);
    border-radius:12px;
    color:#fff;
    font-size:22px;
  }
  .ig-text{flex:1;min-width:0}
  .ig-handle{
    font-family:'Space Grotesk',sans-serif;
    font-size:12px;
    color:var(--pearl);
    margin-bottom:2px;
  }
  .ig-desc{
    font-size:14px;
    color:#fff;
  }
  .ig-arrow{
    color:var(--sapphire-glow);
    font-size:20px;
  }

  /* ELF 專屬分頁樣式 */
  .elf-only{
    text-align:center;
    padding:40px 0;
  }
  .elf-only .video-section{
    text-align:left;
    max-width:100%;
  }
  .elf-intro{
    font-family:'Cormorant Garamond',serif;
    font-style:italic;
    font-size:18px;
    color:var(--pearl);
    margin-bottom:32px;
    line-height:1.8;
  }

  /* ===== Footer ===== */
  footer{
    position:relative;z-index:2;
    text-align:center;
    padding:48px 24px;
    border-top:1px solid rgba(168,197,255,.15);
    color:var(--muted);
    font-size:13px;
    line-height:2;
  }
  footer .heart{color:var(--hot)}
  footer .bracket{color:var(--sapphire-glow);font-family:'Bebas Neue',sans-serif;letter-spacing:.3em;font-size:11px}

  /* ===== Back to top ===== */
  .top-btn{
    position:fixed;
    bottom:24px;right:24px;
    width:48px;height:48px;
    border-radius:50%;
    background:var(--sapphire);
    border:1px solid var(--sapphire-glow);
    color:#fff;
    font-size:20px;
    cursor:pointer;
    z-index:60;
    display:none;
    align-items:center;justify-content:center;
    box-shadow:0 4px 20px rgba(30,78,200,.5);
    transition:all .3s ease;
  }
  .top-btn:hover{transform:translateY(-3px);box-shadow:0 6px 25px rgba(77,125,255,.7)}
  .top-btn.show{display:flex}

  /* ===== Mobile ===== */
  @media (max-width:640px){
    .hero{min-height:80vh;padding:60px 20px 40px}
    .legend{gap:10px;padding:18px}
    .legend-item{font-size:12px}
    main{padding:40px 18px 100px}
    .lyrics{font-size:15px;line-height:2}
    .lyrics .stanza{padding:14px 16px}
    .nav-btn{padding:8px 14px;font-size:12px}
  }
</style>
</head>
<body>

<section class="hero">
  <div class="hero-tag">FANCHANT GUIDE ・ TWELF EDITION</div>
  <h1>D <span class="amp">&amp;</span> E</h1>
  <div class="hero-sub">Super Junior — Donghae & Eunhyuk</div>
  <div class="hero-zh">應 援 口 號 整 理</div>

  <div class="legend">
    <div class="legend-title">— 顏色說明 / Color Guide —</div>
    <div class="legend-item kor"><span class="legend-dot"></span><span>韓文歌詞 / Lyrics</span></div>
    <div class="legend-item vocal"><span class="legend-dot"></span><span>跟唱 / 跟唸 Sing-along</span></div>
    <div class="legend-item cheer"><span class="legend-dot"></span><span>應援詞 Fanchant</span></div>
  </div>

  <div class="note">
    🔔 <strong>注意事項</strong>　以下內容為轉載自網路資源整理影片，希望能協助 E.L.F. / & (애니) 多多熟悉應援口號，一起加油！部分曲目將依首爾場曲目持續更新。來源請見原影片發佈者。
  </div>
</section>

<nav class="nav" id="nav">
  <div class="nav-inner" id="navInner">
    <button class="nav-btn active" data-target="song-haetnae">해 떴네</button>
    <button class="nav-btn" data-target="song-ggb">GGB 지지배</button>
    <button class="nav-btn" data-target="song-bout">'Bout You</button>
    <button class="nav-btn" data-target="song-oppa">Oppa Oppa</button>
    <button class="nav-btn" data-target="song-cali">California Love</button>
    <button class="nav-btn" data-target="song-perfect">太完美</button>
    <button class="nav-btn" data-target="song-elf">我們是 E.L.F.</button>
  </div>
</nav>

<main>

  <!-- ===== 해 떴네 ===== -->
  <article class="song active" id="song-haetnae">
    <div class="song-header">
      <div class="song-num">TRACK 01 / SOLO DEBUT</div>
      <h1 class="song-title">해 떴네</h1>
      <div class="song-subtitle">The Sun Has Risen — 李東海 LEE DONG HAE</div>
    </div>

    <div class="lyrics">
      <p class="stanza"><span class="label intro">INTRO</span><br>
        <span class="cheer">(이! 동! 해! 눈! 이! 부! 시! 게! 도!)</span><br>
        <span class="cheer">(Lee! Dong! Hae! 怒! 尼! 步! 細! 給! 豆!)</span>
      </p>

      <p class="stanza">
        해 떴네 uh<br>
        해 떴네 uh<br>
        해 떴네 uh (From me Aye)<br>
        I'm living high high 해 떴네 uh<br>
        (What you want from me)
      </p>

      <p class="stanza">
        Congratulations 이기는 습관이 뱄어<br>
        제대로 물려받은 Passion<br>
        예술가 집안에선 당연한 Question<br>
        Don't stop me now 건들지 마
      </p>

      <p class="stanza">
        급이 달라 너와 달리<br>
        Mic check 귀찮아 Mumbling<br>
        가지마 가지마 하지마 하지마<br>
        이게 내 스타일 <span class="pron">(一給 內 Style)</span>
      </p>

      <p class="stanza">
        골 때리는 Kick-Kick Chak-Chak Freaky<br>
        리듬 감아서 차 Kickflip<br>
        심장 울리는 Bassline<br>
        리듬 따라가 Stalking
      </p>

      <p class="stanza">
        다리 떨어 Day and night 혈액순환<br>
        뒷 박에 Groove 따라서 나와<br>
        남자다운 척 Love or die<br>
        리듬에 Perfume Chik-Chik
      </p>

      <p class="stanza">
        You don't know <span class="vocal">(함성)</span><span class="vocal">(歡呼!)</span><br>
        Too bad untouchable<br>
        해 뜨고 나면 눈부셔 Brand new <span class="cheer">(이!동!해떴네!)</span> <span class="cheer">(Lee! Dong! 嘿豆內!)</span><br>
        해 떴네 uh
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        해 떴네 uh<br>
        눈이 부시게도 해 떴네 (What you want from me)<br>
        I'm living 구름 위 위에 해 떴네 (From me Aye)<br>
        I'm living high high 해 떴네<br>
        What you want from me Aye
      </p>

      <p class="stanza">
        살다가 보니 해 떴네 <span class="cheer">(이!동!해!)</span> <span class="cheer">(Lee! Dong! Hae!)</span><br>
        (Want you my right by my side)<br>
        눈이 부시게도 해 떴네<br>
        (Want you my right by my side love)<br>
        어둠은 사라지고 해 떴네 <span class="cheer">(해!떴!네!)</span> <span class="cheer">(嘿!豆!內!)</span><br>
        (Want you my right by my side)<br>
        저기 막 떴네<br>
        What you want from me Aye<br>
        해 떴네 uh
      </p>

      <p class="stanza">
        Take me to the sky <span class="vocal">(함성)</span><span class="vocal">(歡呼!)</span><br>
        I'm still alive a life<br>
        Nobody can drag me down<br>
        충분해 Beautiful day
      </p>

      <p class="stanza">
        Take me to your heart<br>
        눈을 맞추고<br>
        Pull me Close up<br>
        Yeah I've been losing my mind
      </p>

      <p class="stanza">
        Too bad untouchable<br>
        해 뜨고 나면 눈부셔 Brand new<br>
        Too bad untouchable<br>
        다리 떨어 <span class="pron">(多摟)</span> 폼 나게 걸어 <span class="pron">(勾摟)</span>
      </p>

      <p class="stanza">
        눈 감고 폼 나게 뛰어 버려<br>
        화끈하게 들어와 Skydive<br>
        뛰어 버려 패기 하나 걸치고 낙하<br>
        필요 없는 Parachute
      </p>

      <p class="stanza">
        해 떴네 uh <span class="pron">(嘿豆內 uh)</span>
      </p>

      <p class="stanza"><span class="label chorus">FINAL CHORUS</span><br>
        해 떴네 uh<br>
        눈이 부시게도 해 떴네 (What you want from me)<br>
        I'm living 구름 위 위에 해 떴네 (From me Aye)<br>
        I'm living high high 해 떴네<br>
        What you want from me Aye
      </p>

      <p class="stanza">
        살다가 보니 해 떴네 <span class="cheer">(이!동!해!)</span> <span class="cheer">(Lee! Dong! Hae!)</span><br>
        (Want you my right by my side)<br>
        눈이 부시게도 해 떴네 <span class="cheer">(솔!로!데!뷔!)</span> <span class="cheer">(SO! LO! DE! 必!)</span><br>
        (Want you my right by my side love)<br>
        어둠은 사라지고 해 떴네 <span class="cheer">(해!떴!네!)</span> <span class="cheer">(嘿豆內!)</span><br>
        (Want you my right by my side)<br>
        저기 막 떴네<br>
        What you want from me Aye<br>
        해 떴네 uh
      </p>

      <p style="text-align:center;color:var(--muted);font-size:13px;font-style:italic;margin-top:48px;letter-spacing:.1em;">
        ─── 以下會再依照首爾場曲目更新 ───
      </p>
    </div>
  </article>

  <!-- ===== GGB ===== -->
  <article class="song" id="song-ggb">
    <div class="song-header">
      <div class="song-num">TRACK 02 / D&E TWELF</div>
      <h1 class="song-title">GGB 지지배</h1>
      <div class="song-subtitle">D&E 應援口號教學</div>
    </div>

    <div class="video-section">
      <button class="video-toggle" onclick="toggleVideo(this)">
        <div class="video-toggle-left">
          <div class="video-icon">▶</div>
          <div>
            <span class="video-label">應援教學影片</span>
            <span class="video-title">Watch Tutorial</span>
          </div>
        </div>
        <span class="video-arrow">▼</span>
      </button>
      <div class="video-content">
        <div class="video-grid">
          <div class="video-item">
            <span class="video-tag youtube">▶ YouTube ・ 應援教學</span>
            <div class="video-iframe-wrap">
              <iframe src="https://www.youtube.com/embed/zw-S3wILmMU" title="GGB 응원법 教學" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="lyrics">
      <p class="stanza"><span class="label intro">INTRO</span> SUPER JUNIOR D&E GO</p>

      <p class="stanza">
        계절이 지나 또 다른 온도 <span class="vocal">(다른 온도)</span> <span class="pron">(搭愣翁豆)</span><br>
        여전히 마음은 네게 가 있어 <span class="vocal">(가 있어)</span> <span class="pron">(嘎以搜)</span><br>
        너와 내가 머물던 지난 timeline<br>
        어떻게 내가 잊겠어 나 혼자 여기서<br>
        Yeah 어떻게 지내니?
      </p>

      <p class="stanza">
        나는 혼자 잘 지냈어 <span class="vocal">(혼자 잘 지냈어)</span> <span class="pron">(紅家 才 及內搜)</span><br>
        문득 네 생각에 살짝 정신이 나갔어 <span class="vocal">(정신이 나갔어)</span> <span class="pron">(窮星尼 那嘎搜)</span><br>
        네가 없는 이곳에 oasis는 없어 (Hey, Hey)<br>
        며칠째 목말라 절레절레 내려줘 단비
      </p>

      <p class="stanza">
        우리 그때의 <span class="pron">(嗚利 苦得誒)</span> Memory<br>
        더 늦기 전에 <span class="pron">(偷 ne gi 秋內)</span> I'm sorry
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        네가 있는 곳은 어디 <span class="vocal">(어디)</span> <span class="pron">(歐低)</span><br>
        날 데려가 줘 빨리 <span class="vocal">(빨리)</span> <span class="pron">(八力)</span><br>
        좀 벗어나자 둘이 <span class="vocal">(둘이)</span> <span class="pron">(杜力)</span><br>
        내 손 잡아 We can fly
      </p>

      <p class="stanza">
        네 생각에 불 켜는 밤 <span class="vocal">(이 밤에)</span> <span class="pron">(以半美)</span><br>
        끝을 몰라 뒤척이는 나 (So lonely)<br>
        너 없이도 잘 돌아가는 밤 <span class="vocal">(밤, 밤)</span> <span class="pron">(邦邦)</span><br>
        좀 슬퍼도 어쩌겠어 지켜볼게 멀리서
      </p>

      <p class="stanza">
        너무 예쁜 입술에 <span class="vocal">(입 맞추던 네 모습에)</span> <span class="pron">(衣嘛 秋登 內某素杯)</span><br>
        같이 보던 무지개 <span class="vocal">(무지개 같은 입술에)</span> <span class="pron">(木吉給 嘎登 衣素內)</span><br>
        떠나간 네 모습에 <span class="vocal">(모습 Bae Bae)</span> <span class="pron">(某素杯杯)</span><br>
        좀 슬퍼도 어쩌겠어 지켜볼게 멀리서
      </p>

      <p class="stanza">
        아직도<br>
        넌 나만의 bucket list<br>
        매일 같이 듣던 음악은 아직 playlist에<br>
        우리 story의 장르는 romance가 아냐<br>
        Fantasy가 섞인 action<br>
        복잡한 scenario
      </p>

      <p class="stanza">
        딴 생각 안 나 I'm fallin' (fallin')<br>
        너와 같이 있는 love story (story)<br>
        잊지 못해 널 기다리고 있어
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        네가 있는 곳은 어디 <span class="vocal">(어디)</span> <span class="pron">(歐低)</span><br>
        날 데려가 줘 빨리 <span class="vocal">(빨리)</span> <span class="pron">(八力)</span><br>
        좀 벗어나자 둘이 <span class="vocal">(둘이)</span> <span class="pron">(杜力)</span><br>
        내 손 잡아 We can fly
      </p>

      <p class="stanza">
        네 생각에 불 켜는 밤 <span class="vocal">(이 밤에)</span> <span class="pron">(以半美)</span><br>
        끝을 몰라 뒤척이는 나 (So lonely)<br>
        너 없이도 잘 돌아가는 밤 <span class="vocal">(밤, 밤)</span> <span class="pron">(邦邦)</span>
      </p>

      <p class="stanza">
        너무 예쁜 입술에 <span class="vocal">(입 맞추던 네 모습에)</span> <span class="pron">(衣嘛 秋登 內某素杯)</span><br>
        같이 보던 무지개 <span class="vocal">(무지개 같은 입술에)</span> <span class="pron">(木吉給 嘎登 衣素內)</span><br>
        떠나 간네 모습에 <span class="vocal">(모습 Bae Bae)</span> <span class="pron">(某素杯杯)</span><br>
        좀 슬퍼도 어쩌겠어 지켜볼게 멀리서
      </p>

      <p class="stanza">
        계절이 지나 또 다른 온도 <span class="vocal">(다른 온도)</span> <span class="pron">(搭愣翁豆)</span><br>
        여전히 마음은 네게 가 있어 <span class="vocal">(가 있어)</span> <span class="pron">(嘎以搜)</span><br>
        네가 있는 곳은 어디 <span class="vocal">(어디)</span> <span class="pron">(歐低)</span><br>
        날 데려가 줘 빨리 <span class="vocal">(빨리)</span> <span class="pron">(八力)</span><br>
        좀 벗어나자 둘이 <span class="vocal">(둘이)</span> <span class="pron">(杜力)</span><br>
        내 손 잡아 We can fly<br>
        <span class="cheer">D&E GO!</span>
      </p>

      <p class="stanza"><span class="label bridge">BRIDGE</span><br>
        잠시 머물러간 사랑이었나?<br>
        우리 인연 여기까지였나?<br>
        그 예쁜 미소 다신 볼 수는 없나? Yeah<br>
        외로운 내 맘에 잠깐 와줄 순 없나
      </p>

      <p class="stanza">
        너무 예쁜 입술에 <span class="vocal">(입 맞추던 네 모습에)</span> <span class="pron">(衣嘛 秋登 內某素杯)</span><br>
        같이 보던 무지개 <span class="vocal">(무지개 같은 입술에)</span> <span class="pron">(木吉給 嘎登 衣素內)</span><br>
        떠나 간네 모습에 <span class="vocal">(모습 Bae Bae)</span> <span class="pron">(某素杯杯)</span><br>
        좀 슬퍼도 어쩌겠어 지켜볼게 멀리서
      </p>
    </div>
  </article>

  <!-- ===== 'Bout You ===== -->
  <article class="song" id="song-bout">
    <div class="song-header">
      <div class="song-num">TRACK 03 / D&E</div>
      <h1 class="song-title">'Bout You</h1>
      <div class="song-subtitle">SUPER JUNIOR D&E — All About You</div>
    </div>

    <div class="video-section">
      <button class="video-toggle" onclick="toggleVideo(this)">
        <div class="video-toggle-left">
          <div class="video-icon">▶</div>
          <div>
            <span class="video-label">應援教學影片</span>
            <span class="video-title">Watch Tutorial</span>
          </div>
        </div>
        <span class="video-arrow">▼</span>
      </button>
      <div class="video-content">
        <div class="video-grid">
          <div class="video-item">
            <span class="video-tag youtube">▶ YouTube ・ 應援教學</span>
            <div class="video-iframe-wrap">
              <iframe src="https://www.youtube.com/embed/lsey0aJlOI4" title="'Bout You 應援教學" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="lyrics">
      <p class="stanza"><span class="label intro">INTRO</span><br>
        登登登登~登登登 <span class="cheer">(SU! PER! JUNI! OR! D! N! E!)</span>
      </p>

      <p class="stanza">
        머리부터 발끝까지 <span class="cheer">【이 동 해】</span> <span class="pron">(Lee Dong Hae)</span><br>
        너무 내게 눈이 부셔 <span class="cheer">【이 혁 재】</span> <span class="pron">(Lee Hyuk Jae)</span>
      </p>

      <p class="stanza">
        넌 참 짜릿짜릿해 가끔은 또 여리여리해<br>
        시간이 갈수록 더 난 달려 너라는 방향의 Road<br>
        북적북적한 거리 <span class="pron">(摳哩)</span> 같이 걸어볼까 우리 <span class="pron">(巫哩)</span><br>
        난 네가 좋다면 Yeah 그 어디든 갈 수 있어
      </p>

      <p class="stanza">
        내 맘을 전부 설명할 수 조차 없어<br>
        그냥 하는 말이 아니야<br>
        너만 떠오르는 거야 Yeah<br>
        I want to know you, Just all about you<br>
        이유는 묻지 마 내게 그냥 답은 너야 <span class="pron">(NO呀)</span>
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        머리부터 발끝까지 <span class="vocal">(Wow Wow Wow Wow)</span><br>
        너무 내게 눈이 부셔 <span class="vocal">(Sha La La La)</span><br>
        너는 내게 공기 <span class="vocal">(Air Air)</span><br>
        나를 보며 웃어줘 Yeah<br>
        난 그걸로 충분해 Yeah
      </p>

      <p class="stanza">
        내가 찾던 사람 바로 너야 <span class="cheer">【이 동 해】</span> <span class="pron">(Lee Dong Hae)</span> <span class="vocal">(All about you)</span><br>
        네가 찾고 있는 사람 나야 <span class="cheer">【이 혁 재】</span> <span class="pron">(Lee Hyuk Jae)</span> <span class="vocal">(All about you)</span><br>
        I am just thinking all about you, you<br>
        내가 같이하고 싶은 사람 너야 <span class="cheer">(D N E)</span> All about you
      </p>

      <p class="stanza">
        너의 손을 잡고 나의 품 안에 Ye Ye<br>
        거의 모든 날에 또 나의 순간엔 너 Ye<br>
        눈이 부신 햇살 <span class="pron">(嘿沙)</span> 그보다 빛나던 나의 세상 <span class="pron">(誰尚)</span><br>
        다시 데려가 줘요 <span class="pron">(揪喲)</span> 날아 다니게 해줘요 <span class="pron">(揪喲)</span><br>
        너의 하늘에서 자유롭게
      </p>

      <p class="stanza">
        넌 정말 쉽진 않아 내겐 참 어려워<br>
        내 머리가 아니야 내 가슴이 널 불러 Yeah<br>
        I want to know you, Just all about you<br>
        이유는 묻지 마 내게 그냥 답은 너야 <span class="pron">(NO呀)</span>
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        머리부터 발끝까지 <span class="vocal">(Wow Wow Wow Wow)</span><br>
        너무 내게 눈이 부셔 <span class="vocal">(Sha La La La)</span><br>
        너는 내게 공기 <span class="vocal">(Air, Air)</span><br>
        나를 보며 웃어줘 Yeah<br>
        난 그걸로 충분해 Yeah
      </p>

      <p class="stanza">
        내가 찾던 사람 바로 너야 <span class="cheer">【이 혁 재】</span> <span class="pron">(Lee Hyuk Jae)</span> <span class="vocal">(All about you)</span><br>
        네가 찾고 있는 사람 나야 <span class="cheer">【이 동 해】</span> <span class="pron">(Lee Dong Hae)</span> <span class="vocal">(All about you)</span><br>
        I am just thinking all about you, you<br>
        내가 같이하고 싶은 사람 너야 <span class="cheer">(D N E)</span> All about you
      </p>

      <p class="stanza"><span class="label bridge">BRIDGE</span><br>
        시간이 됐다 말해 같이 있고 싶다 말해<br>
        또 다치고 아파도 난 너니까 라고 말해<br>
        시간이 됐다 말해 같이 있고 싶다 말해<br>
        또 다시 다치고 아파도 그래도 너니까 너니까 <span class="pron">(弄你嘎 弄你嘎)</span> <span class="cheer">(D N E)</span>
      </p>

      <p class="stanza">
        너란 여잔 나를 너무 몰라<br>
        나란 남잔 이별을 아주 몰라<br>
        쉽진 않아 내게 너라는 여잔<br>
        그래도 난 계속 너이길 바래 난 바래<br>
        내가 찾던 사람 바로 너야 <span class="cheer">【머리부터】</span> <span class="pron">(摸力不偷)</span> <span class="vocal">(All about you)</span><br>
        네가 찾고 있는 사람 나야 <span class="cheer">【발끝까지】</span> <span class="pron">(怕更嘎季)</span> <span class="vocal">(All about you)</span><br>
        I am just thinking all about you, you<br>
        내가 같이하고 싶은 사람 너야 <span class="cheer">(D N E)</span> <span class="vocal">(All about you)</span>
      </p>
    </div>
  </article>

  <!-- ===== Oppa Oppa ===== -->
  <article class="song" id="song-oppa">
    <div class="song-header">
      <div class="song-num">TRACK 04 / CLASSIC</div>
      <h1 class="song-title">Oppa, Oppa</h1>
      <div class="song-subtitle">Super Junior D&E — 國際的歐巴</div>
    </div>

    <div class="video-section">
      <button class="video-toggle" onclick="toggleVideo(this)">
        <div class="video-toggle-left">
          <div class="video-icon">▶</div>
          <div>
            <span class="video-label">應援教學影片</span>
            <span class="video-title">Watch Tutorial</span>
          </div>
        </div>
        <span class="video-arrow">▼</span>
      </button>
      <div class="video-content">
        <div class="video-grid">
          <div class="video-item">
            <span class="video-tag youtube">▶ YouTube ・ 應援教學</span>
            <div class="video-iframe-wrap">
              <iframe src="https://www.youtube.com/embed/Et-XJ71l86A" title="Oppa Oppa 應援教學" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="lyrics">
      <p class="stanza"><span class="label intro">INTRO</span><br>
        Ah, Ah, 하나, 둘, 셋. Welcome to the Super Show! Let's Go~!!<br>
        My name is DongHae. Let's party tonight!! <span class="cheer">(싸! 싸!)</span> <span class="pron">(薩！薩！)</span>
      </p>

      <p class="stanza">
        그대의 마음에 불을 질러 <span class="vocal">(질러)</span> <span class="pron">(季漏)</span> 내가 원조 여자 킬러 <span class="vocal">(킬러)</span> <span class="pron">(key漏)</span><br>
        문자 썼다 지웠다가 썼다 지웠다가 하게 확 꼬셔 볼라<br>
        밤에 잠 못 자게 미치도록 가만두지 않아<br>
        나를 말릴 생각 하지 마라 그러다가 다친다
      </p>

      <p class="stanza">
        아싸 <span class="pron">(啊薩)</span> 삘 받았어 밤새도록 달릴까 A SA<br>
        누굴 내 맘대로 밤새 불을 지를까<br>
        Hey won't you take me to funky town<br>
        I'm international Baby 1,2,3 Let's go
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        내가 떴다 하면 다 외쳐 오빠, 오빠. <span class="cheer">(歐巴)(歐巴)</span><br>
        Tokyo, London, New York, Paris, 오빠, 오빠. <span class="cheer">(歐巴)(歐巴)</span><br>
        I'm so cool, I'm so cool, Party like a superstar,<br>
        이쁜이들 다 모여라 떴다 오빠, 오빠. <span class="cheer">(歐巴)(歐巴)</span>
      </p>

      <p class="stanza">
        이리저리 이쁜이 있는 곳에 가서 <span class="vocal">(HOLLA)</span><br>
        요리조리 다니면서 Shawty Shawty <span class="vocal">(HOLLA)</span><br>
        오빠오빠 라고 다 불러 난 국제적인 오빠 <span class="cheer">(歐巴)</span><br>
        집에 가지마 라고 하지마 난 모든 이의 오빠 <span class="cheer">(歐巴)</span>
      </p>

      <p class="stanza">
        아싸 <span class="pron">(啊薩)</span> 기분 좋다 오늘 계속 달릴까<br>
        누굴 내 맘대로 밤새 불을 지를까<br>
        Hey won't you take me to funky town<br>
        I'm international Baby 1,2,3 Let's go
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        내가 떴다 하면 다 외쳐 오빠, 오빠. <span class="cheer">(歐巴)(歐巴)</span><br>
        Tokyo, London, New York, Paris, 오빠, 오빠. <span class="cheer">(歐巴)(歐巴)</span><br>
        I'm so cool, I'm so cool, Party like a superstar,<br>
        이쁜이들 다 모여라 떴다 오빠, 오빠. <span class="cheer">(歐巴)(歐巴)</span>
      </p>

      <p class="stanza"><span class="label bridge">CALL & RESPONSE</span><br>
        I say Dong Hae, you say 오빠, Dong Hae <span class="cheer">(오빠)(歐巴)</span> Dong Hae <span class="cheer">(오빠)(歐巴)</span><br>
        I say Eun Hyuk, you say 오빠, Eun Hyuk <span class="cheer">(오빠)(歐巴)</span> Eun Hyuk <span class="cheer">(오빠)(歐巴)</span><br>
        I say SU JU, you say 오빠, SU JU <span class="cheer">(오빠)(歐巴)</span> SU JU <span class="cheer">(오빠)(歐巴)</span>
      </p>

      <p class="stanza"><span class="label chorus">FINAL CHORUS</span><br>
        내가 떴다 하면 다 외쳐 오빠, 오빠. <span class="cheer">(歐巴)(歐巴)</span><br>
        Tokyo, London, New York, Paris, 오빠, 오빠. <span class="cheer">(歐巴)(歐巴)</span><br>
        I'm so cool, I'm so cool, Party like a superstar,<br>
        이쁜이들 다 모여라 떴다 오빠, 오빠. <span class="cheer">(歐巴)(歐巴)</span>
      </p>
    </div>
  </article>

  <!-- ===== California Love ===== -->
  <article class="song" id="song-cali">
    <div class="song-header">
      <div class="song-num">TRACK 05 / DONGHAE</div>
      <h1 class="song-title">California Love</h1>
      <div class="song-subtitle">東海 — Let's Feel The Sunshine</div>
    </div>

    <div class="video-section">
      <button class="video-toggle" onclick="toggleVideo(this)">
        <div class="video-toggle-left">
          <div class="video-icon">▶</div>
          <div>
            <span class="video-label">應援教學影片</span>
            <span class="video-title">Watch Tutorial</span>
          </div>
        </div>
        <span class="video-arrow">▼</span>
      </button>
      <div class="video-content">
        <div class="video-grid">
          <div class="video-item">
            <span class="video-tag instagram">◎ Instagram Reel ・ 應援教學</span>
            <a class="ig-card" href="https://www.instagram.com/dh65_elf/reel/DA982fGTDXf/" target="_blank" rel="noopener noreferrer">
              <div class="ig-icon-wrap">📷</div>
              <div class="ig-text">
                <div class="ig-handle">@dh65_elf</div>
                <div class="ig-desc">California Love 應援教學 Reel</div>
              </div>
              <div class="ig-arrow">↗</div>
            </a>
          </div>
        </div>
      </div>
    </div>

    <div class="lyrics">
      <p class="stanza"><span class="label intro">INTRO</span><br>
        <span class="cheer">【이 동 해】</span> <span class="pron">(Lee Dong Hae)</span><br>
        <span class="cheer">【이 동 해】</span> <span class="pron">(Lee Dong Hae)</span><br>
        <span class="cheer">【이 동 해】</span> <span class="pron">(Lee Dong Hae)</span>
      </p>

      <p class="stanza">
        It's California Love Oh<br>
        우리 둘의 Love <span class="pron">(屋哩禿欸 Love)</span> Oh Oh<br>
        We gotta go (go) Where we goin' (go)<br>
        I just feel like I'm in paradise
      </p>

      <p class="stanza">
        예쁘장한 너의 얼굴은 참 조그매<br>
        솜사탕 같은 너의 말투는 날 자극해<br>
        Sexy 하게 탄 네 피부는 Gree Gree<br>
        내 생각엔 우린 잘 어울려 끼리끼리 <span class="pron">(ㄍ一哩 ㄍ一哩)</span><br>
        네 몸매는 마치 California 빛<br>
        무모한 베팅에 따라오는 빚처럼<br>
        내 모든 걸 네게 걸게<br>
        오늘도 머릿속에 그려<br>
        너와의 곡을 그려
      </p>

      <p class="stanza">
        Woo 내 귓가에 들려 네 숨결<br>
        오늘은 가지 마 All Night<br>
        끝이 없단 걸 너도 알잖아 Baby<br>
        이 시간이 영원하길 바라 Lady Yeah<br>
        Not Today Not Today Uh<br>
        But Today But Today 나<br>
        지금 시작된 이 Party Alright<br>
        On Fire Fire
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        It's California Love Oh<br>
        우리 둘의 Love <span class="pron">(屋哩禿欸 Love)</span> Oh Oh<br>
        We gotta go (go) Where we goin' (go)<br>
        I just feel like I'm in dream Oh<br>
        Love Oh<br>
        It's California Love Oh Oh<br>
        네게서 두 눈을 뗄 수 없어 Baby<br>
        둘이만 더 올라가자 Keep it on
      </p>

      <p class="stanza">
        It's California Love Uh Yeah<br>
        끝나지 않을 우리 밤 Uh Yeah<br>
        Real Light Savage Light<br>
        I just feel like I'm in paradise
      </p>

      <p class="stanza">
        난 없진 않지 눈치<br>
        미래를 보지 마치<br>
        네 목에 걸려질 나의 Kiss<br>
        It's like a GUCCI<br>
        난 원래 잘해 거래 <span class="pron">(勾類)</span><br>
        너와는 다르게 갈래 <span class="pron">(嘎類)</span><br>
        하지만 아무 생각 없이<br>
        지금 너를 원해 <span class="pron">(翁嘿)</span><br>
        내게 다른 답은 없는 걸<br>
        뜨거운 태양처럼 빛난 널<br>
        나의 상상 속에 걸어 매일 <span class="pron">(每一)</span><br>
        이제는 현실이 돼<br>
        우리 Day Day
      </p>

      <p class="stanza">
        시간이 더 다가오잖아<br>
        네 몸에 더 눈이 가잖아<br>
        That's right<br>
        지독하게 취해 더<br>
        너의 품에 취해 Too Hot<br>
        Not Today Not Today Uh<br>
        But Today But Today 나<br>
        지금 시작된 이 Party Alright<br>
        On Fire Fire
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        It's California Love Oh<br>
        우리 둘의 Love <span class="pron">(屋哩禿欸 Love)</span> Oh Oh<br>
        We gotta go (go) Where we goin' (go)<br>
        I just feel like I'm in dream Oh<br>
        Love Oh<br>
        It's California Love Oh Oh<br>
        네게서 두 눈을 뗄 수 없어 Baby<br>
        둘이만 더 올라가자 Keep it on
      </p>

      <p class="stanza">
        지금 날 만진 손길로<br>
        또 날이 밝아 Fly it Home<br>
        어제완 다른 매일을 약속해<br>
        또 잊지 못할 순간들을 기억해<br>
        너 하나로 난 That's enough<br>
        나 숨이 벅차 Let me love<br>
        Oh Help me Help me<br>
        So Tell me Tell me
      </p>

      <p class="stanza"><span class="label outro">OUTRO</span><br>
        It's California Love Oh<br>
        우리 둘의 Love <span class="pron">(屋哩禿欸 Love)</span> Oh Oh<br>
        We gotta go (go) Where we goin' (go)<br>
        I just feel like I'm in dream Oh<br>
        Love Oh<br>
        It's California Love Oh Oh<br>
        네게서 두 눈을 뗄 수 없어 Baby<br>
        둘이만 더 올라가자 Keep it on
      </p>

      <p class="stanza">
        It's California Love Uh Yeah<br>
        끝나지 않을 우리 밤 Uh Yeah<br>
        Real Light Savage Light<br>
        What do you wanna do wanna do<br>
        It's California Love Uh Yeah<br>
        뜨겁게 불탈 우리 밤 Uh Yeah<br>
        Real Light Savage Light<br>
        I just feel like I'm in paradise
      </p>
    </div>
  </article>

  <!-- ===== 太完美 ===== -->
  <article class="song" id="song-perfect">
    <div class="song-header">
      <div class="song-num">TRACK 06 / SUPER JUNIOR-M</div>
      <h1 class="song-title">太完美</h1>
      <div class="song-subtitle">SUPER JUNIOR-M — Perfection (Mandarin Ver.)</div>
    </div>

    <div class="video-section">
      <button class="video-toggle" onclick="toggleVideo(this)">
        <div class="video-toggle-left">
          <div class="video-icon">▶</div>
          <div>
            <span class="video-label">應援教學影片</span>
            <span class="video-title">Watch Tutorial</span>
          </div>
        </div>
        <span class="video-arrow">▼</span>
      </button>
      <div class="video-content">
        <div class="video-grid">
          <div class="video-item">
            <span class="video-tag youtube">▶ YouTube ・ 應援教學</span>
            <div class="video-iframe-wrap">
              <iframe src="https://www.youtube.com/embed/Dl2xYVHAg9A" title="太完美 應援教學" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="lyrics">
      <p class="stanza"><span class="label intro">INTRO</span><br>
        她迷住我視線　她迷住我視線
      </p>

      <p class="stanza">
        在愛情裡的寶藏被我發現 <span class="cheer">(이동해)</span> <span class="pron">(李東海)</span><br>
        你就是我尋找的稀世寶貝<br>
        你就不斷地在正反我世界 <span class="cheer">(이동해)</span> <span class="pron">(李東海)</span><br>
        連冰塊遇見你都燃起火焰
      </p>

      <p class="stanza">
        太過心急不對 <span class="vocal">(不對)</span><br>
        用力愛會碎<br>
        太過緩慢不對 <span class="vocal">(不對)</span><br>
        我隨你進或退
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        oh 太完美 <span class="cheer">(슈주 M)</span> <span class="pron">(SUJU-M)</span><br>
        你眼裡我出現<br>
        oh 不讓誰 <span class="vocal">(太完美)</span><br>
        替我在你身邊　Woo Wo u O<br>
        你的眉眼　你的側臉　你的頸肩　你的嫵媚　你的一切　從頭到尾　我已淪陷
      </p>

      <p class="stanza">
        我的心變成了口袋的一面 <span class="cheer">(이동해)</span> <span class="pron">(李東海)</span><br>
        Just for you 不停地給不停地給<br>
        這樣子愛你到底是對不對 <span class="cheer">(이동해)</span> <span class="pron">(李東海)</span><br>
        我一邊迷惑一邊更加迷戀
      </p>

      <p class="stanza">
        太過心急不對 <span class="vocal">(不對)</span><br>
        用力愛會碎<br>
        太過緩慢不對 <span class="vocal">(不對)</span><br>
        我隨你進或退
      </p>

      <p class="stanza"><span class="label chorus">CHORUS</span><br>
        oh 太完美 <span class="cheer">(슈주 M)</span> <span class="pron">(SUJU-M)</span><br>
        你眼裡我出現<br>
        oh 不讓誰 <span class="vocal">(太完美)</span><br>
        替我在你身邊　Woo Wo u O<br>
        你的眉眼　你的側臉　你的頸肩　你的嫵媚　你的一切　從頭到尾　我已淪陷
      </p>

      <p class="stanza"><span class="label bridge">間奏 ・ FANCHANT</span><br>
        oh 太完美　oh 不讓誰　oh 太完美<br>
        <span class="cheer">(이동해！이동해！이동해！이동해！이동해！이동해！이동해！이동해！</span><br>
        <span class="cheer">사랑해요 슈주 M！완전대박 슈주 M！슈 퍼 주 니 어 M 太 完 美！)</span><br>
        <span class="pron">(李東海！李東海！李東海！李東海！李東海！李東海！李東海！李東海！</span><br>
        <span class="pron">莎郎嘿唷 SUJU-M！完炯TE吧 SUJU-M！SUPER JUNIOR-M 太 完 美！)</span>
      </p>

      <p class="stanza">
        每次見面是脈搏就當機了　它在我全身狂跳不由己
      </p>

      <p class="stanza">
        一直跳　一直跳　想見你<br>
        一直跳　一直跳　喜歡你<br>
        一直跳　一直跳　都是你<br>
        一直跳　一直跳　我愛你<br>
        一直跳　一直跳　一直跳　一直跳
      </p>

      <p class="stanza">
        太過心急不對 <span class="vocal">(不對)</span><br>
        用力愛會碎<br>
        太過緩慢不對 <span class="vocal">(不對)</span><br>
        我隨你進或退
      </p>

      <p class="stanza"><span class="label chorus">FINAL CHORUS</span><br>
        oh 太完美 <span class="cheer">(슈주 M)</span> <span class="pron">(SUJU-M)</span><br>
        你眼裡我出現<br>
        oh 不讓誰 <span class="vocal">(太完美)</span><br>
        替我在你身邊　Woo Wo u O<br>
        你的眉眼　你的側臉　你的頸肩　你的嫵媚　你的一切　從頭到尾　我已淪陷
      </p>

      <p class="stanza">
        Bounce to the music, let your feet go round<br>
        To the floor and I'ma break it down<br>
        Let me in, let me show you, all my bling, bling<br>
        And all my kiss, kiss, baby, dance with me<br>
        Boom, boom, boom<br>
        Can I get another? Clap, clap, clap, let's go<br>
        Shake your body, move your body, pick your feet up<br>
        I'ma move to the groove, baby, I'ma go all out (yeah-yeah)
      </p>

      <p class="stanza"><span class="label outro">OUTRO</span><br>
        給我說你想我 <span class="vocal">(我想你)</span><br>
        給我說你愛我 <span class="vocal">(我愛你)</span><br>
        給我說你想我　給我說你想我<br>
        給我說你愛我 <span class="vocal">(我愛你)</span> Yeah~~
      </p>

      <p class="stanza">
        給我說你想我 <span class="vocal">(我想你)</span><br>
        給我說你愛我 <span class="vocal">(我愛你)</span><br>
        給我說你想我　給我說你想我<br>
        給我說你愛我 <span class="cheer">(슈 퍼 주 니 어 M)</span> <span class="pron">(SUPER JUNIOR-M)</span>
      </p>
    </div>
  </article>

  <!-- ===== 我們是 E.L.F. ===== -->
  <article class="song" id="song-elf">
    <div class="song-header">
      <div class="song-num">SPECIAL / TWELF</div>
      <h1 class="song-title">我們是 E.L.F.</h1>
      <div class="song-subtitle">Always Keep The Faith — TWELF 應援口號教學</div>
    </div>

    <div class="elf-only">
      <p class="elf-intro">
        E.L.F. 是 Super Junior 的官方粉絲名稱<br>
        — Ever Lasting Friends —<br>
        我們會永遠守護他們，他們也會永遠陪著我們 💙
      </p>

      <div class="video-section open">
        <button class="video-toggle" onclick="toggleVideo(this)">
          <div class="video-toggle-left">
            <div class="video-icon">▶</div>
            <div>
              <span class="video-label">TWELF 應援教學</span>
              <span class="video-title">我們是 E.L.F.</span>
            </div>
          </div>
          <span class="video-arrow">▼</span>
        </button>
        <div class="video-content">
          <div class="video-grid">
            <div class="video-item">
              <span class="video-tag youtube">▶ YouTube ・ 應援教學</span>
              <div class="video-iframe-wrap">
                <iframe src="https://www.youtube.com/embed/KaI_L_Dt5z4" title="我們是 E.L.F. 應援教學" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </article>

</main>

<button class="top-btn" id="topBtn" aria-label="回頂部">↑</button>

<footer>
  <div class="bracket">— TWELF · 2026 —</div>
  <div>整理 with <span class="heart">♥</span> for E.L.F. & 애니</div>
  <div style="margin-top:8px;font-size:11px;letter-spacing:.2em;text-transform:uppercase;">Always Keep The Faith</div>
</footer>

<script>
  // 影片區塊展開/收合
  function toggleVideo(btn){
    btn.parentElement.classList.toggle('open');
  }

  // 切換歌曲
  const buttons = document.querySelectorAll('.nav-btn');
  const songs = document.querySelectorAll('.song');

  buttons.forEach(btn=>{
    btn.addEventListener('click',()=>{
      buttons.forEach(b=>b.classList.remove('active'));
      songs.forEach(s=>s.classList.remove('active'));
      btn.classList.add('active');
      document.getElementById(btn.dataset.target).classList.add('active');
      // 平滑滾動到內容
      window.scrollTo({
        top: document.querySelector('.nav').offsetTop - 0,
        behavior:'smooth'
      });
    });
  });

  // 回頂部
  const topBtn = document.getElementById('topBtn');
  window.addEventListener('scroll',()=>{
    if(window.scrollY > 400) topBtn.classList.add('show');
    else topBtn.classList.remove('show');
  });
  topBtn.addEventListener('click',()=>{
    window.scrollTo({top:0,behavior:'smooth'});
  });
</script>

</body>
</html>
