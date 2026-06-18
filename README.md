<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<meta name="theme-color" content="#ff8a6a">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<meta name="apple-mobile-web-app-title" content="Bangkok Trip">
<title>2026 曼谷自由行 Travel App</title>
<link rel="manifest" href="data:application/manifest+json,{&quot;name&quot;:&quot;2026 曼谷自由行 Travel App&quot;,&quot;short_name&quot;:&quot;Bangkok&quot;,&quot;start_url&quot;:&quot;.&quot;,&quot;display&quot;:&quot;standalone&quot;,&quot;background_color&quot;:&quot;#fff6f1&quot;,&quot;theme_color&quot;:&quot;#ff8a6a&quot;,&quot;icons&quot;:[{&quot;src&quot;:&quot;data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'%3E%3Crect width='512' height='512' rx='120' fill='%23ff8a6a'/%3E%3Ctext x='50%25' y='56%25' dominant-baseline='middle' text-anchor='middle' font-size='240'%3E✈️%3C/text%3E%3C/svg%3E&quot;,&quot;sizes&quot;:&quot;512x512&quot;,&quot;type&quot;:&quot;image/svg+xml&quot;}]}">
<style>
:root{--bg:#fff6f1;--card:#ffffffcc;--text:#33211d;--muted:#8c6d63;--primary:#ff8a6a;--primary2:#ffb199;--accent:#ffd6c9;--line:#ffe2d8;--shadow:0 18px 45px rgba(255,118,88,.18);--safe:env(safe-area-inset-bottom)}
[data-theme=dark]{--bg:#18110f;--card:#241816dd;--text:#fff1eb;--muted:#caa79d;--primary:#ff987a;--primary2:#ffbca8;--accent:#4b2b24;--line:#3a2824;--shadow:0 18px 45px rgba(0,0,0,.35)}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{margin:0;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Noto Sans TC",sans-serif;background:radial-gradient(circle at top left,#ffe1d4,transparent 35%),radial-gradient(circle at top right,#ffd2e0,transparent 35%),var(--bg);color:var(--text);padding-bottom:calc(86px + var(--safe))}
button,input,select,textarea{font:inherit}
button{border:0;cursor:pointer}
.app{max-width:520px;margin:0 auto;min-height:100vh}
.hero{padding:20px 18px 12px;position:sticky;top:0;z-index:20;background:linear-gradient(to bottom,var(--bg) 78%,transparent);backdrop-filter:blur(12px)}
.top{display:flex;justify-content:space-between;align-items:center;gap:12px}
.badge{display:inline-flex;align-items:center;gap:6px;background:var(--card);border:1px solid var(--line);padding:8px 12px;border-radius:999px;color:var(--muted);box-shadow:var(--shadow);font-size:13px}
h1{font-size:29px;line-height:1.08;margin:14px 0 8px;letter-spacing:-.6px}
.subtitle{color:var(--muted);font-size:14px}
.iconbtn{width:42px;height:42px;border-radius:16px;background:var(--card);color:var(--text);box-shadow:var(--shadow);border:1px solid var(--line)}
main{padding:0 16px 22px}
.section{display:none;animation:pop .35s ease}
.section.active{display:block}
@keyframes pop{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}
.card{background:var(--card);border:1px solid var(--line);border-radius:26px;padding:16px;margin:12px 0;box-shadow:var(--shadow);backdrop-filter:blur(16px)}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.stat{border-radius:22px;padding:14px;background:linear-gradient(135deg,var(--primary),var(--primary2));color:white;min-height:94px}
.stat small{opacity:.86}
.stat b{display:block;font-size:23px;margin-top:8px}
.row{display:flex;gap:10px;align-items:center;justify-content:space-between}
.pill{display:inline-flex;padding:8px 11px;border-radius:999px;background:var(--accent);color:var(--text);font-size:13px;margin:4px 4px 4px 0}
.tabs{display:flex;gap:8px;overflow:auto;padding:8px 0 4px}
.daytab{min-width:78px;border-radius:20px;padding:10px;background:var(--card);border:1px solid var(--line);color:var(--muted)}
.daytab.active{background:linear-gradient(135deg,var(--primary),var(--primary2));color:white}
.timeline{position:relative;margin-top:10px}
.item{display:flex;gap:12px;padding:12px 0;border-bottom:1px solid var(--line)}
.item:last-child{border-bottom:0}
.time{width:58px;flex:0 0 58px;color:var(--primary);font-weight:800}
.itembody{flex:1}
.itembody h3{margin:0 0 6px;font-size:16px}
.meta{font-size:13px;color:var(--muted);line-height:1.55}
.actions{display:flex;gap:6px;margin-top:8px;flex-wrap:wrap}
.smallbtn,.mapbtn{border-radius:14px;padding:8px 10px;background:var(--accent);color:var(--text);font-size:13px}
.primary{background:linear-gradient(135deg,var(--primary),var(--primary2));color:white}
input,textarea,select{width:100%;border:1px solid var(--line);background:var(--card);color:var(--text);border-radius:16px;padding:12px;margin:6px 0;outline:none}
textarea{min-height:76px;resize:vertical}
.nav{position:fixed;left:50%;bottom:12px;transform:translateX(-50%);width:min(500px,calc(100% - 22px));background:var(--card);border:1px solid var(--line);border-radius:28px;padding:8px calc(8px + var(--safe)/4);display:grid;grid-template-columns:repeat(5,1fr);gap:4px;z-index:50;box-shadow:0 20px 50px rgba(0,0,0,.18);backdrop-filter:blur(20px)}
.nav button{background:transparent;color:var(--muted);border-radius:20px;padding:8px 2px;font-size:11px}
.nav b{display:block;font-size:19px}
.nav button.active{background:linear-gradient(135deg,var(--primary),var(--primary2));color:white}
.listitem{display:flex;align-items:center;gap:10px;border-bottom:1px solid var(--line);padding:10px 0}
.listitem.done{opacity:.55;text-decoration:line-through}
.check{width:22px;height:22px}
.progress{height:10px;background:var(--line);border-radius:999px;overflow:hidden;margin:8px 0}
.bar{height:100%;background:linear-gradient(90deg,var(--primary),var(--primary2));width:0}
.canvaswrap{height:220px;display:flex;align-items:center;justify-content:center}
.photoGrid{display:grid;grid-template-columns:repeat(3,1fr);gap:8px}
.photoGrid img{width:100%;aspect-ratio:1;border-radius:18px;object-fit:cover}
.notice{border-left:5px solid var(--primary);background:var(--accent);border-radius:18px;padding:12px;line-height:1.6;color:var(--text)}
.floatTop{position:fixed;right:16px;bottom:106px;border-radius:50%;width:48px;height:48px;background:var(--primary);color:white;box-shadow:var(--shadow);z-index:40}
.searchbox{position:sticky;top:132px;z-index:10}
@media print{.nav,.hero,.floatTop,.actions,.formbox{display:none!important}body{background:white;color:black;padding:0}.section{display:block}.card{box-shadow:none;border:1px solid #ddd;background:white}}
.settingsOnly{display:none}
#itinerary .card:has(button[onclick="exportJSON()"]){display:none}
.homeUpgrade{background:linear-gradient(135deg,#fff,#ffe3d7);border:1px solid var(--line)}
[data-theme=dark] .homeUpgrade{background:linear-gradient(135deg,#241816,#3a211c)}
.bigNumber{font-size:34px;font-weight:900;color:var(--primary);letter-spacing:-1px}
.flightCard{display:grid;grid-template-columns:1fr auto 1fr;gap:10px;align-items:center;text-align:center}
.flightCard b{font-size:20px}
.planeLine{font-size:24px;color:var(--primary)}
.toolGrid{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.toolTile{border-radius:22px;padding:14px;background:var(--accent);min-height:82px}
.toolTile b{display:block;font-size:18px;margin-bottom:4px}
.budgetHero{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.budgetHero .stat.usd{grid-column:1/3;background:linear-gradient(135deg,#ffd6c9,#ffb199)}
.budgetProgress{height:14px;background:var(--line);border-radius:999px;overflow:hidden;margin:12px 0}
.budgetProgressBar{height:100%;background:linear-gradient(90deg,var(--primary),var(--primary2));width:0}
.legendItem{display:flex;justify-content:space-between;align-items:center;padding:8px 0;border-bottom:1px solid var(--line);font-size:14px}
.legendDot{width:12px;height:12px;border-radius:50%;display:inline-block;margin-right:8px}
.expenseCard{position:relative;padding:12px 46px 12px 12px;border-radius:20px;background:var(--accent);margin:10px 0}
.expenseCard b{display:block;font-size:16px}
.expenseCat{font-size:13px;color:var(--muted);margin-top:4px}
.trashBtn{position:absolute;right:10px;top:50%;transform:translateY(-50%);width:34px;height:34px;border-radius:50%;background:var(--card)}
.memberCard,.settleCard{background:var(--accent);border-radius:20px;padding:12px;margin:10px 0}
.memberAvatar{width:38px;height:38px;border-radius:50%;background:linear-gradient(135deg,var(--primary),var(--primary2));color:white;display:flex;align-items:center;justify-content:center;font-weight:900}
.memberRow{display:flex;align-items:center;gap:10px}
.splitBox{display:grid;grid-template-columns:1fr 1fr;gap:8px}
.memberCheck{display:flex;gap:6px;align-items:center;background:var(--card);border-radius:14px;padding:8px}
.superrichBox{background:linear-gradient(135deg,#fff7ef,#ffe0d2);border-radius:22px;padding:14px;margin:10px 0}
[data-theme=dark] .superrichBox{background:linear-gradient(135deg,#2c1c18,#43251f)}
.settleCard b{color:var(--primary)}
.mapModeCard{
  background:var(--accent);
  border-radius:22px;
  padding:14px;
  margin-top:12px;
}

.routeItem{
  display:flex;
  gap:10px;
  align-items:flex-start;
}

.routeDot{
  width:18px;
  height:18px;
  border-radius:50%;
  background:var(--primary);
  margin-top:4px;
}

.routeLine{
  width:2px;
  height:38px;
  background:var(--primary2);
  margin:4px 0 4px 8px;
}

.routePlace{
  flex:1;
}

.routeTransport{
  color:var(--muted);
  font-size:13px;
  margin-top:4px;
}
.achievementCard{
  background:linear-gradient(135deg,#ffe8bf,#ffd36e);
  border-radius:20px;
  padding:12px;
  margin:10px 0;
  color:#4d3200;
}

.footprintCard{
  background:var(--accent);
  border-radius:20px;
  padding:12px;
  margin:10px 0;
}

.footprintDone{
  border:2px solid #58c27d;
}

.memoryCard{
  background:linear-gradient(135deg,#ffd9cf,#fff0ea);
  border-radius:22px;
  padding:16px;
  margin-top:12px;
}
.aiCard{
  position:fixed;
  right:16px;
  bottom:170px;
  z-index:999;
}

.aiBtn{
  width:60px;
  height:60px;
  border-radius:50%;
  border:none;
  background:linear-gradient(135deg,var(--primary),var(--primary2));
  color:white;
  font-size:28px;
  box-shadow:var(--shadow);
}

.aiPanel{
  position:fixed;
  right:16px;
  bottom:240px;
  width:320px;
  max-width:calc(100vw - 32px);
  height:420px;
  background:var(--card);
  border-radius:24px;
  border:1px solid var(--line);
  box-shadow:var(--shadow);
  display:none;
  flex-direction:column;
  overflow:hidden;
  z-index:999;
}

.aiMessages{
  flex:1;
  overflow:auto;
  padding:12px;
}

.aiMsg{
  padding:10px 12px;
  border-radius:16px;
  margin-bottom:8px;
}

.aiUser{
  background:var(--primary);
  color:white;
}

.aiBot{
  background:var(--accent);
}

.aiInput{
  display:flex;
  gap:6px;
  padding:10px;
}
.travelStatsCard{
  background:linear-gradient(135deg,#fff1e8,#ffd8c8);
  border-radius:22px;
  padding:16px;
  margin-top:12px;
}

.certificateCard{
  background:linear-gradient(135deg,#fff8dc,#ffe58f);
  border:3px solid #f0c75e;
  border-radius:24px;
  padding:20px;
  margin-top:12px;
  text-align:center;
}

.certificateTitle{
  font-size:24px;
  font-weight:800;
  margin-bottom:12px;
}

.statGrid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:10px;
  margin-top:12px;
}

.statItem{
  background:rgba(255,255,255,.5);
  border-radius:16px;
  padding:10px;
}
</style>
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>
</head>
<body>
<div class="app" id="app">
<header class="hero">
<div class="top"><span class="badge">✈️ Bangkok · 2026/6/24–6/29</span><button class="iconbtn" id="themeBtn">🌙</button></div>
<h1>曼谷自由行<br>Travel App</h1>
<div class="subtitle">粉橘系行程、預算、清單、照片與離線旅行工具</div>
</header>
<main>
<section class="section active" id="home">
<div class="grid">
<div class="stat"><small>出發倒數</small><b id="countdown">--</b></div>
<div class="stat"><small>住宿</small><b style="font-size:18px">Diya Hotel<br>Srinakarin</b></div>
</div>
<div class="card">
<div class="row"><h2>今日摘要</h2><span class="pill" id="todayLabel">Trip</span></div>
<p class="meta">6/24 12:10 抵達 BKK｜14:00 後入住｜6/29 15:30 回台灣</p>
<div id="todayPlan"></div>
</div>
<div class="card">
<h2>天氣與安全提醒</h2>
<div class="notice">曼谷 6 月可能炎熱午後雷陣雨。每天帶摺疊傘、薄外套、防曬、行動電源。雨天模式可在工具頁啟用。</div>
</div>
<div class="card">
<h2>快速功能</h2>
<button class="smallbtn primary" onclick="showSec('itinerary')">查看每日行程</button>
<button class="smallbtn" onclick="showSec('budget')">記帳預算</button>
<button class="smallbtn" onclick="window.print()">一鍵列印</button>
</div>
</section>
<section class="section" id="itinerary">
<div class="card searchbox"><input id="search" placeholder="搜尋行程、地點、備註…"></div>
<div class="tabs" id="dayTabs"></div>
<div class="card"><div class="row"><h2 id="dayTitle">Day</h2><button class="smallbtn primary" onclick="openForm()">＋新增</button></div><div id="timeline" class="timeline"></div></div>
<div class="card formbox" id="formBox" style="display:none">
<h2 id="formTitle">新增行程</h2>
<input id="fTime" placeholder="時間，例如 13:30">
<input id="fTitle" placeholder="地點 / 行程名稱">
<input id="fTransport" placeholder="交通方式">
<input id="fStay" placeholder="預估停留時間">
<textarea id="fNote" placeholder="備註"></textarea>
<input id="fMap" placeholder="Google Maps 關鍵字或網址">
<button class="smallbtn primary" onclick="saveItem()">儲存</button>
<button class="smallbtn" onclick="closeForm()">取消</button>
</div>
<div class="card">
<h2>資料管理</h2>
<button class="smallbtn" onclick="exportJSON()">匯出 JSON</button>
<label class="smallbtn">匯入 JSON<input type="file" accept="application/json" onchange="importJSON(event)" style="display:none"></label>
<button class="smallbtn" onclick="resetData()">重置資料</button>
</div>
</section>
<section class="section" id="budget">
<div class="card">
<h2>匯率設定</h2>
<div class="grid"><input id="rateTWD" type="number" step="0.01"><input id="rateUSD" type="number" step="0.01"></div>
<p class="meta">1 THB = TWD；1 USD = THB</p>
</div>
<div class="card">
<h2>新增花費</h2>
<input id="bName" placeholder="項目，例如 船票、芒果糯米飯">
<select id="bCat"><option>美食</option><option>交通</option><option>購物</option><option>門票</option><option>其他</option></select>
<div class="grid"><input id="bTHB" type="number" placeholder="THB"><input id="bTWD" type="number" placeholder="TWD"><input id="bUSD" type="number" placeholder="USD"></div>
<button class="smallbtn primary" onclick="addExpense()">新增</button>
</div>
<div class="card">
<h2>總花費</h2>
<div class="grid"><div class="stat"><small>THB</small><b id="sumTHB">0</b></div><div class="stat"><small>TWD</small><b id="sumTWD">0</b></div></div>
<p class="pill">USD <b id="sumUSD">0</b></p>
<div class="canvaswrap"><canvas id="chart" width="220" height="220"></canvas></div>
<div id="expenses"></div>
</div>
</section>
<section class="section" id="lists">
<div id="listsWrap"></div>
</section>
<section class="section" id="tools">
<div class="card">
<h2>旅行工具</h2>
<button class="smallbtn primary" onclick="toggleRain()">雨天備案模式：<span id="rainState">OFF</span></button>
<div id="rainBox" class="notice" style="display:none;margin-top:10px">雨天建議：CentralWorld、Big C、ICONSIAM、Terminal 21、按摩、咖啡甜點店，減少戶外寺廟與市集停留。</div>
</div>
<div class="card"><h2>行程衝突提醒</h2><div id="conflicts" class="meta"></div></div>
<div class="card">
<h2>照片牆</h2>
<input type="file" accept="image/*" multiple onchange="savePhotos(event)">
<div class="photoGrid" id="photoGrid"></div>
</div>
<div class="card">
<h2>緊急資訊</h2>
<p class="meta">泰國緊急電話：191｜觀光警察：1155｜台灣駐泰國代表處：建議出發前自行儲存最新聯絡方式。</p>
<div class="notice">護照、保險、機票、飯店訂房截圖請離線保存；護照影本與電子檔分開存放。</div>
</div>
<div class="card">
<h2>安全提醒</h2>
<div class="notice">大麻與相關商品可能涉及健康、法律與入境風險，請自行確認最新規定並避免攜帶出入境。</div>
<div class="notice" style="margin-top:10px">曼谷海軍射擊場列為待確認行程；本 App 不提供實彈射擊預約、操作教學或導航資訊，請以官方規範與現場安全指示為準。</div>
</div>
</section>
</main>
<nav class="nav">
<button class="active" onclick="showSec('home')"><b>🏠</b>首頁</button>
<button onclick="showSec('itinerary')"><b>🗓️</b>行程</button>
<button onclick="showSec('budget')"><b>💸</b>預算</button>
<button onclick="showSec('lists')"><b>✅</b>清單</button>
<button onclick="showSec('tools')"><b>🧰</b>工具</button>
</nav>
<button class="floatTop" onclick="scrollTo({top:0,behavior:'smooth'})">↑</button>
</div>
<script>
const STORE="bkk_luxury_final_v1";
const defaultData={
theme:"light",activeDay:0,rates:{twd:0.88,usd:36.7},rain:false,photos:[],
days:[
{date:"6/24（三）",title:"Day1 抵達與市區採買",items:[
{time:"12:10",title:"抵達 BKK 機場",transport:"入境、領行李、叫車",stay:"約 1.5–2 小時",note:"先買水、換網卡確認 eSIM、確認 Bolt/Grab。",map:"BKK Airport"},
{time:"14:00",title:"Diya Hotel Srinakarin 入住",transport:"機場叫車前往飯店",stay:"約 1 小時",note:"放行李、休息、整理現金與行動電源。",map:"Diya Hotel Srinakarin"},
{time:"16:30",title:"CentralWorld",transport:"計程車 / BTS 轉乘",stay:"約 1.5 小時",note:"冷氣商場、逛街、吃點心。",map:"CentralWorld Bangkok"},
{time:"18:00",title:"Big C 採買",transport:"步行",stay:"約 1 小時",note:"先買零食伴手禮，最後一天再補貨。",map:"Big C Ratchadamri"},
{time:"19:20",title:"水門市場",transport:"步行 / 短程車",stay:"約 1 小時",note:"服飾、小物、批發感逛街。",map:"Pratunam Market"},
{time:"21:00",title:"JODD FAIRS",transport:"MRT / 計程車",stay:"約 1.5 小時",note:"夜市晚餐、拍照、飲料。",map:"JODD FAIRS Bangkok"}]},
{date:"6/25（四）",title:"Day2 泰服、鄭王廟、美甲與唐人街",items:[
{time:"09:30",title:"MAHASANÉ 泰服體驗",transport:"叫車前往",stay:"約 2 小時",note:"妝髮、泰服、拍照前確認押金與歸還時間。",map:"MAHASANE Thai Costume"},
{time:"11:30",title:"鄭王廟 Wat Arun",transport:"步行 / 船 / 計程車",stay:"約 1 小時",note:"注意服裝規定、防曬補水。",map:"Wat Arun"},
{time:"12:30",title:"Tha Arun",transport:"河岸附近移動",stay:"約 45 分鐘",note:"湄南河景觀，適合拍照與看夕陽候補。",map:"Tha Arun Bangkok"},
{time:"13:30",title:"Take Away Studio 美甲",transport:"叫車",stay:"約 2 小時",note:"固定預約：13:30。",map:"Take Away Studio Bangkok"},
{time:"16:00",title:"GOLEM HOUR",transport:"步行 / 叫車",stay:"約 45 分鐘",note:"咖啡甜點休息。",map:"GOLEM HOUR Bangkok"},
{time:"17:00",title:"DizzySweetie",transport:"短程移動",stay:"約 45 分鐘",note:"甜點、拍照。",map:"DizzySweetie Bangkok"},
{time:"18:30",title:"三聘市場",transport:"叫車",stay:"約 1 小時",note:"飾品、小物、批發採買。",map:"Sampeng Market"},
{time:"20:00",title:"唐人街 Yaowarat",transport:"步行",stay:"約 2 小時",note:"晚餐、小吃、夜景。",map:"Yaowarat Road"}]},
{date:"6/26（五）",title:"Day3 大城一日遊",items:[
{time:"08:00",title:"大城交通方案比較",transport:"包車方案：彈性高、可放行李、適合多景點；Bolt 方案：單趟可能便宜但回程與跨點不穩定",stay:"整日",note:"建議出發前一天確認司機、價格、等候時間與回程。",map:"Ayutthaya Thailand"},
{time:"10:00",title:"大城獅子動物園",transport:"包車 / Bolt 待確認",stay:"約 2–3 小時",note:"注意動物互動規範、防曬補水。",map:"Sriayuthaya Lion Park"},
{time:"13:30",title:"Wat Mahathat",transport:"包車 / 當地移動",stay:"約 1 小時",note:"樹中佛頭、古蹟拍照，注意服裝。",map:"Wat Mahathat Ayutthaya"},
{time:"15:30",title:"Mr Joe 脆皮豬",transport:"回曼谷後前往",stay:"約 1 小時",note:"熱門餐廳可彈性改外帶或排隊。",map:"Mr Joe Crispy Pork Bangkok"}]},
{date:"6/27（六）",title:"Day4 洽圖洽、按摩與商場",items:[
{time:"10:00",title:"洽圖洽市集",transport:"BTS/MRT 或叫車",stay:"約 3–4 小時",note:"週末市集，注意補水、防扒、分區逛。",map:"Chatuchak Weekend Market"},
{time:"14:00",title:"Polo Fried Chicken",transport:"叫車",stay:"約 1 小時",note:"炸雞名店，可當午晚餐。",map:"Polo Fried Chicken Bangkok"},
{time:"16:00",title:"曼谷海軍射擊場待確認",transport:"自行確認",stay:"待確認",note:"僅列待確認；不提供預約、操作教學或導航資訊，請以官方安全規範為準。",map:""},
{time:"18:00",title:"Health Land",transport:"叫車",stay:"約 2 小時",note:"按摩放鬆，建議提前預約合法正規分店。",map:"Health Land Bangkok"},
{time:"20:30",title:"Terminal 21",transport:"BTS / MRT",stay:"約 1.5 小時",note:"晚餐、逛街、冷氣備案。",map:"Terminal 21 Asok"}]},
{date:"6/28（日）",title:"Day5 寺廟、ICONSIAM、Asiatique 與 Calypso",items:[
{time:"09:00",title:"大皇宮",transport:"叫車 / 船",stay:"約 1.5 小時",note:"服裝規定嚴格，避免短褲細肩帶。",map:"Grand Palace Bangkok"},
{time:"10:30",title:"玉佛寺",transport:"同區步行",stay:"約 1 小時",note:"寺廟禮儀、不可喧嘩。",map:"Temple of the Emerald Buddha"},
{time:"12:00",title:"臥佛寺 Wat Pho",transport:"步行 / 短程車",stay:"約 1 小時",note:"可安排附近午餐。",map:"Wat Pho"},
{time:"14:30",title:"ICONSIAM",transport:"船 / BTS / 叫車",stay:"約 2.5 小時",note:"商場、河景、室內備案。",map:"ICONSIAM"},
{time:"16:30",title:"Yenly Yours",transport:"ICONSIAM 內或分店",stay:"約 30 分鐘",note:"芒果甜點。",map:"Yenly Yours ICONSIAM"},
{time:"18:30",title:"Asiatique",transport:"船 / 叫車",stay:"約 1.5 小時",note:"河岸夜景、晚餐、逛街。",map:"Asiatique The Riverfront"},
{time:"20:00",title:"Calypso 人妖秀",transport:"Asiatique 內",stay:"約 1.5 小時",note:"確認場次與票券時間。",map:"Calypso Cabaret Bangkok"}]},
{date:"6/29（一）",title:"Day6 補貨與返台",items:[
{time:"10:00",title:"Big C 補貨",transport:"叫車 / BTS",stay:"約 1.5 小時",note:"伴手禮最後採買，注意行李重量。",map:"Big C Bangkok"},
{time:"12:00",title:"回飯店拿行李",transport:"叫車",stay:"約 40 分鐘",note:"檢查護照、錢包、充電器、退房。",map:"Diya Hotel Srinakarin"},
{time:"13:00",title:"前往 BKK 機場",transport:"叫車",stay:"約 1–1.5 小時",note:"預留塞車與退稅時間。",map:"BKK Airport"},
{time:"15:30",title:"回台灣",transport:"航班",stay:"—",note:"起飛前確認登機門。",map:""}]}],
expenses:[],
lists:{
"必吃清單":["芒果糯米飯","船麵","泰奶","Polo Fried Chicken","Mr Joe 脆皮豬","唐人街小吃","Yenly Yours"],
"Big C 必買清單":["Pocky 泰國限定","小老闆海苔","泰奶粉","Mama 麵","榴槤乾","青草膏","防蚊液"],
"水門市場清單":["平價服飾","包包","飾品","拖鞋","拍照小物"],
"洽圖洽清單":["香氛","衣服","手作小物","杯套","耳環","寵物用品"],
"三聘市場清單":["髮飾","耳環","手機掛繩","貼紙","包裝袋","小禮物"],
"行李清單":["護照","機票截圖","保險資料","信用卡","泰銖現金","行動電源","雨傘","防曬","轉接頭","常備藥","薄外套"]
},
checks:{}
};
let data=JSON.parse(localStorage.getItem(STORE)||"null")||defaultData,editIndex=null;
function save(){localStorage.setItem(STORE,JSON.stringify(data))}
function $(id){return document.getElementById(id)}
function showSec(id){document.querySelectorAll(".section").forEach(s=>s.classList.remove("active"));$(id).classList.add("active");document.querySelectorAll(".nav button").forEach(b=>b.classList.remove("active"));[...document.querySelectorAll(".nav button")].find(b=>b.textContent.includes({home:"首頁",itinerary:"行程",budget:"預算",lists:"清單",tools:"工具"}[id])).classList.add("active");renderAll();scrollTo(0,0)}
function renderAll(){document.documentElement.dataset.theme=data.theme;renderHome();renderDays();renderBudget();renderLists();renderTools();save()}
function renderHome(){
let target=new Date("2026-06-24T12:10:00+08:00"),now=new Date(),diff=target-now;
$("countdown").textContent=diff>0?Math.ceil(diff/864e5)+" 天":"旅行中";
let idx=Math.min(Math.max(Math.floor((now-new Date("2026-06-24T00:00:00+08:00"))/864e5),0),5);
$("todayLabel").textContent=data.days[idx].date;
$("todayPlan").innerHTML=data.days[idx].items.slice(0,4).map(i=>`<div class="item"><div class="time">${i.time}</div><div class="itembody"><h3>${i.title}</h3><div class="meta">${i.note}</div></div></div>`).join("");
}
function renderDays(){
$("dayTabs").innerHTML=data.days.map((d,i)=>`<button class="daytab ${i===data.activeDay?'active':''}" onclick="data.activeDay=${i};renderAll()"><b>Day${i+1}</b><br>${d.date.split("（")[0]}</button>`).join("");
let d=data.days[data.activeDay];$("dayTitle").textContent=d.title;
let q=($("search").value||"").toLowerCase();
$("timeline").innerHTML=d.items.map((i,idx)=>({...i,idx})).filter(i=>(i.title+i.note+i.transport).toLowerCase().includes(q)).map(i=>`<div class="item" draggable="true" ondragstart="dragStart(event,${i.idx})" ondragover="event.preventDefault()" ondrop="dropItem(event,${i.idx})"><div class="time">${i.time}</div><div class="itembody"><h3>${i.title}</h3><div class="meta">🚗 ${i.transport||"自由移動"}<br>⏱️ ${i.stay||"彈性"}<br>📝 ${i.note||""}</div><div class="actions">${i.map?`<button class="mapbtn" onclick="openMap('${encodeURIComponent(i.map)}')">Google Maps</button>`:""}<button class="smallbtn" onclick="openForm(${i.idx})">編輯</button><button class="smallbtn" onclick="delItem(${i.idx})">刪除</button></div></div></div>`).join("");
}
function openMap(q){if(!q)return;window.open("https://www.google.com/maps/search/?api=1&query="+q,"_blank")}
function openForm(idx=null){editIndex=idx;$("formBox").style.display="block";let it=idx!==null?data.days[data.activeDay].items[idx]:{time:"",title:"",transport:"",stay:"",note:"",map:""};$("formTitle").textContent=idx!==null?"編輯行程":"新增行程";["Time","Title","Transport","Stay","Note","Map"].forEach(k=>$("f"+k).value=it[k.toLowerCase()]||"")}
function closeForm(){$("formBox").style.display="none";editIndex=null}
function saveItem(){let it={time:fTime.value,title:fTitle.value,transport:fTransport.value,stay:fStay.value,note:fNote.value,map:fMap.value};if(!it.title)return;if(editIndex!==null)data.days[data.activeDay].items[editIndex]=it;else data.days[data.activeDay].items.push(it);closeForm();renderAll()}
function delItem(i){if(confirm("刪除此行程？")){data.days[data.activeDay].items.splice(i,1);renderAll()}}
let dragI=null;function dragStart(e,i){dragI=i}function dropItem(e,i){let arr=data.days[data.activeDay].items,m=arr.splice(dragI,1)[0];arr.splice(i,0,m);renderAll()}
$("search").addEventListener("input",renderDays);
$("themeBtn").onclick=()=>{data.theme=data.theme==="dark"?"light":"dark";$("themeBtn").textContent=data.theme==="dark"?"☀️":"🌙";renderAll()};
function bindMoney(){
["bTHB","bTWD","bUSD"].forEach(id=>$(id).oninput=e=>{
let thb=0;if(id==="bTHB")thb=+e.target.value;if(id==="bTWD")thb=+e.target.value/data.rates.twd;if(id==="bUSD")thb=+e.target.value*data.rates.usd;
if(document.activeElement.id!=="bTHB")$("bTHB").value=thb?thb.toFixed(0):"";
if(document.activeElement.id!=="bTWD")$("bTWD").value=thb?(thb*data.rates.twd).toFixed(0):"";
if(document.activeElement.id!=="bUSD")$("bUSD").value=thb?(thb/data.rates.usd).toFixed(2):"";
});
["rateTWD","rateUSD"].forEach(id=>$(id).oninput=e=>{data.rates[id==="rateTWD"?"twd":"usd"]=+e.target.value||1;save()});
}
function addExpense(){let thb=+$("bTHB").value;if(!$("bName").value||!thb)return;data.expenses.push({name:bName.value,cat:bCat.value,thb});["bName","bTHB","bTWD","bUSD"].forEach(id=>$(id).value="");renderAll()}
function renderBudget(){
$("rateTWD").value=data.rates.twd;$("rateUSD").value=data.rates.usd;
let sum=data.expenses.reduce((a,e)=>a+e.thb,0);$("sumTHB").textContent=sum.toFixed(0);$("sumTWD").textContent=(sum*data.rates.twd).toFixed(0);$("sumUSD").textContent=(sum/data.rates.usd).toFixed(2);
$("expenses").innerHTML=data.expenses.map((e,i)=>`<div class="listitem"><div style="flex:1"><b>${e.name}</b><div class="meta">${e.cat}｜${e.thb.toFixed(0)} THB｜${(e.thb*data.rates.twd).toFixed(0)} TWD</div></div><button class="smallbtn" onclick="data.expenses.splice(${i},1);renderAll()">刪除</button></div>`).join("");
drawChart();
}
function drawChart(){let c=$("chart"),ctx=c.getContext("2d"),cats=["美食","交通","購物","門票","其他"],vals=cats.map(cat=>data.expenses.filter(e=>e.cat===cat).reduce((a,e)=>a+e.thb,0)),sum=vals.reduce((a,b)=>a+b,0),start=-Math.PI/2;ctx.clearRect(0,0,220,220);if(!sum){ctx.fillStyle=getComputedStyle(document.documentElement).getPropertyValue("--muted");ctx.textAlign="center";ctx.fillText("尚無花費",110,110);return}vals.forEach((v,i)=>{let ang=v/sum*Math.PI*2;ctx.beginPath();ctx.moveTo(110,110);ctx.arc(110,110,90,start,start+ang);ctx.closePath();ctx.fillStyle=["#ff8a6a","#ffb199","#ffd166","#cdb4db","#a8dadc"][i];ctx.fill();start+=ang});ctx.fillStyle=getComputedStyle(document.documentElement).getPropertyValue("--text");ctx.textAlign="center";ctx.fillText("分類比例",110,112)}
function renderLists(){
$("listsWrap").innerHTML=Object.keys(data.lists).map(name=>{let arr=data.lists[name],done=arr.filter(x=>data.checks[name+"_"+x]).length,p=arr.length?done/arr.length*100:0;return `<div class="card"><div class="row"><h2>${name}</h2><span class="pill">${done}/${arr.length}</span></div><div class="progress"><div class="bar" style="width:${p}%"></div></div><div>${arr.map((x,i)=>`<div class="listitem ${data.checks[name+"_"+x]?'done':''}"><input class="check" type="checkbox" ${data.checks[name+"_"+x]?'checked':''} onchange="data.checks['${name+"_"+x}']=this.checked;renderAll()"><span style="flex:1">${x}</span><button class="smallbtn" onclick="data.lists['${name}'].splice(${i},1);renderAll()">刪除</button></div>`).join("")}</div><input id="add_${name}" placeholder="新增${name}項目"><button class="smallbtn primary" onclick="addListItem('${name}')">新增</button></div>`}).join("");
}
function addListItem(name){let el=$("add_"+name),v=el.value.trim();if(v){data.lists[name].push(v);el.value="";renderAll()}}
function toggleRain(){data.rain=!data.rain;renderAll()}
function renderTools(){
$("rainState").textContent=data.rain?"ON":"OFF";$("rainBox").style.display=data.rain?"block":"none";
let conflicts=[];data.days.forEach(d=>{let seen={};d.items.forEach(i=>{if(seen[i.time])conflicts.push(`${d.date} ${i.time}：${seen[i.time]} / ${i.title}`);seen[i.time]=i.title})});
$("conflicts").innerHTML=conflicts.length?conflicts.join("<br>"):"目前沒有偵測到相同時間的行程。";
$("photoGrid").innerHTML=data.photos.map((p,i)=>`<div><img src="${p}"><button class="smallbtn" onclick="data.photos.splice(${i},1);renderAll()">刪除</button></div>`).join("");
}
function savePhotos(e){[...e.target.files].forEach(file=>{let r=new FileReader();r.onload=()=>{data.photos.push(r.result);renderAll()};r.readAsDataURL(file)})}
function exportJSON(){let a=document.createElement("a");a.href=URL.createObjectURL(new Blob([JSON.stringify(data,null,2)],{type:"application/json"}));a.download="bangkok-trip-data.json";a.click()}
function importJSON(e){let f=e.target.files[0];if(!f)return;let r=new FileReader();r.onload=()=>{try{data=JSON.parse(r.result);renderAll()}catch{alert("JSON 格式錯誤")}};r.readAsText(f)}
function resetData(){if(confirm("重置為預設資料？")){localStorage.removeItem(STORE);data=JSON.parse(JSON.stringify(defaultData));renderAll()}}
if("serviceWorker"in navigator){let sw=`self.addEventListener('install',e=>self.skipWaiting());self.addEventListener('activate',e=>self.clients.claim());self.addEventListener('fetch',e=>e.respondWith(fetch(e.request).catch(()=>caches.match(e.request).then(r=>r||new Response('Offline',{headers:{'Content-Type':'text/plain'}})))))`;navigator.serviceWorker.register(URL.createObjectURL(new Blob([sw],{type:"text/javascript"})))}
bindMoney();renderAll();
function luxuryUpgrade(){
  const home=document.getElementById("home");
  if(home && !document.getElementById("luxuryHome")){
    home.insertAdjacentHTML("afterbegin",`
      <div class="card homeUpgrade" id="luxuryHome">
        <div class="row">
          <div>
            <div class="meta">距離出發</div>
            <div class="bigNumber" id="luxDays">--</div>
          </div>
          <div style="font-size:46px">🛫</div>
        </div>
      </div>

   <div class="card">
        <h2>航班資訊</h2>
        <div class="flightCard">
          <div><div class="meta">抵達</div><b>BKK</b><br><span>6/24 12:10</span></div>
          <div class="planeLine">✈️</div>
          <div><div class="meta">回台灣</div><b>Taiwan</b><br><span>6/29 15:30</span></div>
        </div>
      </div>

      <div class="card">
        <h2>旅行儀表板</h2>
        <div class="toolGrid">
          <div class="toolTile"><b>🏨 飯店</b><span class="meta">Diya Hotel Srinakarin</span></div>
          <div class="toolTile"><b>☁️ 天氣</b><span class="meta">炎熱、午後雷陣雨機率高</span></div>
          <div class="toolTile"><b>💱 匯率</b><span class="meta">可在預算頁手動調整</span></div>
          <div class="toolTile"><b>📌 重點</b><span class="meta">泰服、美甲、大城、Calypso</span></div>
        </div>
      </div>
    `);
  }

  const d=new Date("2026-06-24T12:10:00+08:00")-new Date();
  const luxDays=document.getElementById("luxDays");
  if(luxDays) luxDays.textContent=d>0?Math.ceil(d/86400000)+" 天":"旅行中";

  const tools=document.getElementById("tools");
  const dataCard=[...document.querySelectorAll(".card")].find(c=>c.innerText.includes("資料管理")&&c.innerText.includes("匯出 JSON"));
  if(tools && dataCard && !document.getElementById("movedDataBox")){
    const clone=dataCard.cloneNode(true);
    clone.id="movedDataBox";
    clone.querySelector("h2").textContent="設定與資料備份";
    tools.appendChild(clone);
    dataCard.classList.add("settingsOnly");
  }
}

const oldRenderAll=renderAll;
renderAll=function(){
  oldRenderAll();
  luxuryUpgrade();
};
luxuryUpgrade();
function renderBudget(){
  data.rates.twd=data.rates.twd||0.88;
  data.rates.usd=data.rates.usd||36.7;
  data.budget=data.budget||0;

  $("rateTWD").value=data.rates.twd;
  $("rateUSD").value=data.rates.usd;

  const oldBudgetBox=document.getElementById("budgetControlBox");
  if(!oldBudgetBox){
    const firstCard=document.querySelector("#budget .card");
    firstCard.insertAdjacentHTML("afterend",`
      <div class="card" id="budgetControlBox">
        <h2>旅費預算設定</h2>
        <input id="tripBudgetInput" type="number" placeholder="輸入總預算 THB，例如 15000">
        <button class="smallbtn primary" onclick="setTripBudget()">儲存預算</button>
      </div>
    `);
  }

  const tripBudgetInput=document.getElementById("tripBudgetInput");
  if(tripBudgetInput) tripBudgetInput.value=data.budget||"";

  const sum=data.expenses.reduce((a,e)=>a+Number(e.thb||0),0);
  const budget=Number(data.budget||0);
  const left=budget?Math.max(0,budget-sum):0;
  const used=budget?Math.min(100,sum/budget*100):0;

  $("sumTHB").textContent=sum.toFixed(0);
  $("sumTWD").textContent=(sum*data.rates.twd).toFixed(0);
  $("sumUSD").textContent=(sum/data.rates.usd).toFixed(2);

  let progressBox=document.getElementById("budgetProgressBox");
  if(!progressBox){
    document.querySelector("#budget .canvaswrap").insertAdjacentHTML("beforebegin",`
      <div id="budgetProgressBox"></div>
    `);
    progressBox=document.getElementById("budgetProgressBox");
  }

  progressBox.innerHTML=budget?`
    <div style="margin:14px 0">
      <div class="row">
        <b>旅費預算 ${budget.toFixed(0)} THB</b>
        <span class="pill">剩餘 ${left.toFixed(0)} THB</span>
      </div>
      <div class="budgetProgress">
        <div class="budgetProgressBar" style="width:${used}%"></div>
      </div>
      <div class="meta">已使用 ${used.toFixed(1)}%</div>
    </div>
  `:`
    <div class="notice" style="margin:12px 0">尚未設定旅費總預算，可在上方輸入 THB 預算。</div>
  `;

  drawChart();

  const icons={美食:"🍜",交通:"🚕",購物:"🛍️",門票:"🎟️",其他:"✨"};

  $("expenses").innerHTML=data.expenses.map((e,i)=>`
    <div class="expenseCard">
      <b>${icons[e.cat]||"✨"} ${e.name}</b>
      <div class="expenseCat">${e.cat}｜${Number(e.thb).toFixed(0)} THB｜約 NT$${(e.thb*data.rates.twd).toFixed(0)}｜USD ${(e.thb/data.rates.usd).toFixed(2)}</div>
      <button class="trashBtn" onclick="data.expenses.splice(${i},1);renderAll()">🗑️</button>
    </div>
  `).join("") || `<div class="meta">尚無花費。</div>`;
}

function setTripBudget(){
  const v=Number(document.getElementById("tripBudgetInput").value||0);
  data.budget=v;
  save();
  renderAll();
}
data.members=data.members||[{name:"我",id:"me"}];

function ensureSplitUI(){
  if(document.getElementById("splitSection"))return;
  const budget=document.getElementById("budget");
  budget.insertAdjacentHTML("beforeend",`
    <div class="card" id="splitSection">
      <h2>成員與分帳</h2>

      <div class="superrichBox">
        <b>💱 SuperRich 匯率參考</b>
        <p class="meta">可開啟 SuperRich 查最新匯率，再手動填入上方匯率欄位。</p>
        <button class="smallbtn primary" onclick="window.open('https://www.superrichthailand.com/','_blank')">開啟 SuperRich</button>
      </div>

      <h3>旅行成員</h3>
      <div id="membersList"></div>
      <input id="newMemberName" placeholder="新增成員名稱，例如 男友、朋友A">
      <button class="smallbtn primary" onclick="addMember()">新增成員</button>

      <h3 style="margin-top:18px">新增分帳支出</h3>
      <input id="splitName" placeholder="項目，例如 晚餐、Bolt、門票">
      <input id="splitTHB" type="number" placeholder="金額 THB">
      <select id="splitPayer"></select>
      <div class="meta">選擇要一起分攤的人：</div>
      <div id="splitPeople" class="splitBox"></div>
      <button class="smallbtn primary" onclick="addSplitExpense()">新增分帳</button>

      <h3 style="margin-top:18px">誰要給誰多少錢</h3>
      <div id="settleResult"></div>
    </div>
  `);
}

function addMember(){
  const name=document.getElementById("newMemberName").value.trim();
  if(!name)return;
  data.members.push({name,id:"m"+Date.now()});
  document.getElementById("newMemberName").value="";
  save();
  renderAll();
}

function removeMember(id){
  if(id==="me"){alert("不能刪除自己");return;}
  data.members=data.members.filter(m=>m.id!==id);
  save();
renderAll();
}
function addSplitExpense(){
  const name=document.getElementById("splitName").value.trim();
  const thb=Number(document.getElementById("splitTHB").value||0);
  const payer=document.getElementById("splitPayer").value;
  const people=[...document.querySelectorAll(".splitPerson:checked")].map(x=>x.value);
  if(!name||!thb||!payer||!people.length){alert("請填完整分帳資料");return;}

  data.expenses.push({
    name,
    cat:"其他",
    thb,
    payer,
    splitPeople:people,
    isSplit:true
  });

  document.getElementById("splitName").value="";
  document.getElementById("splitTHB").value="";
  save();
  renderAll();
}

function renderSplit(){
  ensureSplitUI();

  document.getElementById("membersList").innerHTML=data.members.map(m=>`
    <div class="memberCard memberRow">
      <div class="memberAvatar">${m.name.slice(0,1)}</div>
      <div style="flex:1">
        <b>${m.name}</b>
        <div class="meta">${m.id==="me"?"旅行建立者":"受邀成員"}</div>
      </div>
      <button class="smallbtn" onclick="removeMember('${m.id}')">刪除</button>
    </div>
  `).join("");

  document.getElementById("splitPayer").innerHTML=data.members.map(m=>`
    <option value="${m.id}">付款人：${m.name}</option>
  `).join("");

  document.getElementById("splitPeople").innerHTML=data.members.map(m=>`
    <label class="memberCheck">
      <input class="splitPerson" type="checkbox" value="${m.id}" checked>
      ${m.name}
    </label>
  `).join("");

  const balance={};
  data.members.forEach(m=>balance[m.id]=0);

  data.expenses.filter(e=>e.isSplit).forEach(e=>{
    const people=e.splitPeople||[];
    const each=Number(e.thb||0)/people.length;
    balance[e.payer]+=Number(e.thb||0);
    people.forEach(id=>balance[id]-=each);
  });

  let debtors=Object.entries(balance).filter(([id,v])=>v<-.01).map(([id,v])=>({id,amount:-v}));
  let creditors=Object.entries(balance).filter(([id,v])=>v>.01).map(([id,v])=>({id,amount:v}));
  const results=[];

  debtors.forEach(d=>{
    creditors.forEach(c=>{
      if(d.amount<=0||c.amount<=0)return;
      const pay=Math.min(d.amount,c.amount);
      results.push({from:d.id,to:c.id,amount:pay});
      d.amount-=pay;
      c.amount-=pay;
    });
  });

  const getName=id=>(data.members.find(m=>m.id===id)||{}).name||"未知成員";

  document.getElementById("settleResult").innerHTML=results.length?results.map(r=>`
    <div class="settleCard">
      <b>${getName(r.from)}</b> 要給 <b>${getName(r.to)}</b><br>
      ${r.amount.toFixed(0)} THB ｜約 NT$${(r.amount*(data.rates.twd||0.88)).toFixed(0)}
    </div>
  `).join(""):`<div class="notice">目前沒有需要分帳的款項。</div>`;
}

const oldRenderAllSplit=renderAll;
renderAll=function(){
  oldRenderAllSplit();
  renderSplit();
};

renderAll();
loadBangkokWeather();
async function loadBangkokWeather(){

  const weatherCard = `
  <div class="card" id="weatherCard">
    <h2>☁️ 曼谷天氣</h2>
    <div id="weatherContent">
      讀取天氣中...
    </div>
  </div>
  `;

  if(!document.getElementById("weatherCard")){
    const home=document.getElementById("home");
    const firstCard=home.querySelector(".card");
    firstCard.insertAdjacentHTML("afterend",weatherCard);
  }

  try{

    const url =
    "https://api.open-meteo.com/v1/forecast?latitude=13.7563&longitude=100.5018&current=temperature_2m,weather_code&daily=temperature_2m_max,temperature_2m_min,precipitation_probability_max&timezone=Asia%2FBangkok";

    const res = await fetch(url);
    const data = await res.json();

    const currentTemp =
      data.current.temperature_2m;

    const days =
      data.daily.time;

    const rain =
      data.daily.precipitation_probability_max;

    let html=`
      <div style="font-size:28px;font-weight:700">
        🌡️ ${currentTemp}°C
      </div>
      <div class="meta">
        Bangkok Current Weather
      </div>
      <hr style="margin:12px 0;border:none;border-top:1px solid var(--line)">
    `;

    for(let i=0;i<6;i++){

      const d=new Date(days[i]);

      html+=`
      <div class="row" style="margin:6px 0">
        <span>${d.getMonth()+1}/${d.getDate()}</span>
        <span>
          🌧️ ${rain[i]}%
        </span>
      </div>
      `;
    }

    const maxRain=Math.max(...rain.slice(0,6));

    if(maxRain>=60){
      html+=`
      <div class="notice" style="margin-top:12px">
      ⚠️ 旅行期間有高降雨機率，建議攜帶雨傘。
      </div>
      `;
    }

    document.getElementById("weatherContent").innerHTML=html;

  }catch(err){

    document.getElementById("weatherContent").innerHTML=
      "天氣資料載入失敗";
  }
}
function addMapMode(){

  const itineraryPage=document.getElementById("itinerary");

  if(!itineraryPage) return;

  if(document.getElementById("mapModeSection")) return;

  const box=document.createElement("div");

  box.className="card";
  box.id="mapModeSection";

  box.innerHTML=`
    <h2>📍 地圖模式</h2>

    <select id="mapDaySelect"></select>

    <div id="mapRouteResult"></div>
  `;

  itineraryPage.appendChild(box);

  const select=document.getElementById("mapDaySelect");

  data.days.forEach((d,i)=>{
    const op=document.createElement("option");
    op.value=i;
    op.textContent=d.title;
    select.appendChild(op);
  });

  select.addEventListener("change",renderMapRoute);

  renderMapRoute();
}

function renderMapRoute(){

  const routeBox=document.getElementById("mapRouteResult");

  if(!routeBox) return;

  const dayIndex=
    Number(document.getElementById("mapDaySelect").value||0);

  const day=data.days[dayIndex];

  let html=`<div class="mapModeCard">`;

  day.items.forEach((item,index)=>{

    html+=`
      <div class="routeItem">

        <div>

          <div class="routeDot"></div>

          ${
            index<day.items.length-1
            ? `<div class="routeLine"></div>`
            : ``
          }

        </div>

        <div class="routePlace">

          <b>${item.title}</b>

          <div class="meta">
            ${item.time||""}
          </div>

          <div class="routeTransport">
            🚗 ${item.transport||"自由移動"}
          </div>

        </div>

      </div>
    `;
  });

  html+=`</div>`;

  routeBox.innerHTML=html;
}

setTimeout(()=>{
  addMapMode();
},1000);
data.footprints=data.footprints||{};
data.achievements=data.achievements||[];

function initTravelMemory(){

  if(document.getElementById("travelMemorySection")) return;

  const tools=document.getElementById("tools");

  const card=document.createElement("div");

  card.className="card";
  card.id="travelMemorySection";

  card.innerHTML=`
    <h2>📍 足跡打卡</h2>

    <div id="footprintList"></div>

    <h2 style="margin-top:20px">🏆 成就系統</h2>

    <div id="achievementList"></div>

    <h2 style="margin-top:20px">🤖 AI旅行回顧</h2>

    <button class="smallbtn primary" onclick="generateMemory()">
      生成旅行回顧
    </button>

    <div id="memoryResult"></div>
  `;

  tools.appendChild(card);

  renderFootprints();
}

function renderFootprints(){

  const places=[];

  data.days.forEach(day=>{
    day.items.forEach(item=>{
      places.push(item.title);
    });
  });

  const unique=[...new Set(places)];

  document.getElementById("footprintList").innerHTML=
  unique.map(place=>{

    const done=data.footprints[place];

    return `
      <div class="footprintCard ${done?'footprintDone':''}">
        <b>${place}</b>

        <div class="meta">
          ${done?'✅ 已完成打卡':'❌ 尚未打卡'}
        </div>

        <input
          type="file"
          accept="image/*"
          onchange="footprintUpload(event,'${place.replace(/'/g,'')}')">

      </div>
    `;
  }).join("");

  checkAchievements();
}

function footprintUpload(event,place){

  const file=event.target.files[0];

  if(!file) return;

  const reader=new FileReader();

  reader.onload=function(){

    data.footprints[place]=reader.result;

    save();

    renderFootprints();
  };

  reader.readAsDataURL(file);
}

function checkAchievements(){

  const completed=
    Object.keys(data.footprints).length;

  const achievements=[];

  if(completed>=3)
    achievements.push("🏆 初級旅人");

  if(completed>=8)
    achievements.push("🏆 景點達人");

  if(completed>=12)
    achievements.push("🏆 曼谷探險家");

  if(data.footprints["鄭王廟"] &&
     data.footprints["大皇宮"] &&
     data.footprints["臥佛寺"])
    achievements.push("🏆 寺廟巡禮");

  if(data.footprints["JODD FAIRS"] &&
     data.footprints["唐人街"])
    achievements.push("🏆 夜市王");

  if(data.footprints["大城獅子動物園"] &&
     data.footprints["Wat Mahathat"])
    achievements.push("🏆 大城探險家");

  data.achievements=achievements;

  document.getElementById("achievementList").innerHTML=
    achievements.length
    ? achievements.map(a=>`
      <div class="achievementCard">
        ${a}
      </div>
    `).join("")
    : `<div class="meta">尚未解鎖成就</div>`;
}

function generateMemory(){

  const photoCount=
    Object.keys(data.footprints).length;

  const expense=
    data.expenses.reduce(
      (a,b)=>a+Number(b.thb||0),0
    );

  document.getElementById("memoryResult").innerHTML=`
    <div class="memoryCard">

      <h3>✈️ 2026 曼谷自由行</h3>

      <p>
      完成景點：
      ${photoCount} 個
      </p>

      <p>
      總花費：
      ${expense.toFixed(0)} THB
      </p>

      <p>
      解鎖成就：
      ${data.achievements.length} 個
      </p>

      <p>
      已造訪：
      ${Object.keys(data.footprints).join("、") || "尚無"}
      </p>

    </div>
  `;
}

setTimeout(()=>{
  initTravelMemory();
},1500);
function initTravelAI(){

  if(document.getElementById("travelAI")) return;

  document.body.insertAdjacentHTML("beforeend",`

  <div class="aiPanel" id="travelAI">

    <div style="padding:12px;font-weight:700;border-bottom:1px solid var(--line)">
      🤖 曼谷旅行助理
    </div>

    <div class="aiMessages" id="aiMessages">

      <div class="aiMsg aiBot">
        嗨！可以問我：
        <br>• 今天行程
        <br>• Day2 行程
        <br>• 誰欠誰錢
        <br>• 今日花費
        <br>• Big C 必買
      </div>

    </div>

    <div class="aiInput">
      <input id="aiQuestion" placeholder="輸入問題...">
      <button class="smallbtn primary" onclick="askTravelAI()">送出</button>
    </div>

  </div>

  <div class="aiCard">
    <button class="aiBtn" onclick="toggleTravelAI()">🤖</button>
  </div>

  `);
}

function toggleTravelAI(){

  const panel=document.getElementById("travelAI");

  panel.style.display=
    panel.style.display==="flex"
    ? "none"
    : "flex";
}

function addAIMessage(text,type){

  const box=document.getElementById("aiMessages");

  box.innerHTML+=`
    <div class="aiMsg ${type}">
      ${text}
    </div>
  `;

  box.scrollTop=box.scrollHeight;
}

function askTravelAI(){

  const input=document.getElementById("aiQuestion");

  const q=input.value.trim();

  if(!q) return;

  addAIMessage(q,"aiUser");

  const answer=getTravelAnswer(q);

  setTimeout(()=>{
    addAIMessage(answer,"aiBot");
  },300);

  input.value="";
}

function getTravelAnswer(q){

  q=q.toLowerCase();

  if(q.includes("今天") && q.includes("行程")){

    const day=data.days[data.activeDay];

    return day.items
      .map(x=>`${x.time} ${x.title}`)
      .join("<br>");
  }

  if(q.includes("day1")) return data.days[0].items.map(x=>x.title).join(" → ");

  if(q.includes("day2")) return data.days[1].items.map(x=>x.title).join(" → ");

  if(q.includes("day3")) return data.days[2].items.map(x=>x.title).join(" → ");

  if(q.includes("day4")) return data.days[3].items.map(x=>x.title).join(" → ");

  if(q.includes("day5")) return data.days[4].items.map(x=>x.title).join(" → ");

  if(q.includes("day6")) return data.days[5].items.map(x=>x.title).join(" → ");

  if(q.includes("big c")){

    return (data.lists["Big C 必買清單"]||[])
      .join("、");
  }

  if(q.includes("花費")){

    const total=data.expenses.reduce(
      (a,b)=>a+Number(b.thb||0),0
    );

    return `目前總花費 ${total.toFixed(0)} THB`;
  }

  if(q.includes("大城")){

    return "大城建議優先包車，景點較分散，Bolt 作為備案。";
  }

  if(q.includes("下雨")){

    return "可改去 ICONSIAM、CentralWorld、Terminal 21、Health Land。";
  }

  return `
  我可以回答：
  <br>• 今天行程
  <br>• Day1~Day6
  <br>• Big C 必買
  <br>• 花費
  <br>• 下雨怎麼辦
  <br>• 大城交通
  `;
}

setTimeout(()=>{
  initTravelAI();
},2000);
function initTravelStats(){

  if(document.getElementById("travelStatsSection")) return;

  const tools=document.getElementById("tools");

  const card=document.createElement("div");

  card.className="card";
  card.id="travelStatsSection";

  card.innerHTML=`
    <h2>📊 旅行統計</h2>

    <div id="travelStatsResult"></div>

    <h2 style="margin-top:20px">🏆 紀念證書</h2>

    <button class="smallbtn primary"
      onclick="generateCertificate()">
      生成紀念證書
    </button>

    <div id="certificateResult"></div>
  `;

  tools.appendChild(card);

  renderTravelStats();
}

function renderTravelStats(){

  const places=
    Object.keys(data.footprints||{});

  const photoCount=
    places.length;

  const totalExpense=
    (data.expenses||[])
      .reduce((a,b)=>a+Number(b.thb||0),0);

  const achievementCount=
    (data.achievements||[]).length;

  const totalPlanned=
    data.days.reduce(
      (sum,d)=>sum+d.items.length,
      0
    );

  const completion=
    totalPlanned
      ? Math.round(
          photoCount/totalPlanned*100
        )
      : 0;

  document.getElementById(
    "travelStatsResult"
  ).innerHTML=`

    <div class="travelStatsCard">

      <div class="statGrid">

        <div class="statItem">
          <b>📍 景點完成</b><br>
          ${photoCount}
        </div>

        <div class="statItem">
          <b>🏆 成就</b><br>
          ${achievementCount}
        </div>

        <div class="statItem">
          <b>💰 花費</b><br>
          ${totalExpense.toFixed(0)} THB
        </div>

        <div class="statItem">
          <b>✅ 完成率</b><br>
          ${completion}%
        </div>

      </div>

    </div>
  `;
}

function generateCertificate(){

  const places=
    Object.keys(data.footprints||{});

  const totalExpense=
    (data.expenses||[])
      .reduce((a,b)=>a+Number(b.thb||0),0);

  const achievementCount=
    (data.achievements||[]).length;

  const totalPlanned=
    data.days.reduce(
      (sum,d)=>sum+d.items.length,
      0
    );

  const completion=
    totalPlanned
      ? Math.round(
          places.length/totalPlanned*100
        )
      : 0;

  document.getElementById(
    "certificateResult"
  ).innerHTML=`

    <div class="certificateCard">

      <div class="certificateTitle">
        🏆 Bangkok Adventure Certificate
      </div>

      <p>
        恭喜完成
      </p>

      <h2>
        2026 曼谷自由行
      </h2>

      <p>
        2026/06/24 ～ 2026/06/29
      </p>

      <hr>

      <p>
        景點完成：
        ${places.length}
      </p>

      <p>
        花費：
        ${totalExpense.toFixed(0)} THB
      </p>

      <p>
        成就：
        ${achievementCount} 個
      </p>

      <p>
        完成率：
        ${completion}%
      </p>

      <div style="margin-top:14px">

        ${(data.achievements||[])
          .join("<br>")}

      </div>

      <div style="
        margin-top:20px;
        font-size:12px;
        opacity:.7;
      ">
        Generated by Travel App
      </div>

    </div>
  `;
}

setTimeout(()=>{
  initTravelStats();
},2500);
/* ===== Supabase ===== */

const SUPABASE_URL="https://ajgqtsdczzgvuqorulbd.supabase.co";

const SUPABASE_KEY="sb_publishable_VvQst4oND6bNOtj3m06-rQ_z6XHfYCx";

const sb = window.supabase.createClient(
  SUPABASE_URL,
  SUPABASE_KEY
);

console.log("Supabase Connected");
</script>
</body>
</html>
