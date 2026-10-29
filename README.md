[MATEMERCADO_2099.html](https://github.com/user-attachments/files/34136565/MATEMERCADO_2099.html)# matemercado-2099
Jogo educativo de matemática financeira.
[Upload<!DOCTYPE html>
<html lang="pt-BR"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>MATEMERCADO 2099</title>
<link href="https://fonts.googleapis.com/css2?family=Rajdhani:wght@600;700&display=swap" rel="stylesheet">
<style>
:root{--bg:#05060f;--pn:#0d1024;--ln:#252a52;--tx:#e6ecff;--mu:#8a93b8;--cy:#22e5ff;--pu:#9b5cff;--up:#2ee6a0;--dn:#ff6b86;color-scheme:dark;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--tx);font:16px/1.4 system-ui,sans-serif;min-height:100vh}
h1,h2,h3,.big{font-family:Rajdhani,system-ui,sans-serif;letter-spacing:.04em;margin:.2em 0}
h1{font-size:clamp(34px,8vw,60px);color:var(--cy);text-shadow:0 0 12px #22e5ff66;text-align:center}
#app{max-width:900px;margin:0 auto;padding:14px}
.card{background:var(--pn);border:1px solid var(--ln);border-radius:12px;padding:14px;margin:10px 0}
button,input,select,textarea{font:inherit;color:var(--tx);background:#141838;border:1px solid var(--ln);border-radius:10px;padding:12px 14px}
button{cursor:pointer;background:linear-gradient(90deg,#0aa7c0,#6b3fd0);border:0;font-weight:700;min-height:46px}
button.g{background:#141838;border:1px solid var(--ln)}button:disabled{opacity:.4}
button:focus-visible,input:focus-visible,select:focus-visible{outline:2px solid var(--cy)}
.row{display:flex;gap:10px;flex-wrap:wrap;align-items:center}.row>*{flex:1}
.hug{padding:30px 10px;font-size:26px;font-family:Rajdhani,sans-serif}
.mu{color:var(--mu);font-size:14px}.up{color:var(--up)}.dn{color:var(--dn)}
.top{position:sticky;top:env(safe-area-inset-top,0px);background:var(--bg);z-index:5;padding:6px 0}
.big{font-size:28px;font-weight:700}
.bar{height:8px;background:#141838;border-radius:6px;overflow:hidden}.bar>i{display:block;height:100%;background:var(--pu)}
table{width:100%;border-collapse:collapse}td,th{padding:8px 4px;text-align:left;border-bottom:1px solid var(--ln)}
.sc{overflow-x:auto}
.mod{position:fixed;inset:0;background:#000c;display:grid;place-items:center;padding:14px;z-index:9}
.mod .card{max-width:480px;width:100%}
.code{font:700 clamp(30px,9vw,54px) Rajdhani,monospace;color:var(--cy);text-align:center;word-break:break-all}
.shake{animation:sh .3s}@keyframes sh{25%{transform:translateX(-6px)}75%{transform:translateX(6px)}}
@media (prefers-reduced-motion:reduce){.shake{animation:none}}
label{display:inline-flex;gap:6px;align-items:center;margin:4px 10px 4px 0}
.nav{display:flex;justify-content:space-between;align-items:center;gap:8px;flex-wrap:wrap;padding:6px 0 14px;border-bottom:1px solid var(--ln)}
.hero{padding:34px 0 18px}.kick{color:var(--pu);font:700 13px Rajdhani,sans-serif;letter-spacing:.18em}
.hero h1{text-align:left;font-size:clamp(40px,10vw,72px);line-height:1}
.modes,.tiles{display:grid;gap:10px;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));margin:12px 0}
.modes .card{text-align:left;height:100%;margin:0}
.tile{background:var(--pn);border:1px solid var(--ln);border-radius:12px;padding:14px}.tile b{display:block;font:700 26px Rajdhani,sans-serif;color:var(--cy)}
.chip{background:var(--pn);border:1px solid var(--ln);border-radius:999px;padding:8px 14px;display:inline-block;margin:4px 4px 4px 0}
h2.sec{margin-top:30px;font-size:30px}
.asset{display:grid;grid-template-columns:1fr auto;gap:8px 12px;align-items:center;padding:12px 0;border-bottom:1px solid var(--ln)}.col{display:flex;gap:6px}.cd{grid-column:1/-1;width:100%;height:auto;background:#000;border:1px solid var(--ln);border-radius:10px}
.hero2{display:grid;grid-template-columns:repeat(auto-fit,minmax(290px,1fr));gap:20px;align-items:center;padding:26px 0}.hero2 h1{text-align:left;font-size:clamp(34px,8vw,56px);line-height:1.05}.hero2 .card{margin:0;text-align:center}
.shop-item{display:grid;grid-template-columns:1fr auto;gap:8px;padding:10px 0;border-bottom:1px solid var(--ln);align-items:center}
.badge{display:inline-block;background:var(--pu);color:#fff;font-size:12px;padding:2px 8px;border-radius:999px;margin-left:6px}
.tabbar{display:flex;gap:6px;flex-wrap:wrap;margin:8px 0}
.tabbar button{flex:1;min-width:90px;font-size:14px;padding:10px 8px}
.mission{background:#0a0e20;border:1px solid var(--ln);border-radius:10px;padding:10px;margin:6px 0}
.mission.done{border-color:var(--up);opacity:.85}
.title-chip{background:linear-gradient(90deg,#0aa7c0,#6b3fd0);padding:4px 10px;border-radius:8px;font-size:13px;font-weight:700}
.sec-title{font-size:18px;color:var(--cy);margin:0 0 8px;font-family:Rajdhani,sans-serif;letter-spacing:.06em}
.stat-row{display:flex;gap:12px;flex-wrap:wrap;margin:8px 0}
.stat{background:#0a0e20;border:1px solid var(--ln);border-radius:10px;padding:10px 14px;min-width:110px}
.stat .mu{font-size:12px}.stat .big{font-size:20px}
.asset{padding:14px 0}
.asset b{font-size:18px}
.hint{font-size:13px;color:var(--mu);margin-top:6px}
.news{background:#0a1020;border-left:3px solid var(--pu);padding:8px 12px;margin:6px 0;font-size:13px;border-radius:0 8px 8px 0}
.goalbar{height:14px;background:#141838;border-radius:8px;overflow:hidden;margin:6px 0}.goalbar>i{display:block;height:100%;background:linear-gradient(90deg,#22e5ff,#9b5cff)}
</style></head><body><div id="app"></div>
<script>
// ===== utilidades =====
const $=s=>document.querySelector(s),R=(a,b)=>a+Math.floor(Math.random()*(b-a+1)),P=a=>a[R(0,a.length-1)];
const f=n=>String(+(+n).toFixed(2)).replace('.',','),M=n=>'R$ '+(+n).toLocaleString('pt-BR',{minimumFractionDigits:2,maximumFractionDigits:2});
const hs=s=>{let h=2166136261;for(const c of s)h=Math.imul(h^c.charCodeAt(0),16777619);return h>>>0};
const chk=(s,n,w)=>hs(s+'|'+n+'|'+Math.round(w)).toString(36).slice(0,4).toUpperCase();
const rng=s=>{let a=hs(s);return()=>{a|=0;a=a+0x6D2B79F5|0;let t=Math.imul(a^a>>>15,1|a);t=t+Math.imul(t^t>>>7,61|t)^t;return((t^t>>>14)>>>0)/4294967296}};
const ST=(k,v)=>{try{return v===undefined?localStorage.getItem(k):localStorage.setItem(k,v)}catch(e){return null}};
// ===== constantes da economia =====
const SAL=150,BILLS_BASE={aluguel:300,compras:400,luz:80,internet:60,transporte:70},FEE=.02,TAX=.1,DEBT=.05,MAXOPS=3,MULT=[1,1.5,2],QT=[30,45,60],LV=['Fácil','Médio','Difícil'];
const TH=[['pct','Porcentagem'],['md','Multiplicação e divisão'],['dec','Decimais'],['eq','Equações com x'],['int','Números inteiros'],['fr','Frações simples'],['ex','Expressões numéricas'],['r3','Regra de três']];
const AS=[['NEOCOIN',200,.004,0,1],['SOLARIS',100,.002,0,2],['AQUA-X',150,0,.06,1],['TECHNOVA',250,.006,0,1.5],['ORBIT',120,-.002,.07,1.5]];
// ===== LOJA DE REDUÇÃO DE CONTAS (feature 1) =====

// ===== EMPREGOS (trabalhar alem do day trade) =====
const JOBS=[
  {id:'caixa',name:'Caixa de mercado',pay:80,xp:1,desc:'Calcule trocos e totais',themes:['dec','pct'],energy:1},
  {id:'entregador',name:'Entregador',pay:95,xp:1,desc:'Rotas e tempos',themes:['md','r3'],energy:1},
  {id:'assistente',name:'Assistente financeiro',pay:120,xp:2,desc:'Porcentagens e juros',themes:['pct','eq'],energy:1},
  {id:'analista',name:'Analista junior',pay:150,xp:2,desc:'Expressoes e medias',themes:['ex','dec'],energy:2},
  {id:'professor',name:'Monitor de matematica',pay:110,xp:2,desc:'Ensine resolvendo',themes:['eq','fr'],energy:1},
  {id:'dev',name:'Dev estagiario',pay:180,xp:3,desc:'Logica e padroes',themes:['ex','md'],energy:2}
];
const SHOP=[
  {id:'solar',name:'Painel Solar',desc:'-30% na conta de luz',cost:450,bill:'luz',pct:0.30,math:'pct'},
  {id:'bike',name:'Bicicleta Elétrica',desc:'-40% no transporte',cost:380,bill:'transporte',pct:0.40,math:'pct'},
  {id:'net',name:'Plano Fibra',desc:'-25% na internet',cost:220,bill:'internet',pct:0.25,math:'pct'},
  {id:'fridge',name:'Geladeira Eficiente',desc:'-15% nas compras',cost:520,bill:'compras',pct:0.15,math:'pct'},
  {id:'led',name:'Iluminação LED',desc:'-20% na luz',cost:180,bill:'luz',pct:0.20,math:'pct'}
];
// ===== CURSOS / UPGRADES DE SKILL (feature 6) =====
const COURSES=[
  {id:'streak',name:'Curso de Sequência',desc:'+20% no bônus de streak',cost:300,effect:'streakMul',val:1.2},
  {id:'speed',name:'Técnica Rápida',desc:'-5s no tempo da trava',cost:280,effect:'lockTime',val:-5},
  {id:'focus',name:'Foco Total',desc:'+1 operação por rodada',cost:400,effect:'maxOps',val:1}
];
// ===== CONQUISTAS (feature 9) =====
const ACH=[
  {id:'first5',name:'Primeiros Passos',cond:g=> (g.cor||0)>=5, reward:30, title:null},
  {id:'pct10',name:'Rei da %',cond:g=> (g.ok.pct||[0,0])[0]>=8, reward:50, title:'Rei da %'},
  {id:'noDebt',name:'Sem Dívida',cond:g=> g.debt===0 && g.r>=14, reward:40, title:'Livre de Dívida'},
  {id:'rich',name:'Patrimônio 3k',cond:g=> nw()>=3000, reward:80, title:'Investidor'},
  {id:'shopper',name:'Economista',cond:g=> Object.keys(g.owned||{}).length>=3, reward:60, title:'Economista'},
  {id:'saver',name:'Poupador',cond:g=> (g.sav||0)>=800, reward:45, title:'Poupador'}
];
// ===== gerador de perguntas =====
function pctQ(l,asset){
  const up=R(0,1);let p,v;
  if(l==0){p=P([10,20,25,50]);v=P([100,200,400,500])}
  else if(l==1){p=P([5,15,30,40,75]);v=P([80,120,200,240,400])}
  else{p=P([8,12,35,45]);v=P([50,150,250,400])}
  const d=v*p/100,a=up?v+d:v-d;
  return{q:asset?`${M(v)} em ${asset} ${up?'subiram':'caíram'} ${p}%. Quanto valem agora?`:`Um item de ${M(v)} ${up?'sobe':'tem desconto de'} ${p}%. Qual o preço final?`,a,e:`${p}% de ${v} = ${f(d)}. ${v} ${up?'+':'-'} ${f(d)} = ${f(a)}`}
}
function Q(t,l){let a,b,c,d,x,k;switch(t){
 case'pct':k=R(0,2);
  if(l==0||k==0)return pctQ(l);
  if(l==1){const p=P([5,15,30,40,75]),v=P([80,120,200,240,400]);return{q:`Quanto é ${p}% de ${M(v)}?`,a:v*p/100,e:`${v} × ${p} ÷ 100 = ${f(v*p/100)}`}}
  if(k==1){v=P([100,200,500]);return{q:`Um preço de ${M(v)} sobe 20% e depois cai 10%. Qual o preço final?`,a:v*1.08,e:`+20%: ${f(v*1.2)}. -10% de ${f(v*1.2)} = ${f(v*.12)} → ${f(v*1.08)}`}}
  {const w=P([200,400,50,250]),p=P([12,30,35,45,60]),pt=w*p/100;return{q:`${f(pt)} é quantos % de ${w}?`,a:p,e:`${f(pt)} ÷ ${w} × 100 = ${p}%`}}
 case'md':if(l==0){a=R(2,10);b=R(2,10);return R(0,1)?{q:`${a} × ${b}`,a:a*b,e:`${a} × ${b} = ${a*b}`}:{q:`${a*b} ÷ ${b}`,a,e:`${b} × ${a} = ${a*b}`}}
  if(l==1){a=R(12,25);b=R(3,9);return R(0,1)?{q:`${a} × ${b}`,a:a*b,e:`${a}×${b}: ${a}×${b} = ${a*b}`}:{q:`${a*b} ÷ ${b}`,a,e:`${b} × ${a} = ${a*b}`}}
  a=R(12,25);b=R(12,25);x=P([1.5,2.5,12.5,.75]);d=P([4,8,12]);return R(0,1)?{q:`${a} × ${b}`,a:a*b,e:`${a}×${b} = ${a*b}`}:{q:`${f(x)} × ${d}`,a:x*d,e:`${f(x)} × ${d} = ${f(x*d)}`}
 case'dec':if(l==0){a=R(11,99)/10;b=R(11,99)/10;return{q:`${f(a)} + ${f(b)}`,a:a+b,e:`Alinhe as vírgulas: ${f(a+b)}`}}
  if(l==1){a=R(500,9999)/100;b=R(10,499)/100;return R(0,1)?{q:`${f(a)} + ${f(b)}`,a:a+b,e:`Alinhe as vírgulas: ${f(a+b)}`}:{q:`${f(a)} - ${f(b)}`,a:a-b,e:`Alinhe as vírgulas: ${f(a-b)}`}}
  a=P([50,100,200]);b=R(1000,a*100-100)/100;return{q:`Você pagou ${M(a)} por algo de ${M(b)}. Qual o troco?`,a:a-b,e:`${f(a)} - ${f(b)} = ${f(a-b)}`}
 case'eq':if(l==0){x=R(2,15);a=R(2,9);return{q:`x + ${a} = ${x+a}. Quanto vale x?`,a:x,e:`x = ${x+a} - ${a} = ${x}`}}
  if(l==1){x=R(2,12);a=R(2,9);b=R(1,9);return R(0,1)?{q:`${a}x = ${a*x}. Quanto vale x?`,a:x,e:`x = ${a*x} ÷ ${a} = ${x}`}:{q:`${a}x + ${b} = ${a*x+b}. Quanto vale x?`,a:x,e:`${a}x = ${a*x+b} - ${b} = ${a*x}; x = ${x}`}}
  x=R(3,12);a=R(3,6);b=R(1,5);c=a*x-b-x;return{q:`${a}x - ${b} = x + ${c}. Quanto vale x?`,a:x,e:`${a}x - x = ${c} + ${b} → ${a-1}x = ${c+b} → x = ${x}`}
 case'int':if(l==0){a=R(1,20);b=R(1,20);return{q:`Seu saldo é -${a}. Você recebe ${b}. Qual o novo saldo?`,a:b-a,e:`-${a} + ${b} = ${b-a}`}}
  if(l==1){a=R(2,9);b=R(2,9);return R(0,1)?{q:`(-${a}) × ${b}`,a:-a*b,e:`Sinais diferentes dão negativo: -${a*b}`}:{q:`${a} - ${a+b}`,a:-b,e:`${a} - ${a+b} = -${b}`}}
  a=R(5,20);b=R(2,15);c=R(1,10);return{q:`-${a} - (-${b}) + ${c}`,a:-a+b+c,e:`Menos com menos vira mais: -${a} + ${b} + ${c} = ${-a+b+c}`}
 case'fr':d=l==0?P([2,4,5]):l==1?P([4,5,10]):P([3,6,8,12]);a=l==0?1:R(2,d-1);v=d*R(3,12);return{q:`${a}/${d} de ${v}`,a:v/d*a,e:`${v} ÷ ${d} = ${v/d}; × ${a} = ${v/d*a}`}
 case'ex':a=R(2,9);b=R(2,9);c=R(2,9);d=R(2,9);if(l==0)return{q:`${a} + ${b} × ${c}`,a:a+b*c,e:`Primeiro ×: ${b*c}; depois + ${a} = ${a+b*c}`};
  if(l==1)return{q:`(${a} + ${b}) × ${c} - ${d}`,a:(a+b)*c-d,e:`Parênteses: ${a+b}; × ${c} = ${(a+b)*c}; - ${d} = ${(a+b)*c-d}`};
  k=R(2,6);x=P([2,3]);return{q:`${a} + ${b} × (${c} + ${d}) - ${k*x} ÷ ${x}`,a:a+b*(c+d)-k,e:`(${c+d}); ${b}×${c+d}=${b*(c+d)}; ${k*x}÷${x}=${k}; total ${a+b*(c+d)-k}`}
 default:if(l==0){a=R(2,4);k=R(2,4);b=R(5,20);return{q:`${a} canetas custam ${M(a*b)}. Quanto custam ${a*k}?`,a:b*a*k,e:`1 caneta = ${b}; × ${a*k} = ${b*a*k}`}}
  if(l==1){a=R(2,6);b=R(3,12);c=R(3,15);return{q:`${a} kg custam ${M(a*c)}. Quanto custam ${b} kg?`,a:b*c,e:`1 kg = ${c}; × ${b} = ${b*c}`}}
  a=P([2,3,4,6]);d=R(2,6);return{q:`12 operários levam ${d} dias. Com ${a} operários, quantos dias?`,a:12*d/a,e:`Menos operários, mais dias: 12×${d} = ${12*d}; ÷ ${a} = ${12*d/a}`}}}
const pick=()=>{const t=g.th;return P(t)};
// ===== estado =====
let g=null,PR=[],tick=null;
const px=(i,r=g.r)=>Math.max(8,Math.round(PR[i][HI+Math.max(-HI+1,Math.min(r,g.N))]/5)*5);
const nw=()=>g.cash+(g.sav||0)+AS.reduce((s,_,i)=>s+(g.h[i]?g.h[i].q*px(i):0),0)-g.debt;
const HI=40;
let WK=[];
function mkMarket(){
  const r=rng(g.seed), w=rng(g.seed+'w'), rs=rng(g.seed+'p');
  // personalidade de cada ativo: tendência base, amplitude de ciclo, volatilidade, chance de choque
  const personality=AS.map((_,i)=>({
    drift: rs()*0.012 - 0.004,          // tendência leve
    cycleAmp: 0.012 + rs()*0.025,       // ciclo mais forte
    cycleSpd: 0.35 + rs()*0.55,         // velocidade do ciclo
    phase: rs()*6.28,
    vol: 0.018 + rs()*0.035,            // ruído diário maior
    shockChance: 0.04 + rs()*0.06,      // chance de salto
    meanRev: 0.08 + rs()*0.12           // puxa de volta à média
  }));
  WK=AS.map(()=>Array.from({length:g.N+HI+2},()=>[w(),w()]));
  PR=AS.map(([n,b,dr,am,vo],i)=>{
    const pe=personality[i];
    let p=b, o=[p], mean=b;
    for(let t=1;t<=g.N+HI+1;t++){
      // ciclo + tendência
      const cycle = pe.cycleAmp * Math.sin(pe.cycleSpd * t + pe.phase);
      // ruído
      const noise = (r()-0.5) * 2 * pe.vol * vo;
      // mean-reversion suave
      const rev = pe.meanRev * (mean - p) / mean;
      // choque ocasional (notícia boa/ruim)
      let shock=0;
      if(r() < pe.shockChance) shock = (r()<0.5?-1:1) * (0.04 + r()*0.09) * vo;
      // momentum leve (continua o movimento anterior)
      const prevRet = t>1 ? (o[t-1]-o[t-2])/o[t-2] : 0;
      const mom = prevRet * 0.25;
      p *= 1 + pe.drift + cycle + noise + rev + shock + mom;
      p = Math.max(p, b*0.25); // não quebra
      mean = mean*0.97 + p*0.03;
      o.push(p);
    }
    // normaliza para começar perto do preço base
    const k=b/o[HI];
    return o.map(x=>x*k);
  });
}
function parse(c){const [s,l,h,m,t]=c.trim().toUpperCase().split('-'),H=parseInt(h,16);
  if(!s||s.length<5||!(+l>=0&&+l<3)||!H||!(+m>=1&&+m<=6)||!(+t>=45&&+t<=150))return null;
  return{seed:s,lvl:+l,th:TH.filter((_,i)=>H>>i&1).map(x=>x[0]),N:+m*7,secs:+t}}
// ===== contas mensais dinâmicas (com upgrades) =====
function billsNow(){
  let total=0, parts={};
  for(const [k,v] of Object.entries(BILLS_BASE)){
    let red=0;
    for(const id of Object.keys(g.owned||{})){
      const it=SHOP.find(x=>x.id===id);
      if(it&&it.bill===k)red+=it.pct;
    }
    red=Math.min(red,0.7);
    if(k==='aluguel'&&g.rentOwn){parts[k]=0;continue} parts[k]=Math.round(v*(1-red));
    total+=parts[k];
  }
  return{total,parts};
}
// ===== telas =====
const A=h=>{$('#app').innerHTML=h};
const go=id=>$('#'+id).scrollIntoView();
function solo(){g={seed:'SOLO'+R(1,99999),lvl:0,th:['pct'],N:21,secs:75,nick:'Treino',r:0,cash:1000,debt:0,h:{},streak:0,ops:0,ok:{},t:0,m:null,tab:0,msg:'',fb:null,done:false,owned:{},sav:0,ins:0,streakMul:1,lockBonus:0,maxOpsBonus:0,streakShield:0,divMul:1,team:'',titles:[],achDone:{},missions:[],event:null,loan:0,goal:P([1200,1800,2400]),goalPaid:0,goalDone:false,divTotal:0,opsOk:0,missionsDone:0,inflation:0,noHint:false,sideJob:0,news:'',imprev:null,rentDisc:0,rentOffer:false,monthLog:[],cashback:0,tot:0,cor:0,chartMode:'vela',job:null,jobLvl:0,jobXp:0,energy:3,promo:0,tips:0,autoInvest:0,watchlist:[],alerts:[],badgeXP:0,seasonPass:0,combo:0,lucky:0,research:0,mentor:0,cryptoOn:0,bond:0,rentOwn:0,taxPaid:0,fame:0};mkMarket();genMissions();newRound()}
function menu(){const sv=ST('mm');A(`<div class="nav"><b class="big">📈 matemercado <span class="mu">2099</span></b><button class="g" onclick="prof()">Sou professor</button></div>
<div class="hero2"><div><div class="kick">MATEMÁTICA PARA A VIDA</div><div class="mu" style="letter-spacing:.12em;font-size:13px;margin-top:4px">TRÊS MESES. CONTAS QUE VENCEM. ESCOLHAS QUE CUSTAM.</div>
<h1>Seu salário. Seu plano. Seu próximo investimento.</h1>
<p class="mu">Salário, contas, Day Trade, dívidas, upgrades e equipes. As contas chegam mesmo para quem fica parado, e quem entende de matemática chega mais longe.</p>
<div><span class="chip">Calcular rápido</span><span class="chip">Investir com cabeça</span><span class="chip">Pagar em dia</span><span class="chip">Reduzir gastos</span></div></div>
<div class="card"><div style="font-size:54px">📈</div><h3>Dinheiro é só parte da história.</h3><p class="mu">Ações, dívidas, upgrades e planejamento decidem quem termina com mais patrimônio.</p>
<div class="row"><button onclick="go('fm')">Sou aluno</button><button class="g" onclick="prof()">Sou professor</button></div>
<button class="g" style="width:100%;margin-top:8px" onclick="solo()">Testar sozinho</button>${sv?'<button class="g" style="width:100%;margin-top:8px" onclick="resume()">Continuar jogo salvo</button>':''}</div></div>
<h2 class="sec" id="fm">Entrar na sala</h2><div class="card"><p class="mu">Cada aluno entra com seu próprio apelido, nunca o nome completo. Digite o código que o professor mostrou no quadro.</p>
<input id="c" placeholder="Código da sala" style="width:100%;margin-bottom:8px"><input id="n" maxlength="14" placeholder="Seu apelido" style="width:100%;margin-bottom:8px">
<input id="tm" maxlength="8" placeholder="Código de equipe (opcional)" style="width:100%;margin-bottom:8px">
<button style="width:100%" onclick="start()">Entrar no mercado</button></div>
<p class="mu" style="text-align:center;margin-top:24px">Até 40 jogadores • Só apelido, sem cadastro • Progresso salvo neste computador</p>`)}
function prof(){A(`<h2>Professor - criar sala</h2><div class="card"><div class="row"><div><label>Nível</label><select id="l"><option value="0">Fácil (×1)</option><option value="1">Médio (×1,5)</option><option value="2">Difícil (×2)</option></select></div>
<div><label>Meses (7 rodadas cada)</label><select id="m">${[1,2,3,4,5,6].map(i=>`<option ${i==3?'selected':''}>${i}</option>`).join('')}</select></div>
<div><label>Segundos por rodada</label><select id="t">${[60,75,90,120].map(i=>`<option ${i==75?'selected':''}>${i}</option>`).join('')}</select></div></div>
<p>Temas (vários = modo misto):</p>${TH.map((x,i)=>`<label><input type="checkbox" class="th" value="${i}" ${i==0?'checked':''}> ${x[1]}</label>`).join('')}
<button style="width:100%;margin-top:10px" onclick="mk()">Gerar código da sala</button><div id="o"></div></div>
<div class="card"><h3>Resultados da turma</h3><p class="mu">Cada aluno vê um “código de resultado” no fim. Cole um por linha:</p>
<input id="rs" placeholder="Código da sala" style="width:100%;margin-bottom:8px"><textarea id="rr" rows="5" style="width:100%" placeholder="Nick~1234~AB12  ou  Nick~1234~AB12~EQUIPE"></textarea>
<button style="width:100%;margin-top:8px" onclick="rank()">Montar ranking</button><div id="rk" class="sc"></div></div><button class="g" onclick="menu()">Voltar</button>`)}
function mk(){const H=[...document.querySelectorAll('.th:checked')].reduce((s,e)=>s|1<<+e.value,0);if(!H)return alert('Escolha ao menos um tema.');
  const s=Array.from({length:5},()=>P([...'ABCDEFGHJKMNPQRSTUVWXYZ23456789'])).join(''),c=`${s}-${$('#l').value}-${H.toString(16).toUpperCase()}-${$('#m').value}-${$('#t').value}`;
  $('#o').innerHTML=`<p class="mu">Passe este código aos alunos (projete no quadro):</p><div class="code">${c}</div>`;$('#rs').value=c}
function rank(){const c=parse($('#rs').value);if(!c)return alert('Código da sala inválido.');
  const L=$('#rr').value.split('\n').map(x=>x.trim().split('~')).filter(x=>x.length>=3).map(([n,w,k,t])=>({n,w:+w,ok:chk(c.seed,n,+w)==k.toUpperCase(),team:(t||'').toUpperCase()})).sort((a,b)=>b.w-a.w);
  const teams={};L.forEach(x=>{if(x.team){teams[x.team]=teams[x.team]||{sum:0,n:0};teams[x.team].sum+=x.w;teams[x.team].n++}});
  let html=`<table><tr><th>#</th><th>Aluno</th><th>Patrimônio</th><th>Equipe</th><th></th></tr>${L.map((x,i)=>`<tr><td>${i+1}</td><td>${x.n.replace(/</g,'&lt;')}</td><td>${M(x.w)}</td><td>${x.team||'-'}</td><td class="${x.ok?'up':'dn'}">${x.ok?'▲ válido':'▼ código alterado'}</td></tr>`).join('')}</table>`;
  if(Object.keys(teams).length){html+=`<h3 style="margin-top:16px">Ranking de equipes</h3><table><tr><th>Equipe</th><th>Média</th><th>Membros</th></tr>${Object.entries(teams).sort((a,b)=>b[1].sum/b[1].n-a[1].sum/a[1].n).map(([t,v])=>`<tr><td>${t}</td><td>${M(v.sum/v.n)}</td><td>${v.n}</td></tr>`).join('')}</table>`}
  $('#rk').innerHTML=html}
function start(){const c=parse($('#c').value),n=$('#n').value.replace(/[~<>|]/g,'').trim(),tm=($('#tm')?$('#tm').value:'').replace(/[^A-Za-z0-9]/g,'').toUpperCase().slice(0,8);
  if(!c)return alert('Código da sala inválido.');if(n.length<3)return alert('Apelido com 3 a 14 letras.');
  g={...c,nick:n,r:0,cash:1000,debt:0,h:{},streak:0,ops:0,ok:{},t:0,m:null,tab:0,msg:'',fb:null,done:false,owned:{},sav:0,ins:0,streakMul:1,lockBonus:0,maxOpsBonus:0,streakShield:0,divMul:1,team:tm,titles:[],achDone:{},missions:[],event:null,loan:0,goal:P([1200,1800,2400]),goalPaid:0,goalDone:false,divTotal:0,opsOk:0,missionsDone:0,inflation:0,noHint:false,sideJob:0,news:'',imprev:null,rentDisc:0,rentOffer:false,monthLog:[],cashback:0,tot:0,cor:0,chartMode:'vela',job:null,jobLvl:0,jobXp:0,energy:3,promo:0,tips:0,autoInvest:0,watchlist:[],alerts:[],badgeXP:0,seasonPass:0,combo:0,lucky:0,research:0,mentor:0,cryptoOn:0,bond:0,rentOwn:0,taxPaid:0,fame:0};mkMarket();genMissions();newRound()}
function resume(){try{g=JSON.parse(ST('mm'));mkMarket();run();draw()}catch(e){ST('mm','');menu()}}
function save(){ST('mm',g.done?'':JSON.stringify(g))}
// ===== missões mensais (feature 7) =====
function genMissions(){
  const opts=[
    {id:'pct3',txt:'Acerte 3 desafios de porcentagem',type:'pct',need:3,prog:0,rew:60},
    {id:'ops4',txt:'Faça 4 operações de mercado com sucesso',type:'ops',need:4,prog:0,rew:70},
    {id:'save200',txt:'Guarde pelo menos R$ 200 na poupança',type:'sav',need:200,prog:0,rew:50},
    {id:'nodebt',txt:'Termine o mês sem dívida',type:'nodebt',need:1,prog:0,rew:80},
    {id:'bonus2',txt:'Pegue bônus em 2 desafios seguidos',type:'streak',need:2,prog:0,rew:55}
  ];
  const a=P(opts),b=P(opts.filter(x=>x.id!==a.id));
  g.missions=[{...a,prog:0,done:false,claimed:false},{...b,prog:0,done:false,claimed:false}];
}
// ===== eventos aleatórios (feature 3) =====
function maybeEvent(){
  if(g.r%5!==0||g.r===0)return;
  const evs=[
    {id:'infl',q:'Inflação de 8% nas contas! Quanto fica a conta de luz base (R$ 80) com +8%?',a:86.4,e:'80 × 1,08 = 86,4',effect:()=>{g.cash-=40;g.msg='▼ Inflação cobrou R$ 40 extra.'}},
    {id:'opp',q:'Oportunidade: ação X subiu 25%. Se valia R$ 200, quanto vale agora?',a:250,e:'200 × 1,25 = 250',effect:()=>{g.cash+=80;g.msg='▲ Você aproveitou a oportunidade: +R$ 80.'}},
    {id:'crisis',q:'Crise: patrimônio cai 10%. Se você tem R$ 1500, quanto perde?',a:150,e:'1500 × 0,10 = 150',effect:()=>{const loss=Math.min(g.cash,Math.round(nw()*0.05));g.cash-=loss;g.msg=`▼ Crise: -${M(loss)}`}},
    {id:'bonus',q:'Bônus do governo: 15% do seu salário (R$ 150). Quanto recebe?',a:22.5,e:'150 × 0,15 = 22,5',effect:()=>{g.cash+=40;g.msg='▲ Bônus governamental: +R$ 40'}}
  ];
  g.event=P(evs);
}
// ===== rodada =====
function newRound(){g.r++;g.cash+=SAL;g.t=g.secs;g.ops=0;g.energy=3+((g.jobLvl||0)>2?1:0);g.msg='';g.fb=null;const l=g.lvl,q=Q(pick(),l);g.ch={...q,l,t0:Date.now()};g.chDone=false;
  if(g.sav>0){const j=Math.round(g.sav*0.01*100)/100;g.sav+=j;g.msg=`▲ Poupança rendeu ${M(j)} (1%).`}
  if(g.r%7===0){let div=0;AS.forEach((_,i)=>{if(g.h[i]&&g.h[i].q>0)div+=px(i)*g.h[i].q*0.03*(g.divMul||1)});
    if(div>0){div=Math.round(div*100)/100;g.cash+=div;g.divTotal=(g.divTotal||0)+div;g.msg=`▲ Dividendos ${M(div)}`}}
  if(g.loan>0){const pay=Math.min(g.loan,Math.round(g.loan*0.15)+20);g.cash-=pay;g.loan=Math.max(0,g.loan-pay);if(g.loan<=0)g.msg+=' Empréstimo quitado!'}
  const p=Math.min(g.debt,g.cash);g.cash-=p;g.debt-=p;
  if(g.r%3===1)g.news=P(['TECHNOVA anuncia produto.','ORBIT sofre rumor.','SOLARIS sobe com energia limpa.','NEOCOIN volátil.','AQUA-X estável.']);
  if(g.r>3&&g.r%8===0&&!g.imprev){g.imprev=P([
    {name:'Geladeira quebrou',cost:280,q:'Conserto R$ 280 + 10% cartão. Total?',a:308,e:'280×1,10=308'},
    {name:'Pneu furado',cost:90,q:'R$ 90 + 15% deslocamento. Total?',a:103.5,e:'90×1,15=103,5'},
    {name:'Remédio',cost:65,q:'R$ 65 com 20% off. Paga quanto?',a:52,e:'65×0,8=52'}
  ])}
  maybeEvent();checkAch();save();run();draw()}
function endRound(){g.m=null;g.event=null;
  if(g.r%7==0){
    g.inflation=(g.inflation||0)+R(0,3);
    if(g.bond>0){const bj=Math.round(g.bond*0.02*100)/100;g.bond+=bj;g.msg=(g.msg||'')+` Titulo +${M(bj)}.`;}
    if(g.autoInvest&&g.cash>SAL){const inv=Math.round(SAL*0.1);const p=px(0);const n=Math.max(1,Math.floor(inv/p));
      if(n*p*(1+FEE)<=g.cash){const c=n*p*(1+FEE);g.cash-=c;const h=g.h[0]=g.h[0]||{q:0,c:0};h.q+=n;h.c+=c;}}
    
    const b=billsNow();
    let total=b.total;
    if(g.rentDisc>0){total-=Math.round((b.parts.aluguel||0)*g.rentDisc);g.rentDisc=0}
    g.cash-=total;
    if(g.cash<0){g.debt+=-g.cash;g.cash=0}
    const rate=g.ins>0?DEBT*0.5:DEBT;
    g.debt*=1+rate;
    if(g.ins>0)g.ins--;
    g.missions.forEach(m=>{
      if(m.type==='nodebt'&&g.debt===0){m.prog=1;m.done=true}
      if(m.type==='sav'&&g.sav>=m.need){m.prog=m.need;m.done=true}
      if(m.done&&!m.claimed){g.cash+=m.rew;m.claimed=true;g.missionsDone=(g.missionsDone||0)+1;g.msg=`▲ Missão "${m.txt}" concluída! +${M(m.rew)}`}
    });
    g.monthLog=g.monthLog||[];g.monthLog.push({mo:Math.ceil(g.r/7),pat:Math.round(nw()),bills:total});
    if(Math.ceil(g.r/7)%2===0)g.rentOffer=true;
    genMissions();
  }
  if(g.r>=g.N)return fin();
  newRound()}
function run(){clearInterval(tick);tick=setInterval(()=>{if(!g||g.done)return;g.t--;if(g.m){g.m.t--;if(g.m.t<=0){if(g.m.type){g.m=null;g.msg='▼ Tempo esgotado.';save();draw();return}return ans(1)}}
  if(g.t<=0)return endRound();const e=$('#tm');if(e)e.textContent=g.t+'s';const q=$('#mt');if(q&&g.m)q.textContent=g.m.t+'s'},1000)}
function norm(s){return parseFloat(String(s).replace(/R\$|%|\s/g,'').replace('-','-').replace(',','.'))}
function log(l,ok){const k=g.lt||'';g.ok[k]=g.ok[k]||[0,0];g.ok[k][1]++;if(ok)g.ok[k][0]++}
// responder desafio da rodada (bônus)
function bonus(){const v=norm($('#bi').value);if(isNaN(v)||g.chDone)return;const ok=Math.abs(v-g.ch.a)<.006,l=g.ch.l;g.chDone=true;
  g.tot=(g.tot||0)+1;if(ok)g.cor=(g.cor||0)+1;
  if(ok){g.streak++;const b=Math.min(50,10*g.streak)*MULT[l]*(g.streakMul||1);g.cash+=b;g.fb=`▲ Acertou! Bônus ${M(b)} (sequência ${g.streak}).`;
    // missões
    g.missions.forEach(m=>{if(m.type==='streak'&&g.streak>=m.need){m.prog=m.need;m.done=true}if(m.type==='pct'&&g.ch.q.includes('%')){m.prog=(m.prog||0)+1;if(m.prog>=m.need)m.done=true}});
  }else{g.streak=0;g.fb=`▼ Errou. Resposta: ${f(g.ch.a)}. ${g.ch.e}`}
  save();draw()}
// operação de mercado com trava matemática
function trade(i,side){const n=Math.floor(+$('#qty').value);if(!n||n<1)return g.msg='Quantidade inválida (use 1 ou mais).',draw();const p=px(i);
  const maxO=MAXOPS+(g.maxOpsBonus||0);
  if(g.ops>=maxO)return g.msg='Limite de operações por rodada.',draw();
  if(side=='b'&&p*n*(1+FEE)>g.cash)return g.msg='Saldo insuficiente.',draw();
  if(side=='s'&&!(g.h[i]&&g.h[i].q>0))return g.msg='Você não tem esta ação.',draw();
  const q=pctQ(g.lvl,AS[i][0]);g.m={...q,i,side,n,t:Math.max(15,QT[g.lvl]+(g.lockBonus||0))};draw();setTimeout(()=>$('#ai')&&$('#ai').focus(),50)}
function ans(timeout){const m=g.m;if(!m)return;const v=norm($('#ai')?$('#ai').value:'');if(!timeout&&isNaN(v))return;
  const ok=!timeout&&Math.abs(v-m.a)<.006;g.m=null;
  g.tot=(g.tot||0)+1;if(ok)g.cor=(g.cor||0)+1;
  if(ok){exec(m.i,m.side,m.n);g.ops++;
    g.missions.forEach(mm=>{if(mm.type==='ops'){mm.prog=(mm.prog||0)+1;if(mm.prog>=mm.need)mm.done=true}});
  }else{g.ops=MAXOPS+(g.maxOpsBonus||0);g.msg=`▼ ${timeout?'Tempo esgotado':'Errou'}: operação perdida nesta rodada. ${m.e}`}save();draw()}
function exec(i,side,n){const p=px(i),h=g.h[i]=g.h[i]||{q:0,c:0};
  if(side=='b'){const c=p*n*(1+FEE);g.cash-=c;h.q+=n;h.c+=c;g.msg=`▲ Comprou ${n} × ${AS[i][0]} por ${M(c)} (com corretagem de 2%).`}
  else{n=Math.min(n,h.q);const gross=p*n,fee=gross*FEE,basis=h.c*n/h.q,pf=gross-fee-basis,tax=Math.max(0,pf)*TAX;g.cash+=gross-fee-tax;h.q-=n;h.c-=basis;
    g.msg=`${pf>=0?'▲':'▼'} Vendeu ${n} × ${AS[i][0]}: ${pf>=0?'lucro':'prejuízo'} ${M(Math.abs(pf))}${pf>0?` (imposto ${M(tax)})`:''}.`}}
// ===== LOJA (feature 1) =====
function buyItem(id){
  const it=SHOP.find(x=>x.id===id);if(!it||g.owned[id])return;
  if(g.cash<it.cost)return g.msg='Saldo insuficiente para a compra.',draw();
  // trava matemática: calcular o desconto
  const q={q:`O item custa ${M(it.cost)}. Você tem ${M(g.cash)}. Quanto sobra depois da compra?`,a:g.cash-it.cost,e:`${f(g.cash)} - ${f(it.cost)} = ${f(g.cash-it.cost)}`};
  g.m={...q,type:'shop',item:id,t:45};draw();
}
function confirmShop(){
  const m=g.m;if(!m||m.type!=='shop')return;
  const v=norm($('#ai').value);if(isNaN(v))return;
  const ok=Math.abs(v-m.a)<.05;
  g.m=null;
  if(ok){const it=SHOP.find(x=>x.id===m.item);g.cash-=it.cost;g.owned[it.id]=1;g.msg=`▲ Comprou ${it.name}! ${it.desc}`;checkAch()}
  else g.msg=`▼ Errou o cálculo. Compra cancelada. ${m.e}`;
  save();draw();
}
// ===== POUPANÇA (feature 4) =====
function toSav(){
  const v=norm($('#sv').value);if(isNaN(v)||v<=0||v>g.cash)return g.msg='Valor inválido.',draw();
  g.cash-=v;g.sav=(g.sav||0)+v;g.msg=`▲ Transferiu ${M(v)} para a poupança.`;save();draw();
}
function fromSav(){
  const v=norm($('#sv').value);if(isNaN(v)||v<=0||v>g.sav)return g.msg='Valor inválido.',draw();
  g.sav-=v;g.cash+=v;g.msg=`▲ Sacou ${M(v)} da poupança.`;save();draw();
}
// ===== SEGURO (feature 5) =====
function buyIns(){
  if(g.cash<120)return g.msg='Precisa de R$ 120.',draw();
  g.cash-=120;g.ins=(g.ins||0)+2;g.msg='▲ Seguro ativo por 2 meses (juros da dívida -50%).';save();draw();
}
// ===== CURSOS (feature 6) =====
function buyCourse(id){
  const c=COURSES.find(x=>x.id===id);if(!c||g['course_'+id])return;
  if(g.cash<c.cost)return g.msg='Saldo insuficiente.',draw();
  g.cash-=c.cost;g['course_'+id]=1;
  if(c.effect==='streakMul')g.streakMul=(g.streakMul||1)*c.val;
  if(c.effect==='lockTime')g.lockBonus=(g.lockBonus||0)+c.val;
  if(c.effect==='maxOps')g.maxOpsBonus=(g.maxOpsBonus||0)+c.val;
  g.msg=`▲ Curso "${c.name}" concluído! ${c.desc}`;save();draw();
}
// ===== EMPRÉSTIMO (feature 8) =====
function askLoan(){
  if(g.loan>0)return g.msg='Você já tem empréstimo ativo.',draw();
  const q=Q('eq',Math.min(2,g.lvl+1));
  g.m={...q,type:'loan',t:50};draw();
}
function confirmLoan(){
  const m=g.m;if(!m||m.type!=='loan')return;
  const v=norm($('#ai').value);if(isNaN(v))return;
  const ok=Math.abs(v-m.a)<.006;
  g.m=null;
  if(ok){g.loan=400;g.cash+=400;g.msg='▲ Empréstimo de R$ 400 aprovado (15% ao mês + amortização).';}
  else g.msg=`▼ Crédito negado. ${m.e}`;
  save();draw();
}
// ===== EVENTO (feature 3) =====
function ansEvent(){
  const v=norm($('#ev').value);if(isNaN(v)||!g.event)return;
  const ok=Math.abs(v-g.event.a)<.1;
  if(ok){g.event.effect();g.cor=(g.cor||0)+1}
  else{g.msg=`▼ Errou o evento. ${g.event.e}`;g.cash=Math.max(0,g.cash-25)}
  g.tot=(g.tot||0)+1;g.event=null;save();draw();
}
// ===== CONQUISTAS (feature 9) =====
function checkAch(){
  ACH.forEach(a=>{
    if(g.achDone[a.id])return;
    if(a.cond(g)){g.achDone[a.id]=1;g.cash+=a.reward;
      if(a.title&&!g.titles.includes(a.title))g.titles.push(a.title);
      g.msg=`▲ Conquista: ${a.name}! +${M(a.reward)}${a.title?' · Título: '+a.title:''}`;
    }
  });
}
function fin(){g.done=true;clearInterval(tick);const w=nw();ST('mm','');
  const teamPart=g.team?`~${g.team}`:'';
  A(`<h1>FIM DE JOGO</h1><div class="card"><p>${g.nick}${g.titles.length?` <span class="title-chip">${g.titles[g.titles.length-1]}</span>`:''}, seu patrimônio final:</p><div class="code">${M(w)}</div>
<p>Entregue este código ao professor:</p><div class="code" id="cd">${g.nick}~${Math.round(w)}~${chk(g.seed,g.nick,w)}${teamPart}</div>
<button style="width:100%" onclick="navigator.clipboard&&navigator.clipboard.writeText($('#cd').textContent)">Copiar código</button></div>
<div class="card"><h3>Seus acertos</h3><p class="mu">Desafios e operações respondidos corretamente.</p><p>${g.cor||0} de ${g.tot||0}</p>
${g.titles.length?`<p>Títulos: ${g.titles.map(t=>`<span class="title-chip">${t}</span>`).join(' ')}</p>`:''}
${Object.keys(g.owned||{}).length?`<p class="mu">Upgrades: ${Object.keys(g.owned).map(id=>SHOP.find(x=>x.id===id)?.name).join(', ')}</p>`:''}
</div><button class="g" onclick="menu()">Voltar ao menu</button>`)}
// ===== desenho do jogo =====

function toGoal(){const v=norm($('#gv')?$('#gv').value:'');if(isNaN(v)||v<=0||v>g.cash)return g.msg='Valor inválido.',draw();
  g.cash-=v;g.goalPaid=(g.goalPaid||0)+v;
  if(g.goalPaid>=(g.goal||1200)){g.goalDone=true;g.cash+=80;g.msg='▲ META BATIDA! +R$ 80';checkAch()}
  else g.msg=`▲ Guardou ${M(v)} na meta (${M(g.goalPaid)}/${M(g.goal)})`;
  save();draw()}
function sideJob(){if((g.sideJob||0)>=2)return g.msg='Máx. 2 bicos por partida.',draw();
  const q=Q(pick(),g.lvl);g.m={...q,type:'side',t:35};draw()}
function confirmSide(){const m=g.m;if(!m||m.type!=='side')return;const v=norm($('#ai').value);if(isNaN(v))return;
  const ok=Math.abs(v-m.a)<.008;g.m=null;g.tot=(g.tot||0)+1;
  if(ok){const pay=40+R(10,40);g.cash+=pay;g.sideJob=(g.sideJob||0)+1;g.cor=(g.cor||0)+1;g.msg=`▲ Bico +${M(pay)}`}
  else g.msg=`▼ Bico falhou. ${m.e}`;save();draw()}
function solveImprev(){if(!g.imprev)return;g.m={...g.imprev,type:'imprev',t:40};draw()}
function confirmImprev(){const m=g.m;if(!m||m.type!=='imprev')return;const v=norm($('#ai').value);if(isNaN(v))return;
  const ok=Math.abs(v-m.a)<.15;g.m=null;g.tot=(g.tot||0)+1;
  if(ok){g.cash-=m.a;g.cor=(g.cor||0)+1;g.msg=`▲ ${m.name}: pagou ${M(m.a)}`}
  else{g.cash-=Math.round(m.cost*1.2);g.msg=`▼ Errou. Pagou ${M(Math.round(m.cost*1.2))}`}
  g.imprev=null;save();draw()}
function tryRent(){if(!g.rentOffer)return;g.m={...Q('eq',g.lvl),type:'rent',t:40};draw()}
function confirmRent(){const m=g.m;if(!m||m.type!=='rent')return;const v=norm($('#ai').value);if(isNaN(v))return;
  const ok=Math.abs(v-m.a)<.008;g.m=null;g.rentOffer=false;g.tot=(g.tot||0)+1;
  if(ok){g.rentDisc=0.12;g.cor=(g.cor||0)+1;g.msg='▲ Aluguel -12% no próximo vencimento'}
  else g.msg=`▼ Negociação falhou. ${m.e}`;save();draw()}
function toggleHint(){g.noHint=!g.noHint;g.msg=g.noHint?'▲ Modo sem dica ATIVO':'▲ Dicas ligadas';draw()}

function draw(){if(g.done)return;const w=nw(),mo=Math.ceil(g.r/7),left=7-((g.r-1)%7),bills=billsNow();
  const hd=`<div class="top"><div class="row"><div><div class="mu">Dinheiro</div><div class="big">${M(g.cash)}</div></div><div><div class="mu">Patrimônio</div><div class="big">${M(w)}</div></div>
<div><div class="mu">Rodada ${g.r}/${g.N} · Mês ${mo}</div><div class="big" id="tm">${g.t}s</div></div></div>
<div class="mu">Contas de ${M(bills.total)} vencem em ${left} rodada(s)${g.debt>0?` · <span class="dn">▼ Dívida ${M(g.debt)} (juros ${g.ins>0?'2,5':'5'}%/mês)</span>`:''}${g.sav>0?` · <span class="up">Poupança ${M(g.sav)}</span>`:''}${g.loan>0?` · <span class="dn">Empréstimo ${M(g.loan)}</span>`:''}</div>
<div class="bar"><i style="width:${(7-left+1)/7*100}%"></i></div>
<div class="mu">Nível: ${LV[g.lvl]} · ${g.th.map(t=>TH.find(x=>x[0]==t)[1]).join(', ')}${g.team?` · Equipe: <b>${g.team}</b>`:''}${g.titles.length?` · <span class="title-chip">${g.titles[g.titles.length-1]}</span>`:''}</div></div>
<div class="tabbar">
<button class="${g.tab==0?'':'g'}" onclick="g.tab=0;draw()">📈 Mercado</button>
<button class="${g.tab==1?'':'g'}" onclick="g.tab=1;draw()">🏦 Banco</button>
<button class="${g.tab==2?'':'g'}" onclick="g.tab=2;draw()">🛒 Loja</button>
<button class="${g.tab==3?'':'g'}" onclick="g.tab=3;draw()">🎯 Missões</button>
<button class="${g.tab==4?'':'g'}" onclick="g.tab=4;draw()">⚡ Extra</button>
<button class="${g.tab==5?'':'g'}" onclick="g.tab=5;draw()">💼 Trabalho</button>
</div>`;
  let b='';
  if(g.tab==0){
    if(g.news)b+=`<div class="news">📰 ${g.news}</div>`;
    if(g.imprev)b+=`<div class="card" style="border-color:var(--dn)"><h3>🔧 Imprevisto: ${g.imprev.name}</h3><button onclick="solveImprev()">Calcular e pagar</button></div>`;
    b+=`<div class="card"><h3>Desafio da rodada (bônus)</h3>${g.chDone?`<p class="${g.fb&&g.fb[0]=='▲'?'up':'dn shake'}">${g.fb}</p>`:`<p>${g.ch.q}</p><div class="row"><input id="bi" inputmode="decimal" autocomplete="off" onkeydown="event.key=='Enter'&&bonus()" placeholder="Sua resposta"><button onclick="bonus()">Responder</button></div>`}</div>`;
    if(g.event){b+=`<div class="card" style="border-color:var(--pu)"><h3>⚡ Evento aleatório!</h3><p>${g.event.q}</p><div class="row"><input id="ev" inputmode="decimal" placeholder="Resposta"><button onclick="ansEvent()">Resolver</button></div></div>`}
    b+=`<div class="card"><div class="row" style="margin-bottom:8px;justify-content:flex-start">
<span class="mu" style="flex:0;margin-right:6px">Grafico:</span>
<button class="g" style="flex:0;padding:8px 12px;${(g.chartMode||'vela')==='vela'?'outline:2px solid var(--cy)':''}" onclick="setChart('vela')">Velas</button>
<button class="g" style="flex:0;padding:8px 12px;${g.chartMode==='linha'?'outline:2px solid var(--cy)':''}" onclick="setChart('linha')">Linha</button>
<button class="g" style="flex:0;padding:8px 12px;${g.chartMode==='area'?'outline:2px solid var(--cy)':''}" onclick="setChart('area')">Area</button>
</div>
<div class="card"><div class="row" style="margin-bottom:4px"><h3>Day Trade (${g.ops}/${MAXOPS+(g.maxOpsBonus||0)} operações)</h3><input id="qty" type="number" min="1" step="1" value="1" inputmode="numeric" style="max-width:110px" aria-label="Quantidade de cotas" placeholder="Qtd"></div>
${AS.map((a,i)=>{const p=px(i),o=px(i,g.r-1),c=(p/o-1)*100,h=g.h[i],pl=h&&h.q>0?p*h.q-h.c:0;
 return`<div class="asset"><div><b>${a[0]}</b><div class="${c>=0?'up':'dn'}" style="font-weight:700">${M(p)} ${c>=0?'▲ +':'▼ '}${f(c)}%</div>${h&&h.q>0?`<div class="mu">Você tem ${f(h.q)} · <span class="${pl>=0?'up':'dn'}">${pl>=0?'▲ +':'▼ -'}${M(Math.abs(pl))}</span></div>`:''}</div><div class="col"><button onclick="trade(${i},'b')">Comprar</button><button class="g" onclick="trade(${i},'s')">Vender</button></div>${chartSVG(i)}</div>`}).join('')}
<p class="mu">Corretagem 2% · imposto 10% sobre o lucro. Para operar, acerte a conta.</p>${g.msg?`<p class="${g.msg[0]=='▼'?'dn shake':'up'}">${g.msg}</p>`:''}</div>`}
  else if(g.tab==1){
    b+=`<div class="card"><h3>Contas do mês (com seus upgrades)</h3><table>
${Object.entries(bills.parts).map(([k,v])=>`<tr><td>${{aluguel:'Aluguel',compras:'Compras',luz:'Luz e água',internet:'Internet',transporte:'Transporte'}[k]}</td><td>${M(v)}${v<BILLS_BASE[k]?` <span class="up">(-${M(BILLS_BASE[k]-v)})</span>`:''}</td></tr>`).join('')}
<tr><td><b>Total</b></td><td><b>${M(bills.total)}</b> ${bills.total<910?`<span class="up">economia de ${M(910-bills.total)}</span>`:''}</td></tr></table>
<p class="mu">Salário: R$ 150 por rodada. Contas saem só do dinheiro em mãos. Guarde reserva!</p></div>
<div class="card"><h3>Poupança (1% ao mês)</h3><p class="mu">Juros simples creditados no início de cada rodada. Separar dinheiro força planejamento.</p>
<p>Saldo poupança: <b class="up">${M(g.sav||0)}</b></p>
<div class="row"><input id="sv" inputmode="decimal" placeholder="Valor"><button onclick="toSav()">Depositar</button><button class="g" onclick="fromSav()">Sacar</button></div></div>
<div class="card"><h3>Meta de sonho: ${M(g.goal||1200)}</h3>
<div class="goalbar"><i style="width:${Math.min(100,(g.goalPaid||0)/(g.goal||1200)*100)}%"></i></div>
<p class="mu">${M(g.goalPaid||0)} / ${M(g.goal||1200)}${g.goalDone?' · ✅':''}</p>
<div class="row"><input id="gv" inputmode="decimal" placeholder="Guardar na meta"><button onclick="toGoal()">Guardar</button></div></div>
<div class="card"><h3>Seguro e Empréstimo</h3>
<p class="mu">Seguro: R$ 120 → 2 meses com juros da dívida pela metade.</p>
<button onclick="buyIns()" ${g.cash<120?'disabled':''}>Comprar Seguro (R$ 120)</button>
<p class="mu" style="margin-top:12px">Empréstimo de R$ 400 (precisa acertar equação). Juros + amortização automática.</p>
<button class="g" onclick="askLoan()" ${g.loan>0?'disabled':''}>Solicitar Empréstimo</button>
${g.loan>0?`<p class="dn">Empréstimo restante: ${M(g.loan)}</p>`:''}
</div>`}
  else if(g.tab==2){
    b+=`<div class="card"><h3>Loja de Redução de Gastos</h3><p class="mu">Compre itens permanentes. Cada compra exige um cálculo. Economia real nas contas mensais.</p>
${SHOP.map(it=>{const own=g.owned[it.id];
  return`<div class="shop-item"><div><b>${it.name}</b> ${own?'<span class="badge">COMPRADO</span>':''}<div class="mu">${it.desc} · ${M(it.cost)}</div></div>
${own?'':`<button onclick="buyItem('${it.id}')" ${g.cash<it.cost?'disabled':''}>Comprar</button>`}</div>`}).join('')}
</div>
<div class="card"><h3>Cursos de Habilidade</h3><p class="mu">Invista em você. Efeitos permanentes nesta partida.</p>
${COURSES.map(c=>{const own=g['course_'+c.id];
  return`<div class="shop-item"><div><b>${c.name}</b> ${own?'<span class="badge">FEITO</span>':''}<div class="mu">${c.desc} · ${M(c.cost)}</div></div>
${own?'':`<button onclick="buyCourse('${c.id}')" ${g.cash<c.cost?'disabled':''}>Fazer curso</button>`}</div>`}).join('')}
</div>`}
  else if(g.tab==3){
    b+=`<div class="card"><h3>Missões do mês</h3><p class="mu">Complete para ganhar bônus extra. Novas missões todo mês.</p>
${(g.missions||[]).map(m=>`<div class="mission ${m.done?'done':''}"><b>${m.txt}</b><div class="mu">${m.done?'✅ Concluída':`Progresso: ${m.prog||0}/${m.need}`} · Recompensa ${M(m.rew)}</div></div>`).join('')}
</div>
<div class="card"><h3>Conquistas</h3>
${ACH.map(a=>`<div class="mu">${g.achDone[a.id]?'✅':'🔒'} ${a.name}${a.title?` → título "${a.title}"`:''} (+${M(a.reward)})</div>`).join('')}
${g.titles.length?`<p style="margin-top:10px">Seus títulos: ${g.titles.map(t=>`<span class="title-chip">${t}</span>`).join(' ')}</p>`:''}
</div>
<div class="card"><h3>Equipe</h3><p class="mu">${g.team?`Você está na equipe <b>${g.team}</b>. No ranking do professor a média da equipe aparece.`:'Nenhuma equipe. Entre com código de equipe no início para competir em grupo.'}</p></div>`}
  
  else if(g.tab==4){
    b+=`<div class="card"><h3>Bico extra</h3><p class="mu">Resolva uma conta e ganhe R$ 50-80. Max 2.</p>
<button onclick="sideJob()" ${(g.sideJob||0)>=2?'disabled':''}>Fazer bico (${g.sideJob||0}/2)</button></div>
<div class="card"><h3>Modo sem dica</h3><p class="mu">Erros nao mostram a resolucao.</p>
<button class="g" onclick="toggleHint()">${g.noHint?'Ligar dicas':'Ativar sem dica'}</button></div>
<div class="card"><h3>Negociar aluguel</h3>
${g.rentOffer?'<button onclick="tryRent()">Tentar -12% no aluguel</button>':'<p class="mu">Disponivel a cada 2 meses.</p>'}</div>
<div class="card"><h3>Historico mensal</h3>
${(g.monthLog||[]).length?`<table><tr><th>Mes</th><th>Patrimonio</th><th>Contas</th></tr>${g.monthLog.map(x=>`<tr><td>${x.mo}</td><td>${M(x.pat)}</td><td>${M(x.bills)}</td></tr>`).join('')}</table>`:'<p class="mu">Nenhum mes fechado ainda.</p>'}</div>
<div class="card"><h3>Dividendos acumulados</h3><p class="up">${M(g.divTotal||0)}</p></div>`;
  }

  
  else if(g.tab==5){
    const job=g.job?JOBS.find(x=>x.id===g.job):null;
    b+=`<div class="card"><h3>Energia: ${g.energy||0} · Emprego</h3>
<p class="mu">Alem do day trade: trabalhe em turnos. Cada turno exige uma conta. Energia recarrega por rodada.</p>
${job?`<p><b>${job.name}</b> · Nivel ${g.jobLvl||0} · XP ${g.jobXp||0} · Combo ${g.combo||0}</p>
<button onclick="doJobShift()" ${(g.energy||0)<=0?'disabled':''}>Fazer turno (~${M(job.pay+(g.jobLvl||0)*15)})</button>
<button class="g" onclick="quitJob()" style="margin-left:6px">Demissao</button>`
:`<p class="mu">Escolha um emprego:</p>${JOBS.map(j=>`<div class="shop-item"><div><b>${j.name}</b><div class="mu">${j.desc} · ~${M(j.pay)}/turno</div></div>
<button onclick="takeJob('${j.id}')">Aceitar</button></div>`).join('')}`}
</div>
<div class="card"><h3>Boosts</h3>
<button onclick="activateLucky()" ${g.cash<60?'disabled':''}>Sorte +25% (R$60)</button>
<button class="g" onclick="hireMentor()" ${g.cash<200||g.mentor?'disabled':''} style="margin-left:6px">Mentor +15% bonus (R$200)</button>
<p class="mu" style="margin-top:8px">Fama: <b>${g.fame||0}</b> · Turnos: ${g.badgeXP||0}</p>
</div>
<div class="card"><h3>Auto-invest e titulos</h3>
<button onclick="toggleAutoInvest()">${g.autoInvest?'Desligar':'Ligar'} auto-invest 10% salario</button>
<button class="g" onclick="buyBond()" ${g.cash<200?'disabled':''} style="margin-left:6px">Titulo R$200 (+2%/mes)</button>
${g.bond?`<p class="up">Titulos: ${M(g.bond)}</p>`:''}
</div>
<div class="card"><h3>Pesquisa e casa</h3>
<button onclick="buyResearch()" ${g.cash<150?'disabled':''}>Pesquisa R$150</button>
<button class="g" onclick="buyHome()" ${g.cash<2500||g.rentOwn?'disabled':''} style="margin-left:6px">Casa propria R$2500</button>
${g.rentOwn?'<p class="up">Aluguel zerado!</p>':''}
</div>`;
  }

  // modals
  if(g.m){
    const map={shop:['confirmShop()','Trava da compra'],loan:['confirmLoan()','Crédito'],imprev:['confirmImprev()','Imprevisto'],rent:['confirmRent()','Negociação'],side:['confirmSide()','Bico'],job:['confirmJob()','Turno de trabalho']};
    const t=g.m.type, fn=t&&map[t]?map[t][0]:'ans()', title=t&&map[t]?map[t][1]:'Trava da operação';
    b+=`<div class="mod"><div class="card"><div class="row"><h3>${title}</h3><span class="big" id="mt">${g.m.t}s</span></div>
<p>${g.m.q}</p><input id="ai" inputmode="decimal" autocomplete="off" style="width:100%;margin-bottom:8px" onkeydown="if(event.key=='Enter')${fn}" placeholder="Digite a resposta e Enter">
<button style="width:100%" onclick="${fn}">Confirmar</button></div></div>`;
  }
  $('#app').innerHTML=hd+b;
}
// gráfico de velas

function setChart(m){g.chartMode=m;draw()}
function chartSVG(i){
  if((g.chartMode||'vela')==='vela')return candles(i);
  if(g.chartMode==='area')return areaChart(i);
  return lineChart(i);
}
function lineChart(i){
  const n=Math.min(HI,52), r0=g.r-n+1, pts=[];
  for(let r=r0;r<=g.r;r++) pts.push(px(i,r));
  const hi=Math.max(...pts), lo=Math.min(...pts), W=330, H=125;
  const step=(W-14)/(pts.length-1||1);
  const Y=y=>H-8-(y-lo)/(hi-lo||1)*(H-16);
  const path=pts.map((p,k)=>`${k?'L':'M'}${(7+step*k).toFixed(1)},${Y(p).toFixed(1)}`).join(' ');
  const last=pts[pts.length-1], up=pts.length>1&&last>=pts[pts.length-2];
  const col=up?'#2ee6a0':'#ff4d6d';
  return `<svg viewBox="0 0 ${W} ${H}" class="cd" role="img"><polyline fill="none" stroke="${col}" stroke-width="2.2" points="${pts.map((p,k)=>`${(7+step*k).toFixed(1)},${Y(p).toFixed(1)}`).join(' ')}"/>
  <circle cx="${(7+step*(pts.length-1)).toFixed(1)}" cy="${Y(last).toFixed(1)}" r="3.5" fill="${col}"/>
  <text x="8" y="14" fill="#8a93b8" font-size="11">${M(last)}</text></svg>`;
}
function areaChart(i){
  const n=Math.min(HI,52), r0=g.r-n+1, pts=[];
  for(let r=r0;r<=g.r;r++) pts.push(px(i,r));
  const hi=Math.max(...pts), lo=Math.min(...pts), W=330, H=125;
  const step=(W-14)/(pts.length-1||1);
  const Y=y=>H-8-(y-lo)/(hi-lo||1)*(H-16);
  const line=pts.map((p,k)=>`${(7+step*k).toFixed(1)},${Y(p).toFixed(1)}`).join(' ');
  const area=`7,${H-8} `+pts.map((p,k)=>`${(7+step*k).toFixed(1)},${Y(p).toFixed(1)}`).join(' ')+` ${(7+step*(pts.length-1)).toFixed(1)},${H-8}`;
  const last=pts[pts.length-1], up=pts.length>1&&last>=pts[pts.length-2];
  const col=up?'#2ee6a0':'#ff4d6d';
  return `<svg viewBox="0 0 ${W} ${H}" class="cd" role="img">
  <polygon points="${area}" fill="${col}" opacity="0.18"/>
  <polyline fill="none" stroke="${col}" stroke-width="2" points="${line}"/>
  <circle cx="${(7+step*(pts.length-1)).toFixed(1)}" cy="${Y(last).toFixed(1)}" r="3.5" fill="${col}"/>
  </svg>`;
}
function doJobShift(){
  if(!g.job)return g.msg='Escolha um emprego primeiro.',draw();
  if((g.energy||0)<=0)return g.msg='Sem energia. Volta na proxima rodada.',draw();
  const job=JOBS.find(x=>x.id===g.job);
  if(!job)return;
  const th=P(job.themes);
  const q=Q(th, Math.min(2, g.lvl + (g.jobLvl||0)>2?1:0));
  g.m={...q,type:'job',jobId:job.id,t:40};draw();
}
function confirmJob(){
  const m=g.m;if(!m||m.type!=='job')return;
  const v=norm($('#ai').value);if(isNaN(v))return;
  const ok=Math.abs(v-m.a)<.008;g.m=null;g.tot=(g.tot||0)+1;
  const job=JOBS.find(x=>x.id===m.jobId);
  g.energy=Math.max(0,(g.energy||0)-(job.energy||1));
  if(ok){
    g.cor=(g.cor||0)+1;
    let pay=job.pay + (g.jobLvl||0)*15 + (g.promo||0)*20;
    if(g.lucky){pay=Math.round(pay*1.25);g.lucky=0}
    if(g.tips)pay+=R(5,25);
    g.cash+=pay;g.jobXp=(g.jobXp||0)+(job.xp||1);
    g.combo=(g.combo||0)+1;
    if(g.jobXp>=5+(g.jobLvl||0)*4){g.jobLvl=(g.jobLvl||0)+1;g.jobXp=0;g.msg=`▲ Promovido no emprego! Nivel ${g.jobLvl}. +${M(pay)}`;g.promo=(g.promo||0)+1;g.fame=(g.fame||0)+1}
    else g.msg=`▲ Turno de ${job.name}: +${M(pay)} (combo ${g.combo})`;
    g.badgeXP=(g.badgeXP||0)+1;
  }else{g.combo=0;g.msg=`▼ Errou no trabalho. ${m.e}`;g.fame=Math.max(0,(g.fame||0)-1)}
  save();draw();
}
function takeJob(id){
  const job=JOBS.find(x=>x.id===id);if(!job)return;
  g.job=id;g.jobLvl=g.jobLvl||0;g.msg=`▲ Contratado: ${job.name}`;save();draw();
}
function quitJob(){g.job=null;g.combo=0;g.msg='▼ Voce pediu demissao.';save();draw()}
function buyBond(){
  if(g.cash<200)return g.msg='Precisa de R$ 200.',draw();
  g.cash-=200;g.bond=(g.bond||0)+200;g.msg='▲ Comprou titulo (renda fixa +2%/mes)';save();draw();
}
function toggleAutoInvest(){
  g.autoInvest=g.autoInvest?0:1;g.msg=g.autoInvest?'▲ Auto-invest ON: 10% do salario em NEOCOIN':'▲ Auto-invest OFF';save();draw();
}
function buyResearch(){
  if(g.cash<150)return g.msg='Precisa R$ 150.',draw();
  g.cash-=150;g.research=(g.research||0)+1;g.msg='▲ Pesquisa: proxima trava +5s e dica extra';g.lockBonus=(g.lockBonus||0)+5;save();draw();
}
function activateLucky(){
  if(g.cash<60)return g.msg='R$ 60.',draw();
  g.cash-=60;g.lucky=1;g.msg='▲ Sorte ativa: proximo turno de trabalho +25%';save();draw();
}
function hireMentor(){
  if(g.cash<200||g.mentor)return g.msg=g.mentor?'Ja tem mentor.':'Precisa R$ 200.',draw();
  g.cash-=200;g.mentor=1;g.streakMul=(g.streakMul||1)*1.15;g.msg='▲ Mentor: +15% nos bonus de desafio';save();draw();
}
function buyHome(){
  if(g.cash<2500||g.rentOwn)return g.msg=g.rentOwn?'Ja tem casa.':'Precisa R$ 2500.',draw();
  g.cash-=2500;g.rentOwn=1;g.msg='▲ Casa propria! Aluguel zerado nas contas';save();draw();
}

function candles(i){
  const n=Math.min(HI, 52), r0=g.r-n+1, v=AS[i][4], C=[];
  for(let r=r0;r<=g.r;r++){
    const o=px(i,r-1), c=px(i,r);
    const k=WK[i][r+HI]||[0.5,0.5];
    // pavios mais realistas e variáveis
    const bodyTop=Math.max(o,c), bodyBot=Math.min(o,c);
    const range=Math.max(bodyTop-bodyBot, bodyTop*0.008);
    const upWick = range*(0.3 + k[0]*1.8)*v;
    const dnWick = range*(0.3 + k[1]*1.8)*v;
    C.push({o,c,h:bodyTop+upWick, l:Math.max(5,bodyBot-dnWick)});
  }
  const hi=Math.max(...C.map(x=>x.h)), lo=Math.min(...C.map(x=>x.l));
  const W=320, H=120, step=(W-12)/C.length, bw=Math.min(12, step*0.65);
  const Y=y=>H-8-(y-lo)/(hi-lo||1)*(H-16);
  // linha de preço atual
  const last=C[C.length-1], midY=Y((last.o+last.c)/2);
  return `<svg viewBox="0 0 ${W} ${H}" class="cd" role="img" aria-label="Gráfico de velas de ${AS[i][0]}">
    <line x1="0" x2="${W}" y1="${midY.toFixed(1)}" y2="${midY.toFixed(1)}" stroke="#252a52" stroke-width="1" stroke-dasharray="4 3"/>
    ${C.map((x,k)=>{
      const cx=6+step*k+step/2;
      const up=x.c>=x.o;
      const col=up?'#2ee6a0':'#ff4d6d';
      const t=Y(Math.max(x.o,x.c)), bt=Y(Math.min(x.o,x.c));
      return `<line x1="${cx.toFixed(1)}" x2="${cx.toFixed(1)}" y1="${Y(x.h).toFixed(1)}" y2="${Y(x.l).toFixed(1)}" stroke="${col}" stroke-width="1.4"/>
      <rect x="${(cx-bw/2).toFixed(1)}" y="${t.toFixed(1)}" width="${bw.toFixed(1)}" height="${Math.max(1.8,bt-t).toFixed(1)}" fill="${col}" rx="1.2"/>`;
    }).join('')}
  </svg>`;
}
menu();
</script></body></html>
ing MATEMERCADO_2099.html…]()
