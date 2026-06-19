<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover" />
<meta name="theme-color" content="#ff8a65" />
<meta name="apple-mobile-web-app-capable" content="yes" />
<title>Bangkok Travel Companion 2026</title>
<style>
:root{
  --bg:#fff7f3;--card:#ffffffdd;--text:#2d1b16;--muted:#8d6d63;
  --brand:#ff8a65;--brand2:#ffb199;--line:#f0d5ca;
  --good:#2fbf71;--warn:#ff9f1c;--wait:#f6c744;--bad:#ff5630;--gray:#8a8f98;
  --shadow:0 18px 40px rgba(105,49,28,.13);--r:24px;
}
.dark{
  --bg:#15100f;--card:#241b19dd;--text:#fff3ee;--muted:#c8aaa0;
  --brand:#ff9b7a;--brand2:#c4664e;--line:#3d2b27;--shadow:0 18px 40px rgba(0,0,0,.35);
}
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
body{margin:0;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Noto Sans TC",Arial,sans-serif;background:radial-gradient(circle at 50% -10%,#ffe0d2,var(--bg) 42%);color:var(--text);padding-bottom:96px}
.app{max-width:560px;margin:0 auto;min-height:100vh}
header{position:sticky;top:0;z-index:10;padding:14px 16px 10px;background:linear-gradient(180deg,var(--bg),rgba(255,247,243,.7));backdrop-filter:blur(18px)}
.dark header{background:linear-gradient(180deg,var(--bg),rgba(21,16,15,.7))}
.top{display:flex;align-items:center;justify-content:space-between;gap:10px}
h1{font-size:22px;margin:0;letter-spacing:-.6px}
.sub{font-size:13px;color:var(--muted);margin-top:4px}
.page{display:none;padding:8px 16px 20px;animation:fade .22s ease}
.page.active{display:block}
@keyframes fade{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:none}}
.card{background:var(--card);border:1px solid var(--line);border-radius:var(--r);box-shadow:var(--shadow);padding:15px;margin:12px 0;backdrop-filter:blur(16px)}
.card h2,.card h3{margin:0 0 10px}
.card h2{font-size:18px}.card h3{font-size:16px}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.kpi{font-size:24px;font-weight:950;letter-spacing:-.4px}
.muted{color:var(--muted);font-size:13px;line-height:1.45}
.row{display:flex;align-items:center;justify-content:space-between;gap:10px}
.btn,.iconbtn{border:0;border-radius:999px;background:var(--card);color:var(--text);box-shadow:var(--shadow);padding:10px 13px;font-weight:850}
.btn.primary{background:linear-gradient(135deg,var(--brand),var(--brand2));color:#fff}
.btn.small{font-size:12px;padding:7px 10px}
.actions{display:flex;gap:8px;flex-wrap:wrap;margin-top:9px}
.item{border:1px solid var(--line);border-radius:20px;padding:12px;margin:10px 0;background:rgba(255,255,255,.42)}
.dark .item{background:rgba(255,255,255,.04)}
.time{font-weight:950;color:var(--brand)}
.chips{display:flex;gap:8px;overflow:auto;padding:2px 0 6px}
.chip{white-space:nowrap;border:1px solid var(--line);background:var(--card);color:var(--muted);border-radius:999px;padding:9px 12px;font-weight:850}
.chip.active{background:var(--brand);border-color:var(--brand);color:#fff}
input,select,textarea{width:100%;border:1px solid var(--line);background:var(--card);color:var(--text);border-radius:16px;padding:12px;margin:6px 0;font-size:15px}
textarea{min-height:98px;resize:vertical}
label.inline{display:flex;align-items:center;gap:8px}
input[type=checkbox]{width:auto;margin:0}
.tag{font-size:12px;border-radius:999px;padding:4px 8px;font-weight:950}
.tag.good{background:#dcf7ec;color:#087549}
.tag.warn{background:#fff0cf;color:#9a5a00}
.tag.wait{background:#fff7c9;color:#8a6500}
.tag.gray{background:#eceff3;color:#58606b}
.progress{height:9px;background:rgba(120,90,80,.16);border-radius:999px;overflow:hidden;margin:8px 0}
.progress i{display:block;height:100%;width:0;background:linear-gradient(90deg,var(--brand),var(--good));transition:.25s}
.map{height:210px;border-radius:22px;background:linear-gradient(135deg,#ffd8c7,#fff6f2,#ffb199);display:grid;place-items:center;color:#9b4e39;font-weight:950;text-align:center}
.dark .map{background:linear-gradient(135deg,#3a241f,#241b19,#5b3026)}
.nav{position:fixed;left:0;right:0;bottom:0;z-index:20;background:rgba(255,255,255,.84);backdrop-filter:blur(22px);border-top:1px solid var(--line);padding:7px 6px calc(7px + env(safe-area-inset-bottom));display:flex;gap:4px;overflow-x:auto}
.dark .nav{background:rgba(24,17,15,.88)}
.nav button{min-width:68px;border:0;background:transparent;color:var(--muted);font-size:11px;font-weight:850;padding:7px 4px;border-radius:16px}
.nav button.active{color:#fff;background:linear-gradient(135deg,var(--brand),var(--brand2))}
canvas{width:100%;max-height:260px}
.notice{padding:10px 12px;border-radius:18px;background:rgba(255,138,101,.12);border:1px solid var(--line);margin:8px 0}
@media(min-width:720px){.app{max-width:820px}.grid{grid-template-columns:repeat(3,1fr)}}
</style>
</head>
<body>
<div class="app">
<header>
  <div class="top">
    <div>
      <h1>Bangkok Travel Companion 2026</h1>
      <div class="sub">2026/06/24–06/29 · Diya Hotel Srinakarin · China Airlines</div>
    </div>
    <button class="iconbtn" onclick="toggleDark()">☾</button>
  </div>
</header>
<main id="pages"></main>
<nav class="nav" id="nav"></nav>
</div>

<script>
const KEY="bangkok_travel_companion_2026_v2";
const $=s=>document.querySelector(s);
const navs=[
 ["home","首頁"],["trip","行程"],["check","打卡"],["ach","成就"],["log","紀錄"],
 ["near","附近"],["budget","預算"],["booking","預約"],["ai","AI助理"],["more","更多"]
];
const rawDays=[
["Day1","2026-06-24","6/24（三）",[
["12:10","BKK抵達、換匯","機場流程","入境、領行李、換匯","90分","0分",0,"400m","中等"],
["14:15-15:15","BENKOFF Cafe","Bolt","咖啡廳休息","60分","35分",220,"300m","中等"],
["15:15-16:00","Diya Hotel Check In","Bolt","放行李、整理","45分","30分",180,"200m","低"],
["16:30-18:30","水門市場","Bolt/BTS","逛街採買","120分","35分",180,"1.2km","高"],
["18:30-20:30","CentralWorld","步行","百貨、晚餐","120分","15分",0,"900m","高"],
["21:30-22:00","JODD FAIRS","MRT/Bolt","夜市","30分","35分",160,"900m","高"],
["22:00-23:00","Big C","Bolt","採買零食伴手禮","60分","25分",150,"800m","中等"]
]],
["Day2","2026-06-25","6/25（四）",[
["09:30-11:30","MAHASANÉ 泰服體驗","Bolt","泰服拍照體驗","120分","35分",220,"500m","中等"],
["11:40-12:30","AantArm Cafe","步行","咖啡廳","50分","10分",0,"450m","低"],
["13:30","Take Away Studio","Bolt","美甲","150分","30分",180,"300m","低"],
["17:00","The Arun","Bolt","湄南河夕陽晚餐","120分","35分",220,"500m","高"],
["19:30","唐人街","Bolt/MRT","晚餐夜市","120分","30分",160,"1.5km","高"]
]],
["Day3","2026-06-26","6/26（五）",[
["08:00","包車出發","包車","大城一日遊","120分","120分",0,"300m","中等"],
["10:00-13:00","大城獅子動物園","包車","動物園拍照","180分","0分",0,"2km","中等"],
["13:30-15:00","Wat Mahathat","包車","樹中佛頭","90分","30分",0,"1km","中等"],
["19:30","Health Land","Bolt","按摩放鬆","120分","45分",220,"400m","低"]
]],
["Day4","2026-06-27","6/27（六）",[
["10:00-12:45","洽圖洽","BTS/MRT","週末市集","165分","45分",80,"2.5km","高"],
["13:15-14:15","曼谷海軍射擊場","Bolt","射擊體驗","60分","30分",180,"300m","中等"],
["15:30-16:40","Polo Fried Chicken","Bolt","炸雞名店","70分","35分",180,"500m","中等"],
["17:00-20:00","Terminal21","BTS","百貨、晚餐","180分","20分",50,"1.2km","高"]
]],
["Day5","2026-06-28","6/28（日）",[
["09:00-12:00","大皇宮、玉佛寺","Bolt","寺廟穿著遮肩過膝","180分","45分",220,"2km","高"],
["12:00-12:30","臥佛寺","步行","臥佛","30分","10分",0,"600m","高"],
["12:45-13:45","Mr.Joe","Bolt","午餐","60分","20分",120,"300m","中等"],
["14:30-16:15","ICONSIAM","船/Bolt","百貨、河景","105分","35分",120,"1km","高"],
["16:15-17:00","Yenly Yours","步行","芒果甜點","45分","5分",0,"200m","中等"],
["17:15-18:00","接駁船","船","湄南河交通","45分","20分",30,"300m","中等"],
["18:00-19:00","Asiatique","船","碼頭夜市","60分","15分",30,"1km","高"],
["19:00-20:30","Calypso","步行","人妖秀","90分","5分",0,"200m","高"],
["21:00-22:00","Big C","Bolt","最後補貨","60分","35分",200,"800m","中等"]
]],
["Day6","2026-06-29","6/29（一）",[
["07:30","出發機場","Bolt","退房、前往 BKK","80分","50分",300,"400m","中等"],
["10:50","華航起飛","飛機","BKK → 桃園 15:30","280分","0分",0,"300m","低"]
]]
];

function uid(){return Math.random().toString(36).slice(2,10)}
function seed(){
 return {
  dark:false,day:0,mode:"normal",
  budget:{total:30000,rates:{THB:.88,TWD:1,USD:32},expenses:[]},
  itinerary:rawDays.map(d=>({d:d[0],date:d[1],name:d[2],items:d[3].map(x=>({
    id:uid(),time:x[0],place:x[1],transport:x[2],note:x[3],stay:x[4],trafficTime:x[5],
    cost:x[6],walk:x[7],crowd:x[8],booking:"不適用",done:false,photo:false
  }))})),
  bookings:[
   {id:uid(),type:"機票",name:"China Airlines 去程 桃園→BKK",date:"2026-06-24",time:"09:25-12:10",status:"已預約"},
   {id:uid(),type:"機票",name:"China Airlines 回程 BKK→桃園",date:"2026-06-29",time:"10:50-15:30",status:"已預約"},
   {id:uid(),type:"飯店",name:"Diya Hotel Srinakarin",date:"2026-06-24",time:"15:15",status:"已預約"},
   {id:uid(),type:"體驗",name:"MAHASANÉ 泰服體驗",date:"2026-06-25",time:"09:30",status:"待確認"},
   {id:uid(),type:"美甲",name:"Take Away Studio",date:"2026-06-25",time:"13:30",status:"待確認"},
   {id:uid(),type:"餐廳",name:"The Arun",date:"2026-06-25",time:"17:00",status:"待確認"},
   {id:uid(),type:"按摩",name:"Health Land",date:"2026-06-26",time:"19:30",status:"待確認"},
   {id:uid(),type:"表演",name:"Calypso",date:"2026-06-28",time:"19:00",status:"待確認"}
  ],
  logs:["泰奶","按摩","芒果糯米飯","咖啡廳","夜市","Bolt","BTS","MRT","船","Big C"].map(n=>({id:uid(),name:n,cat:catOf(n),count:0})),
  mate:["一起喝泰奶","一起搭船","一起搭 BTS","一起完成大城一日遊","一起完成 Big C 採購"].map(n=>({id:uid(),name:n,done:false})),
  lists:{
   eat:["泰奶","芒果糯米飯","Polo Fried Chicken","Mr.Joe","唐人街小吃"],
   buy:["Big C零食","泰國藥妝","防曬","伴手禮","泰奶包","小老闆海苔"],
   pack:["護照","機票","現金","信用卡","雨傘","防曬","行動電源","轉接頭"]
  },
  listChecks:{eat:{},buy:{},pack:{}},
  reviews:{},steps:{}
 }
}
let db=JSON.parse(localStorage.getItem(KEY)||"null")||seed();
function save(){localStorage.setItem(KEY,JSON.stringify(db));render()}
function allItems(){return db.itinerary.flatMap((d,di)=>d.items.map((i,ii)=>({...i,di,ii,day:d.name,date:d.date})))}
function pct(a,b){return b?Math.round(a/b*100):0}
function spent(){return db.budget.expenses.reduce((s,e)=>s+(+e.amount||0)*(+db.budget.rates[e.cur]||1),0)}
function completeRate(){let a=allItems();return pct(a.filter(x=>x.done).length,a.length)}
function mateRate(){return pct(db.mate.filter(x=>x.done).length,db.mate.length)}
function listRate(k){
 const arr=db.lists[k]||[], checks=(db.listChecks&&db.listChecks[k])||{};
 if(!arr.length)return 0;
 return pct(arr.filter((_,i)=>checks[i]).length,arr.length);
}
function catOf(n){if(/泰奶|芒果|夜市|Big C/.test(n))return"美食";if(/咖啡/.test(n))return"飲料";if(/Bolt|BTS|MRT|船/.test(n))return"交通";if(/按摩/.test(n))return"按摩";return"其他"}
function statusTag(s){
 if(s==="已預約")return `<span class="tag good">已預約</span>`;
 if(s==="尚未預約")return `<span class="tag warn">尚未預約</span>`;
 if(s==="待確認")return `<span class="tag wait">待確認</span>`;
 if(s==="已取消")return `<span class="tag gray">已取消</span>`;
 return "";
}
let liveWeather=null;
let weatherLoading=true;

const BANGKOK_LAT=13.7563;
const BANGKOK_LON=100.5018;

function weatherCodeText(code){
 const map={
  0:"晴朗",1:"大致晴朗",2:"局部多雲",3:"陰天",
  45:"霧",48:"霧凇",
  51:"小毛雨",53:"毛雨",55:"大毛雨",
  61:"小雨",63:"雨",65:"大雨",
  80:"短暫陣雨",81:"陣雨",82:"強陣雨",
  95:"雷雨",96:"雷雨冰雹",99:"強雷雨冰雹"
 };
 return map[code]||"天氣變化";
}

async function fetchWeather(){
 try{
  weatherLoading=true;

  const forecastUrl=
   `https://api.open-meteo.com/v1/forecast?latitude=${BANGKOK_LAT}&longitude=${BANGKOK_LON}`+
   `&current=temperature_2m,apparent_temperature,precipitation,rain,weather_code,wind_speed_10m`+
   `&daily=weather_code,temperature_2m_max,temperature_2m_min,apparent_temperature_max,precipitation_probability_max,uv_index_max`+
   `&timezone=Asia%2FBangkok&forecast_days=7`;

  const airUrl=
   `https://air-quality-api.open-meteo.com/v1/air-quality?latitude=${BANGKOK_LAT}&longitude=${BANGKOK_LON}`+
   `&current=european_aqi,pm2_5&timezone=Asia%2FBangkok`;

  const [forecastRes,airRes]=await Promise.all([fetch(forecastUrl),fetch(airUrl)]);
  const forecast=await forecastRes.json();
  const air=await airRes.json();

  liveWeather={
   current:{
    temp:Math.round(forecast.current.temperature_2m),
    feel:Math.round(forecast.current.apparent_temperature),
    rainNow:forecast.current.rain||forecast.current.precipitation||0,
    code:forecast.current.weather_code,
    desc:weatherCodeText(forecast.current.weather_code),
    wind:Math.round(forecast.current.wind_speed_10m),
    aqi:air.current&&air.current.european_aqi?Math.round(air.current.european_aqi):null,
    pm25:air.current&&air.current.pm2_5?Math.round(air.current.pm2_5):null
   },
   daily:forecast.daily.time.map((date,i)=>({
    d:i===0?"今天":i===1?"明天":date.slice(5).replace("-","/"),
    date,
    hi:Math.round(forecast.daily.temperature_2m_max[i]),
    lo:Math.round(forecast.daily.temperature_2m_min[i]),
    feel:Math.round(forecast.daily.apparent_temperature_max[i]),
    rain:forecast.daily.precipitation_probability_max[i]??0,
    uv:Math.round(forecast.daily.uv_index_max[i]||0),
    aqi:air.current&&air.current.european_aqi?Math.round(air.current.european_aqi):null,
    code:forecast.daily.weather_code[i],
    desc:weatherCodeText(forecast.daily.weather_code[i])
   }))
  };

  weatherLoading=false;
  render();
 }catch(e){
  weatherLoading=false;
  liveWeather=null;
  render();
 }
}

function weather(){
 if(liveWeather&&liveWeather.daily)return liveWeather.daily;

 return ["今天","明天","後天","6/24","6/25","6/26","6/27"].map((d,i)=>({
  d,
  hi:[35,34,35,34,35,33,34][i],
  lo:[27,27,28,27,28,27,27][i],
  feel:[39,38,40,38,39,37,38][i],
  rain:[70,55,68,45,62,50,72][i],
  uv:[10,9,10,8,9,8,10][i],
  aqi:[78,62,86,55,72,80,69][i],
  desc:"備用天氣"
 }));
}

function smartWeather(w){
 let a=[];
 if(w.rain>=60)a.push("☔ 降雨機率高，建議帶傘");
 if(w.feel>=38)a.push("🥵 體感炎熱，注意補水");
 if(w.uv>=8)a.push("☀ 紫外線高，補防曬");
 if(w.aqi&&w.aqi>=80)a.push("💨 空氣品質偏差，可戴口罩");
 if(w.desc&&/雷雨|陣雨|雨/.test(w.desc))a.push("🌧 可能有雨，室內行程可優先");
 return a.join(" · ")||"天氣適合外出";
}
const achRules=[
 ["曼谷美食家","美食紀錄達10次","food",10,"rare"],["泰奶富翁","泰奶達5次","泰奶",5,"epic"],["芒果控","芒果甜點達3次","芒果",3,"rare"],["咖啡獵人","咖啡廳達5間","咖啡廳",5,"rare"],
 ["寺廟巡禮者","完成大皇宮、玉佛寺、臥佛寺、鄭王廟","temple",4,"legend"],["大城探險家","完成大城獅子動物園與 Wat Mahathat","ayut",2,"rare"],["曼谷征服者","景點完成率100%","all",100,"legend"],
 ["BTS初學者","BTS紀錄達1次","BTS",1,"common"],["水上旅人","搭船達1次","船",1,"common"],["Bolt VIP","Bolt紀錄達10次","Bolt",10,"epic"],
 ["掃貨王","必買清單完成率100%","buy",100,"rare"],["Big C狂熱者","Big C購物紀錄達3次","Big C",3,"rare"],["按摩人生","按摩達2次","按摩",2,"rare"],["夜市探險家","完成 JODD FAIRS、唐人街、Asiatique","night",3,"rare"],
 ["特種兵旅人","單日行程完成率100%","day100",1,"epic"],["暴走王","單日步數超過20000","steps",20000,"epic"],["完美旅程","景點、預約、任務全部完成","perfect",100,"legend"],["神隊友","旅伴任務完成率90%","mate90",90,"epic"],["最佳旅伴","默契值達100","mate100",100,"legend"]
];
function logCount(key){let l=db.logs.find(x=>x.name.includes(key));return l?+l.count:0}
function achProgress(k){
 if(k==="food")return db.logs.filter(x=>x.cat==="美食").reduce((a,b)=>a+(+b.count||0),0);
 if(["泰奶","芒果","咖啡廳","BTS","船","Bolt","按摩"].includes(k))return logCount(k);
 if(k==="Big C")return logCount("Big C")+allItems().filter(x=>x.place.includes("Big C")&&x.done).length;
 if(k==="buy")return listRate("buy");
 if(k==="all")return completeRate();
 if(k==="temple")return ["大皇宮","玉佛寺","臥佛寺","鄭王廟"].filter(n=>allItems().some(i=>i.place.includes(n)&&i.done)).length;
 if(k==="ayut")return ["大城獅子動物園","Wat Mahathat"].filter(n=>allItems().some(i=>i.place.includes(n)&&i.done)).length;
 if(k==="night")return ["JODD FAIRS","唐人街","Asiatique"].filter(n=>allItems().some(i=>i.place.includes(n)&&i.done)).length;
 if(k==="day100")return db.itinerary.some(d=>d.items.length&&d.items.every(i=>i.done))?1:0;
 if(k==="steps")return Math.max(0,...Object.values(db.steps||{}));
 if(k==="mate90")return mateRate();
 if(k==="mate100")return mateRate();
 if(k==="perfect")return completeRate()===100&&mateRate()===100&&listRate("buy")===100&&db.bookings.every(b=>b.status==="已預約"||b.status==="不適用")?100:0;
 return 0;
}
function achievements(){
 return achRules.map(r=>{
  let cur=achProgress(r[2]),ok=cur>=r[3],key="achDate_"+r[0];
  if(ok&&!localStorage.getItem(key))localStorage.setItem(key,new Date().toLocaleDateString());
  return {name:r[0],desc:r[1],cur,need:r[3],rare:r[4],ok,date:ok?localStorage.getItem(key):"未解鎖"};
 });
}
function render(){
 document.body.classList.toggle("dark",!!db.dark);
 let current=location.hash.replace("#","")||"home";
 $("#nav").innerHTML=navs.map(n=>`<button class="${current===n[0]?"active":""}" onclick="show('${n[0]}')">${n[1]}</button>`).join("");
 $("#pages").innerHTML=navs.map(n=>`<section id="${n[0]}" class="page ${current===n[0]?"active":""}">${pages[n[0]]()}</section>`).join("");
 setTimeout(drawBudgetCharts,30);
}
function show(id){location.hash=id;render()}
window.onhashchange=render;
function toggleDark(){db.dark=!db.dark;save()}
function maps(q){window.open("https://www.google.com/maps/search/?api=1&query="+encodeURIComponent(q),"_blank")}

const pages={
home(){
 let w=weather()[0],daysLeft=Math.ceil((new Date("2026-06-24T09:25:00+08:00")-new Date())/86400000);
 let today=db.itinerary[db.day],rem=db.bookings.filter(b=>["已預約","待確認"].includes(b.status)).slice(0,6),ach=achievements();
 return `
 <div class="grid">
  <div class="card"><div class="muted">出發倒數</div><div class="kpi">${Math.max(0,daysLeft)}天</div></div>
  <div class="card"><div class="muted">今日日期</div><div class="kpi">${new Date().toLocaleDateString()}</div></div>
  <div class="card"><div class="muted">已花費</div><div class="kpi">TWD ${Math.round(spent())}</div></div>
  <div class="card"><div class="muted">剩餘預算</div><div class="kpi">TWD ${Math.round(db.budget.total-spent())}</div></div>
  <div class="card"><div class="muted">景點完成率</div><div class="kpi">${completeRate()}%</div></div>
  <div class="card"><div class="muted">默契指數</div><div class="kpi">${mateRate()}%</div></div>
 </div>
 <div class="card"><h2>🌦 今日提醒</h2><p>今日最高溫 ${w.hi}°C，最低 ${w.lo}°C，體感 ${w.feel}°C，降雨機率 ${w.rain}%，UV ${w.uv}，AQI ${w.aqi}。</p><div class="notice">${smartWeather(w)}</div><p class="muted">若午後雷陣雨，建議切換懶人版行程：ICONSIAM、CentralWorld、Terminal21、Big C、按摩、美甲、咖啡廳。</p></div>
 <div class="card"><h2>未來7天天氣</h2>${weather().map(x=>`<div class="item row"><b>${x.d}</b><span>${x.lo}-${x.hi}°C · 雨${x.rain}% · UV${x.uv}</span></div>`).join("")}</div>
 <div class="card"><h2>今日行程</h2>${today.items.map(i=>`<div class="item"><span class="time">${i.time}</span> <b>${i.place}</b><div class="muted">${i.transport} · ${i.note}</div></div>`).join("")}</div>
 <div class="card"><h2>今日預約提醒</h2>${rem.map(b=>`<div class="item"><b>${b.name}</b><div>${b.date} ${b.time} ${statusTag(b.status)}</div></div>`).join("")||"無"}</div>
 <div class="card"><h2>今日旅遊戰報</h2><p>成就 ${ach.filter(a=>a.ok).length}/${ach.length} · 必買完成率 ${listRate("buy")}% · 行李完成率 ${listRate("pack")}%</p><div class="progress"><i style="width:${completeRate()}%"></i></div></div>
 <div class="card"><h2>今日最佳路線建議</h2><p>先完成固定預約，再安排同區景點；尖峰時段優先 BTS/MRT，夜間與跨區用 Bolt。雨天優先室內百貨、按摩、美甲、咖啡廳。</p></div>
 <div class="card"><h2>最新旅遊提醒</h2><p>寺廟穿著需遮肩過膝；尊重王室與宗教場所；雨季午後容易雷陣雨；大型活動與官方公告請以泰國官方資訊為準。</p></div>`;
},
trip(){
 let d=db.itinerary[db.day],items=db.mode==="lazy"?d.items.filter((_,i)=>i%2===0||/機場|飯店|預約|The Arun|Calypso|大皇宮|動物園/.test(d.items[i].place)):d.items;
 return `<div class="chips">${db.itinerary.map((x,i)=>`<button class="chip ${db.day===i?"active":""}" onclick="db.day=${i};save()">${x.name}</button>`).join("")}</div>
 <div class="card"><div class="row"><h2>${d.d} ${d.name}</h2><button class="btn small" onclick="db.mode=db.mode==='normal'?'lazy':'normal';save()">${db.mode==="normal"?"標準模式":"懶人模式"}</button></div>
 ${db.mode==="lazy"?`<div class="notice">已切換懶人版：保留核心景點、減少移動與暴走。</div>`:""}
 ${items.map(i=>itItem(i,db.day,d.items.indexOf(i))).join("")}
 <button class="btn primary" onclick="editItin(${db.day})">＋新增行程</button></div>`;
},
check(){
 let a=allItems();
 return `<div class="card"><h2>打卡系統</h2><p>完成 ${a.filter(x=>x.done).length}/${a.length} · ${completeRate()}%</p><div class="progress"><i style="width:${completeRate()}%"></i></div><div class="map">曼谷足跡地圖<br>${a.filter(x=>x.done).map(x=>"📍").join(" ")||"尚未打卡"}</div></div>
 ${a.map(i=>`<div class="card"><div class="row"><b>${i.place}</b><span>${i.done?"✅ 已完成":"⬜ 未完成"}</span></div><div class="muted">${i.day} · ${i.time}</div><div class="actions"><button class="btn small" onclick="checkItem('${i.id}')">手動確認</button><button class="btn small" onclick="gpsCheck('${i.id}')">GPS打卡</button><label class="btn small">上傳照片<input hidden type="file" accept="image/*" onchange="photoCheck('${i.id}',this)"></label><button class="btn small" onclick="reviewPlace('${i.place}')">評價</button></div></div>`).join("")}`;
},
ach(){
 let a=achievements();
 return `${a.map(x=>`<div class="card"><div class="row"><h3>${x.ok?"🏆":"🔒"} ${x.name}</h3><span class="tag ${x.ok?"good":"gray"}">${x.rare}</span></div><p>${x.desc}</p><div class="progress"><i style="width:${Math.min(100,pct(x.cur,x.need))}%"></i></div><div class="muted">目前 ${x.cur}/${x.need} · 解鎖日期：${x.date}</div></div>`).join("")}
 ${mateBox()}`;
},
log(){
 return `<div class="card"><h2>旅行紀錄</h2><button class="btn primary" onclick="addLog()">＋新增紀錄</button></div>
 ${db.logs.map((l,i)=>`<div class="card"><div class="row"><div><b>${l.name}</b><div class="muted">${l.cat}</div></div><div class="kpi">${l.count}</div></div><div class="actions"><button class="btn small" onclick="db.logs[${i}].count++;save()">＋</button><button class="btn small" onclick="db.logs[${i}].count=Math.max(0,db.logs[${i}].count-1);save()">－</button><button class="btn small" onclick="editLog(${i})">編輯</button><button class="btn small" onclick="db.logs.splice(${i},1);save()">刪除</button></div></div>`).join("")}`;
},
near(){
 let cats=["餐廳","咖啡廳","大麻店","按摩館","商店","百貨","ATM","廁所","BTS","MRT"];
 return `<div class="card"><h2>附近探索</h2><select id="nearCat">${cats.map(c=>`<option>${c}</option>`).join("")}</select><select id="nearSort"><option>最近</option><option>評分最高</option><option>營業中</option></select><button class="btn primary" onclick="nearSearch()">搜尋附近</button><div id="nearResult" class="muted">會使用 Google Maps 開啟附近搜尋。</div></div>`;
},
budget(){
 return `<div class="card"><h2>預算系統</h2><label>總預算 TWD</label><input type="number" value="${db.budget.total}" onchange="db.budget.total=+this.value;save()"><p>已花費 TWD ${Math.round(spent())} · 剩餘 TWD ${Math.round(db.budget.total-spent())}</p><canvas id="pie"></canvas><canvas id="bar"></canvas><button class="btn primary" onclick="addExpense()">＋新增花費</button></div>
 <div class="card"><h2>匯率中心</h2>${["THB","TWD","USD"].map(c=>`<label>${c} → TWD</label><input type="number" step=".01" value="${db.budget.rates[c]}" onchange="db.budget.rates['${c}']=+this.value;save()">`).join("")}<button class="btn" onclick="window.open('https://www.superrichthailand.com','_blank')">SuperRich 官方網站</button></div>
 ${db.budget.expenses.map((e,i)=>`<div class="card"><b>${e.name}</b><div>${e.cat} · ${e.cur} ${e.amount} · TWD ${Math.round(e.amount*db.budget.rates[e.cur])}</div><div class="actions"><button class="btn small" onclick="editExpense(${i})">編輯</button><button class="btn small" onclick="db.budget.expenses.splice(${i},1);save()">刪除</button></div></div>`).join("")}
 <div class="card"><h2>省錢建議</h2><p>${budgetTip()}</p></div>`;
},
booking(){
 let f=sessionStorage.getItem("bookingFilter")||"全部";
 let arr=db.bookings.filter(b=>f==="全部"||b.status===f);
 return `<div class="card"><h2>預約專區</h2><select onchange="sessionStorage.setItem('bookingFilter',this.value);render()"><option ${f==="全部"?"selected":""}>全部</option><option ${f==="已預約"?"selected":""}>已預約</option><option ${f==="待確認"?"selected":""}>待確認</option><option ${f==="尚未預約"?"selected":""}>尚未預約</option><option ${f==="已取消"?"selected":""}>已取消</option></select><button class="btn primary" onclick="addBooking()">＋新增預約</button></div>
 ${arr.map((b,i)=>`<div class="card"><div class="row"><b>${b.name}</b>${statusTag(b.status)}</div><div>${b.type} · ${b.date} ${b.time}</div><div class="actions"><button class="btn small" onclick="editBooking('${b.id}')">編輯</button><button class="btn small" onclick="delBooking('${b.id}')">刪除</button></div></div>`).join("")||`<div class="card">沒有符合的預約。</div>`}`;
},
ai(){
 return `<div class="card"><h2>AI旅遊助理</h2><textarea id="q" placeholder="今天下雨怎麼辦、哪些景點還沒完成、哪些預約快到了、今天附近有什麼好吃、哪裡花最多錢、幫我優化今天行程、幫我產生懶人版行程、今天最佳交通方式"></textarea><button class="btn primary" onclick="askAI()">送出</button><div id="ans" class="item">我會根據本地行程、預算、打卡、成就、預約、天氣回答。</div></div>`;
},
more(){
 return `<div class="card"><h2>旅遊工具</h2><h3>BTS / MRT 教學</h3><p>看路線顏色與終點站方向，購票可用現金、感應卡或 Rabbit Card；尖峰時段比計程車穩定。</p><h3>泰文常用句</h3>${thaiPhrases().map(x=>`<div class="item"><b>${x[0]}</b><br>${x[1]} · ${x[2]} · ${x[3]}</div>`).join("")}<h3>泰國實用App</h3><p>Grab、Bolt：叫車；foodpanda、LINE MAN：外送；Google Maps：導航；Eatigo、Chope：訂餐；Klook、KKday：票券與體驗。</p></div>
 <div class="card"><h2>提醒中心</h2><p>官方天氣警報、淹水警報、交通管制、大型活動、王室公告、節慶活動請以官方公告為準。寺廟需遮肩過膝；不摸頭、不用腳指人、不冒犯王室。</p></div>
 <div class="card"><h2>緊急聯絡</h2>
<p><b>飯店：Diya Hotel Srinakarin</b></p>
<p>英文地址：597, 2 Srinagarindra Rd, Phatthanakan, Suan Luang, Bangkok 10250 泰國</p>
<p>泰文地址：597 2 ถ. ศรีนครินทร์ แขวงพัฒนาการ เขตสวนหลวง กรุงเทพมหานคร 10250</p>
<div class="actions">
<button class="btn" onclick="copyText('597, 2 Srinagarindra Rd, Phatthanakan, Suan Luang, Bangkok 10250 Thailand')">複製英文地址</button>
<button class="btn" onclick="copyText('597 2 ถ. ศรีนครินทร์ แขวงพัฒนาการ เขตสวนหลวง กรุงเทพมหานคร 10250')">複製泰文地址</button>
<button class="btn" onclick="maps('Diya Hotel Srinakarin 597 2 Srinagarindra Rd Bangkok')">Google Maps</button>
</div>
<p>泰國緊急電話：191 警察、1669 救護、1155 觀光警察。</p>
</div>
 ${listCenter("eat","必吃清單")}${listCenter("buy","必買清單")}${listCenter("pack","行李清單")}
 <div class="card"><h2>旅行證書</h2><button class="btn primary" onclick="certificate()">產生並下載 PNG</button><button class="btn" onclick="window.print()">下載 PDF / 列印</button><canvas id="cert" height="520"></canvas></div>
 <div class="card"><h2>資料管理</h2><div class="actions"><button class="btn" onclick="exportJSON()">匯出 JSON</button><label class="btn">匯入 JSON<input hidden type="file" accept="application/json" onchange="importJSON(this)"></label><button class="btn" onclick="printTrip()">一鍵列印行程</button><button class="btn" onclick="resetData()">重置資料</button></div></div>`;
}
};

function itItem(i,di,ii){
 return `<div class="item" draggable="true" ondragstart="dragI=${ii}" ondragover="event.preventDefault()" ondrop="dropItin(${di},${ii})">
 <div class="row"><div><span class="time">${i.time}</span> <b>${i.place}</b> ${statusTag(i.booking)}</div><label class="inline"><input type="checkbox" ${i.done?"checked":""} onchange="db.itinerary[${di}].items[${ii}].done=this.checked;save()">完成</label></div>
 <div class="muted">交通：${i.transport} · 停留 ${i.stay} · 交通 ${i.trafficTime} · 交通費 ฿${i.cost} · 步行 ${i.walk} · 壅塞 ${i.crowd}</div>
 <div class="muted">${i.note}</div>
 <div class="actions"><button class="btn small" onclick="maps('${i.place.replaceAll("'","")}')">Google Maps</button><button class="btn small" onclick="reviewPlace('${i.place.replaceAll("'","")}')">評價</button><button class="btn small" onclick="editItin(${di},${ii})">編輯</button><button class="btn small" onclick="delItin(${di},${ii})">刪除</button></div></div>`;
}
let dragI=null;
function dropItin(di,to){let a=db.itinerary[di].items,b=a.splice(dragI,1)[0];a.splice(to,0,b);save()}
function editItin(di,ii){
 let old=ii!=null?db.itinerary[di].items[ii]:{id:uid(),time:"",place:"",transport:"Bolt",note:"",stay:"60分",trafficTime:"20分",cost:100,walk:"500m",crowd:"中等",booking:"不適用",done:false};
 let place=prompt("地點",old.place);if(place===null)return;
 old.time=prompt("時間",old.time)||old.time;old.place=place;old.transport=prompt("交通",old.transport)||old.transport;old.note=prompt("備註",old.note)||old.note;old.stay=prompt("停留時間",old.stay)||old.stay;old.trafficTime=prompt("預估交通時間",old.trafficTime)||old.trafficTime;old.cost=+(prompt("交通費 THB",old.cost)||old.cost);old.walk=prompt("步行距離",old.walk)||old.walk;old.crowd=prompt("壅塞程度",old.crowd)||old.crowd;old.booking=prompt("預約狀態：不適用/尚未預約/已預約/待確認/已取消",old.booking)||old.booking;
 if(ii!=null)db.itinerary[di].items[ii]=old;else db.itinerary[di].items.push(old);save();
}
function delItin(di,ii){if(confirm("刪除此行程？")){db.itinerary[di].items.splice(ii,1);save()}}
function findItem(id){for(let d of db.itinerary){let i=d.items.find(x=>x.id===id);if(i)return i}}
function checkItem(id){let i=findItem(id);if(i){i.done=true;save()}}
function gpsCheck(id){navigator.geolocation?navigator.geolocation.getCurrentPosition(()=>checkItem(id),()=>alert("定位失敗，請改用手動確認")):alert("此裝置不支援定位")}
function photoCheck(id,input){if(input.files&&input.files[0]){let i=findItem(id);i.photo=true;i.done=true;save()}}
function reviewPlace(name){let r=db.reviews[name]||{star:5,text:""};let s=prompt("1-5星",r.star);if(s===null)return;let t=prompt("心得",r.text)||"";db.reviews[name]={star:Math.max(1,Math.min(5,+s||5)),text:t};save()}
function addLog(){let n=prompt("項目名稱");if(!n)return;db.logs.push({id:uid(),name:n,cat:prompt("分類：美食/飲料/交通/按摩/景點/購物/其他",catOf(n))||"其他",count:0});save()}
function editLog(i){db.logs[i].name=prompt("名稱",db.logs[i].name)||db.logs[i].name;db.logs[i].cat=prompt("分類",db.logs[i].cat)||db.logs[i].cat;save()}
function mateBox(){
 return `<div class="card"><h2>旅伴默契系統</h2><p>默契值 ${mateRate()}% · 等級：${mateRate()>=100?"最佳旅伴":mateRate()>=90?"神隊友":mateRate()>=50?"默契培養中":"新手旅伴"}</p><div class="progress"><i style="width:${mateRate()}%"></i></div><button class="btn primary" onclick="addMate()">＋新增任務</button>${db.mate.map((m,i)=>`<div class="item row"><label class="inline"><input type="checkbox" ${m.done?"checked":""} onchange="db.mate[${i}].done=this.checked;save()">${m.name}</label><span><button class="btn small" onclick="editMate(${i})">編</button><button class="btn small" onclick="db.mate.splice(${i},1);save()">刪</button></span></div>`).join("")}</div>`;
}
function addMate(){let n=prompt("旅伴任務");if(n){db.mate.push({id:uid(),name:n,done:false});save()}}
function editMate(i){db.mate[i].name=prompt("任務",db.mate[i].name)||db.mate[i].name;save()}
function nearSearch(){let c=$("#nearCat").value,s=$("#nearSort").value;$("#nearResult").innerHTML=`已開啟 Google Maps：附近${c} · 排序偏好：${s}`;window.open("https://www.google.com/maps/search/nearby+"+encodeURIComponent(c),"_blank")}
function addExpense(){db.budget.expenses.push({id:uid(),name:prompt("名稱","餐費")||"花費",cat:prompt("類別：美食/交通/購物/門票/按摩/其他","美食")||"其他",amount:+(prompt("金額",100)||0),cur:prompt("幣別 THB/TWD/USD","THB")||"THB"});save()}
function editExpense(i){let e=db.budget.expenses[i];e.name=prompt("名稱",e.name)||e.name;e.cat=prompt("類別",e.cat)||e.cat;e.amount=+(prompt("金額",e.amount)||e.amount);e.cur=prompt("幣別",e.cur)||e.cur;save()}
function budgetTip(){let m={};db.budget.expenses.forEach(e=>m[e.cat]=(m[e.cat]||0)+(+e.amount||0)*(db.budget.rates[e.cur]||1));let top=Object.entries(m).sort((a,b)=>b[1]-a[1])[0];return top?`目前花最多的是「${top[0]}」約 TWD ${Math.round(top[1])}。可用 BTS/MRT、百貨美食街、同區景點集中安排來省錢。`:"尚無花費紀錄。"}
function addBooking(){db.bookings.push({id:uid(),type:prompt("類型","餐廳")||"其他",name:prompt("名稱")||"預約",date:prompt("日期","2026-06-25")||"",time:prompt("時間","17:00")||"",status:prompt("狀態：不適用/尚未預約/已預約/待確認/已取消","待確認")||"待確認"});save()}
function editBooking(id){let b=db.bookings.find(x=>x.id===id);b.type=prompt("類型",b.type)||b.type;b.name=prompt("名稱",b.name)||b.name;b.date=prompt("日期",b.date)||b.date;b.time=prompt("時間",b.time)||b.time;b.status=prompt("狀態",b.status)||b.status;save()}
function delBooking(id){if(confirm("刪除此預約？")){db.bookings=db.bookings.filter(x=>x.id!==id);save()}}
function askAI(){
 let q=$("#q").value,ans="";
 if(/雨|下雨|天氣/.test(q))ans="雨天建議：切換懶人版行程，優先 ICONSIAM、CentralWorld、Terminal21、Big C、按摩、美甲、咖啡廳。戶外寺廟改早上，The Arun 帶傘並提早叫車。";
 else if(/沒完成|未完成|景點/.test(q))ans=allItems().filter(i=>!i.done).map(i=>`${i.day} ${i.place}`).join("<br>")||"全部景點都完成了！";
 else if(/預約/.test(q))ans=db.bookings.filter(b=>["已預約","待確認"].includes(b.status)).map(b=>`${b.date} ${b.time} ${b.name} ${statusTag(b.status)}`).join("<br>")||"目前沒有待提醒預約。";
 else if(/附近|好吃/.test(q))ans="附近好吃建議可開 Google Maps 搜尋：餐廳、咖啡廳、夜市。若在市中心，優先看 CentralWorld、Terminal21、ICONSIAM 美食街。";
 else if(/花|預算|錢/.test(q))ans=budgetTip();
 else if(/懶人|優化/.test(q))ans="最佳化建議：每天只保留 2-3 個核心區域，固定預約不可動，雨天改室內；尖峰走 BTS/MRT，晚上或跨區搭 Bolt。";
 else if(/交通/.test(q))ans="市區短距離用 BTS/MRT，河岸用船，夜間與跨區用 Bolt；大城維持包車最省體力。";
 else ans="你可以問我：今天下雨怎麼辦、哪些景點還沒完成、哪些預約快到了、哪裡花最多錢、幫我產生懶人版行程、今天最佳交通方式。";
 $("#ans").innerHTML=ans;
}
function thaiPhrases(){return [["你好","สวัสดีค่ะ","sà-wàt-dii-khâ","撒挖滴咖"],["謝謝","ขอบคุณค่ะ","khɔ̀ɔp-khun-khâ","扣坤咖"],["多少錢","เท่าไหร่คะ","thâo-rài-khá","套賴咖"],["不要辣","ไม่เผ็ดค่ะ","mâi-phèt-khâ","麥配咖"],["去這裡","ไปที่นี่ค่ะ","bpai-thîi-nîi-khâ","掰替你咖"],["可以拍照嗎","ถ่ายรูปได้ไหมคะ","thàai-rûup-dâai-mái-khá","泰路代麥咖"]]}
function listCenter(k,title){
 db.listChecks=db.listChecks||{};db.listChecks[k]=db.listChecks[k]||{};
 let arr=db.lists[k]||[],rate=listRate(k);
 return `<div class="card"><h2>${title}</h2><p>完成率 ${rate}%</p><div class="progress"><i style="width:${rate}%"></i></div><button class="btn small" onclick="addList('${k}')">＋新增</button>
 ${arr.map((x,i)=>`<div class="item row"><label class="inline"><input type="checkbox" ${db.listChecks[k][i]?"checked":""} onchange="db.listChecks['${k}'][${i}]=this.checked;save()">${x}</label><span><button class="btn small" onclick="editList('${k}',${i})">編</button><button class="btn small" onclick="delList('${k}',${i})">刪</button></span></div>`).join("")}</div>`;
}
function addList(k){let n=prompt("新增項目");if(n){db.lists[k].push(n);save()}}
function editList(k,i){let n=prompt("編輯",db.lists[k][i]);if(n){db.lists[k][i]=n;save()}}
function delList(k,i){db.lists[k].splice(i,1);delete db.listChecks[k][i];let old=db.listChecks[k],nw={};Object.keys(old).forEach(x=>{let n=+x;if(n<i)nw[n]=old[x];if(n>i)nw[n-1]=old[x]});db.listChecks[k]=nw;save()}
function copyText(t){navigator.clipboard.writeText(t);alert("已複製")}
function topReviewed(){let e=Object.entries(db.reviews).sort((a,b)=>(b[1].star||0)-(a[1].star||0))[0];return e?e[0]:"尚未評價"}
function certificate(){
 let c=$("#cert"),x=c.getContext("2d");c.width=420;c.height=520;
 x.fillStyle="#fff7f3";x.fillRect(0,0,420,520);
 x.fillStyle="#ff8a65";x.font="bold 30px -apple-system";x.fillText("Bangkok 2026",36,72);
 x.fillStyle="#2d1b16";x.font="bold 22px -apple-system";x.fillText("Travel Certificate",36,108);
 x.font="16px -apple-system";
 [`旅行天數：6天`,`景點完成率：${completeRate()}%`,`成就數：${achievements().filter(a=>a.ok).length}/${achRules.length}`,`默契指數：${mateRate()}%`,`最愛景點：${topReviewed()}`,`總花費：TWD ${Math.round(spent())}`].forEach((l,i)=>x.fillText(l,42,170+i*42));
 x.fillStyle="#ff8a65";x.font="bold 18px -apple-system";x.fillText("Bangkok Travel Companion 2026",42,470);
 let a=document.createElement("a");a.href=c.toDataURL("image/png");a.download="Bangkok-2026-Travel-Certificate.png";a.click();
}
function exportJSON(){let a=document.createElement("a");a.href=URL.createObjectURL(new Blob([JSON.stringify(db,null,2)],{type:"application/json"}));a.download="bangkok-travel-2026.json";a.click()}
function importJSON(input){let f=input.files[0];if(!f)return;let r=new FileReader();r.onload=()=>{db=JSON.parse(r.result);save()};r.readAsText(f)}
function printTrip(){let w=window.open("","_blank");w.document.write(`<h1>Bangkok Travel Companion 2026</h1>${db.itinerary.map(d=>`<h2>${d.name}</h2><ul>${d.items.map(i=>`<li>${i.time} ${i.place}｜${i.transport}｜${i.note}</li>`).join("")}</ul>`).join("")}`);w.print()}
function resetData(){if(confirm("確定重置所有資料？")){localStorage.removeItem(KEY);location.reload()}}
function drawBudgetCharts(){
 let p=$("#pie"),b=$("#bar");if(!p||!b)return;
 let cats={};db.budget.expenses.forEach(e=>cats[e.cat]=(cats[e.cat]||0)+(+e.amount||0)*(db.budget.rates[e.cur]||1));
 drawChart(p,cats,"pie");drawChart(b,cats,"bar");
}
function drawChart(c,cats,type){
 c.width=380;c.height=230;let x=c.getContext("2d"),labs=Object.keys(cats),vals=Object.values(cats),total=vals.reduce((a,b)=>a+b,0);
 x.clearRect(0,0,c.width,c.height);x.font="13px -apple-system";
 if(!labs.length){x.fillStyle=getComputedStyle(document.body).color;x.fillText("尚無花費資料",20,40);return}
 if(type==="pie"){
  let start=0;vals.forEach((v,i)=>{x.beginPath();x.moveTo(110,110);x.arc(110,110,82,start,start+Math.PI*2*v/total);x.fillStyle=`hsl(${18+i*48},82%,70%)`;x.fill();start+=Math.PI*2*v/total;x.fillStyle=getComputedStyle(document.body).color;x.fillText(`${labs[i]} ${Math.round(v)}`,220,45+i*25)});
 }else{
  let max=Math.max(...vals);vals.forEach((v,i)=>{x.fillStyle=`hsl(${18+i*48},82%,70%)`;x.fillRect(100,25+i*32,230*v/max,18);x.fillStyle=getComputedStyle(document.body).color;x.fillText(labs[i],12,39+i*32)});
 }
}
if("serviceWorker"in navigator){
 const sw=`self.addEventListener('install',e=>e.waitUntil(caches.open('bt2026-v2').then(c=>c.addAll(['./']))));self.addEventListener('fetch',e=>e.respondWith(caches.match(e.request).then(r=>r||fetch(e.request).catch(()=>caches.match('./')))))`;
 navigator.serviceWorker.register(URL.createObjectURL(new Blob([sw],{type:"text/javascript"}))).catch(()=>{});
}
render();
fetchWeather();
</script>
</body>
</html>
