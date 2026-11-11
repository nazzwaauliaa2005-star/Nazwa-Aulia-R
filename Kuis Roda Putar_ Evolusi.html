<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Kuis Roda Putar: Evolusi</title>
<style>
:root{--bg:#f3f8f2;--card:#fff;--text:#1d2b22;--muted:#5d6f63;--accent:#2e8b57;--line:#d5e3d8;--ok:#2e8b57;--bad:#c0392b;color-scheme:light;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#121a15;--card:#1b261f;--text:#e8f1ea;--muted:#9bb0a1;--accent:#4fb37c;--line:#2b3b30;color-scheme:dark}}
:root[data-theme="dark"]{--bg:#121a15;--card:#1b261f;--text:#e8f1ea;--muted:#9bb0a1;--accent:#4fb37c;--line:#2b3b30;color-scheme:dark}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--text);font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;line-height:1.5}
main{max-width:980px;margin:0 auto;padding:20px 16px 40px}
h1{font-size:clamp(1.5rem,4vw,2.2rem);margin:0 0 4px}
.sub{color:var(--muted);margin:0 0 20px}
.card{background:var(--card);border:1px solid var(--line);border-radius:16px;padding:20px}
label{font-weight:600;display:block;margin:0 0 6px}
input,textarea{width:100%;padding:10px 12px;border:1px solid var(--line);border-radius:10px;background:var(--bg);color:var(--text);font:inherit}
button{font:inherit;cursor:pointer;border:0;border-radius:12px;padding:12px 20px;font-weight:700;background:var(--accent);color:#fff}
button.alt{background:transparent;color:var(--accent);border:2px solid var(--accent)}
button:disabled{opacity:.5;cursor:default}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(150px,1fr));gap:8px;margin:14px 0}
.row{display:flex;gap:10px;flex-wrap:wrap;margin-top:14px}
.hide{display:none!important}
.game{display:grid;grid-template-columns:1fr 280px;gap:20px;align-items:start}
@media(max-width:760px){.game{grid-template-columns:1fr}}
.wheelbox{position:relative;text-align:center}
canvas{width:min(92vw,520px);height:auto;aspect-ratio:1}
.pointer{position:absolute;left:50%;top:-4px;transform:translateX(-50%);width:0;height:0;border-left:16px solid transparent;border-right:16px solid transparent;border-top:34px solid #e74c3c;filter:drop-shadow(0 2px 2px rgba(0,0,0,.35));z-index:2}
#spin{font-size:1.3rem;padding:14px 40px;margin-top:10px}
.sb{list-style:none;margin:0;padding:0}
.sb li{display:flex;justify-content:space-between;padding:6px 0;border-bottom:1px solid var(--line)}
.sb li.done{color:var(--muted)}
.ov{position:fixed;inset:0;background:rgba(0,0,0,.6);display:flex;align-items:center;justify-content:center;padding:16px;z-index:10;overflow:auto}
.modal{max-width:640px;width:100%}
.who{font-size:1.4rem;font-weight:800;color:var(--accent);margin:0}
.tag{font-size:.8rem;color:var(--muted);text-transform:uppercase;letter-spacing:.05em}
.opt{display:block;width:100%;text-align:left;background:var(--bg);color:var(--text);border:2px solid var(--line);margin-top:8px;font-weight:500}
.opt.ok{border-color:var(--ok);background:rgba(46,139,87,.2)}
.opt.bad{border-color:var(--bad);background:rgba(192,57,43,.2)}
.fb{margin-top:12px;padding:12px;border-radius:10px;background:var(--bg);border:1px solid var(--line)}
table{width:100%;border-collapse:collapse}
td,th{padding:8px;border-bottom:1px solid var(--line);text-align:left}
</style>
</head>
<body>
<main>
<h1>🎡 Kuis Roda Putar: Evolusi</h1>
<p class="sub">Bukti evolusi, adaptasi, dan spesiasi · Biologi kelas 12</p>

<section id="setup" class="card">
  <label for="jml">Jumlah peserta (2–40)</label>
  <input id="jml" type="number" min="2" max="40" value="5">
  <div id="names" class="grid"></div>
  <details><summary>Tempel daftar nama (satu nama per baris)</summary>
    <textarea id="paste" rows="5" placeholder="Andi&#10;Budi&#10;Citra"></textarea>
    <div class="row"><button class="alt" id="apply" type="button">Isi kolom dari daftar</button></div>
  </details>
  <p id="err" style="color:var(--bad);font-weight:600"></p>
  <div class="row"><button id="start" type="button">Mulai permainan</button></div>
</section>

<section id="gamebox" class="game hide">
  <div class="card wheelbox">
    <div class="pointer"></div>
    <canvas id="wheel" width="900" height="900"></canvas><br>
    <button id="spin" type="button">PUTAR</button>
  </div>
  <div class="card">
    <h3 style="margin:0 0 8px">Papan skor</h3>
    <p id="prog" style="color:var(--muted);margin:0 0 8px"></p>
    <ul id="sb" class="sb"></ul>
  </div>
</section>

<section id="result" class="card hide">
  <h2 style="margin-top:0">🏆 Hasil akhir</h2>
  <p id="champ" style="font-size:1.2rem;font-weight:700"></p>
  <table><thead><tr><th>#</th><th>Nama</th><th>Skor</th></tr></thead><tbody id="rt"></tbody></table>
  <div class="row"><button id="again" type="button">Main lagi (nama sama)</button><button class="alt" id="reset" type="button">Ubah peserta</button></div>
</section>
</main>

<div id="ov" class="ov hide"><div class="card modal">
  <p class="tag" id="topik"></p>
  <p class="who" id="giliran"></p>
  <p id="soal" style="font-size:1.1rem;font-weight:600"></p>
  <div id="opts"></div>
  <div id="fb" class="fb hide"></div>
  <div class="row"><button id="next" class="hide" type="button">Lanjut</button></div>
</div></div>

<script>
// ===== BANK SOAL (edit di sini). jawaban = indeks opsi benar (0=A, 1=B, 2=C, 3=D) =====
const Q=[
{t:"Bukti evolusi",q:"Sisa-sisa makhluk hidup masa lampau yang terawetkan di dalam batuan disebut…",o:["fosil","organ homolog","organ analog","embrio"],a:0,p:"Fosil adalah bukti evolusi yang paling langsung karena menunjukkan makhluk hidup yang pernah ada di masa lalu."},
{t:"Bukti evolusi",q:"Tangan manusia dan sirip paus punya susunan tulang yang sama tetapi fungsinya berbeda. Struktur seperti ini disebut…",o:["organ analog","organ vestigial","organ homolog","fosil hidup"],a:2,p:"Organ homolog: asal sama, fungsi berbeda. Ini menunjukkan nenek moyang yang sama."},
{t:"Bukti evolusi",q:"Sayap burung dan sayap kupu-kupu bentuknya berbeda tetapi sama-sama untuk terbang. Struktur seperti ini disebut…",o:["organ homolog","organ analog","organ vestigial","embrio"],a:1,p:"Organ analog: fungsi sama, asal berbeda."},
{t:"Bukti evolusi",q:"Usus buntu dan tulang ekor pada manusia merupakan contoh…",o:["organ analog","organ homolog","fosil","organ vestigial"],a:3,p:"Organ vestigial adalah organ sisa yang fungsinya sudah menyusut atau hilang."},
{t:"Bukti evolusi",q:"Embrio ikan, ayam, dan manusia pada tahap awal terlihat mirip. Hal ini termasuk bukti evolusi dari…",o:["anatomi perbandingan","embriologi perbandingan","biogeografi","fosil"],a:1,p:"Kemiripan tahap awal perkembangan embrio menunjukkan kekerabatan antarmakhluk hidup."},
{t:"Adaptasi",q:"Burung finch di Kepulauan Galápagos punya bentuk paruh yang berbeda-beda. Hal ini terjadi karena…",o:["semua finch makan makanan yang sama","paruh berubah setiap hari","bentuk paruh menyesuaikan jenis makanannya","finch dipelihara manusia"],a:2,p:"Bentuk paruh yang cocok dengan makanannya membuat burung bertahan hidup. Ini adaptasi morfologi (bentuk tubuh)."},
{t:"Adaptasi",q:"Menurut Darwin, jerapah memiliki leher panjang karena…",o:["leher terus diregangkan lalu sifatnya diwariskan","jerapah berleher panjang lebih mudah mendapat daun, bertahan hidup, dan mewariskan sifatnya","jerapah sengaja ingin berleher panjang","leher panjang muncul tiba-tiba pada semua jerapah"],a:1,p:"Ini seleksi alam: individu yang cocok dengan lingkungan bertahan dan mewariskan sifatnya. Pendapat pertama adalah teori Lamarck."},
{t:"Adaptasi",q:"Burung yang bermigrasi ke daerah hangat saat musim dingin termasuk adaptasi…",o:["morfologi","fisiologi","anatomi","tingkah laku"],a:3,p:"Migrasi adalah perubahan perilaku untuk bertahan hidup, jadi termasuk adaptasi tingkah laku."},
{t:"Spesiasi",q:"Terbentuknya spesies baru dari spesies yang sudah ada disebut…",o:["kepunahan","perubahan warna tubuh","spesiasi","migrasi"],a:2,p:"Spesiasi adalah proses terbentuknya spesies baru."},
{t:"Spesiasi",q:"Dua kelompok hewan sejenis dipisahkan laut atau gunung sehingga tidak bisa bertemu dan kawin. Penghalang ini disebut isolasi…",o:["geografis","makanan","warna","suara"],a:0,p:"Isolasi geografis menghentikan perkawinan antarpopulasi dan dapat berujung pada spesies baru."}
];
const COL=["#2e8b57","#1f78b4","#e67e22","#8e44ad","#c0392b","#16a085","#d4a017","#34495e"];
const TAU=Math.PI*2, $=id=>document.getElementById(id);
let names=[],rem=[],score={},rot=0,spinning=false,deck=[],cur=null,pick=null;

function buildInputs(vals){
  let n=Math.max(2,Math.min(40,parseInt($("jml").value)||2));
  $("jml").value=n;
  const box=$("names"),old=vals||[...box.querySelectorAll("input")].map(i=>i.value);
  box.innerHTML="";
  for(let i=0;i<n;i++){const e=document.createElement("input");e.placeholder="Nama "+(i+1);e.value=old[i]||"";box.appendChild(e);}
}
$("jml").addEventListener("input",()=>buildInputs());
$("apply").onclick=()=>{
  const l=$("paste").value.split("\n").map(s=>s.trim()).filter(Boolean).slice(0,40);
  if(l.length<2){$("err").textContent="Tempel minimal 2 nama.";return;}
  $("jml").value=l.length;buildInputs(l);$("err").textContent="";
};
$("start").onclick=()=>{
  const v=[...$("names").querySelectorAll("input")].map(i=>i.value.trim());
  if(v.some(x=>!x)){$("err").textContent="Semua nama harus diisi.";return;}
  if(new Set(v.map(x=>x.toLowerCase())).size<v.length){$("err").textContent="Ada nama yang kembar. Beri pembeda (mis. Andi A.).";return;}
  names=v;$("err").textContent="";begin();
};
function begin(){
  rem=[...names];score={};names.forEach(n=>score[n]=0);deck=[];
  $("setup").classList.add("hide");$("result").classList.add("hide");$("gamebox").classList.remove("hide");
  draw();board();
}
function nextQ(){
  if(!deck.length){deck=Q.map((_,i)=>i);for(let i=deck.length-1;i>0;i--){const j=Math.floor(Math.random()*(i+1));[deck[i],deck[j]]=[deck[j],deck[i]];}}
  return Q[deck.pop()];
}
function draw(){
  const c=$("wheel"),x=c.getContext("2d"),W=c.width,R=W/2-10,n=rem.length,seg=TAU/n;
  x.clearRect(0,0,W,W);x.save();x.translate(W/2,W/2);
  for(let i=0;i<n;i++){
    x.beginPath();x.moveTo(0,0);x.arc(0,0,R,rot+i*seg,rot+(i+1)*seg);x.closePath();
    x.fillStyle=COL[i%COL.length];x.fill();x.strokeStyle="#fff";x.lineWidth=4;x.stroke();
    x.save();x.rotate(rot+(i+.5)*seg);x.fillStyle="#fff";x.textAlign="right";x.textBaseline="middle";
    x.font="bold "+Math.max(20,Math.min(46,300/Math.sqrt(n)))+"px system-ui,sans-serif";
    let s=rem[i];if(s.length>14)s=s.slice(0,13)+"…";x.fillText(s,R-26,0);x.restore();
  }
  x.beginPath();x.arc(0,0,44,0,TAU);x.fillStyle="#fff";x.fill();x.strokeStyle="#2e8b57";x.lineWidth=8;x.stroke();
  x.restore();
}
function board(){
  const done=names.length-rem.length;
  $("prog").textContent="Giliran selesai: "+done+" / "+names.length;
  $("sb").innerHTML=names.map(n=>'<li class="'+(rem.includes(n)?"":"done")+'"><span></span><b>'+score[n]+'</b></li>').join("");
  [...$("sb").children].forEach((li,i)=>li.firstChild.textContent=names[i]+(rem.includes(names[i])?"":" ✓"));
}
$("spin").onclick=()=>{
  if(spinning||!rem.length)return;spinning=true;$("spin").disabled=true;
  const start=rot,total=TAU*(5+Math.random()*3)+Math.random()*TAU,dur=5200,t0=performance.now();
  (function f(now){
    const p=Math.min(1,(now-t0)/dur),e=1-Math.pow(1-p,3);
    rot=start+total*e;draw();
    if(p<1)return requestAnimationFrame(f);
    rot=rot%TAU;spinning=false;
    const n=rem.length,seg=TAU/n,ang=((-Math.PI/2-rot)%TAU+TAU)%TAU;
    pick=rem[Math.min(n-1,Math.floor(ang/seg))];
    ask();
  })(t0);
};
function ask(){
  cur=nextQ();
  $("topik").textContent=cur.t;$("giliran").textContent="Giliran: "+pick;$("soal").textContent=cur.q;
  $("opts").innerHTML="";$("fb").classList.add("hide");$("next").classList.add("hide");
  cur.o.forEach((t,i)=>{
    const b=document.createElement("button");b.className="opt";b.textContent="ABCD"[i]+". "+t;
    b.onclick=()=>answer(i);$("opts").appendChild(b);
  });
  $("ov").classList.remove("hide");
}
function answer(i){
  const bs=[...$("opts").children];bs.forEach(b=>b.disabled=true);
  bs[cur.a].classList.add("ok");
  const ok=i===cur.a;if(!ok)bs[i].classList.add("bad");else score[pick]+=10;
  $("fb").innerHTML="<b>"+(ok?"Benar! +10 poin":"Belum tepat.")+"</b> Jawaban: "+"ABCD"[cur.a]+".<br>"+cur.p;
  $("fb").classList.remove("hide");$("next").classList.remove("hide");
}
$("next").onclick=()=>{
  $("ov").classList.add("hide");
  rem=rem.filter(n=>n!==pick);board();
  $("spin").disabled=false;
  if(!rem.length)return finish();
  draw();
};
function finish(){
  $("gamebox").classList.add("hide");$("result").classList.remove("hide");
  const r=[...names].sort((a,b)=>score[b]-score[a]);
  $("champ").textContent="Juara: "+r[0]+" ("+score[r[0]]+" poin)";
  $("rt").innerHTML="";
  r.forEach((n,i)=>{const tr=document.createElement("tr");[i+1,n,score[n]].forEach(v=>{const td=document.createElement("td");td.textContent=v;tr.appendChild(td);});$("rt").appendChild(tr);});
}
$("again").onclick=begin;
$("reset").onclick=()=>{$("result").classList.add("hide");$("setup").classList.remove("hide");};
buildInputs();
</script>
</body>
</html>
