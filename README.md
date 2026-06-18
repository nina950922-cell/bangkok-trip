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
</style>
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
</script>
</body>
</html>
