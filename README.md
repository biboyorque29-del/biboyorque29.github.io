<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>CivicSnap – Ilaya Barangka Integrated School</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Poppins:wght@500;600;700&display=swap" rel="stylesheet">
<style>
:root{--p:#2563EB;--s:#10B981;--a:#F59E0B;--bg:#F8FAFC;--tx:#1E293B;--card:#fff;--bd:#E2E8F0;--mut:#64748B;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0F172A;--tx:#E2E8F0;--card:#1E293B;--bd:#334155;--mut:#94A3B8}}
:root[data-theme="dark"]{--bg:#0F172A;--tx:#E2E8F0;--card:#1E293B;--bd:#334155;--mut:#94A3B8}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--tx);font:15px/1.55 Inter,system-ui,sans-serif}
h1,h2,h3{font-family:Poppins,Inter,sans-serif;margin:0 0 .5rem;line-height:1.2}
button,input,select,textarea{font:inherit;color:inherit}
:focus-visible{outline:3px solid var(--a);outline-offset:2px}
.nav{display:flex;align-items:center;gap:12px;padding:12px 20px;background:var(--card);border-bottom:1px solid var(--bd);flex-wrap:wrap;position:sticky;top:env(safe-area-inset-top,0px);z-index:5}
.logo{font:700 20px Poppins;color:var(--p);cursor:pointer;display:flex;align-items:center;gap:8px}
.logo i{width:26px;height:26px;border-radius:8px;background:var(--p);display:inline-block;position:relative}
.logo i:after{content:"";position:absolute;inset:7px;border:2.5px solid #fff;border-radius:50%}
.sp{flex:1}
.btn{border:0;border-radius:10px;padding:9px 16px;font-weight:600;cursor:pointer;background:var(--p);color:#fff}
.btn.g{background:transparent;color:var(--tx);border:1px solid var(--bd)}
.btn.s{background:var(--s)}.btn.sm{padding:5px 10px;font-size:13px}
.wrap{max-width:1100px;margin:0 auto;padding:20px}
.hero{padding:56px 20px 40px;max-width:1100px;margin:0 auto;display:grid;gap:32px;grid-template-columns:1.2fr 1fr;align-items:center}
.hero h1{font-size:clamp(2.6rem,7vw,4.4rem);letter-spacing:-.02em}
.tag{font:600 clamp(1.2rem,3vw,1.6rem) Poppins;color:var(--s);margin-bottom:12px}
.row{display:flex;gap:10px;flex-wrap:wrap}
.grid{display:grid;gap:14px;grid-template-columns:repeat(auto-fit,minmax(200px,1fr))}
.card{background:var(--card);border:1px solid var(--bd);border-radius:14px;padding:18px}
.kpi b{display:block;font:700 28px Poppins}
.mut{color:var(--mut);font-size:13px}
.badge{display:inline-block;padding:2px 10px;border-radius:99px;font-size:12px;font-weight:600;color:#fff;white-space:nowrap}
label{display:block;font-weight:500;margin:10px 0 4px;font-size:14px}
input,select,textarea{width:100%;padding:9px 12px;border:1px solid var(--bd);border-radius:10px;background:var(--bg)}
.tabs{display:flex;gap:6px;margin-bottom:16px;overflow-x:auto}
.tabs button{border:0;background:transparent;padding:8px 14px;border-radius:99px;cursor:pointer;font-weight:500;white-space:nowrap}
.tabs button.on{background:var(--p);color:#fff}
.tw{overflow-x:auto}table{width:100%;border-collapse:collapse;font-size:14px}
th,td{text-align:left;padding:9px 10px;border-bottom:1px solid var(--bd);white-space:nowrap}
.bar{height:10px;border-radius:6px;background:var(--bd);overflow:hidden}.bar i{display:block;height:100%}
.ov{position:fixed;inset:0;background:rgba(15,23,42,.6);display:flex;align-items:flex-start;justify-content:center;padding:20px;overflow:auto;z-index:20}
.mod{background:var(--card);border-radius:16px;padding:22px;max-width:640px;width:100%}
.tl{border-left:3px solid var(--bd);margin:8px 0 8px 6px;padding-left:14px}.tl div{margin-bottom:8px;position:relative}
.tl div:before{content:"";position:absolute;left:-21px;top:5px;width:11px;height:11px;border-radius:50%;background:var(--s)}
.thumbs{display:flex;gap:8px;flex-wrap:wrap;margin-top:8px}.thumbs img{width:84px;height:84px;object-fit:cover;border-radius:10px}
.heat{display:grid;grid-template-columns:repeat(auto-fill,minmax(110px,1fr));gap:8px}.heat div{padding:10px;border-radius:10px;font-size:13px;color:#1E293B}
.note{background:rgba(245,158,11,.14);border-left:4px solid var(--a);padding:8px 12px;border-radius:8px;margin:6px 0;font-size:14px}
.err{background:#FEE2E2;color:#991B1B;padding:10px 12px;border-radius:10px;margin-top:10px}
.toast{position:fixed;bottom:calc(20px + env(safe-area-inset-bottom,0px));left:50%;transform:translateX(-50%);background:var(--tx);color:var(--bg);padding:10px 18px;border-radius:10px;z-index:30}
.auth{max-width:420px;margin:30px auto}
@media(max-width:760px){.hero{grid-template-columns:1fr;padding-top:32px}}
@media(prefers-reduced-motion:no-preference){.hero .card{animation:up .6s both}@keyframes up{from{opacity:0;transform:translateY(14px)}}}
</style>
</head>
<body>
<div id="app"></div>
<script>
const CATS=["Classroom Damage","Furniture Damage","Electrical Issues","Plumbing Problems","Sanitation Concerns","Safety Hazards","Campus Facility Damage","Other Concerns"];
const PRI=["Low","Medium","High","Critical"];
const KEY="CIVICSNAP-ADMIN-2027";
const esc=s=>String(s??"").replace(/[&<>"']/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]));
const now=()=>new Date().toLocaleString("en-PH",{dateStyle:"medium",timeStyle:"short"});
let users=[
 {name:"System Administrator",id:"EMP-0001",email:"admin@civicsnap-ibis.edu.ph",pw:"CivicSnap@IBIS2027!",role:"Administrator"},
 {name:"Ana Reyes",id:"2027-0142",email:"student@ibis.edu",pw:"student123",role:"Student"},
 {name:"Mr. Dela Cruz",id:"EMP-0231",email:"teacher@ibis.edu",pw:"teacher123",role:"Teacher"},
 {name:"Mang Ben",id:"EMP-0310",email:"maint@ibis.edu",pw:"maint123",role:"Maintenance Personnel"}];
let statuses=[["Pending","#F59E0B","Received, waiting for review"],["Under Review","#F97316","Being checked by an administrator"],["In Progress","#2563EB","Repair is underway"],["For Verification","#8B5CF6","Waiting for the reporter or admin to confirm"],["Resolved","#10B981","Fixed and confirmed"],["Rejected","#EF4444","Not accepted as a facility concern"]].map(([n,c,d])=>({n,c,d,on:true}));
let reps=[
 {rid:"CS-2027-0001",title:"Broken armchair in Grade 8-Rizal",cat:"Furniture Damage",desc:"Two armchairs have loose legs.",loc:"Grade 8-Rizal",pr:"Medium",st:"In Progress",uid:"2027-0142",as:"EMP-0310",imgs:[],hist:[["Pending","Oct 3, 2026"],["Under Review","Oct 4, 2026"],["In Progress","Oct 8, 2026"]],notes:["Awaiting replacement screws."],date:"Oct 3, 2026"},
 {rid:"CS-2027-0002",title:"Flickering lights in Room 12",cat:"Electrical Issues",desc:"Ceiling lights flicker all day.",loc:"Room 12",pr:"High",st:"Pending",uid:"EMP-0231",as:"",imgs:[],hist:[["Pending","Nov 10, 2026"]],notes:[],date:"Nov 10, 2026"},
 {rid:"CS-2027-0003",title:"Leaking faucet at boys’ restroom",cat:"Plumbing Problems",desc:"Constant dripping, floor is wet.",loc:"Restroom, Building A",pr:"High",st:"Resolved",uid:"2027-0142",as:"EMP-0310",imgs:[],hist:[["Pending","Sep 12, 2026"],["In Progress","Sep 14, 2026"],["Resolved","Sep 16, 2026"]],notes:["Washer replaced."],date:"Sep 12, 2026"},
 {rid:"CS-2027-0004",title:"Exposed wiring near the canteen",cat:"Safety Hazards",desc:"Wires hanging from the wall.",loc:"Canteen",pr:"Critical",st:"Under Review",uid:"EMP-0231",as:"",imgs:[],hist:[["Pending","Nov 20, 2026"],["Under Review","Nov 21, 2026"]],notes:[],date:"Nov 20, 2026"},
 {rid:"CS-2027-0005",title:"Overflowing trash bins at the quadrangle",cat:"Sanitation Concerns",desc:"Bins not collected for days.",loc:"Quadrangle",pr:"Low",st:"Resolved",uid:"2027-0142",as:"",imgs:[],hist:[["Pending","Aug 5, 2026"],["Resolved","Aug 7, 2026"]],notes:[],date:"Aug 5, 2026"}];
let notifs=[{uid:"2027-0142",m:"CS-2027-0001 is now In Progress.",t:"Oct 8, 2026",read:false}];
let S={view:"home",user:null,tab:"",mode:"login",pending:null,err:"",f:{q:"",st:"",cat:"",pr:""},open:null,draft:[],toast:""};
const isAdm=()=>S.user?.role==="Administrator",isMt=()=>S.user?.role==="Maintenance Personnel";
const stOf=n=>statuses.find(s=>s.n===n)||{c:"#64748B"};
const badge=n=>`<span class="badge" style="background:${stOf(n).c}">${esc(n)}</span>`;
const nameOf=id=>users.find(u=>u.id===id)?.name||"—";
const visible=r=>isAdm()||(isMt()?r.as===S.user.id:r.uid===S.user.id);
const notify=(uid,m)=>notifs.unshift({uid,m,t:now(),read:false});
const toast=m=>{S.toast=m;render();setTimeout(()=>{S.toast="";render()},2200)};
function go(v){S.view=v;S.err="";if(v==="app"){S.tab=isAdm()?"Overview":isMt()?"Assigned":"My reports"}render();scrollTo(0,0)}
function theme(){const r=document.documentElement;const d=r.dataset.theme==="dark"||(!r.dataset.theme&&matchMedia("(prefers-color-scheme:dark)").matches);r.dataset.theme=d?"light":"dark"}
function logout(){S.user=null;S.pending=null;go("home")}

function nav(){return `<header class="nav"><div class="logo" onclick="go('home')"><i></i>CivicSnap</div><span class="mut">${esc(cfg.school)}</span><span class="sp"></span>
<button class="btn g sm" onclick="theme()" aria-label="Toggle dark mode">Dark mode</button>
${S.user?`<span class="mut">${esc(S.user.name)} (${esc(S.user.role)})</span><button class="btn g sm" onclick="go('app')">Dashboard</button><button class="btn sm" onclick="logout()">Log out</button>`:`<button class="btn sm" onclick="S.mode='login';go('auth')">Log in</button>`}</header>`}

function home(){const ben=[["Faster reporting","Submit concerns instantly using any device."],["Transparency","Monitor concern status from submission to resolution."],["Better communication","Connect students, teachers, maintenance personnel, and school administrators."],["Improved school environment","Promote safety, cleanliness, and effective facility maintenance."]];
return `<section class="hero"><div><div class="tag">Snap. Report. Improve.</div><h1>CivicSnap</h1><p style="max-width:52ch">CivicSnap is a digital reporting platform that empowers students, teachers, and school personnel to efficiently report, monitor, and track school facility concerns. Through better communication, transparency, and accountability, CivicSnap helps create a safer and more conducive learning environment.</p>
<div class="row"><button class="btn" onclick="S.user?(S.tab='New concern',go('app')):(S.mode='login',go('auth'))">Report a concern</button><button class="btn g" onclick="document.getElementById('about').scrollIntoView({behavior:'smooth'})">Learn more</button></div></div>
<div class="card"><b style="font-family:Poppins">Live status board</b>${statuses.filter(s=>s.on).map(s=>`<div style="display:flex;justify-content:space-between;margin-top:10px">${badge(s.n)}<b>${reps.filter(r=>r.st===s.n).length}</b></div>`).join("")}<p class="mut">Try the demo: student@ibis.edu / student123, teacher@ibis.edu / teacher123, or maint@ibis.edu / maint123.</p></div></section>
<section class="wrap" id="about"><h2>Why CivicSnap</h2><p style="max-width:70ch">Traditional reporting methods often rely on verbal communication, paper notes, or informal reporting processes, resulting in delayed responses and unresolved concerns. CivicSnap transforms this process into a centralized digital reporting system that allows users to submit concerns, upload photographic evidence, and track updates until resolution.</p>
<div class="grid">${ben.map(b=>`<div class="card"><h3>${b[0]}</h3><span class="mut">${b[1]}</span></div>`).join("")}</div></section>`}

function auth(){
if(S.granted)return `<div class="card auth" role="status"><h2>Access Granted</h2><p>Redirecting to Administrator Dashboard...</p></div>`;
if(S.pending)return `<div class="card auth"><h2>Administrator verification</h2><p class="mut">Step 2 of 2. Enter the Administrator Verification Code.</p><label for="ak">Administrator Verification Code</label><input id="ak" type="password" autocomplete="off"><button class="btn" style="margin-top:12px" onclick="adminKey()">Verify and continue</button>${S.err?`<div class="err">${S.err}</div>`:""}</div>`;
const reg=S.mode==="register";
return `<div class="card auth"><div class="tabs"><button class="${!reg?"on":""}" onclick="S.mode='login';S.err='';render()">Log in</button><button class="${reg?"on":""}" onclick="S.mode='register';S.err='';render()">Register</button></div>
${reg?`<label for="rn">Full name</label><input id="rn"><label for="ri">Student ID / Employee ID</label><input id="ri"><label for="rr">Role</label><select id="rr"><option>Student</option><option>Teacher</option><option>Maintenance Personnel</option></select>`:""}
<label for="em">Email address</label><input id="em" type="email" autocomplete="username"><label for="pw">Password</label><input id="pw" type="password" autocomplete="current-password">
${reg?`<label for="pc">Confirm password</label><input id="pc" type="password">`:""}
<button class="btn" style="margin-top:14px;width:100%" onclick="${reg?"register()":"login()"}">${reg?"Create account":"Log in"}</button>
${!reg?`<p><a href="#" onclick="forgot();return false">Forgot password?</a></p>`:""}${S.err?`<div class="err">${S.err}</div>`:""}
<p class="mut">Administrator accounts are added by the system owner and cannot be registered here.</p></div>`}
const v=id=>document.getElementById(id)?.value.trim()||"";
function login(){const u=users.find(u=>u.email.toLowerCase()===v("em").toLowerCase()&&u.pw===document.getElementById("pw").value);
 if(!u){S.err="Email or password is incorrect.";return render()}
 if(u.role==="Administrator"){S.pending=u;S.err="";return render()}
 S.user=u;go("app")}
function adminKey(){if(document.getElementById("ak").value===KEY){S.user=S.pending;S.pending=null;S.granted=true;S.err="";render();setTimeout(()=>{S.granted=false;go("app")},1200)}else{S.err="<b>Access Denied</b><br>Administrator Verification Failed.<br>Please contact the System Administrator.";render()}}
function register(){const pw=document.getElementById("pw").value,pc=document.getElementById("pc").value;
 if(!v("rn")||!v("ri")||!v("em"))S.err="Fill in every field.";
 else if(pw.length<8)S.err="Use a password with at least 8 characters.";
 else if(pw!==pc)S.err="Passwords don’t match.";
 else if(users.some(u=>u.email.toLowerCase()===v("em").toLowerCase()))S.err="That email is already registered.";
 else{const u={name:v("rn"),id:v("ri"),email:v("em"),pw,role:v("rr")||"Student"};users.push(u);S.user=u;return go("app")}
 render()}
function forgot(){S.err="Password reset isn’t available in this prototype. In production, a reset link is emailed to the registered address.";render()}

function app(){const tabs=isAdm()?["Overview","All concerns","Legends","Users","Announcements","Reports","Activity","Settings"]:isMt()?["Assigned","Notifications"]:["My reports","New concern","Notifications"];
const un=notifs.filter(n=>n.uid===S.user.id&&!n.read).length;
let b="";
if(S.tab==="Overview")b=overview();else if(S.tab==="All concerns"||S.tab==="Assigned"||S.tab==="My reports")b=`<div class="card">${filters()}<div class="tw" id="tbl">${table()}</div></div>`;
else if(S.tab==="New concern")b=form();else if(S.tab==="Legends")b=legends();else if(S.tab==="Users")b=usersTab();else if(S.tab==="Announcements")b=annTab();else if(S.tab==="Reports")b=repTab();else if(S.tab==="Settings")b=setTab();else if(S.tab==="Notifications")b=nots();else b=activity();
return `<div class="wrap">${!isAdm()&&anns[0]?`<div class="note"><b>${esc(anns[0].t)}</b> ${esc(anns[0].b)}</div>`:""}<div class="tabs">${tabs.map(t=>`<button class="${S.tab===t?"on":""}" onclick="S.tab='${t}';render()">${t}${t==="Notifications"&&un?` (${un})`:""}</button>`).join("")}</div>${b}</div>`}

function overview(){const R=reps,tot=R.length,res=R.filter(r=>r.st==="Resolved").length;
const k=[["Total reports",tot],["Pending",R.filter(r=>r.st==="Pending").length],["In progress",R.filter(r=>r.st==="In Progress").length],["Resolved",res],["Critical",R.filter(r=>r.pr==="Critical").length],["Resolution rate",tot?Math.round(res/tot*100)+"%":"0%"],["Avg resolution time",(()=>{const d=R.filter(r=>r.st==="Resolved").map(r=>{const h=r.hist.find(h=>h[0]==="Resolved");return h?(Date.parse(h[1])-Date.parse(r.date))/864e5:null}).filter(x=>x!==null&&!isNaN(x));return d.length?(d.reduce((a,b)=>a+b,0)/d.length).toFixed(1)+" days":"—"})()]];
const bars=(items,col)=>items.map(([n,c,cl])=>`<div style="margin:8px 0"><div style="display:flex;justify-content:space-between"><span>${esc(n)}</span><b>${c}</b></div><div class="bar"><i style="width:${tot?c/tot*100:0}%;background:${cl||col}"></i></div></div>`).join("");
const locs={};R.forEach(r=>locs[r.loc]=(locs[r.loc]||0)+1);const mx=Math.max(1,...Object.values(locs));
const mon={};R.forEach(r=>{const m=r.date.slice(0,3);mon[m]=(mon[m]||0)+1});
return `<div class="grid">${k.map(([l,n])=>`<div class="card kpi"><span class="mut">${l}</span><b>${n}</b></div>`).join("")}</div>
<div class="grid" style="margin-top:14px"><div class="card"><h3>By category</h3>${bars(CATS.map(c=>[c,R.filter(r=>r.cat===c).length]).filter(x=>x[1]),"#2563EB")}</div>
<div class="card"><h3>Status distribution</h3>${bars(statuses.map(s=>[s.n,R.filter(r=>r.st===s.n).length,s.c]),"#2563EB")}</div>
<div class="card"><h3>Monthly trend</h3>${bars(Object.entries(mon).map(([m,c])=>[m,c]),"#10B981")}</div></div>
<div class="card" style="margin-top:14px"><h3>Location heat map</h3><div class="heat">${Object.entries(locs).map(([l,c])=>`<div style="background:rgba(245,158,11,${.2+.8*c/mx})">${esc(l)}<br><b>${c}</b></div>`).join("")}</div></div>`}

function filters(){const f=S.f;const sel=(id,l,o)=>`<select id="${id}" aria-label="${l}" onchange="fl()" style="width:auto"><option value="">${l}</option>${o.map(x=>`<option ${f[id]===x?"selected":""}>${esc(x)}</option>`).join("")}</select>`;
return `<div class="row" style="margin-bottom:12px"><input id="q" placeholder="Search reports" value="${esc(f.q)}" oninput="fl()" style="max-width:260px">${sel("st","All statuses",statuses.map(s=>s.n))}${sel("cat","All categories",CATS)}${sel("pr","All priorities",PRI)}${sel("loc","All locations",[...new Set(reps.filter(visible).map(r=>r.loc))])}${isAdm()?sel("rep","All reporters",[...new Set(reps.map(r=>nameOf(r.uid)))]):""}<input id="from" type="date" value="${f.from||""}" onchange="fl()" aria-label="From date" style="width:auto">${sel("sort","Newest first",["Oldest first","Priority","Status"])}</div>`}
function fl(){["q","st","cat","pr","loc","rep","from","sort"].forEach(k=>S.f[k]=document.getElementById(k)?.value||"");document.getElementById("tbl").innerHTML=table()}
function table(){const f=S.f,q=f.q.toLowerCase();
const L=reps.filter(visible).filter(r=>(!q||(r.title+r.rid+r.loc).toLowerCase().includes(q))&&(!f.st||r.st===f.st)&&(!f.cat||r.cat===f.cat)&&(!f.pr||r.pr===f.pr)&&(!f.loc||r.loc===f.loc)&&(!f.rep||nameOf(r.uid)===f.rep)&&(!f.from||Date.parse(r.date)>=Date.parse(f.from))).sort((a,b)=>{const d=Date.parse(b.date)-Date.parse(a.date)||b.rid.localeCompare(a.rid);return f.sort==="Oldest first"?-d:f.sort==="Priority"?PRI.indexOf(b.pr)-PRI.indexOf(a.pr):f.sort==="Status"?a.st.localeCompare(b.st):d});
if(!L.length)return `<p class="mut">No reports match. ${isAdm()||isMt()?"":"Use New concern to submit your first report."}</p>`;
return `<table><thead><tr><th>ID</th>${isAdm()?"<th>Reporter</th><th>Role</th>":""}<th>Concern</th><th>Category</th><th>Location</th><th>Date</th><th>Priority</th><th>Status</th><th></th></tr></thead><tbody>${L.map(r=>`<tr><td>${r.rid}</td>${isAdm()?`<td>${esc(nameOf(r.uid))}</td><td>${esc(users.find(u=>u.id===r.uid)?.role)}</td>`:""}<td>${esc(r.title)}</td><td>${esc(r.cat)}</td><td>${esc(r.loc)}</td><td>${r.date}</td><td>${r.pr}</td><td>${badge(r.st)}</td><td><button class="btn sm" onclick="S.open='${r.rid}';render()">View</button>${isAdm()?` <button class="btn sm s" onclick="quickRes('${r.rid}')">Resolve</button> <button class="btn sm g" onclick="del('${r.rid}')">Delete</button>`:""}</td></tr>`).join("")}</tbody></table>`}
function del(id){if(confirm("Delete "+id+"? This is recorded in the activity log.")){reps=reps.filter(r=>r.rid!==id);log("Deleted "+id);render()}}

function form(){return `<div class="card" style="max-width:640px"><h2>Report a concern</h2>
<label for="t">Concern title</label><input id="t"><label for="c">Category</label><select id="c">${CATS.map(c=>`<option>${c}</option>`).join("")}</select>
<label for="d">Details</label><textarea id="d" rows="4"></textarea><label for="l">Location</label><input id="l" placeholder="e.g. Room 12, Building B">
<label for="p">Priority</label><select id="p">${PRI.map(p=>`<option ${p==="Medium"?"selected":""}>${p}</option>`).join("")}</select>
<label for="im">Photos (one or more)</label><input id="im" type="file" accept="image/*" ${cfg.multi?"multiple":""} onchange="prev(this)"><div class="thumbs" id="pv">${S.draft.map(u=>`<img src="${u}" alt="Preview">`).join("")}</div>
<button class="btn s" style="margin-top:14px" onclick="submit()">Submit concern</button>${S.err?`<div class="err">${S.err}</div>`:""}</div>`}
function prev(i){S.draft=[...i.files].map(f=>URL.createObjectURL(f));document.getElementById("pv").innerHTML=S.draft.map(u=>`<img src="${u}" alt="Preview">`).join("")}
function submit(){if(!v("t")||!v("d")||!v("l")){S.err="Add a title, details, and a location.";return render()}
 const rid="CS-2027-"+String(reps.length+1).padStart(4,"0"),d=new Date().toLocaleDateString("en-PH",{dateStyle:"medium"});
 reps.unshift({rid,title:v("t"),cat:v("c"),desc:v("d"),loc:v("l"),pr:v("p"),st:statuses.find(s=>s.on).n,uid:S.user.id,as:"",imgs:S.draft,hist:[[statuses.find(s=>s.on).n,d]],notes:[],date:d,time:new Date().toLocaleTimeString("en-PH",{timeStyle:"short"})});
 notify(S.user.id,`${rid} was submitted. We’ll update you as it moves forward.`);users.filter(u=>u.role==="Administrator").forEach(u=>notify(u.id,`New ${v("p")} concern ${rid}: ${v("t")}`));
 log("Submitted "+rid);S.draft=[];S.err="";S.tab="My reports";toast("Submitted as "+rid)}

function modal(){const r=reps.find(x=>x.rid===S.open);if(!r)return"";const staff=isAdm()||isMt();
const maint=users.filter(u=>u.role==="Maintenance Personnel"),rep=users.find(u=>u.id===r.uid)||{};
return `<div class="ov" onclick="if(event.target===this){S.open=null;render()}"><div class="mod" role="dialog" aria-modal="true"><div class="row"><h2 style="flex:1">${esc(r.title)}</h2><button class="btn g sm" onclick="S.open=null;render()">Close</button></div>
<p>${r.rid} ${badge(r.st)} <span class="mut">${r.pr} priority</span></p><p>${esc(r.desc)}</p>
<p class="mut">${esc(r.cat)} · ${esc(r.loc)} · ${r.date} ${r.time||""}${isAdm()?`<br>Reporter: ${esc(rep.name)} (${esc(rep.id)})`:""}<br>Assigned to: ${esc(nameOf(r.as))}</p>
${r.imgs.length?`<div class="thumbs">${r.imgs.map(u=>`<img src="${u}" alt="Evidence">`).join("")}</div>`:`<p class="mut">No photos attached.</p>`}
<h3 style="margin-top:14px">Timeline</h3><div class="tl">${r.hist.map(h=>`<div>${esc(h[0])} <span class="mut">${h[1]}</span></div>`).join("")}</div>
${staff?`<h3>Update</h3><div class="row"><select id="ns" style="width:auto">${statuses.filter(s=>s.on).map(s=>`<option ${s.n===r.st?"selected":""}>${esc(s.n)}</option>`).join("")}</select><button class="btn sm" onclick="setSt('${r.rid}')">Update status</button></div>
${isAdm()?`<div class="row" style="margin-top:8px"><select id="as" style="width:auto"><option value="">Unassigned</option>${maint.map(m=>`<option value="${m.id}" ${m.id===r.as?"selected":""}>${esc(m.name)}</option>`).join("")}</select><button class="btn sm s" onclick="assign('${r.rid}')">Assign</button></div>`:""}
${isMt()?`<button class="btn sm s" style="margin-top:8px" onclick="complete('${r.rid}')">Mark repair completed</button>`:""}${isMt()?`<label for="ev">Upload repair evidence</label><input id="ev" type="file" accept="image/*" multiple onchange="evid('${r.rid}',this)">`:""}
<h3 style="margin-top:14px">Internal notes</h3>${r.notes.map(n=>`<div class="note">${esc(n)}</div>`).join("")||`<p class="mut">No notes yet.</p>`}
<div class="row"><input id="nt" placeholder="Add a note or repair remark (staff only)" style="flex:1"><button class="btn sm" onclick="addNote('${r.rid}')">Add note</button></div>`:""}</div></div>`}
function setSt(id){const s=document.getElementById("ns").value;return setTo(id,s)}
function setStOld(id){const r=reps.find(x=>x.rid===id),s=document.getElementById("ns").value;if(s===r.st)return;r.st=s;r.hist.push([s,new Date().toLocaleDateString("en-PH",{dateStyle:"medium"})]);notify(r.uid,`${id} is now ${s}.`);log(`${id} → ${s}`);toast("Status updated")}
function assign(id){const r=reps.find(x=>x.rid===id);r.as=document.getElementById("as").value;if(r.as){notify(r.as,`You were assigned ${id}.`);notify(r.uid,`${id} was assigned for repair.`)}log(`Assigned ${id}`);toast("Assignment saved")}
function addNote(id){const n=v("nt");if(!n)return;reps.find(x=>x.rid===id).notes.push(n);log("Note on "+id);render()}
function evid(id,i){reps.find(x=>x.rid===id).imgs.push(...[...i.files].map(f=>URL.createObjectURL(f)));toast("Evidence uploaded")}

function legends(){return `<div class="card"><h3>Status legends</h3><p class="mut">Only administrators can change these. Order sets the workflow.</p>${statuses.map((s,i)=>`<div class="row" style="align-items:center;margin:10px 0"><input type="color" value="${s.c}" onchange="statuses[${i}].c=this.value;render()" style="width:46px;padding:2px" aria-label="Color"><input value="${esc(s.n)}" onchange="rn(${i},this.value)" style="width:170px" aria-label="Name"><input value="${esc(s.d)}" onchange="statuses[${i}].d=this.value" style="flex:1;min-width:180px" aria-label="Description"><button class="btn sm g" onclick="mv(${i},-1)" aria-label="Move up">↑</button><button class="btn sm g" onclick="mv(${i},1)" aria-label="Move down">↓</button><button class="btn sm ${s.on?"":"g"}" onclick="statuses[${i}].on=!statuses[${i}].on;render()">${s.on?"Enabled":"Disabled"}</button><button class="btn sm g" onclick="delSt(${i})">Delete</button></div>`).join("")}
<button class="btn s" onclick="statuses.push({n:'New status',c:'#64748B',d:'Describe this status',on:true});render()">Add status</button></div>`}
function rn(i,n){const o=statuses[i].n;statuses[i].n=n||o;reps.forEach(r=>{if(r.st===o)r.st=statuses[i].n;r.hist.forEach(h=>{if(h[0]===o)h[0]=statuses[i].n})});log(`Renamed status ${o} → ${n}`);render()}
function mv(i,d){const j=i+d;if(j<0||j>=statuses.length)return;[statuses[i],statuses[j]]=[statuses[j],statuses[i]];render()}
function usersTab(){return `<div class="card tw"><table><thead><tr><th>Name</th><th>ID</th><th>Email</th><th>Role</th></tr></thead><tbody>${users.map(u=>`<tr><td>${esc(u.name)}</td><td>${esc(u.id)}</td><td>${esc(u.email)}</td><td>${esc(u.role)}</td></tr>`).join("")}</tbody></table></div>`}
let logs=[["Prototype started",now()]];function log(m){logs.unshift([`${S.user?.name}: ${m}`,now()])}
function activity(){return `<div class="card"><h3>Activity log</h3>${logs.map(l=>`<div style="padding:6px 0;border-bottom:1px solid var(--bd)">${esc(l[0])} <span class="mut">${l[1]}</span></div>`).join("")}</div>`}
function nots(){const L=notifs.filter(n=>n.uid===S.user.id);notifs.forEach(n=>{if(n.uid===S.user.id)n.read=true});
return `<div class="card"><h3>Notifications</h3>${L.map(n=>`<div style="padding:8px 0;border-bottom:1px solid var(--bd)">${esc(n.m)} <span class="mut">${n.t}</span></div>`).join("")||`<p class="mut">You’re all caught up.</p>`}</div>`}

let anns=[{t:"Welcome to CivicSnap",b:"Report facility concerns with a photo and track every repair here.",d:"Nov 24, 2026"}];
let cfg={school:"Ilaya Barangka Integrated School",email:true,multi:true};
function annTab(){return `<div class="card" style="max-width:640px"><h3>New announcement</h3><label for="at">Title</label><input id="at"><label for="ab">Message</label><textarea id="ab" rows="3"></textarea><button class="btn s" style="margin-top:10px" onclick="addAnn()">Post announcement</button></div>${anns.map((a,i)=>`<div class="card" style="margin-top:12px"><b>${esc(a.t)}</b> <span class="mut">${a.d}</span><p>${esc(a.b)}</p><button class="btn sm g" onclick="anns.splice(${i},1);render()">Remove</button></div>`).join("")}`}
function addAnn(){if(!v("at")||!v("ab"))return toast("Add a title and a message");anns.unshift({t:v("at"),b:v("ab"),d:new Date().toLocaleDateString("en-PH",{dateStyle:"medium"})});log("Posted announcement");toast("Announcement posted")}
function repTab(){const q=x=>'"'+String(x??"").replace(/"/g,'""')+'"';const csv=["Report ID,Reporter,Role,Title,Category,Location,Date,Priority,Status",...reps.map(r=>[r.rid,nameOf(r.uid),users.find(u=>u.id===r.uid)?.role,r.title,r.cat,r.loc,r.date,r.pr,r.st].map(q).join(","))].join("\n");
return `<div class="card"><h3>Generate report</h3><div class="grid">${statuses.map(s=>`<div class="kpi">${badge(s.n)}<b>${reps.filter(r=>r.st===s.n).length}</b></div>`).join("")}</div><label for="csv">Spreadsheet-ready data (CSV)</label><textarea id="csv" rows="8" readonly onfocus="this.select()">${esc(csv)}</textarea><p class="mut">Select and copy this into Excel or Google Sheets. One-click PDF and Excel downloads need the backend.</p></div>`}
function setTab(){return `<div class="card" style="max-width:560px"><h3>System settings</h3><label for="sn">School name</label><input id="sn" value="${esc(cfg.school)}" onchange="cfg.school=this.value;render()"><label><input type="checkbox" ${cfg.email?"checked":""} onchange="cfg.email=this.checked" style="width:auto"> Send email notifications</label><label><input type="checkbox" ${cfg.multi?"checked":""} onchange="cfg.multi=this.checked;render()" style="width:auto"> Allow multiple photos per report</label><p class="mut">Settings apply to this demo session only.</p></div>`}
function setTo(id,s){const r=reps.find(x=>x.rid===id);if(!r||r.st===s)return;if(s==="Resolved"&&r.st==="For Verification")notify(r.uid,`Verification completed for ${id}.`);r.st=s;r.hist.push([s,new Date().toLocaleDateString("en-PH",{dateStyle:"medium"})]);notify(r.uid,`${id} is now ${s}.`);log(`${id} → ${s}`);toast("Status updated")}
function quickRes(id){setTo(id,"Resolved")}
function complete(id){setTo(id,statuses.find(s=>s.n==="For Verification"&&s.on)?"For Verification":"Resolved")}
function delSt(i){const n=statuses[i].n;if(reps.some(r=>r.st===n))return toast("Move reports out of “"+n+"” before deleting it");if(confirm("Delete status "+n+"?")){statuses.splice(i,1);log("Deleted status "+n);render()}}
function render(){const a=document.activeElement?.id;
 document.getElementById("app").innerHTML=nav()+(S.view==="home"?home():S.view==="auth"?auth():(S.user?app():home()))+(S.open&&S.user?modal():"")+(S.toast?`<div class="toast" role="status">${esc(S.toast)}</div>`:"");
 if(S.tab==="Notifications"&&S.user)notifs.forEach(n=>{if(n.uid===S.user.id)n.read=true});
 if(a&&["q"].includes(a)){const e=document.getElementById(a);e&&e.focus()}}
render();
</script>
</body>
</html>
