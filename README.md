<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<meta name="theme-color" content="#ff9f7a">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="default">
<meta name="apple-mobile-web-app-title" content="Bangkok 2026">
<title>2026 曼谷自由行 Travel App</title>
<style>
:root{--bg:#fff7f3;--card:#fff;--text:#30231f;--muted:#8d746b;--brand:#ff9f7a;--brand2:#ffd1bd;--accent:#ff6f91;--line:#f2d9cf;--shadow:0 12px 35px rgba(130,70,45,.12);--good:#32b47b;--warn:#f5a623;--bad:#ff5a5f;--nav:rgba(255,255,255,.88)}
.dark{--bg:#171211;--card:#241b19;--text:#fff3ee;--muted:#c7aaa0;--brand:#ff9f7a;--brand2:#5a332a;--accent:#ff8ead;--line:#3c2a26;--shadow:0 12px 35px rgba(0,0,0,.35);--nav:rgba(36,27,25,.88)}
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
html{scroll-behavior:smooth}
body{margin:0;font-family:-apple-system,BlinkMacSystemFont,"SF Pro Display","Noto Sans TC",Arial,sans-serif;background:radial-gradient(circle at top left,var(--brand2),transparent 36%),var(--bg);color:var(--text);padding:env(safe-area-inset-top) 0 calc(92px + env(safe-area-inset-bottom));}
.app{max-width:560px;margin:auto;min-height:100vh;padding:18px 16px}
.top{display:flex;justify-content:space-between;align-items:center;gap:12px;position:sticky;top:0;z-index:10;padding:8px 0 12px;background:linear-gradient(var(--bg) 70%,transparent)}
.logo{display:flex;align-items:center;gap:10px}.logo .mark{width:44px;height:44px;border-radius:16px;background:linear-gradient(135deg,var(--brand),var(--accent));display:grid;place-items:center;color:white;font-size:22px;box-shadow:var(--shadow)}h1{font-size:20px;margin:0}.sub{font-size:12px;color:var(--muted);margin-top:2px}
.iconbtn,.btn{border:0;border-radius:16px;background:var(--card);color:var(--text);box-shadow:var(--shadow);padding:11px 13px;font-weight:700}
.btn.primary{background:linear-gradient(135deg,var(--brand),var(--accent));color:#fff}.btn.ghost{background:transparent;border:1px solid var(--line);box-shadow:none}.btn.small{padding:8px 10px;font-size:12px;border-radius:12px}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:12px}.card{background:var(--card);border:1px solid var(--line);border-radius:24px;padding:16px;margin:12px 0;box-shadow:var(--shadow);animation:pop .28s ease both}.hero{background:linear-gradient(135deg,var(--brand),#ffc2a3 55%,#ffe8dc);color:#4b2118;overflow:hidden;position:relative}.hero:after{content:"✈︎";position:absolute;right:18px;top:8px;font-size:82px;opacity:.18}.stat{font-size:28px;font-weight:900}.label{font-size:12px;color:var(--muted)}.hero .label{color:#744034}.section-title{font-size:17px;font-weight:900;margin:20px 2px 8px;display:flex;justify-content:space-between;align-items:center}
.tabs{display:flex;gap:8px;overflow:auto;padding:4px 0 10px}.tab{white-space:nowrap;border:0;border-radius:999px;padding:10px 14px;background:var(--card);color:var(--muted);font-weight:800;border:1px solid var(--line)}.tab.active{background:linear-gradient(135deg,var(--brand),var(--accent));color:white}
.timeline{position:relative}.item{display:grid;grid-template-columns:62px 1fr;gap:10px;padding:12px 0;border-bottom:1px solid var(--line)}.time{font-weight:900;color:var(--accent)}.place{font-weight:900}.meta{font-size:12px;color:var(--muted);line-height:1.55}.note{font-size:13px;margin-top:6px;padding:9px;border-radius:14px;background:rgba(255,159,122,.12)}.actions{display:flex;gap:6px;margin-top:8px;flex-wrap:wrap}.pill{display:inline-flex;align-items:center;gap:5px;border-radius:999px;padding:6px 9px;background:rgba(255,159,122,.14);font-size:12px;color:var(--muted);font-weight:700}
input,select,textarea{width:100%;border:1px solid var(--line);background:var(--card);color:var(--text);border-radius:16px;padding:12px;font:inherit;outline:none}textarea{min-height:74px}.form{display:grid;gap:10px}.row{display:grid;grid-template-columns:1fr 1fr;gap:10px}.hidden{display:none!important}
.nav{position:fixed;left:50%;transform:translateX(-50%);bottom:0;z-index:30;width:min(560px,100%);padding:8px 10px calc(8px + env(safe-area-inset-bottom));background:var(--nav);backdrop-filter:blur(18px);border-top:1px solid var(--line);display:grid;grid-template-columns:repeat(6,1fr);gap:4px}.nav button{border:0;background:transparent;color:var(--muted);font-size:10px;font-weight:800;padding:7px 2px;border-radius:16px}.nav b{display:block;font-size:20px;margin-bottom:2px}.nav button.active{color:var(--accent);background:rgba(255,159,122,.16)}
.check{display:flex;align-items:center;gap:10px;padding:11px;border:1px solid var(--line);border-radius:18px;margin:8px 0;background:var(--card)}.check input{width:20px;height:20px}.done{text-decoration:line-through;color:var(--muted)}
.progress{height:10px;background:rgba(255,159,122,.18);border-radius:999px;overflow:hidden}.bar{height:100%;background:linear-gradient(90deg,var(--brand),var(--accent));width:0}
.photoGrid{display:grid;grid-template-columns:repeat(3,1fr);gap:8px}.photoGrid img{width:100%;aspect-ratio:1;border-radius:18px;object-fit:cover}
.floatTop{position:fixed;right:16px;bottom:96px;z-index:25;width:46px;height:46px;border-radius:50%;border:0;background:linear-gradient(135deg,var(--brand),var(--accent));color:white;box-shadow:var(--shadow);font-size:20px}
.alert{border-left:5px solid var(--warn);background:rgba(245,166,35,.12);padding:12px;border-radius:16px;margin:10px 0;font-size:13px}.danger{border-left-color:var(--bad);background:rgba(255,90,95,.12)}
.chart{height:180px;display:flex;align-items:end;gap:10px;border-bottom:1px solid var(--line);padding-top:18px}.chart div{flex:1;background:linear-gradient(180deg,var(--accent),var(--brand));border-radius:14px 14px 0 0;min-height:4px;text-align:center;color:white;font-size:10px;padding-top:5px}
@keyframes pop{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:none}}@media print{.nav,.top,.floatTop,.noPrint{display:none!important}body{padding:0;background:white}.card{box-shadow:none;break-inside:avoid}.app{max-width:none}}
</style>
</head>
<body>
<div class="app">
    <main id="home" class="page">
    <section class="card hero"><div class="label">距離出發還有</div><div class="stat" id="countdown">-- 天</div><div>粉橘高級版曼谷小旅行啟動 ♡</div></section>
    <div class="grid">
      <div class="card"><div class="label">去程</div><b>6/24 12:10 抵達 BKK</b></div>
      <div class="card"><div class="label">回程</div><b>6/29 15:30 回台灣</b></div>
      <div class="card"><div class="label">住宿</div><b>Diya Hotel Srinakarin</b><div class="meta">14:00 後入住</div></div>
      <div class="card"><div class="label">預約</div><b>6/25 13:30</b><div class="meta">Take Away Studio 美甲</div></div>
    </div>
    <div class="section-title">今日行程 <button class="btn small" onclick="print()">列印</button></div>
    <div class="card" id="todayPlan"></div>
    <div class="card"><b>☔ 天氣提醒</b><p class="meta">曼谷雨季建議每天帶摺疊傘、防水袋、薄外套。午後雷陣雨時可切換雨天備案。</p><button class="btn primary" onclick="showPage('rain')">開啟雨天備案</button></div>
    <div class="card"><b>花費統計</b><div id="totalBox" class="stat">฿0</div><div class="meta" id="totalFx"></div></div>
  </main>

  <header class="top noPrint">
    <div class="logo"><div class="mark">🌸</div><div><h1>Bangkok Travel App</h1><div class="sub">2026/6/24～6/29 曼谷自由行</div></div></div>
    <button class="iconbtn" onclick="toggleDark()">☾</button>
  </header>
  <main id="plan" class="page hidden">
    <div class="section-title">每日行程 <input id="search" placeholder="搜尋行程…" oninput="renderPlan()" style="max-width:170px"></div>
    <div class="tabs" id="dayTabs"></div>
    <div id="conflicts"></div>
    <div class="card noPrint">
      <div class="form">
        <div class="row"><input id="fTime" placeholder="時間 例 13:30"><input id="fStay" placeholder="停留 例 90分"></div>
        <input id="fPlace" placeholder="地點">
        <div class="row"><input id="fTrans" placeholder="交通"><input id="fMap" placeholder="Google Maps 連結"></div>
        <textarea id="fNote" placeholder="備註"></textarea>
        <button class="btn primary" onclick="saveItem()">新增 / 更新行程</button>
      </div>
    </div>
    <div class="timeline" id="timeline"></div>
  </main>
  <main id="plan" class="page hidden">
    <div class="section-title">每日行程 <input id="search" placeholder="搜尋行程…" oninput="renderPlan()" style="max-width:170px"></div>
    <div class="tabs" id="dayTabs"></div>
    <div id="conflicts"></div>
    <div class="card noPrint">
      <div class="form">
        <div class="row"><input id="fTime" placeholder="時間 例 13:30"><input id="fStay" placeholder="停留 例 90分"></div>
        <input id="fPlace" placeholder="地點">
        <div class="row"><input id="fTrans" placeholder="交通"><input id="fMap" placeholder="Google Maps 連結"></div>
        <textarea id="fNote" placeholder="備註"></textarea>
        <button class="btn primary" onclick="saveItem()">新增 / 更新行程</button>
      </div>
    </div>
    <div class="timeline" id="timeline"></div>
  </main>
  <main id="budget" class="page hidden">
    <div class="section-title">預算系統</div>
    <div class="card form">
      <div class="row"><input id="rateTwd" type="number" step="0.01" value="0.95" onchange="saveRates()"><input id="rateUsd" type="number" step="0.01" value="0.027" onchange="saveRates()"></div>
      <div class="meta">1 THB = TWD / USD，可手動修改</div>
      <div class="row"><input id="amtTHB" type="number" placeholder="THB" oninput="convert('THB')"><input id="amtTWD" type="number" placeholder="TWD" oninput="convert('TWD')"></div>
      <input id="amtUSD" type="number" placeholder="USD" oninput="convert('USD')">
    </div>
    <div class="card form">
      <div class="row"><input id="bName" placeholder="項目"><select id="bCat"><option>美食</option><option>交通</option><option>購物</option><option>門票</option><option>其他</option></select></div>
      <input id="bAmt" type="number" placeholder="金額 THB">
      <button class="btn primary" onclick="addExpense()">加入花費</button>
    </div>
    <div class="card"><b>分類花費</b><div class="chart" id="chart"></div></div>
    <div id="expenses"></div>
  </main>
  <main id="lists" class="page hidden">
    <div class="section-title">必吃清單</div><div class="card" id="foodList"></div>
    <div class="section-title">購物清單</div><div class="card"><div class="progress"><div class="bar" id="shopProg"></div></div><div id="shopList"></div></div>
    <div class="section-title">行李清單</div><div class="card"><div class="form noPrint"><input id="bagNew" placeholder="新增行李"><button class="btn primary" onclick="addBag()">新增</button></div><div id="bagList"></div></div>
  </main>
  <main id="rain" class="page hidden">
    <div class="section-title">雨天備案模式</div>
    <div class="card"><b>☔ 自動推薦室內備案</b><p class="meta">CentralWorld、Big C、ICONSIAM、Terminal 21、Health Land、Take Away Studio、百貨美食街、室內咖啡廳、飯店休息。</p></div>
    <div id="rainList"></div>
  </main>
  <main id="more" class="page hidden">
    <div class="section-title">照片牆</div>
    <div class="card noPrint"><input type="file" accept="image/*" multiple onchange="addPhotos(event)"></div><div class="photoGrid" id="photos"></div>
    <div class="section-title">緊急資訊</div>
    <div class="card form">
      <b>Diya Hotel Srinakarin</b><div class="meta">機場：BKK Suvarnabhumi Airport｜護照、保險、現金、信用卡請分開備份。</div>
      <textarea id="emergency" placeholder="緊急聯絡人、保險、護照備註…" oninput="localStorage.bkkEmergency=this.value"></textarea>
      <div class="alert danger">安全提醒：大麻與實彈射擊僅列為「待自行確認／安全注意」項目。本網站不提供購買、使用、預約、操作教學或導航資訊。</div>
    </div>
    <div class="section-title">資料管理</div>
    <div class="card form noPrint">
      <button class="btn" onclick="exportJSON()">匯出 JSON</button>
      <input type="file" accept=".json" onchange="importJSON(event)">
      <button class="btn ghost" onclick="resetAll()">重置資料</button>
    </div>
  </main>
</div>
<nav class="nav noPrint">
  <button class="active" onclick="showPage('home',this)"><b>🏠</b>首頁</button>
  <button onclick="showPage('plan',this)"><b>🗓️</b>行程</button>
  <button onclick="showPage('budget',this)"><b>💸</b>預算</button>
  <button onclick="showPage('lists',this)"><b>🛍️</b>清單</button>
  <button onclick="showPage('rain',this)"><b>☔</b>雨備</button>
  <button onclick="showPage('more',this)"><b>⋯</b>更多</button>
</nav>
<script>
const $=id=>document.getElementById(id);
let activeDay=0,editId=null;
const defaultDays=[
{date:"6/24（三）",title:"Day1 抵達曼谷",items:[
{time:"12:10",place:"抵達 BKK",stay:"60分",trans:"入境＋領行李",map:"",note:"確認網卡、現金、交通。"},
{time:"14:00",place:"Diya Hotel Srinakarin",stay:"60分",trans:"機場前往飯店",map:"https://maps.google.com/?q=Diya+Hotel+Srinakarin",note:"14:00 後入住。"},
{time:"16:30",place:"CentralWorld",stay:"90分",trans:"BTS / Bolt",map:"https://maps.google.com/?q=CentralWorld",note:"逛街吹冷氣。"},
{time:"18:00",place:"Big C",stay:"70分",trans:"步行",map:"https://maps.google.com/?q=Big+C+Ratchadamri",note:"零食伴手禮初採買。"},
{time:"19:30",place:"水門市場",stay:"60分",trans:"步行 / Bolt",map:"https://maps.google.com/?q=Pratunam+Market",note:"服飾、小物。"},
{time:"21:00",place:"JODD FAIRS",stay:"90分",trans:"MRT / Bolt",map:"https://maps.google.com/?q=JODD+FAIRS",note:"夜市晚餐。"}]},
{date:"6/25（四）",title:"Day2 泰服＋鄭王廟＋美甲",items:[
{time:"09:30",place:"MAHASANÉ 泰服",stay:"60分",trans:"Bolt",map:"https://maps.google.com/?q=MAHASANE+Thai+costume",note:"妝髮與服裝時間要抓寬。"},
{time:"10:45",place:"鄭王廟 Wat Arun",stay:"75分",trans:"船 / Bolt",map:"https://maps.google.com/?q=Wat+Arun",note:"拍泰服照，注意防曬。"},
{time:"12:00",place:"Tha Arun",stay:"60分",trans:"步行",map:"https://maps.google.com/?q=Tha+Arun",note:"媚南河景觀，建議看夕陽或河景。"},
{time:"13:30",place:"Take Away Studio 美甲",stay:"120分",trans:"Bolt",map:"https://maps.google.com/?q=Take+Away+Studio+Bangkok",note:"固定預約。"},
{time:"16:00",place:"GOLEM HOUR",stay:"45分",trans:"步行 / Bolt",map:"https://maps.google.com/?q=GOLEM+HOUR+Bangkok",note:"咖啡甜點。"},
{time:"17:00",place:"DizzySweetie",stay:"45分",trans:"步行 / Bolt",map:"https://maps.google.com/?q=DizzySweetie+Bangkok",note:"可愛甜點。"},
{time:"18:30",place:"三聘市場",stay:"75分",trans:"Bolt",map:"https://maps.google.com/?q=Sampeng+Market",note:"批發小物。"},
{time:"20:00",place:"唐人街",stay:"100分",trans:"步行",map:"https://maps.google.com/?q=Yaowarat+Road",note:"晚餐小吃。"}]},
{date:"6/26（五）",title:"Day3 大城",items:[
{time:"08:00",place:"大城交通方案比較",stay:"30分",trans:"包車 / Bolt",map:"",note:"包車：較穩、適合多點移動。Bolt：單趟彈性高，但跨城回程與等車風險較大。"},
{time:"10:00",place:"大城獅子動物園",stay:"150分",trans:"包車建議",map:"https://maps.google.com/?q=Sriayuthaya+Lion+Park",note:"注意動物互動安全與時間。"},
{time:"13:30",place:"Wat Mahathat",stay:"75分",trans:"包車",map:"https://maps.google.com/?q=Wat+Mahathat+Ayutthaya",note:"樹中佛頭經典景點。"},
{time:"17:30",place:"Mr Joe 脆皮豬",stay:"70分",trans:"回曼谷後用餐",map:"https://maps.google.com/?q=Mr+Joe+Crispy+Pork+Bangkok",note:"必吃清單。"}]},
{date:"6/27（六）",title:"Day4 洽圖洽＋按摩",items:[
{time:"10:00",place:"洽圖洽市集",stay:"180分",trans:"BTS / MRT",map:"https://maps.google.com/?q=Chatuchak+Weekend+Market",note:"週末市集，注意補水。"},
{time:"14:00",place:"Polo Fried Chicken",stay:"60分",trans:"Bolt",map:"https://maps.google.com/?q=Polo+Fried+Chicken+Bangkok",note:"炸雞必吃。"},
{time:"16:00",place:"曼谷海軍射擊場（待自行確認）",stay:"0分",trans:"不提供導航",map:"",note:"僅列安全提醒／待確認，不提供預約、操作或導航資訊。"},
{time:"17:30",place:"Health Land",stay:"120分",trans:"Bolt",map:"https://maps.google.com/?q=Health+Land+Bangkok",note:"按摩放鬆。"},
{time:"20:00",place:"Terminal 21",stay:"90分",trans:"BTS",map:"https://maps.google.com/?q=Terminal+21+Bangkok",note:"室內逛街晚餐。"}]},
{date:"6/28（日）",title:"Day5 經典寺廟＋ICONSIAM＋人妖秀",items:[
{time:"09:00",place:"大皇宮",stay:"90分",trans:"Bolt / 船",map:"https://maps.google.com/?q=The+Grand+Palace+Bangkok",note:"服裝需端莊。"},
{time:"10:45",place:"玉佛寺",stay:"60分",trans:"步行",map:"https://maps.google.com/?q=Temple+of+the+Emerald+Buddha",note:"與大皇宮同區。"},
{time:"12:30",place:"臥佛寺",stay:"70分",trans:"步行 / Tuk Tuk",map:"https://maps.google.com/?q=Wat+Pho",note:"可順便按摩學院。"},
{time:"15:00",place:"ICONSIAM",stay:"150分",trans:"船 / BTS",map:"https://maps.google.com/?q=ICONSIAM",note:"室內、河岸、百貨。"},
{time:"16:30",place:"Yenly Yours",stay:"30分",trans:"館內",map:"https://maps.google.com/?q=Yenly+Yours+ICONSIAM",note:"芒果甜點。"},
{time:"18:30",place:"Asiatique",stay:"90分",trans:"船 / Bolt",map:"https://maps.google.com/?q=Asiatique+The+Riverfront",note:"河濱夜景。"},
{time:"20:00",place:"Calypso",stay:"90分",trans:"步行",map:"https://maps.google.com/?q=Calypso+Cabaret+Bangkok",note:"人妖秀。"}]},
{date:"6/29（一）",title:"Day6 補貨＋返台",items:[
{time:"10:00",place:"Big C 補貨",stay:"90分",trans:"Bolt",map:"https://maps.google.com/?q=Big+C+Bangkok",note:"最後伴手禮。"},
{time:"12:00",place:"回飯店拿行李",stay:"45分",trans:"Bolt",map:"https://maps.google.com/?q=Diya+Hotel+Srinakarin",note:"確認護照、錢包、行李。"},
{time:"13:00",place:"前往 BKK 機場",stay:"90分",trans:"Bolt / 機場交通",map:"https://maps.google.com/?q=Suvarnabhumi+Airport",note:"15:30 回台灣，建議提早到。"}]}];
let data=JSON.parse(localStorage.bkkData||"null")||{days:defaultDays,expenses:[],shop:["Big C 零食","水門市場衣服","洽圖洽小物","三聘市場飾品"],shopDone:{},bags:["護照","機票/訂房截圖","泰銖/信用卡","行動電源","摺疊傘","防曬","薄外套","常備藥","轉接頭"],bagDone:{},photos:[],rates:{twd:.95,usd:.027}};
function persist(){localStorage.bkkData=JSON.stringify(data);renderAll()}
function showPage(id,btn){document.querySelectorAll(".page").forEach(p=>p.classList.add("hidden"));$(id).classList.remove("hidden");document.querySelectorAll(".nav button").forEach(b=>b.classList.remove("active"));if(btn)btn.classList.add("active");scrollTo(0,0)}
function toggleDark(){document.body.classList.toggle("dark");localStorage.bkkDark=document.body.classList.contains("dark")?"1":"0"} if(localStorage.bkkDark==="1")document.body.classList.add("dark");
function renderTabs(){dayTabs.innerHTML=data.days.map((d,i)=>`<button class="tab ${i===activeDay?'active':''}" onclick="activeDay=${i};renderPlan()">${d.date}</button>`).join("")}
function mins(t){let m=(t||"").match(/(\d{1,2}):(\d{2})/);return m?+m[1]*60+ +m[2]:0}
function renderPlan(){renderTabs();let q=(search.value||"").toLowerCase(),d=data.days[activeDay];let arr=d.items.filter(x=>(x.place+x.note+x.trans).toLowerCase().includes(q));timeline.innerHTML=arr.map((x,i)=>`<div class="item" draggable="true" ondragstart="drag(event,${i})" ondrop="drop(event,${i})" ondragover="event.preventDefault()"><div class="time">${x.time}</div><div><div class="place">${x.place}</div><div class="meta">停留：${x.stay||"未填"}｜交通：${x.trans||"未填"}</div>${x.note?`<div class="note">${x.note}</div>`:""}<div class="actions">${x.map?`<a class="btn small" href="${x.map}" target="_blank">Google Maps</a>`:""}<button class="btn small" onclick="editItem(${data.days[activeDay].items.indexOf(x)})">編輯</button><button class="btn small" onclick="delItem(${data.days[activeDay].items.indexOf(x)})">刪除</button></div></div></div>`).join("");checkConflicts()}
function checkConflicts(){let a=data.days[activeDay].items,c=[];for(let i=0;i<a.length-1;i++){let gap=mins(a[i+1].time)-mins(a[i].time),stay=parseInt(a[i].stay)||60;if(gap&&gap<stay+30)c.push(`${a[i].place} → ${a[i+1].place} 時間偏趕，建議預留交通緩衝。`)}conflicts.innerHTML=c.map(x=>`<div class="alert">⚠️ ${x}</div>`).join("")}
function saveItem(){let x={time:fTime.value,place:fPlace.value,stay:fStay.value,trans:fTrans.value,map:fMap.value,note:fNote.value};if(!x.place)return alert("請輸入地點");if(editId===null)data.days[activeDay].items.push(x);else data.days[activeDay].items[editId]=x;editId=null;["fTime","fPlace","fStay","fTrans","fMap","fNote"].forEach(id=>$(id).value="");persist()}
function editItem(i){let x=data.days[activeDay].items[i];editId=i;fTime.value=x.time;fPlace.value=x.place;fStay.value=x.stay;fTrans.value=x.trans;fMap.value=x.map;fNote.value=x.note;scrollTo(0,0)}
function delItem(i){if(confirm("刪除此行程？")){data.days[activeDay].items.splice(i,1);persist()}}
let dragI=null;function drag(e,i){dragI=i}function drop(e,i){let a=data.days[activeDay].items,x=a.splice(dragI,1)[0];a.splice(i,0,x);persist()}
function renderHome(){let start=new Date("2026-06-24T00:00:00+08:00"),now=new Date(),diff=Math.ceil((start-now)/86400000);countdown.textContent=diff>0?diff+" 天":diff===0?"今天出發！":"旅程已開始";todayPlan.innerHTML=data.days[0].items.slice(0,5).map(x=>`<div class="pill">${x.time} ${x.place}</div>`).join(" ");renderTotals()}
function saveRates(){data.rates={twd:+rateTwd.value||.95,usd:+rateUsd.value||.027};persist()}
function convert(c){let thb=c==="THB"?+amtTHB.value:c==="TWD"?(+amtTWD.value)/(+rateTwd.value||1):(+amtUSD.value)/(+rateUsd.value||1);if(c!=="THB")amtTHB.value=thb.toFixed(2);if(c!=="TWD")amtTWD.value=(thb*data.rates.twd).toFixed(2);if(c!=="USD")amtUSD.value=(thb*data.rates.usd).toFixed(2)}
function addExpense(){if(!bName.value||!bAmt.value)return;data.expenses.push({name:bName.value,cat:bCat.value,amt:+bAmt.value});bName.value=bAmt.value="";persist()}
function renderBudget(){rateTwd.value=data.rates.twd;rateUsd.value=data.rates.usd;expenses.innerHTML=data.expenses.map((e,i)=>`<div class="card"><b>${e.name}</b><div class="meta">${e.cat}｜฿${e.amt}</div><button class="btn small" onclick="data.expenses.splice(${i},1);persist()">刪除</button></div>`).join("");let cats=["美食","交通","購物","門票","其他"],s=cats.map(c=>data.expenses.filter(e=>e.cat===c).reduce((a,b)=>a+b.amt,0)),max=Math.max(...s,1);chart.innerHTML=cats.map((c,i)=>`<div style="height:${s[i]/max*150+10}px">${c}<br>${s[i]}</div>`).join("");renderTotals()}
function renderTotals(){let t=data.expenses.reduce((a,b)=>a+b.amt,0);totalBox.textContent="฿"+t.toFixed(0);totalFx.textContent=`約 NT$${(t*data.rates.twd).toFixed(0)}｜US$${(t*data.rates.usd).toFixed(2)}`}
function renderLists(){foodList.innerHTML=["Mae Varee","Yenly Yours","KHIRI","Mr Joe","Thong Smith","Rung Rueang","Polo Fried Chicken","Lay Lao","唐人街"].map(x=>`<div class="pill">🍽️ ${x}</div>`).join(" ");shopList.innerHTML=data.shop.map((x,i)=>`<label class="check"><input type="checkbox" ${data.shopDone[i]?"checked":""} onchange="data.shopDone[${i}]=this.checked;persist()"><span class="${data.shopDone[i]?'done':''}">${x}</span></label>`).join("");let done=Object.values(data.shopDone).filter(Boolean).length;shopProg.style.width=(done/data.shop.length*100||0)+"%";bagList.innerHTML=data.bags.map((x,i)=>`<label class="check"><input type="checkbox" ${data.bagDone[i]?"checked":""} onchange="data.bagDone[${i}]=this.checked;persist()"><span class="${data.bagDone[i]?'done':''}">${x}</span></label>`).join("")}
function addBag(){if(bagNew.value){data.bags.push(bagNew.value);bagNew.value="";persist()}}
function renderRain(){let r=["CentralWorld","Big C","ICONSIAM","Terminal 21","Health Land","Take Away Studio","百貨美食街","室內咖啡廳"];rainList.innerHTML=r.map(x=>`<div class="card"><b>${x}</b><div class="meta">雨天適合：室內、可休息、交通彈性高。</div></div>`).join("")}
function addPhotos(e){[...e.target.files].forEach(f=>{let r=new FileReader();r.onload=()=>{data.photos.push(r.result);persist()};r.readAsDataURL(f)})}
function renderMore(){photos.innerHTML=data.photos.map((p,i)=>`<img src="${p}" onclick="if(confirm('刪除此照片？')){data.photos.splice(${i},1);persist()}">`).join("");emergency.value=localStorage.bkkEmergency||""}
function exportJSON(){let blob=new Blob([JSON.stringify(data,null,2)],{type:"application/json"}),a=document.createElement("a");a.href=URL.createObjectURL(blob);a.download="bangkok-travel-app-data.json";a.click()}
function importJSON(e){let r=new FileReader();r.onload=()=>{data=JSON.parse(r.result);persist()};r.readAsText(e.target.files[0])}
function resetAll(){if(confirm("確定重置所有資料？")){localStorage.removeItem("bkkData");location.reload()}}
function renderAll(){renderHome();renderPlan();renderBudget();renderLists();renderRain();renderMore()}
renderAll();
const manifest={name:"2026 曼谷自由行 Travel App",short_name:"Bangkok 2026",start_url:".",display:"standalone",background_color:"#fff7f3",theme_color:"#ff9f7a",icons:[{src:"data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 192 192'><rect width='192' height='192' rx='48' fill='%23ff9f7a'/><text x='50%' y='58%' text-anchor='middle' font-size='92'>🌸</text></svg>",sizes:"192x192",type:"image/svg+xml"}]};
let ml=document.createElement("link");ml.rel="manifest";ml.href=URL.createObjectURL(new Blob([JSON.stringify(manifest)],{type:"application/json"}));document.head.appendChild(ml);
if("serviceWorker"in navigator){let sw=`const C='bkk-v1';self.addEventListener('install',e=>e.waitUntil(caches.open(C).then(c=>c.addAll(['./']))));self.addEventListener('fetch',e=>e.respondWith(caches.match(e.request).then(r=>r||fetch(e.request).catch(()=>caches.match('./')))))`;navigator.serviceWorker.register(URL.createObjectURL(new Blob([sw],{type:"text/javascript"}))).catch(()=>{})}
</script>
</body>
</html>
