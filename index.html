from pathlib import Path
import zipfile, re

base = Path("/mnt/data/sasi_sniper_ai_v3")
base.mkdir(exist_ok=True)

html = r'''<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="theme-color" content="#070a12">
<title>SASI SNIPER AI v3</title>
<style>
*{box-sizing:border-box}body{margin:0;background:#070a12;color:#eaf0f7;font:13px Inter,Arial,sans-serif}
button,input,select{font:inherit}.app{display:grid;grid-template-columns:175px 1fr 275px;min-height:100vh;gap:8px;padding:8px}
aside,.panel,.topbar,.card{background:#0d121c;border:1px solid #222c3b;border-radius:9px}
aside{padding:12px}.logo{font-size:18px;font-weight:900;color:#f1c84b;margin:8px}.logo span{display:block;color:#fff;font-size:11px;font-weight:600}
.nav{margin-top:18px}.nav div{padding:12px 10px;margin:4px 0;border-radius:6px;color:#aab4c3}.nav .active{background:#251b61;color:#fff;border:1px solid #6247db}
.main{min-width:0}.topbar{height:58px;display:flex;align-items:center;gap:10px;padding:8px 12px}.select,.live{padding:9px 12px;background:#111927;border:1px solid #2b3647;border-radius:6px}.live{color:#34df79}.tf{margin-left:auto;display:flex;gap:5px}.tf button{background:none;color:#aab4c3;border:0;padding:9px}.tf .on{background:#25255c;color:#fff;border-radius:5px}
.cards{display:grid;grid-template-columns:repeat(4,1fr);gap:7px;margin-top:8px}.card{padding:13px;min-height:90px}.label{font-size:10px;color:#9ba7b7;text-transform:uppercase}.big{font-size:25px;font-weight:800;margin-top:8px}.green{color:#27df73}.red{color:#ff5663}.gold{color:#eec74f}
.layout{display:grid;grid-template-columns:1fr;gap:8px;margin-top:8px}.chart{height:485px;position:relative;overflow:hidden;background:radial-gradient(circle at 55% 35%,#11231f 0,#0b121b 38%,#080d15 75%);}.chart h3{margin:14px}.gridlines{position:absolute;inset:48px 0 0;background:repeating-linear-gradient(0deg,transparent 0 43px,#18212d 44px),repeating-linear-gradient(90deg,transparent 0 70px,#18212d 71px);opacity:.65}
canvas{position:absolute;left:0;right:0;top:55px;width:100%;height:380px}.chart .tag{position:absolute;z-index:2;color:#27df73;font-size:11px}.tag.bos{left:22%;top:38%}.tag.sweep{left:56%;top:18%;color:#fff}.tag.fvg{left:48%;top:56%}.tag.ob{left:38%;top:67%;color:#fff}
.bottom{display:grid;grid-template-columns:1fr;gap:8px}.section{padding:12px}.section h3{margin:0 0 10px;font-size:13px}.mtf{display:grid;grid-template-columns:repeat(7,1fr);gap:5px}.mtf div{background:#0a1019;border:1px solid #273243;border-radius:6px;text-align:center;padding:10px 4px}.mtf b{display:block;margin:7px 0;color:#35df79}.bar{height:4px;background:#193b2a;border-radius:4px}.bar i{display:block;height:100%;background:#22db70;border-radius:4px}
table{width:100%;border-collapse:collapse;font-size:11px}th,td{padding:8px 5px;border-bottom:1px solid #202938;text-align:left}th{color:#7f8a9b}.side{display:flex;flex-direction:column;gap:8px}.side .panel{padding:12px}.signal{font-size:29px;font-weight:900;margin:10px 0}.check{margin:8px 0;color:#b6c0cc}.check b{color:#2fe174;margin-right:5px}.row{display:flex;justify-content:space-between;padding:8px 0;border-bottom:1px solid #202938}.btn{width:100%;padding:12px;border:0;border-radius:5px;background:#2dd36f;color:#07120b;font-weight:900;margin-top:8px}.purple{background:#5638d5;color:white}.danger{background:#29151b;color:#ff7c88}.field{background:#0a1018;border:1px solid #2b3647;color:#fff;border-radius:5px;padding:7px;width:75px}.switch{appearance:none;width:36px;height:19px;background:#354051;border-radius:20px;vertical-align:middle}.switch:checked{background:#29d76e}.mode{border:1px solid #273243;border-radius:6px;padding:10px;margin-top:6px}.small{font-size:10px;color:#8490a0}.footer{text-align:center;color:#566274;padding:12px;font-size:10px}
@media(max-width:1000px){.app{grid-template-columns:150px 1fr}.side{grid-column:1/-1;display:grid;grid-template-columns:repeat(3,1fr)}.cards{grid-template-columns:repeat(2,1fr)}}
@media(max-width:650px){.app{display:block;padding:5px}aside{display:none}.topbar{overflow:auto}.tf{margin-left:0}.cards{grid-template-columns:repeat(2,1fr)}.chart{height:390px}.mtf{grid-template-columns:repeat(4,1fr)}.side{display:block;margin-top:8px}}
</style>
</head>
<body>
<div class="app">
<aside>
<div class="logo">◯ SASI<span>SNIPER AI v3</span></div>
<div class="nav">
<div class="active">▣ DASHBOARD</div><div>⌁ ANALYSIS</div><div>⌁ SIGNALS</div><div>◈ TRADES</div><div>◉ PERFORMANCE</div><div>⚙ SETTINGS</div><div>◌ CONNECTIONS</div><div>?</div>
</div>
<div class="panel" style="margin-top:18px;padding:10px"><b>MT5 CONNECTION</b><p class="small">MetaTrader 5</p><span class="green">● CONNECTED</span></div>
<div class="panel" style="margin-top:8px;padding:10px"><div class="small">ANALYSIS MODE</div><b>◉ No orders placed</b></div>
</aside>

<main class="main">
<div class="topbar"><div class="select">🪙 XAUUSD ▾</div><div class="live">● LIVE</div><div class="tf"><button>D1</button><button>H4</button><button>H1</button><button>M30</button><button>M15</button><button>M5</button><button class="on">M1</button></div><div>🔔</div><div>🌙</div></div>
<div class="cards">
<div class="card"><div class="label">Confluence</div><div class="big green" id="conf">86<span style="font-size:14px">/100</span></div><div class="small">Strong Setup</div></div>
<div class="card"><div class="label">AI Bias</div><div class="big green">BULLISH ↗</div></div>
<div class="card"><div class="label">Volatility</div><div class="big red">HIGH</div></div>
<div class="card"><div class="label">Session</div><div class="big" style="font-size:16px">LONDON</div><div class="small">08:00–17:00 GMT+1</div></div>
</div>
<div class="layout">
<div class="card chart"><h3>XAUUSD · M1 <span class="small">O 2,505.18 H 2,505.45 L 2,505.01 C 2,505.31</span></h3><div class="gridlines"></div><span class="tag bos">BOS</span><span class="tag sweep">LIQUIDITY SWEEP</span><span class="tag fvg">FVG</span><span class="tag ob">ORDER BLOCK</span><canvas id="chart"></canvas></div>
<div class="bottom">
<div class="card section"><h3>MULTI-TIMEFRAME ANALYSIS</h3><div class="mtf" id="mtf"></div></div>
<div class="card section"><h3>CONFLUENCE BREAKDOWN</h3><table><thead><tr><th>FACTOR</th><th>WEIGHT</th><th>SCORE</th></tr></thead><tbody id="factors"></tbody></table></div>
<div class="card section"><h3>OPEN TRADES</h3><table><thead><tr><th>TICKET</th><th>TYPE</th><th>LOT</th><th>ENTRY</th><th>SL</th><th>TP1</th><th>PROFIT</th></tr></thead><tbody id="trades"></tbody></table></div>
</div>
</div>
</main>

<section class="side">
<div class="panel"><div class="label">AI SIGNAL</div><div class="signal green">BUY ↗</div><div class="row"><span>Confidence</span><b>86%</b></div><h4>REASONING</h4><div class="check"><b>✓</b> Trend Alignment</div><div class="check"><b>✓</b> BOS Confirmed</div><div class="check"><b>✓</b> Liquidity Sweep</div><div class="check"><b>✓</b> MSS / CHOCH</div><div class="check"><b>✓</b> FVG Match</div><div class="check"><b>✓</b> Order Block Support</div><div class="check"><b>✓</b> Fibonacci Confluence</div></div>
<div class="panel"><h3>TRADE PLAN</h3><div class="row"><span>ENTRY ZONE</span><b class="green">2505.15–2505.40</b></div><div class="row"><span>STOP LOSS</span><b class="red">2503.80</b></div><div class="row"><span>TP1</span><b class="green">2505.60</b></div><div class="row"><span>TP2</span><b class="green">2505.80</b></div><div class="row"><span>TP3</span><b class="green">2506.00</b></div><div class="small">TP ladder follows the SASI 20-pip steps through TP5.</div></div>
<div class="panel"><h3>POSITION CALCULATOR</h3><div class="row"><span>Lot Size</span><input id="lot" class="field" type="number" step=".01" value=".10"></div><div class="row"><span>Risk %</span><input class="field" value="1.00"></div><div class="row"><span>SL (pips)</span><input class="field" value="20"></div><button class="purple" onclick="calc()">CALCULATE</button><div class="row"><span>Suggested lot</span><b id="suggested" class="green">0.10</b></div></div>
<div class="panel"><h3>TRADE CONTROLS</h3><div class="row"><span>EA ON / OFF</span><input id="ea" class="switch" type="checkbox" checked></div><div class="row"><span>Max positions</span><input class="field" value="3"></div><div class="row"><span>3-loss lock</span><input class="switch" type="checkbox" checked></div><div class="row"><span>Profit protection</span><b class="green">Every 20p</b></div><button class="btn" onclick="toggleEA()">EA ENABLED</button><button class="danger" onclick="alert('Safety lock reset')">RESET SAFETY LOCK</button></div>
</section>
</div>
<script>
const cvs=document.getElementById('chart'),ctx=cvs.getContext('2d');
function resize(){cvs.width=cvs.clientWidth*devicePixelRatio;cvs.height=cvs.clientHeight*devicePixelRatio;ctx.scale(devicePixelRatio,devicePixelRatio);draw()}
function draw(){let w=cvs.clientWidth,h=cvs.clientHeight;ctx.clearRect(0,0,w,h);let x=8,y=h*.7;ctx.lineWidth=1;for(let i=0;i<95;i++){let nx=x+7+i*(w-15)/95,ny=y-(i*.8)+Math.sin(i*.8)*35+(i>65?(i-65)*1.4:0);ctx.strokeStyle='#21d96c';ctx.beginPath();ctx.moveTo(x,y);ctx.lineTo(nx,ny);ctx.stroke();x=nx;y=ny}ctx.strokeStyle='#f05a66';ctx.setLineDash([10,12]);ctx.beginPath();ctx.moveTo(10,h*.18);ctx.lineTo(w-10,h*.18);ctx.stroke();ctx.setLineDash([])}
window.addEventListener('resize',resize);resize();
const tf=['D1','H4','H1','M30','M15','M5','M1'],scores=[72,78,82,85,86,90,86];
document.getElementById('mtf').innerHTML=tf.map((t,i)=>`<div><span>${t}</span><b>↗ BULLISH</b><span class="small">${scores[i]}</span><div class="bar"><i style="width:${scores[i]}%"></i></div></div>`).join('');
const fs=[['Trend Alignment','20%','18/20'],['BOS / Structure','15%','14/15'],['Liquidity Sweep','10%','9/10'],['MSS / CHOCH','10%','9/10'],['FVG','10%','9/10'],['Order Block','10%','9/10'],['Fibonacci','10%','8/10'],['Support / Resistance','5%','4/5'],['Volatility','5%','4/5'],['Spread / Session','5%','2/5']];
document.getElementById('factors').innerHTML=fs.map(x=>`<tr><td>${x[0]}</td><td>${x[1]}</td><td class="green">${x[2]}</td></tr>`).join('');
document.getElementById('trades').innerHTML=[['#4587321','BUY','.10','2505.25','2503.80','2505.60','+$36.48'],['#4587299','BUY','.10','2505.10','2503.80','2505.80','+$18.25'],['#4587230','BUY','.10','2505.45','2503.80','2506.00','+$24.60']].map(x=>`<tr>${x.map((v,i)=>`<td class="${i===1||i===6?'green':''}">${v}</td>`).join('')}</tr>`).join('');
function calc(){document.getElementById('suggested').textContent=document.getElementById('lot').value}
function toggleEA(){let e=document.getElementById('ea');e.checked=!e.checked;event.target.textContent=e.checked?'EA ENABLED':'EA OFF';event.target.className=e.checked?'btn':'danger'}
</script>
</body></html>'''

(base/"index.html").write_text(html)
(base/"README.md").write_text("""# SASI SNIPER AI v3
Premium dashboard UI based on the supplied SASI SNIPER AI reference image.

Includes the visual dashboard, XAUUSD/M1 chart area, AI signal, confluence breakdown, multi-timeframe cards, trade plan, position calculator, EA ON/OFF, 20-pip SL/profit-protection display, 5-stage TP concept, open trades and safety controls.

This is the frontend prototype. Live market data, authenticated MT5 execution and server-side AI analysis still need to be connected before real-money trading.
""")
zip_path=Path("/mnt/data/SASI_SNIPER_AI_V3_DASHBOARD.zip")
with zipfile.ZipFile(zip_path,"w",zipfile.ZIP_DEFLATED) as z:
    for p in base.iterdir(): z.write(p,p.name)
print(zip_path)
