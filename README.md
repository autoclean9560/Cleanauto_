HTML 

<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="SpeedClean Auto – Nettoyage intérieur à domicile, secteur 60/95. Formules Basic, Confort, Premium. 07 72 35 53 54.">
<title>SpeedClean Auto · Nettoyage Intérieur · Secteur 60/95</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Rajdhani:wght@600;700&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#0f1318;--bg2:#161b22;--card:#1c2330;--card2:#222b38;
  --border:rgba(255,255,255,.07);--border2:rgba(255,255,255,.04);
  --blue:#2563eb;--blue-l:#3b82f6;--cyan:#06b6d4;
  --gold:#f59e0b;--green:#10b981;--red:#ef4444;
  --white:#f8fafc;--gray:#94a3b8;--gray2:#64748b;
  --r:10px;--fh:'Rajdhani',sans-serif;--fb:'Inter',sans-serif;
}
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--white);font-family:var(--fb);overflow-x:hidden;-webkit-font-smoothing:antialiased;line-height:1.6}
a{text-decoration:none;color:inherit}
button{font-family:var(--fb);cursor:pointer;border:none;outline:none}
input,select,textarea{font-family:var(--fb)}
img{display:block;max-width:100%}

/* PROMO */
.promo{background:linear-gradient(90deg,#7f1d1d,#991b1b 40%,#b91c1c);padding:9px 16px;text-align:center;font-size:.77rem;font-weight:500;color:#fecaca;z-index:20;position:relative}
.promo strong{color:#fff;font-weight:700}
.promo a{color:#fde68a;font-weight:600;text-decoration:underline;margin-left:7px}

/* HEADER */
header{position:sticky;top:0;z-index:200;background:rgba(15,19,24,.97);backdrop-filter:blur(20px);border-bottom:1px solid var(--border)}
.hdr{max-width:1200px;margin:0 auto;display:flex;align-items:center;justify-content:space-between;padding:0 20px;height:62px;gap:12px}
.brand{display:flex;align-items:center;gap:10px;cursor:pointer;flex-shrink:0}
.brand-logo{height:44px;width:auto;object-fit:contain;filter:drop-shadow(0 0 6px rgba(37,99,235,.4))}
.brand-info{display:flex;flex-direction:column;line-height:1.2}
.brand-name{font-family:var(--fh);font-size:1.1rem;font-weight:700;letter-spacing:1.5px;text-transform:uppercase}
.brand-name b{color:#60a5fa}
.brand-sub{font-size:.55rem;font-weight:500;letter-spacing:3px;text-transform:uppercase;color:var(--gray2)}
.hdr-r{display:flex;align-items:center;gap:9px}
.btn-call{display:flex;align-items:center;gap:6px;font-size:.78rem;font-weight:600;color:var(--cyan);border:1px solid rgba(6,182,212,.28);border-radius:8px;padding:7px 13px;transition:all .2s;background:rgba(6,182,212,.04)}
.btn-call:hover{background:rgba(6,182,212,.1);border-color:var(--cyan)}
.btn-book{display:flex;align-items:center;gap:6px;font-size:.78rem;font-weight:700;color:#fff;background:var(--blue);border-radius:8px;padding:8px 16px;transition:all .2s}
.btn-book:hover{background:var(--blue-l);box-shadow:0 0 18px rgba(37,99,235,.4);transform:translateY(-1px)}
@media(max-width:400px){.btn-call .tel-t{display:none}.brand-info{display:none}}
@media(max-width:520px){.btn-book .bk-t{display:none}}

/* TABS */
.tabs-nav{background:var(--bg2);border-bottom:1px solid var(--border);position:sticky;top:62px;z-index:190;display:flex;justify-content:center;overflow-x:auto;scrollbar-width:none}
.tabs-nav::-webkit-scrollbar{display:none}
.tab-btn{background:none;color:var(--gray2);font-size:.76rem;font-weight:600;letter-spacing:.8px;text-transform:uppercase;padding:13px 26px;transition:color .2s;white-space:nowrap;display:flex;align-items:center;gap:6px;border-bottom:2px solid transparent}
.tab-btn.active{color:var(--white);border-bottom-color:var(--blue-l)}
.tab-btn:hover{color:var(--white)}

/* PAGES */
.page{display:none;position:relative;z-index:1;min-height:calc(100vh - 108px)}
.page.active{display:block}

/* PAGE HERO */
.page-hero{text-align:center;padding:52px 20px 40px;background:linear-gradient(180deg,rgba(37,99,235,.05)0%,transparent 100%);border-bottom:1px solid var(--border2)}
.eyebrow{display:inline-flex;align-items:center;gap:5px;font-size:.68rem;font-weight:600;letter-spacing:3px;text-transform:uppercase;color:var(--cyan);background:rgba(6,182,212,.07);border:1px solid rgba(6,182,212,.18);border-radius:50px;padding:5px 13px;margin-bottom:16px}
.page-title{font-family:var(--fh);font-size:clamp(1.9rem,5vw,3rem);font-weight:700;text-transform:uppercase;line-height:1.05;letter-spacing:-.5px;margin-bottom:11px}
.page-title b{color:#60a5fa}
.page-sub{color:var(--gray);font-size:.91rem;line-height:1.7;max-width:460px;margin:0 auto}

.wrap{max-width:1200px;margin:0 auto;padding:0 20px}

/* ──────────── VEHICLE SELECTOR ──────────── */
.vs{padding:40px 20px 0;max-width:1200px;margin:0 auto}
.vs-lbl{text-align:center;font-size:.65rem;font-weight:600;letter-spacing:3px;text-transform:uppercase;color:var(--gray2);margin-bottom:12px}
.search-row{position:relative;max-width:520px;margin:0 auto 24px}
.s-inp{width:100%;background:var(--card);border:1px solid var(--border);border-radius:10px;color:var(--white);font-size:.88rem;padding:12px 14px 12px 42px;outline:none;transition:border-color .2s,box-shadow .2s}
.s-inp::placeholder{color:var(--gray2)}
.s-inp:focus{border-color:var(--blue-l);box-shadow:0 0 0 3px rgba(59,130,246,.1)}
.s-ico{position:absolute;left:14px;top:50%;transform:translateY(-50%);color:var(--gray2);font-size:.9rem;pointer-events:none}
.sdrop{position:absolute;top:calc(100% + 5px);left:0;right:0;background:var(--card2);border:1px solid var(--border);border-radius:10px;overflow:hidden;z-index:60;max-height:240px;overflow-y:auto;display:none;box-shadow:0 20px 50px rgba(0,0,0,.6)}
.sdrop.open{display:block}
.sdi{padding:11px 14px;font-size:.84rem;cursor:pointer;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid var(--border2);transition:background .13s}
.sdi:last-child{border:none}
.sdi:hover{background:rgba(255,255,255,.04)}
.sdi-year{font-size:.7rem;color:var(--gray2);margin-left:6px}
.sdi-cat{font-size:.6rem;font-weight:600;letter-spacing:1px;text-transform:uppercase;padding:2px 7px;border-radius:3px}
.sdi-cat.cit{background:rgba(16,185,129,.12);color:var(--green)}
.sdi-cat.suv{background:rgba(6,182,212,.12);color:var(--cyan)}
.sdi-cat.ber{background:rgba(99,102,241,.12);color:#a5b4fc}
.sdi-cat.van{background:rgba(245,158,11,.12);color:var(--gold)}

/* TYPE PILLS */
.type-pills{display:flex;justify-content:center;gap:10px;flex-wrap:wrap;margin-bottom:28px}
.type-pill{display:flex;align-items:center;gap:8px;background:var(--card);border:1px solid var(--border);border-radius:50px;padding:10px 20px;cursor:pointer;transition:all .22s;color:var(--gray);font-weight:500;font-size:.83rem}
.type-pill:hover{border-color:rgba(255,255,255,.18);color:var(--white)}
.type-pill.a-cit{border-color:var(--green);background:rgba(16,185,129,.08);color:var(--green);font-weight:600}
.type-pill.a-suv{border-color:var(--cyan);background:rgba(6,182,212,.08);color:var(--cyan);font-weight:600}
.type-pill.a-ber{border-color:#818cf8;background:rgba(99,102,241,.08);color:#a5b4fc;font-weight:600}
.type-pill.a-van{border-color:var(--gold);background:rgba(245,158,11,.08);color:var(--gold);font-weight:600}

/* ──────────── VEHICLE VIEWER ──────────── */
.veh-viewer{max-width:860px;margin:0 auto 36px;display:none}
.veh-viewer.show{display:block}
.vv-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:12px;padding:0 2px}
.vv-title{font-size:.95rem;font-weight:700;color:var(--white);display:flex;align-items:center;gap:10px}
.vv-cat-badge{font-size:.6rem;font-weight:600;letter-spacing:1.5px;text-transform:uppercase;padding:3px 9px;border-radius:4px}
.vv-controls{display:flex;gap:8px}
.vv-btn{background:var(--card);border:1px solid var(--border);color:var(--gray);font-size:.72rem;font-weight:600;letter-spacing:.5px;padding:6px 12px;border-radius:6px;cursor:pointer;transition:all .2s}
.vv-btn:hover{border-color:rgba(255,255,255,.2);color:var(--white)}
.vv-btn.active{background:rgba(37,99,235,.15);border-color:var(--blue-l);color:var(--blue-l)}

/* Gallery mode */
.gallery-wrap{position:relative;border-radius:12px;overflow:hidden;background:var(--card);border:1px solid var(--border);aspect-ratio:16/8}
.g-slide{position:absolute;inset:0;opacity:0;transition:opacity .5s ease;display:flex;align-items:center;justify-content:center;flex-direction:column;gap:8px}
.g-slide.active{opacity:1}
.g-slide img{width:100%;height:100%;object-fit:cover}
.g-fallback{width:100%;height:100%;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:8px;background:linear-gradient(135deg,#1c2330,#222b38)}
.g-fallback .gf-emoji{font-size:3rem}
.g-fallback .gf-name{font-family:var(--fh);font-size:1rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--gray)}
.g-fallback .gf-view{font-size:.62rem;letter-spacing:2px;text-transform:uppercase;color:var(--gray2)}
.g-arrow{position:absolute;top:50%;transform:translateY(-50%);background:rgba(0,0,0,.55);border:1px solid rgba(255,255,255,.12);color:#fff;width:34px;height:34px;border-radius:50%;display:flex;align-items:center;justify-content:center;cursor:pointer;font-size:.88rem;transition:all .2s;z-index:5}
.g-arrow:hover{background:rgba(0,0,0,.85)}
.g-prev{left:10px}.g-next{right:10px}
.g-dots{display:flex;justify-content:center;gap:5px;margin-top:9px}
.g-dot{width:6px;height:6px;border-radius:50%;background:var(--border);cursor:pointer;transition:all .2s}
.g-dot.active{background:var(--blue-l);width:16px;border-radius:3px}

/* 3D Canvas */
.canvas-wrap{position:relative;border-radius:12px;overflow:hidden;background:var(--card);border:1px solid var(--border);aspect-ratio:16/8}
#threeCanvas{width:100%;height:100%;display:block}
.canvas-hint{position:absolute;bottom:10px;left:50%;transform:translateX(-50%);font-size:.65rem;color:var(--gray2);letter-spacing:1px;background:rgba(0,0,0,.5);padding:4px 10px;border-radius:4px;pointer-events:none}

/* Specs */
.vv-specs{background:var(--card);border:1px solid var(--border);border-radius:var(--r);padding:16px 20px;margin-top:12px;display:none}
.vv-specs.show{display:block}
.specs-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(160px,1fr));gap:10px;margin-top:10px}
.spec-item{background:var(--bg2);border-radius:7px;padding:10px 12px}
.spec-label{font-size:.6rem;font-weight:600;letter-spacing:2px;text-transform:uppercase;color:var(--gray2);margin-bottom:3px}
.spec-value{font-size:.84rem;font-weight:600;color:var(--white)}

/* ──────────── PRICING CARDS ──────────── */
.pricing-sect{padding:0 20px 52px;max-width:1200px;margin:0 auto}
.cards-g{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
@media(max-width:820px){.cards-g{grid-template-columns:1fr}}
.pc{background:var(--card);border:1px solid var(--border);border-radius:var(--r);overflow:hidden;display:flex;flex-direction:column;transition:transform .24s,box-shadow .24s,border-color .24s}
.pc:hover{transform:translateY(-4px);box-shadow:0 20px 48px rgba(0,0,0,.45);border-color:rgba(255,255,255,.13)}
.pc.feat{border-color:rgba(245,158,11,.22);background:linear-gradient(155deg,rgba(245,158,11,.04),var(--card))}
.pc.feat:hover{border-color:rgba(245,158,11,.42)}
.pc-head{padding:22px 22px 18px;border-bottom:1px solid var(--border2)}
.pc-tier{font-size:.58rem;font-weight:600;letter-spacing:3px;text-transform:uppercase;color:var(--gray2);margin-bottom:5px}
.pc-name{font-family:var(--fh);font-size:1.95rem;font-weight:700;text-transform:uppercase;margin-bottom:6px}
.nm-g{color:var(--green)}.nm-b{color:#60a5fa}.nm-go{color:var(--gold)}
.pc-tag{display:inline-block;font-size:.6rem;font-weight:600;letter-spacing:1.5px;text-transform:uppercase;padding:3px 9px;border-radius:4px}
.tg{background:rgba(16,185,129,.1);color:var(--green);border:1px solid rgba(16,185,129,.2)}
.tb{background:rgba(59,130,246,.1);color:#93c5fd;border:1px solid rgba(59,130,246,.2)}
.tgo{background:rgba(245,158,11,.1);color:var(--gold);border:1px solid rgba(245,158,11,.2)}
.pc-body{padding:18px 22px;flex:1;display:flex;flex-direction:column}
.pc-feats{list-style:none;margin-bottom:20px;flex:1}
.pc-feats li{display:flex;align-items:flex-start;gap:9px;font-size:.83rem;color:var(--gray);padding:6px 0;border-bottom:1px solid var(--border2);line-height:1.45}
.pc-feats li:last-child{border:none}
.ck{font-weight:700;flex-shrink:0;margin-top:1px;font-size:.86rem}
.cg{color:var(--green)}.cb{color:#60a5fa}.cgo{color:var(--gold)}
.pbox{background:rgba(255,255,255,.03);border-radius:8px;padding:13px 15px;margin-bottom:12px;display:flex;align-items:center;justify-content:space-between}
.pbox.gld{background:rgba(245,158,11,.05)}
.ptype{font-size:.68rem;font-weight:600;letter-spacing:1px;text-transform:uppercase;color:var(--gray2)}
.pval{font-family:var(--fh);font-size:2rem;font-weight:700;display:flex;align-items:baseline;gap:5px}
.pold{text-decoration:line-through;opacity:.35;font-size:1rem}
.pnew{color:var(--red)}
.pc-models{margin-top:11px;padding-top:11px;border-top:1px solid var(--border2)}
.pm-lbl{font-size:.58rem;font-weight:600;letter-spacing:2px;text-transform:uppercase;color:var(--gray2);margin-bottom:7px}
.pm-tags{display:flex;flex-wrap:wrap;gap:4px}
.m-tag{font-size:.66rem;background:rgba(255,255,255,.04);border:1px solid var(--border2);border-radius:4px;padding:2px 7px;color:var(--gray2)}
.pc-cta{width:100%;padding:12px;border-radius:8px;margin-top:16px;font-weight:700;font-size:.84rem;transition:all .2s}
.cc-g{background:var(--green);color:#000}
.cc-g:hover{box-shadow:0 0 18px rgba(16,185,129,.35);transform:translateY(-1px)}
.cc-b{background:var(--blue);color:#fff}
.cc-b:hover{background:var(--blue-l);box-shadow:0 0 18px rgba(37,99,235,.35);transform:translateY(-1px)}
.cc-go{background:var(--gold);color:#000}
.cc-go:hover{box-shadow:0 0 18px rgba(245,158,11,.35);transform:translateY(-1px)}

/* OPTION BAND */
.opt-band{max-width:1200px;margin:0 auto 52px;padding:0 20px}
.opt-in{background:var(--card);border:1px solid var(--border);border-radius:var(--r);padding:18px 26px;display:flex;align-items:center;justify-content:center;gap:18px;flex-wrap:wrap;text-align:center}
.opt-ttl{font-size:.88rem;font-weight:600;color:var(--white)}
.opt-sub{font-size:.76rem;color:var(--gray2);margin-top:2px}
.opt-p{font-family:var(--fh);font-size:1.65rem;font-weight:700;color:var(--gold)}

/* CONTACT STRIP */
.cstrip{background:var(--bg2);border-top:1px solid var(--border);padding:15px 20px;text-align:center;font-size:.81rem;color:var(--gray2)}
.cstrip a{color:#60a5fa;font-weight:600}
.cstrip strong{color:var(--white)}
.soc-row{display:flex;justify-content:center;gap:9px;flex-wrap:wrap;padding:18px 20px 70px;max-width:1200px;margin:0 auto}
.soc{display:inline-flex;align-items:center;gap:6px;background:var(--card);border:1px solid var(--border);border-radius:50px;padding:7px 14px;font-size:.73rem;font-weight:500;color:var(--gray2);transition:all .2s}
.soc:hover{border-color:rgba(255,255,255,.18);color:var(--white)}

/* ──────────── RDV PAGE ──────────── */
.rdv-layout{display:grid;grid-template-columns:320px 1fr;gap:28px;padding:36px 20px 68px;max-width:1200px;margin:0 auto}
@media(max-width:820px){.rdv-layout{grid-template-columns:1fr}}
.rdv-left{display:flex;flex-direction:column;gap:14px}
.icard{background:var(--card);border:1px solid var(--border);border-radius:var(--r);padding:20px 18px}
.ic-lbl{font-size:.58rem;font-weight:600;letter-spacing:3px;text-transform:uppercase;color:var(--cyan);margin-bottom:7px}
.ic-ttl{font-size:1rem;font-weight:700;color:var(--white);margin-bottom:5px}
.ic-txt{font-size:.82rem;color:var(--gray);line-height:1.7}
.big-tel{font-family:var(--fh);font-size:1.75rem;font-weight:700;color:#60a5fa;display:block;margin:9px 0 4px;letter-spacing:.5px;transition:color .2s}
.big-tel:hover{color:var(--white)}
.steps{list-style:none;margin-top:7px}
.steps li{display:flex;gap:9px;font-size:.8rem;color:var(--gray);padding:5px 0;align-items:flex-start;line-height:1.55}
.sn{background:var(--blue);color:#fff;font-weight:700;font-size:.66rem;border-radius:50%;width:19px;height:19px;display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:2px}

/* FORM */
.fcard{background:var(--card);border:1px solid var(--border);border-radius:var(--r);padding:28px 26px}
.f-ttl{font-size:1.45rem;font-weight:800;color:var(--white);margin-bottom:3px}
.f-sub{font-size:.8rem;color:var(--gray2);margin-bottom:22px}
.fg{margin-bottom:14px}
.fg label{display:block;font-size:.64rem;font-weight:600;letter-spacing:2px;text-transform:uppercase;color:var(--gray2);margin-bottom:6px}
.fg input,.fg select,.fg textarea{width:100%;background:var(--bg2);border:1px solid var(--border);border-radius:8px;color:var(--white);font-size:.87rem;padding:11px 13px;outline:none;transition:border-color .2s,box-shadow .2s;appearance:none}
.fg input::placeholder{color:var(--gray2)}
.fg input:focus,.fg select:focus,.fg textarea:focus{border-color:var(--blue-l);box-shadow:0 0 0 3px rgba(59,130,246,.1)}
.fg select option{background:#1c2330}
.fg textarea{resize:vertical;min-height:68px}
.frow{display:grid;grid-template-columns:1fr 1fr;gap:12px}
@media(max-width:480px){.frow{grid-template-columns:1fr}}
.veh-wrap2{position:relative}
.vdrop2{position:absolute;top:calc(100% + 4px);left:0;right:0;background:var(--card2);border:1px solid var(--border);border-radius:8px;overflow:hidden;z-index:50;max-height:190px;overflow-y:auto;display:none;box-shadow:0 16px 44px rgba(0,0,0,.6)}
.vdrop2.open{display:block}
.vi2{padding:10px 13px;font-size:.83rem;cursor:pointer;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid var(--border2);transition:background .13s}
.vi2:last-child{border:none}
.vi2:hover{background:rgba(255,255,255,.04)}
.det{background:rgba(59,130,246,.07);border:1px solid rgba(59,130,246,.18);border-radius:7px;padding:8px 12px;font-size:.83rem;font-weight:500;color:#93c5fd;display:none;margin-top:7px}
.fcards{display:grid;grid-template-columns:repeat(3,1fr);gap:9px;margin-bottom:14px}
@media(max-width:480px){.fcards{grid-template-columns:1fr}}
.fc2{background:var(--bg2);border:1px solid var(--border);border-radius:8px;padding:13px 10px;text-align:center;cursor:pointer;transition:all .2s}
.fc2:hover{border-color:rgba(255,255,255,.16)}
.fc2.s-basic{border-color:var(--green)!important;background:rgba(16,185,129,.07)!important}
.fc2.s-confort{border-color:#3b82f6!important;background:rgba(59,130,246,.07)!important}
.fc2.s-premium{border-color:var(--gold)!important;background:rgba(245,158,11,.07)!important}
.fc2-name{font-family:var(--fh);font-size:.93rem;font-weight:700;text-transform:uppercase}
.fg2{color:var(--green)}.fb2{color:#60a5fa}.fgo2{color:var(--gold)}
.fc2-p{font-size:.71rem;color:var(--gray2);margin-top:3px}
.fc2-p strong{color:var(--gray)}
.opt-tog{display:flex;align-items:center;justify-content:space-between;background:var(--bg2);border:1px solid var(--border);border-radius:8px;padding:13px 14px;cursor:pointer;transition:all .2s;margin-bottom:14px;user-select:none}
.opt-tog.on{border-color:var(--gold);background:rgba(245,158,11,.06)}
.ot-l{display:flex;align-items:center;gap:9px}
.ot-ttl{font-size:.86rem;font-weight:600;color:var(--white)}
.ot-sub{font-size:.71rem;color:var(--gray2);margin-top:1px}
.ot-p{font-family:var(--fh);font-size:1.1rem;font-weight:700;color:var(--gold)}
.knob{width:37px;height:20px;background:rgba(255,255,255,.1);border-radius:50px;position:relative;transition:background .2s;flex-shrink:0}
.knob::after{content:'';position:absolute;top:2.5px;left:2.5px;width:15px;height:15px;border-radius:50%;background:#fff;transition:transform .2s}
.opt-tog.on .knob{background:var(--gold)}
.opt-tog.on .knob::after{transform:translateX(17px)}
.sum-box{background:rgba(37,99,235,.07);border:1px solid rgba(37,99,235,.18);border-radius:8px;padding:13px 15px;margin-bottom:14px;display:none;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:7px}
.sum-lbl{font-size:.76rem;color:var(--gray2)}
.sum-val{font-family:var(--fh);font-size:1.85rem;font-weight:700;color:#60a5fa}
.btn-sub{width:100%;padding:13px;border-radius:8px;background:var(--blue);color:#fff;font-weight:700;font-size:.88rem;transition:all .2s}
.btn-sub:hover{background:var(--blue-l);box-shadow:0 0 22px rgba(37,99,235,.35);transform:translateY(-1px)}
.btn-sub:disabled{opacity:.44;cursor:not-allowed;transform:none}
.f-alert{border-radius:8px;padding:12px 14px;font-size:.82rem;font-weight:500;margin-top:12px;display:none}
.f-alert.show{display:block}
.a-ok{background:rgba(16,185,129,.1);border:1px solid rgba(16,185,129,.22);color:#6ee7b7}
.a-err{background:rgba(239,68,68,.1);border:1px solid rgba(239,68,68,.22);color:#fca5a5}
.f-note{font-size:.68rem;color:var(--gray2);text-align:center;margin-top:11px;line-height:1.6}

/* ──────────── BOUTIQUE ──────────── */
.shop-note{max-width:1200px;margin:0 auto 24px;padding:0 20px}
.shop-note-in{background:var(--card);border:1px solid rgba(245,158,11,.18);border-radius:var(--r);padding:16px 22px;font-size:.82rem;color:var(--gray2);text-align:center;line-height:1.7}
.shop-note-in strong{color:var(--gold)}
.shop-note-in a{color:var(--gold);font-weight:600}
.shop-g{display:grid;grid-template-columns:repeat(auto-fill,minmax(235px,1fr));gap:18px;padding:0 20px 68px;max-width:1200px;margin:0 auto}
.sc{background:var(--card);border:1px solid var(--border);border-radius:var(--r);overflow:hidden;transition:transform .24s,box-shadow .24s}
.sc:hover{transform:translateY(-4px);box-shadow:0 16px 40px rgba(0,0,0,.45)}
.sc-img{height:150px;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:5px;background:linear-gradient(135deg,var(--bg2),var(--card2));border-bottom:1px solid var(--border);position:relative;font-size:3.2rem}
.sc-badge{position:absolute;top:9px;right:9px;background:var(--gold);color:#000;font-size:.54rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;padding:3px 7px;border-radius:4px}
.sc-brand-tag{font-family:var(--fh);font-size:.66rem;font-weight:700;letter-spacing:3px;text-transform:uppercase;color:var(--gray2)}
.sc-body{padding:16px 16px 18px}
.sc-br{font-size:.56rem;letter-spacing:3px;text-transform:uppercase;color:var(--gray2);margin-bottom:3px}
.sc-name{font-size:1rem;font-weight:700;color:var(--white);margin-bottom:6px}
.sc-desc{font-size:.78rem;color:var(--gray2);line-height:1.6;margin-bottom:12px}
.sc-foot{display:flex;align-items:center;justify-content:space-between}
.sc-price{font-family:var(--fh);font-size:1.35rem;font-weight:700;color:var(--gold)}
.sc-btn{background:rgba(37,99,235,.1);border:1px solid rgba(37,99,235,.28);color:#93c5fd;font-size:.72rem;font-weight:600;padding:6px 12px;border-radius:6px;cursor:pointer;transition:all .2s}
.sc-btn:hover{background:var(--blue);color:#fff;border-color:var(--blue)}

/* FOOTER */
footer{border-top:1px solid var(--border);padding:32px 20px 26px}
.footer-g{max-width:1200px;margin:0 auto;display:flex;flex-wrap:wrap;gap:28px;align-items:flex-start;justify-content:space-between}
.f-bn{font-family:var(--fh);font-size:1.1rem;font-weight:700;color:var(--white)}
.f-bn b{color:#60a5fa}
.f-tag{font-size:.75rem;color:var(--gray2);margin-top:3px}
.f-links{display:flex;flex-direction:column;gap:9px}
.f-links a{color:var(--gray2);font-size:.8rem;transition:color .2s}
.f-links a:hover{color:var(--white)}
.footer-bot{max-width:1200px;margin:20px auto 0;padding-top:18px;border-top:1px solid var(--border2);display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:10px;font-size:.72rem;color:var(--gray2)}
.g-btn{display:inline-flex;align-items:center;gap:6px;background:var(--card);border:1px solid var(--border);border-radius:7px;padding:7px 14px;font-size:.75rem;font-weight:600;color:var(--white);transition:all .2s}
.g-btn:hover{border-color:rgba(255,255,255,.18)}

/* FABs */
.fab-call{position:fixed;bottom:20px;right:20px;z-index:400;display:flex;align-items:center;gap:7px;background:var(--green);color:#000;font-weight:700;font-size:.8rem;padding:11px 17px;border-radius:50px;box-shadow:0 4px 20px rgba(16,185,129,.4);transition:transform .2s;animation:fp 3s ease-in-out infinite}
.fab-call:hover{transform:scale(1.04)}
@keyframes fp{0%,100%{box-shadow:0 4px 20px rgba(16,185,129,.4)}50%{box-shadow:0 4px 32px rgba(16,185,129,.65)}}
.fab-rdv{position:fixed;bottom:20px;left:20px;z-index:400;display:flex;align-items:center;gap:7px;background:var(--blue);color:#fff;font-weight:700;font-size:.8rem;padding:11px 17px;border-radius:50px;box-shadow:0 4px 20px rgba(37,99,235,.4);transition:all .2s}
.fab-rdv:hover{transform:scale(1.04);background:var(--blue-l)}
@media(min-width:900px){.fab-call,.fab-rdv{font-size:.76rem;padding:10px 15px}}

[data-a]{opacity:0;transform:translateY(16px);transition:opacity .5s ease,transform .5s ease}
[data-a].in{opacity:1;transform:translateY(0)}
</style>
</head>
<body>

<!-- PROMO -->
<div class="promo" id="promoBar">
  <strong>🔥 OFFRE EXCLUSIVE</strong> — <strong>–40% sur toutes les formules</strong> jusqu'au <strong>20 JUIN 2025</strong>
  <a href="#" onclick="goTab('rdv');return false">Réserver →</a>
</div>

<!-- HEADER -->
<header>
  <div class="hdr">
    <a class="brand" href="#" onclick="goTab('tarifs');return false">
      <img class="brand-logo" src="/mnt/user-data/uploads/IMG_4598.png" alt="SpeedClean Auto 60/95">
      <div class="brand-info">
        <span class="brand-name">SPEED<b>CLEAN</b> AUTO</span>
        <span class="brand-sub">Nettoyage Intérieur · Secteur 60/95</span>
      </div>
    </a>
    <div class="hdr-r">
      <a href="tel:0772355354" class="btn-call">
        <span>📞</span><span class="tel-t">07 72 35 53 54</span>
      </a>
      <button class="btn-book" onclick="goTab('rdv')">
        <span>📅</span><span class="bk-t">Réserver</span>
      </button>
    </div>
  </div>
</header>

<!-- TABS -->
<nav class="tabs-nav">
  <button class="tab-btn active" id="tab-tarifs" onclick="goTab('tarifs')">💰 Formules & Tarifs</button>
  <button class="tab-btn" id="tab-rdv" onclick="goTab('rdv')">📅 Prendre RDV</button>
  <button class="tab-btn" id="tab-shop" onclick="goTab('shop')">🛍️ Boutique</button>
</nav>

<!-- ══════ PAGE TARIFS ══════ -->
<div class="page active" id="page-tarifs">
  <div class="page-hero" data-a>
    <div class="eyebrow">✨ Nettoyage professionnel à domicile</div>
    <h1 class="page-title">Nos <b>Formules</b></h1>
    <p class="page-sub">Sélectionnez votre véhicule pour un tarif adapté · À domicile ou sur place · Secteur 60/95</p>
  </div>

  <div class="vs" data-a>
    <p class="vs-lbl">Recherchez votre véhicule (marque, modèle, année)</p>
    <div class="search-row">
      <span class="s-ico">🔍</span>
      <input class="s-inp" id="mainS" type="text" placeholder="Ex : Peugeot 308 2021, Toyota Yaris 2019, BMW X5 Phase 3…" autocomplete="off" oninput="doS(this.value,'mDrop','pill')">
      <div class="sdrop" id="mDrop"></div>
    </div>
    <div class="type-pills">
      <div class="type-pill" id="p-cit" onclick="setPill('cit')"><span>🚗</span> Citadine</div>
      <div class="type-pill" id="p-suv" onclick="setPill('suv')"><span>🚙</span> SUV / Crossover</div>
      <div class="type-pill" id="p-ber" onclick="setPill('ber')"><span>🚘</span> Berline / Break</div>
      <div class="type-pill" id="p-van" onclick="setPill('van')"><span>🚐</span> Monospace / Van</div>
    </div>

    <!-- Vehicle viewer -->
    <div class="veh-viewer" id="vehViewer">
      <div class="vv-header">
        <div class="vv-title">
          <span id="vvName">—</span>
          <span class="vv-cat-badge" id="vvCat"></span>
        </div>
        <div class="vv-controls">
          <button class="vv-btn active" id="btnGallery" onclick="setMode('gallery')">📷 Photos</button>
          <button class="vv-btn" id="btnSpecs" onclick="toggleSpecs()">📋 Infos</button>
        </div>
      </div>

      <!-- Gallery -->
      <div id="galleryWrap">
        <div class="gallery-wrap" id="gallerySlide">
          <button class="g-arrow g-prev" onclick="gNav(-1)">‹</button>
          <button class="g-arrow g-next" onclick="gNav(1)">›</button>
        </div>
        <div class="g-dots" id="gDots"></div>
      </div>

      <!-- Specs panel -->
      <div class="vv-specs" id="vvSpecs">
        <p style="font-size:.68rem;font-weight:600;letter-spacing:2px;text-transform:uppercase;color:var(--gray2)">Informations véhicule</p>
        <div class="specs-grid" id="specsGrid"></div>
      </div>
    </div>
  </div>

  <!-- CARDS -->
  <div class="pricing-sect" data-a>
    <div class="cards-g">
      <div class="pc">
        <div class="pc-head">
          <p class="pc-tier">Formule</p>
          <p class="pc-name nm-g">BASIC</p>
          <span class="pc-tag tg">L'essentiel · Rapide & Efficace</span>
        </div>
        <div class="pc-body">
          <ul class="pc-feats">
            <li><span class="ck cg">✓</span>Aspiration complète de l'habitacle</li>
            <li><span class="ck cg">✓</span>Tableau de bord nettoyé</li>
          </ul>
          <div class="pbox"><span class="ptype" id="b-lbl">Citadine</span><span class="pval" id="b-val"></span></div>
          <div class="pc-models"><p class="pm-lbl">Exemples</p><div class="pm-tags" id="b-tags"></div></div>
          <button class="pc-cta cc-g" onclick="pick('basic')">Choisir Basic →</button>
        </div>
      </div>
      <div class="pc">
        <div class="pc-head">
          <p class="pc-tier">Formule</p>
          <p class="pc-name nm-b">CONFORT</p>
          <span class="pc-tag tb">Propre & Agréable</span>
        </div>
        <div class="pc-body">
          <ul class="pc-feats">
            <li><span class="ck cb">✓</span>Aspiration complète</li>
            <li><span class="ck cb">✓</span>Sièges & tapis nettoyés</li>
            <li><span class="ck cb">✓</span>Plastiques & tableau de bord</li>
            <li><span class="ck cb">✓</span>Vitres intérieures</li>
          </ul>
          <div class="pbox"><span class="ptype" id="c-lbl">Citadine</span><span class="pval" id="c-val"></span></div>
          <div class="pc-models"><p class="pm-lbl">Exemples</p><div class="pm-tags" id="c-tags"></div></div>
          <button class="pc-cta cc-b" onclick="pick('confort')">Choisir Confort →</button>
        </div>
      </div>
      <div class="pc feat">
        <div class="pc-head" style="background:linear-gradient(135deg,rgba(245,158,11,.04),transparent)">
          <p class="pc-tier">Formule</p>
          <p class="pc-name nm-go">PREMIUM</p>
          <span class="pc-tag tgo">Finition Haut de Gamme</span>
        </div>
        <div class="pc-body">
          <ul class="pc-feats">
            <li><span class="ck cgo">✓</span>Tout de la formule Confort</li>
            <li><span class="ck cgo">✓</span>Shampooing sièges & tissus</li>
            <li><span class="ck cgo">✓</span>Nettoyage détaillé (aérations, recoins)</li>
            <li><span class="ck cgo">✓</span>Résultat comme neuf garanti</li>
          </ul>
          <div class="pbox gld"><span class="ptype" id="p-lbl">Citadine</span><span class="pval nm-go" id="p-val"></span></div>
          <div class="pc-models"><p class="pm-lbl">Exemples</p><div class="pm-tags" id="p-tags"></div></div>
          <button class="pc-cta cc-go" onclick="pick('premium')">Choisir Premium →</button>
        </div>
      </div>
    </div>
  </div>

  <div class="opt-band">
    <div class="opt-in">
      <span style="font-size:1.4rem">✨</span>
      <div><p class="opt-ttl">Option Désinfection & Parfum</p><p class="opt-sub">Élimine bactéries · Parfum longue durée</p></div>
      <span class="opt-p" id="optP"></span>
    </div>
  </div>

  <div class="cstrip">
    📍 <strong>Secteur 60/95</strong> · <a href="tel:0772355354">07 72 35 53 54</a> ·
    <a href="#" onclick="goTab('rdv');return false">📅 Prendre RDV →</a>
  </div>
  <div class="soc-row">
    <a href="https://www.instagram.com/speedcleanauto_6095" target="_blank" class="soc">📸 @speedcleanauto_6095</a>
    <a href="https://www.snapchat.com/add/speedcleanauto_6095" target="_blank" class="soc">👻 @speedcleanauto_6095</a>
    <span class="soc" style="opacity:.5;cursor:default">🎵 TikTok bientôt actif</span>
  </div>
</div>

<!-- ══════ PAGE RDV ══════ -->
<div class="page" id="page-rdv">
  <div class="page-hero" data-a>
    <div class="eyebrow">📅 Réservation</div>
    <h1 class="page-title">Prendre <b>Rendez-Vous</b></h1>
    <p class="page-sub">Remplissez le formulaire · Confirmation par email sous 24h</p>
  </div>
  <div class="rdv-layout">
    <div class="rdv-left" data-a>
      <div class="icard">
        <p class="ic-lbl">Contact direct</p>
        <p class="ic-ttl">Réponse immédiate</p>
        <a href="tel:0772355354" class="big-tel">07 72 35 53 54</a>
        <p class="ic-txt">7j/7 · Laissez un message, je rappelle.</p>
      </div>
      <div class="icard">
        <p class="ic-lbl">Comment ça marche</p>
        <ul class="steps">
          <li><span class="sn">1</span>Remplissez le formulaire</li>
          <li><span class="sn">2</span>Je vérifie ma disponibilité</li>
          <li><span class="sn">3</span>Confirmation par email sous 24h</li>
          <li><span class="sn">4</span>Rappel automatique la veille</li>
        </ul>
      </div>
      <div class="icard">
        <p class="ic-lbl">Zone</p>
        <p class="ic-txt">📍 <strong style="color:var(--white)">Oise (60) & Val d'Oise (95)</strong><br>Déplacement à domicile · Devis gratuit</p>
      </div>
      <div class="soc-row" style="padding:0;justify-content:flex-start;gap:8px">
        <a href="https://www.instagram.com/speedcleanauto_6095" target="_blank" class="soc">📸 Instagram</a>
        <a href="https://www.snapchat.com/add/speedcleanauto_6095" target="_blank" class="soc">👻 Snapchat</a>
      </div>
    </div>
    <div class="fcard" data-a style="transition-delay:.1s">
      <p class="f-ttl">Demande de RDV</p>
      <p class="f-sub">Champs * obligatoires · Confirmation sous 24h</p>
      <div class="frow">
        <div class="fg"><label>Prénom *</label><input type="text" id="r-pn" placeholder="Jean"></div>
        <div class="fg"><label>Nom *</label><input type="text" id="r-nm" placeholder="Dupont"></div>
      </div>
      <div class="frow">
        <div class="fg"><label>Email *</label><input type="email" id="r-em" placeholder="jean@email.com"></div>
        <div class="fg"><label>Téléphone *</label><input type="tel" id="r-tl" placeholder="06 00 00 00 00"></div>
      </div>
      <div class="fg">
        <label>Marque, Modèle & Année *</label>
        <div class="veh-wrap2">
          <input type="text" id="r-veh" placeholder="Ex : Renault Clio 2020, BMW X5 2022…" autocomplete="off" oninput="doS(this.value,'vDrop','form')">
          <div class="vdrop2" id="vDrop"></div>
        </div>
        <div class="det" id="detType"></div>
      </div>
      <div class="fg" id="manFg">
        <label>Type *</label>
        <select id="r-vt" onchange="updSum()">
          <option value="">Sélectionner…</option>
          <option value="cit">Citadine</option>
          <option value="suv">SUV / Crossover</option>
          <option value="ber">Berline / Break</option>
          <option value="van">Monospace / Van</option>
        </select>
      </div>
      <div class="fg">
        <label>Formule *</label>
        <div class="fcards">
          <div class="fc2" id="fc-b" onclick="pickF('basic')"><p class="fc2-name fg2">BASIC</p><p class="fc2-p" id="fp-b">—</p></div>
          <div class="fc2" id="fc-c" onclick="pickF('confort')"><p class="fc2-name fb2">CONFORT</p><p class="fc2-p" id="fp-c">—</p></div>
          <div class="fc2" id="fc-p" onclick="pickF('premium')"><p class="fc2-name fgo2">PREMIUM</p><p class="fc2-p" id="fp-p">—</p></div>
        </div>
      </div>
      <div class="opt-tog" id="oTog" onclick="togOpt()">
        <div class="ot-l">
          <span style="font-size:1.2rem">✨</span>
          <div><p class="ot-ttl">Désinfection & Parfum</p><p class="ot-sub">Bactéries éliminées · Odeur longue durée</p></div>
        </div>
        <div style="display:flex;align-items:center;gap:10px">
          <span class="ot-p" id="otP">+5€</span>
          <div class="knob"></div>
        </div>
      </div>
      <div class="sum-box" id="sumBox">
        <span class="sum-lbl" id="sumL">Récapitulatif</span>
        <span class="sum-val" id="sumV">—</span>
      </div>
      <div class="frow">
        <div class="fg"><label>Date souhaitée *</label><input type="date" id="r-dt"></div>
        <div class="fg">
          <label>Heure *</label>
          <select id="r-hr">
            <option value="">Choisir…</option>
            <option>8h00</option><option>9h00</option><option>10h00</option>
            <option>11h00</option><option>12h00</option><option>13h00</option>
            <option>14h00</option><option>15h00</option><option>16h00</option>
            <option>17h00</option><option>18h00</option>
          </select>
        </div>
      </div>
      <div class="fg"><label>Adresse & précisions</label><textarea id="r-msg" placeholder="Adresse si à domicile · Infos utiles…"></textarea></div>
      <button class="btn-sub" id="subBtn" onclick="submitRDV()">📅 Envoyer ma demande de rendez-vous</button>
      <div class="f-alert a-ok" id="aOk"></div>
      <div class="f-alert a-err" id="aErr"></div>
      <p class="f-note">🔒 Données confidentielles · Jamais partagées · Confirmation sous 24h</p>
    </div>
  </div>
  <div class="cstrip">📞 <a href="tel:0772355354">07 72 35 53 54</a> · 📍 <strong>Secteur 60/95</strong> · ✉️ <a href="mailto:autoclean9560@gmail.com">autoclean9560@gmail.com</a></div>
</div>

<!-- ══════ PAGE BOUTIQUE ══════ -->
<div class="page" id="page-shop">
  <div class="page-hero" data-a>
    <div class="eyebrow">🛍️ Boutique</div>
    <h1 class="page-title">Produits <b>Signature</b></h1>
    <p class="page-sub">Senteurs exclusives SpeedClean Auto · Fabriquées à notre image</p>
  </div>
  <div class="shop-note"><div class="shop-note-in">🚀 <strong>Bientôt disponible !</strong> Produits en fabrication avec notre logo exclusif. Pré-commandez dès maintenant — <a href="tel:0772355354">07 72 35 53 54</a></div></div>
  <div class="shop-g">
    <div class="sc" data-a><div class="sc-img">🌲<div class="sc-badge">NOUVEAU</div><span class="sc-brand-tag">SpeedClean</span></div><div class="sc-body"><p class="sc-br">SpeedClean Auto</p><p class="sc-name">Spray Forêt Alpine</p><p class="sc-desc">Senteur fraîche et boisée longue durée. Logo SpeedClean gravé.</p><div class="sc-foot"><span class="sc-price">~12€</span><button class="sc-btn" onclick="orderP('Spray Forêt Alpine')">Commander →</button></div></div></div>
    <div class="sc" data-a style="transition-delay:.07s"><div class="sc-img">🍋<span class="sc-brand-tag">SpeedClean</span></div><div class="sc-body"><p class="sc-br">SpeedClean Auto</p><p class="sc-name">Diffuseur Agrumes</p><p class="sc-desc">Éclat citrus, neutralise les mauvaises odeurs. Clip ventilation inclus.</p><div class="sc-foot"><span class="sc-price">~9€</span><button class="sc-btn" onclick="orderP('Diffuseur Agrumes')">Commander →</button></div></div></div>
    <div class="sc" data-a style="transition-delay:.14s"><div class="sc-img" style="background:linear-gradient(135deg,rgba(245,158,11,.1),var(--card2))">🖤<div class="sc-badge">PREMIUM</div><span class="sc-brand-tag" style="color:var(--gold)">SpeedClean</span></div><div class="sc-body"><p class="sc-br">SpeedClean Auto</p><p class="sc-name">Parfum Cuir & Luxe</p><p class="sc-desc">Notes cuir & bois de santal. Fragrance haut de gamme. Édition Premium.</p><div class="sc-foot"><span class="sc-price">~15€</span><button class="sc-btn" onclick="orderP('Parfum Cuir & Luxe')" style="border-color:rgba(245,158,11,.28);color:var(--gold)">Commander →</button></div></div></div>
    <div class="sc" data-a style="transition-delay:.21s"><div class="sc-img">🌊<span class="sc-brand-tag">SpeedClean</span></div><div class="sc-body"><p class="sc-br">SpeedClean Auto</p><p class="sc-name">Pack Océan & Frais</p><p class="sc-desc">Duo spray + désodorisant ventilation. Parfait entre deux nettoyages.</p><div class="sc-foot"><span class="sc-price">~18€</span><button class="sc-btn" onclick="orderP('Pack Océan & Frais')">Commander →</button></div></div></div>
  </div>
  <div class="cstrip">📞 <a href="tel:0772355354">07 72 35 53 54</a> · ✉️ <a href="mailto:autoclean9560@gmail.com">autoclean9560@gmail.com</a></div>
  <div class="soc-row">
    <a href="https://www.instagram.com/speedcleanauto_6095" target="_blank" class="soc">📸 @speedcleanauto_6095</a>
    <a href="https://www.snapchat.com/add/speedcleanauto_6095" target="_blank" class="soc">👻 @speedcleanauto_6095</a>
    <span class="soc" style="opacity:.5;cursor:default">🎵 TikTok bientôt actif</span>
  </div>
</div>

<!-- FOOTER -->
<footer>
  <div class="footer-g">
    <div><div class="f-bn">SPEED<b>CLEAN</b> AUTO</div><div class="f-tag">La propreté qui fait la différence.</div></div>
    <div class="f-links">
      <a href="#" onclick="goTab('tarifs');return false">Formules & Tarifs</a>
      <a href="#" onclick="goTab('rdv');return false">Prendre RDV</a>
      <a href="#" onclick="goTab('shop');return false">Boutique</a>
    </div>
    <div class="f-links">
      <a href="tel:0772355354">📞 07 72 35 53 54</a>
      <a href="mailto:autoclean9560@gmail.com">✉️ autoclean9560@gmail.com</a>
      <a href="https://www.instagram.com/speedcleanauto_6095" target="_blank">📸 Instagram</a>
      <a href="https://www.snapchat.com/add/speedcleanauto_6095" target="_blank">👻 Snapchat</a>
    </div>
  </div>
  <div class="footer-bot">
    <span>© 2025 SpeedClean Auto · Secteur 60/95</span>
    <a href="https://search.google.com/local/writereview" target="_blank" class="g-btn">⭐ Laisser un avis Google</a>
  </div>
</footer>

<a href="tel:0772355354" class="fab-call">📞 Appeler</a>
<button class="fab-rdv" onclick="goTab('rdv')">📅 Réserver</button>

<script>
// ══════════════════════════════════════════════
// CONFIG
// ══════════════════════════════════════════════
var PROMO = true; // false apres le 20 juin
var P = {
  basic:   {cit:PROMO?15:25,suv:PROMO?20:30,ber:PROMO?20:30,van:PROMO?25:35},
  confort: {cit:PROMO?30:40,suv:PROMO?35:45,ber:PROMO?35:45,van:PROMO?40:55},
  premium: {cit:PROMO?50:70,suv:PROMO?55:75,ber:PROMO?55:75,van:PROMO?60:80},
  opt: PROMO?5:10
};
var N = {
  basic:   {cit:25,suv:30,ber:30,van:35},
  confort: {cit:40,suv:45,ber:45,van:55},
  premium: {cit:70,suv:75,ber:75,van:80}
};
var FS = "https://formspree.io/f/mnjlplnd";

// ══════════════════════════════════════════════
// VEHICLE DATABASE — Europe complète
// Format: {n: nom, c: catégorie, y: années, ph: phases}
// c = cit / suv / ber / van
// ══════════════════════════════════════════════
var VDB = [
// ── PEUGEOT ──
{n:"Peugeot 108",c:"cit",y:"2014-2021"},{n:"Peugeot 205",c:"cit",y:"1983-1998"},
{n:"Peugeot 206",c:"cit",y:"1998-2013"},{n:"Peugeot 207",c:"cit",y:"2006-2014"},
{n:"Peugeot 208 Ph.1",c:"cit",y:"2012-2019"},{n:"Peugeot 208 Ph.2",c:"cit",y:"2019-présent"},
{n:"Peugeot 301",c:"ber",y:"2012-présent"},{n:"Peugeot 308 Ph.1",c:"ber",y:"2013-2018"},
{n:"Peugeot 308 Ph.2",c:"ber",y:"2018-2022"},{n:"Peugeot 308 Ph.3",c:"ber",y:"2022-présent"},
{n:"Peugeot 408",c:"suv",y:"2022-présent"},{n:"Peugeot 508 Ph.1",c:"ber",y:"2018-2020"},
{n:"Peugeot 508 Ph.2",c:"ber",y:"2020-présent"},{n:"Peugeot 2008 Ph.1",c:"suv",y:"2013-2020"},
{n:"Peugeot 2008 Ph.2",c:"suv",y:"2020-présent"},{n:"Peugeot 3008 Ph.1",c:"suv",y:"2016-2020"},
{n:"Peugeot 3008 Ph.2",c:"suv",y:"2020-présent"},{n:"Peugeot 5008 Ph.1",c:"van",y:"2009-2017"},
{n:"Peugeot 5008 Ph.2",c:"suv",y:"2017-présent"},{n:"Peugeot Rifter",c:"van",y:"2018-présent"},
{n:"Peugeot Partner",c:"van",y:"1996-présent"},
// ── RENAULT ──
{n:"Renault Twingo 2",c:"cit",y:"2007-2014"},{n:"Renault Twingo 3",c:"cit",y:"2014-présent"},
{n:"Renault Clio 2",c:"cit",y:"1998-2006"},{n:"Renault Clio 3",c:"cit",y:"2005-2012"},
{n:"Renault Clio 4",c:"cit",y:"2012-2019"},{n:"Renault Clio 5",c:"cit",y:"2019-présent"},
{n:"Renault Zoe Ph.1",c:"cit",y:"2012-2019"},{n:"Renault Zoe Ph.2",c:"cit",y:"2019-présent"},
{n:"Renault Megane 3",c:"ber",y:"2008-2016"},{n:"Renault Megane 4",c:"ber",y:"2016-présent"},
{n:"Renault Megane E-Tech",c:"suv",y:"2022-présent"},{n:"Renault Captur Ph.1",c:"suv",y:"2013-2020"},
{n:"Renault Captur Ph.2",c:"suv",y:"2020-présent"},{n:"Renault Kadjar",c:"suv",y:"2015-2022"},
{n:"Renault Scenic 3",c:"van",y:"2009-2016"},{n:"Renault Scenic 4",c:"van",y:"2016-présent"},
{n:"Renault Koleos Ph.2",c:"suv",y:"2016-présent"},{n:"Renault Austral",c:"suv",y:"2022-présent"},
{n:"Renault Rafale",c:"suv",y:"2023-présent"},{n:"Renault Espace 5",c:"suv",y:"2023-présent"},
{n:"Renault Talisman",c:"ber",y:"2016-2022"},{n:"Renault Laguna 3",c:"ber",y:"2007-2015"},
{n:"Renault Kangoo 3",c:"van",y:"2021-présent"},{n:"Renault Lodgy",c:"van",y:"2012-présent"},
// ── CITROEN ──
{n:"Citroen C1",c:"cit",y:"2005-2022"},{n:"Citroen C2",c:"cit",y:"2003-2009"},
{n:"Citroen C3 Ph.1",c:"cit",y:"2002-2009"},{n:"Citroen C3 Ph.2",c:"cit",y:"2009-2017"},
{n:"Citroen C3 Ph.3",c:"cit",y:"2017-présent"},{n:"Citroen C3 Aircross",c:"suv",y:"2017-présent"},
{n:"Citroen C4 Ph.1",c:"ber",y:"2004-2011"},{n:"Citroen C4 Ph.2",c:"ber",y:"2020-présent"},
{n:"Citroen C4 Cactus",c:"suv",y:"2014-2020"},{n:"Citroen C5 Aircross",c:"suv",y:"2018-présent"},
{n:"Citroen C5 X",c:"suv",y:"2022-présent"},{n:"Citroen Berlingo 3",c:"van",y:"2018-présent"},
{n:"Citroen Grand C4 Picasso",c:"van",y:"2014-présent"},{n:"Citroen Ami",c:"cit",y:"2020-présent"},
// ── DS ──
{n:"DS 3 Ph.1",c:"cit",y:"2010-2019"},{n:"DS 3 Crossback",c:"suv",y:"2019-présent"},
{n:"DS 4",c:"suv",y:"2021-présent"},{n:"DS 7 Crossback",c:"suv",y:"2018-présent"},
{n:"DS 9",c:"ber",y:"2021-présent"},
// ── VOLKSWAGEN ──
{n:"VW Polo 5",c:"cit",y:"2009-2017"},{n:"VW Polo 6",c:"cit",y:"2017-présent"},
{n:"VW Up",c:"cit",y:"2011-présent"},{n:"VW Golf 6",c:"ber",y:"2008-2013"},
{n:"VW Golf 7",c:"ber",y:"2013-2020"},{n:"VW Golf 7.5",c:"ber",y:"2017-2020"},
{n:"VW Golf 8",c:"ber",y:"2020-présent"},{n:"VW Golf SW",c:"ber",y:"2013-présent"},
{n:"VW Passat B8",c:"ber",y:"2015-présent"},{n:"VW Tiguan 1",c:"suv",y:"2007-2016"},
{n:"VW Tiguan 2",c:"suv",y:"2016-présent"},{n:"VW T-Roc",c:"suv",y:"2017-présent"},
{n:"VW T-Cross",c:"suv",y:"2019-présent"},{n:"VW Touareg 3",c:"suv",y:"2018-présent"},
{n:"VW Arteon",c:"ber",y:"2017-présent"},{n:"VW ID.3",c:"cit",y:"2020-présent"},
{n:"VW ID.4",c:"suv",y:"2021-présent"},{n:"VW ID.5",c:"suv",y:"2022-présent"},
{n:"VW Touran",c:"van",y:"2006-présent"},{n:"VW Sharan",c:"van",y:"1995-2022"},
{n:"VW Caddy",c:"van",y:"2003-présent"},
// ── SEAT / CUPRA ──
{n:"Seat Ibiza 5",c:"cit",y:"2017-présent"},{n:"Seat Arona",c:"suv",y:"2017-présent"},
{n:"Seat Leon 3",c:"ber",y:"2013-2020"},{n:"Seat Leon 4",c:"ber",y:"2020-présent"},
{n:"Seat Ateca",c:"suv",y:"2016-présent"},{n:"Seat Tarraco",c:"suv",y:"2018-présent"},
{n:"Cupra Born",c:"cit",y:"2021-présent"},{n:"Cupra Formentor",c:"suv",y:"2021-présent"},
{n:"Cupra Ateca",c:"suv",y:"2018-présent"},
// ── SKODA ──
{n:"Skoda Fabia 3",c:"cit",y:"2014-2021"},{n:"Skoda Fabia 4",c:"cit",y:"2021-présent"},
{n:"Skoda Octavia 3",c:"ber",y:"2012-2020"},{n:"Skoda Octavia 4",c:"ber",y:"2020-présent"},
{n:"Skoda Superb 3",c:"ber",y:"2015-présent"},{n:"Skoda Karoq",c:"suv",y:"2017-présent"},
{n:"Skoda Kodiaq",c:"suv",y:"2017-présent"},{n:"Skoda Enyaq",c:"suv",y:"2021-présent"},
// ── OPEL / VAUXHALL ──
{n:"Opel Corsa E",c:"cit",y:"2014-2019"},{n:"Opel Corsa F",c:"cit",y:"2019-présent"},
{n:"Opel Adam",c:"cit",y:"2013-2019"},{n:"Opel Astra K",c:"ber",y:"2015-2022"},
{n:"Opel Astra L",c:"ber",y:"2022-présent"},{n:"Opel Mokka A",c:"suv",y:"2012-2019"},
{n:"Opel Mokka B",c:"suv",y:"2021-présent"},{n:"Opel Grandland X",c:"suv",y:"2017-présent"},
{n:"Opel Insignia B",c:"ber",y:"2017-présent"},{n:"Opel Zafira Life",c:"van",y:"2019-présent"},
{n:"Opel Crossland",c:"suv",y:"2017-présent"},
// ── BMW ──
{n:"BMW Serie 1 F20",c:"ber",y:"2011-2019"},{n:"BMW Serie 1 F40",c:"ber",y:"2019-présent"},
{n:"BMW Serie 2 F22",c:"ber",y:"2013-présent"},{n:"BMW Serie 2 Gran Tourer",c:"van",y:"2015-présent"},
{n:"BMW Serie 3 F30",c:"ber",y:"2012-2019"},{n:"BMW Serie 3 G20",c:"ber",y:"2019-présent"},
{n:"BMW Serie 4 G22",c:"ber",y:"2021-présent"},{n:"BMW Serie 5 G30",c:"ber",y:"2017-présent"},
{n:"BMW Serie 7 G11",c:"ber",y:"2016-présent"},{n:"BMW X1 F48",c:"suv",y:"2015-2022"},
{n:"BMW X1 U11",c:"suv",y:"2022-présent"},{n:"BMW X2",c:"suv",y:"2018-présent"},
{n:"BMW X3 G01",c:"suv",y:"2018-présent"},{n:"BMW X4 G02",c:"suv",y:"2018-présent"},
{n:"BMW X5 G05",c:"suv",y:"2018-présent"},{n:"BMW X6 G06",c:"suv",y:"2019-présent"},
{n:"BMW X7",c:"suv",y:"2019-présent"},{n:"BMW iX",c:"suv",y:"2021-présent"},
{n:"BMW iX3",c:"suv",y:"2020-présent"},
// ── MERCEDES ──
{n:"Mercedes Classe A W176",c:"ber",y:"2012-2018"},{n:"Mercedes Classe A W177",c:"ber",y:"2018-présent"},
{n:"Mercedes Classe B W247",c:"van",y:"2019-présent"},{n:"Mercedes Classe C W205",c:"ber",y:"2014-2021"},
{n:"Mercedes Classe C W206",c:"ber",y:"2021-présent"},{n:"Mercedes Classe E W213",c:"ber",y:"2016-présent"},
{n:"Mercedes Classe S W222",c:"ber",y:"2014-2020"},{n:"Mercedes Classe S W223",c:"ber",y:"2021-présent"},
{n:"Mercedes GLA H247",c:"suv",y:"2020-présent"},{n:"Mercedes GLB",c:"suv",y:"2019-présent"},
{n:"Mercedes GLC X254",c:"suv",y:"2022-présent"},{n:"Mercedes GLE V167",c:"suv",y:"2019-présent"},
{n:"Mercedes GLS",c:"suv",y:"2019-présent"},{n:"Mercedes EQC",c:"suv",y:"2019-présent"},
{n:"Mercedes EQA",c:"suv",y:"2021-présent"},{n:"Mercedes EQB",c:"suv",y:"2022-présent"},
{n:"Mercedes EQS",c:"ber",y:"2021-présent"},
// ── AUDI ──
{n:"Audi A1 GB",c:"cit",y:"2018-présent"},{n:"Audi A3 8V",c:"ber",y:"2012-2020"},
{n:"Audi A3 8Y",c:"ber",y:"2020-présent"},{n:"Audi A4 B9",c:"ber",y:"2016-présent"},
{n:"Audi A5 F5",c:"ber",y:"2016-présent"},{n:"Audi A6 C8",c:"ber",y:"2018-présent"},
{n:"Audi A7 C8",c:"ber",y:"2018-présent"},{n:"Audi A8 D5",c:"ber",y:"2018-présent"},
{n:"Audi Q2",c:"suv",y:"2016-présent"},{n:"Audi Q3 F3",c:"suv",y:"2019-présent"},
{n:"Audi Q4 e-tron",c:"suv",y:"2021-présent"},{n:"Audi Q5 FY",c:"suv",y:"2017-présent"},
{n:"Audi Q7 4M",c:"suv",y:"2015-présent"},{n:"Audi Q8",c:"suv",y:"2018-présent"},
{n:"Audi e-tron 55",c:"suv",y:"2019-présent"},
// ── FORD ──
{n:"Ford Fiesta 7",c:"cit",y:"2017-2022"},{n:"Ford Ka+",c:"cit",y:"2016-2021"},
{n:"Ford Focus 4",c:"ber",y:"2018-présent"},{n:"Ford Kuga 3",c:"suv",y:"2020-présent"},
{n:"Ford Mustang Mach-E",c:"suv",y:"2021-présent"},{n:"Ford Explorer",c:"suv",y:"2019-présent"},
{n:"Ford Edge",c:"suv",y:"2016-présent"},{n:"Ford Galaxy",c:"van",y:"2006-présent"},
{n:"Ford S-Max",c:"van",y:"2006-présent"},{n:"Ford Tourneo Connect",c:"van",y:"2022-présent"},
// ── FIAT ──
{n:"Fiat 500 Classic",c:"cit",y:"2007-2019"},{n:"Fiat 500 Restyling",c:"cit",y:"2015-2023"},
{n:"Fiat 500e",c:"cit",y:"2020-présent"},{n:"Fiat Panda 4",c:"cit",y:"2011-présent"},
{n:"Fiat Tipo",c:"ber",y:"2016-présent"},{n:"Fiat 500X",c:"suv",y:"2015-présent"},
{n:"Fiat 500L",c:"van",y:"2012-présent"},
// ── ALFA ROMEO ──
{n:"Alfa Romeo MiTo",c:"cit",y:"2008-2018"},{n:"Alfa Romeo Giulietta",c:"ber",y:"2010-2020"},
{n:"Alfa Romeo Giulia",c:"ber",y:"2016-présent"},{n:"Alfa Romeo Stelvio",c:"suv",y:"2017-présent"},
{n:"Alfa Romeo Tonale",c:"suv",y:"2022-présent"},
// ── LANCIA ──
{n:"Lancia Ypsilon",c:"cit",y:"2011-présent"},
// ── TOYOTA ──
{n:"Toyota Aygo X",c:"cit",y:"2022-présent"},{n:"Toyota Yaris 4",c:"cit",y:"2020-présent"},
{n:"Toyota Yaris 3",c:"cit",y:"2011-2020"},{n:"Toyota Yaris Cross",c:"suv",y:"2021-présent"},
{n:"Toyota C-HR Ph.1",c:"suv",y:"2016-2023"},{n:"Toyota C-HR Ph.2",c:"suv",y:"2023-présent"},
{n:"Toyota RAV4 5",c:"suv",y:"2019-présent"},{n:"Toyota Corolla",c:"ber",y:"2019-présent"},
{n:"Toyota Camry",c:"ber",y:"2019-présent"},{n:"Toyota Land Cruiser",c:"suv",y:"2021-présent"},
{n:"Toyota Hilux",c:"suv",y:"2015-présent"},{n:"Toyota Prius 4",c:"ber",y:"2016-présent"},
{n:"Toyota bZ4X",c:"suv",y:"2022-présent"},{n:"Toyota Verso",c:"van",y:"2009-2018"},
// ── NISSAN ──
{n:"Nissan Micra 5",c:"cit",y:"2017-2022"},{n:"Nissan Juke Ph.1",c:"suv",y:"2010-2019"},
{n:"Nissan Juke Ph.2",c:"suv",y:"2019-présent"},{n:"Nissan Qashqai J11",c:"suv",y:"2013-2021"},
{n:"Nissan Qashqai J12",c:"suv",y:"2021-présent"},{n:"Nissan X-Trail T32",c:"suv",y:"2014-2022"},
{n:"Nissan X-Trail T33",c:"suv",y:"2022-présent"},{n:"Nissan Leaf 2",c:"cit",y:"2017-présent"},
{n:"Nissan Ariya",c:"suv",y:"2022-présent"},
// ── HYUNDAI ──
{n:"Hyundai i10 3",c:"cit",y:"2020-présent"},{n:"Hyundai i20 3",c:"cit",y:"2020-présent"},
{n:"Hyundai i30 3",c:"ber",y:"2017-présent"},{n:"Hyundai Kona Ph.1",c:"suv",y:"2017-2023"},
{n:"Hyundai Kona Ph.2",c:"suv",y:"2023-présent"},{n:"Hyundai Tucson 4",c:"suv",y:"2020-présent"},
{n:"Hyundai Santa Fe 4",c:"suv",y:"2018-présent"},{n:"Hyundai Ioniq 5",c:"suv",y:"2021-présent"},
{n:"Hyundai Ioniq 6",c:"ber",y:"2022-présent"},
// ── KIA ──
{n:"Kia Picanto 3",c:"cit",y:"2017-présent"},{n:"Kia Rio 4",c:"cit",y:"2017-présent"},
{n:"Kia Ceed 3",c:"ber",y:"2018-présent"},{n:"Kia XCeed",c:"suv",y:"2019-présent"},
{n:"Kia Sportage 5",c:"suv",y:"2021-présent"},{n:"Kia Sorento 4",c:"suv",y:"2020-présent"},
{n:"Kia Stinger",c:"ber",y:"2017-présent"},{n:"Kia EV6",c:"suv",y:"2021-présent"},
{n:"Kia Niro 2",c:"suv",y:"2022-présent"},
// ── HONDA ──
{n:"Honda Jazz 4",c:"cit",y:"2020-présent"},{n:"Honda Civic 11",c:"ber",y:"2022-présent"},
{n:"Honda HR-V 3",c:"suv",y:"2022-présent"},{n:"Honda CR-V 6",c:"suv",y:"2023-présent"},
{n:"Honda e",c:"cit",y:"2020-présent"},
// ── MAZDA ──
{n:"Mazda 2 DJ",c:"cit",y:"2015-présent"},{n:"Mazda 3 BP",c:"ber",y:"2019-présent"},
{n:"Mazda 6 GJ",c:"ber",y:"2012-présent"},{n:"Mazda CX-3",c:"suv",y:"2015-présent"},
{n:"Mazda CX-30",c:"suv",y:"2019-présent"},{n:"Mazda CX-5 KF",c:"suv",y:"2017-présent"},
{n:"Mazda CX-60",c:"suv",y:"2022-présent"},{n:"Mazda MX-30",c:"suv",y:"2020-présent"},
// ── MITSUBISHI ──
{n:"Mitsubishi Space Star",c:"cit",y:"2013-présent"},{n:"Mitsubishi ASX Ph.2",c:"suv",y:"2023-présent"},
{n:"Mitsubishi Eclipse Cross",c:"suv",y:"2018-présent"},{n:"Mitsubishi Outlander 3",c:"suv",y:"2012-présent"},
// ── SUZUKI ──
{n:"Suzuki Swift 5",c:"cit",y:"2017-présent"},{n:"Suzuki Ignis",c:"cit",y:"2016-présent"},
{n:"Suzuki S-Cross",c:"suv",y:"2013-présent"},{n:"Suzuki Vitara",c:"suv",y:"2015-présent"},
// ── DACIA ──
{n:"Dacia Sandero 3",c:"cit",y:"2021-présent"},{n:"Dacia Logan 3",c:"ber",y:"2021-présent"},
{n:"Dacia Duster 2",c:"suv",y:"2018-présent"},{n:"Dacia Jogger",c:"van",y:"2021-présent"},
{n:"Dacia Spring",c:"cit",y:"2021-présent"},{n:"Dacia Bigster",c:"suv",y:"2025-présent"},
// ── VOLVO ──
{n:"Volvo V40",c:"ber",y:"2012-2019"},{n:"Volvo V60 Ph.2",c:"ber",y:"2018-présent"},
{n:"Volvo V90",c:"ber",y:"2016-présent"},{n:"Volvo XC40",c:"suv",y:"2018-présent"},
{n:"Volvo XC60 Ph.2",c:"suv",y:"2017-présent"},{n:"Volvo XC90 Ph.2",c:"suv",y:"2015-présent"},
{n:"Volvo C40 Recharge",c:"suv",y:"2022-présent"},
// ── MINI ──
{n:"Mini 3 portes F56",c:"cit",y:"2014-présent"},{n:"Mini Clubman F54",c:"ber",y:"2015-présent"},
{n:"Mini Countryman F60",c:"suv",y:"2017-présent"},{n:"Mini Countryman U25",c:"suv",y:"2024-présent"},
{n:"Mini Cabrio",c:"cit",y:"2016-présent"},
// ── LAND ROVER / RANGE ROVER ──
{n:"Range Rover Evoque L551",c:"suv",y:"2019-présent"},{n:"Range Rover Velar",c:"suv",y:"2017-présent"},
{n:"Range Rover Sport 3",c:"suv",y:"2022-présent"},{n:"Range Rover 5",c:"suv",y:"2022-présent"},
{n:"Land Rover Defender 90",c:"suv",y:"2020-présent"},{n:"Land Rover Defender 110",c:"suv",y:"2020-présent"},
{n:"Land Rover Discovery 5",c:"suv",y:"2017-présent"},{n:"Land Rover Discovery Sport",c:"suv",y:"2015-présent"},
// ── JEEP ──
{n:"Jeep Renegade",c:"suv",y:"2014-présent"},{n:"Jeep Compass 2",c:"suv",y:"2017-présent"},
{n:"Jeep Avenger",c:"suv",y:"2023-présent"},{n:"Jeep Wrangler 4xe",c:"suv",y:"2021-présent"},
// ── TESLA ──
{n:"Tesla Model 3",c:"ber",y:"2017-présent"},{n:"Tesla Model Y",c:"suv",y:"2020-présent"},
{n:"Tesla Model S",c:"ber",y:"2012-présent"},{n:"Tesla Model X",c:"suv",y:"2015-présent"},
// ── PORSCHE ──
{n:"Porsche Macan 1",c:"suv",y:"2013-présent"},{n:"Porsche Cayenne 3",c:"suv",y:"2018-présent"},
{n:"Porsche Panamera 2",c:"ber",y:"2017-présent"},{n:"Porsche Taycan",c:"ber",y:"2020-présent"},
// ── LEXUS ──
{n:"Lexus UX",c:"suv",y:"2019-présent"},{n:"Lexus NX Ph.2",c:"suv",y:"2022-présent"},
{n:"Lexus RX 5",c:"suv",y:"2023-présent"},{n:"Lexus ES",c:"ber",y:"2018-présent"},
// ── SUBARU ──
{n:"Subaru XV 2",c:"suv",y:"2017-présent"},{n:"Subaru Forester 5",c:"suv",y:"2018-présent"},
{n:"Subaru Outback 6",c:"ber",y:"2021-présent"},{n:"Subaru Solterra",c:"suv",y:"2022-présent"},
// ── POLESTAR ──
{n:"Polestar 2",c:"ber",y:"2020-présent"},{n:"Polestar 4",c:"suv",y:"2024-présent"},
// ── AUTRES EUROPÉENS ──
{n:"Lynk Co 01",c:"suv",y:"2021-présent"},{n:"MG ZS 2",c:"suv",y:"2021-présent"},
{n:"MG4",c:"ber",y:"2022-présent"},{n:"BYD Atto 3",c:"suv",y:"2022-présent"},
{n:"BYD Seal",c:"ber",y:"2023-présent"},{n:"BYD Dolphin",c:"cit",y:"2023-présent"},
{n:"Smart #1",c:"suv",y:"2022-présent"},{n:"Smart #3",c:"suv",y:"2023-présent"},
// ── ESPAGNE / SEAT extras ──
{n:"Seat Mii",c:"cit",y:"2012-2019"},
// ── SUISSE / ALL / BE extras ──
{n:"VW Amarok",c:"suv",y:"2010-présent"},{n:"Mercedes Classe G",c:"suv",y:"2018-présent"},
{n:"BMW M3 G80",c:"ber",y:"2021-présent"},{n:"BMW M5",c:"ber",y:"2018-présent"},
{n:"Audi RS6",c:"ber",y:"2019-présent"},{n:"Audi RS3",c:"ber",y:"2022-présent"}
];

// Specs database (sampled — shown in info panel)
var SPECS = {
  "Peugeot 208 Ph.2":    {Longueur:"4,06m",Largeur:"1,75m",Type:"Citadine",Places:"5",Coffre:"311L",Catégorie:"A"},
  "Peugeot 3008 Ph.2":   {Longueur:"4,45m",Largeur:"1,84m",Type:"SUV",Places:"5",Coffre:"520L",Catégorie:"SUV compact"},
  "Renault Clio 5":      {Longueur:"4,05m",Largeur:"1,80m",Type:"Citadine",Places:"5",Coffre:"391L",Catégorie:"B"},
  "Volkswagen Golf 8":   {Longueur:"4,28m",Largeur:"1,79m",Type:"Berline",Places:"5",Coffre:"380L",Catégorie:"C"},
  "BMW X5 G05":          {Longueur:"4,92m",Largeur:"2,00m",Type:"SUV",Places:"5-7",Coffre:"650L",Catégorie:"SUV grand"},
  "Tesla Model 3":       {Longueur:"4,69m",Largeur:"1,85m",Type:"Berline",Places:"5",Coffre:"425L+88L",Catégorie:"D"},
};

// Demo models for cards
var DEMO = {
  cit:{ basic:["Peugeot 108","Renault Twingo","VW Polo 6","Toyota Aygo"],   confort:["Peugeot 208","Renault Clio 5","Opel Corsa F","Hyundai i20"], premium:["Mini Cooper","Renault Clio 5","Peugeot 208 Ph.2","Citroen C3"] },
  suv:{ basic:["Peugeot 2008","Renault Captur","Dacia Duster","Nissan Juke"],confort:["Peugeot 3008","VW Tiguan","BMW X1","Toyota RAV4"],            premium:["BMW X5","Mercedes GLE","Audi Q7","Porsche Cayenne"] },
  ber:{ basic:["Renault Megane","VW Golf","Opel Astra","Ford Focus"],        confort:["BMW Serie 3","Mercedes Classe C","Audi A4","Skoda Octavia"],  premium:["BMW Serie 5","Mercedes Classe E","Audi A6","Tesla Model 3"] },
  van:{ basic:["Peugeot Rifter","Citroen Berlingo","Dacia Jogger","VW Touran"],confort:["Peugeot 5008","Ford S-Max","Renault Scenic","VW Sharan"],    premium:["Mercedes Classe V","VW Multivan","Citroen SpaceTourer","Ford Galaxy"] }
};

// ══════════════════════════════════════════════
// STATE
// ══════════════════════════════════════════════
var carType = "cit";
var selF    = null;
var optOn   = false;
var vehSel  = null;
var gIdx    = 0;
var gTotal  = 4;
var specOpen = false;

// ══════════════════════════════════════════════
// TABS
// ══════════════════════════════════════════════
function goTab(id) {
  document.querySelectorAll(".page").forEach(function(p){p.classList.remove("active")});
  document.querySelectorAll(".tab-btn").forEach(function(b){b.classList.remove("active")});
  document.getElementById("page-"+id).classList.add("active");
  document.getElementById("tab-"+id).classList.add("active");
  window.scrollTo({top:0,behavior:"smooth"});
}

// ══════════════════════════════════════════════
// SEARCH
// ══════════════════════════════════════════════
function doS(val, dropId, mode) {
  var drop = document.getElementById(dropId);
  if(!val||val.length<2){drop.classList.remove("open");return}
  var q = val.toLowerCase();
  var res = VDB.filter(function(v){
    return v.n.toLowerCase().indexOf(q)!==-1 || (v.y && v.y.indexOf(q)!==-1);
  }).slice(0,16);
  if(!res.length){drop.classList.remove("open");return}
  drop.innerHTML = res.map(function(v){
    var catMap = {cit:"Citadine",suv:"SUV",ber:"Berline/Break",van:"Van"};
    return '<div class="sdi vi2" onclick="selVeh(\''+v.n.replace(/'/g,"\\'")+'\',\''+v.c+'\',\''+mode+'\',\''+v.y+'\')">'+
      '<span>'+v.n+' <span class="sdi-year">'+v.y+'</span></span>'+
      '<span class="sdi-cat '+v.c+'">'+catMap[v.c]+'</span></div>';
  }).join("");
  drop.classList.add("open");
}

function selVeh(name, cat, mode, year) {
  if(mode==="pill"){
    document.getElementById("mainS").value = name;
    document.getElementById("mDrop").classList.remove("open");
    setPill(cat);
    showViewer(name, cat, year);
  } else {
    document.getElementById("r-veh").value = name + (year?" ("+year+")":"");
    document.getElementById("vDrop").classList.remove("open");
    vehSel = {n:name,c:cat,y:year};
    var catMap = {cit:"🟢 Citadine",suv:"🔵 SUV",ber:"🟣 Berline/Break",van:"🟠 Van"};
    var det = document.getElementById("detType");
    det.textContent = catMap[cat] + " — tarif adapté";
    det.style.display = "block";
    document.getElementById("manFg").style.display = "none";
    document.getElementById("r-vt").value = cat==="ber"?"ber":cat==="van"?"van":cat;
    updSum();
  }
}

// ══════════════════════════════════════════════
// VEHICLE VIEWER
// ══════════════════════════════════════════════
function showViewer(name, cat, year) {
  var vv = document.getElementById("vehViewer");
  vv.classList.add("show");
  document.getElementById("vvName").textContent = name;
  var catMap = {cit:"Citadine",suv:"SUV / Crossover",ber:"Berline / Break",van:"Monospace / Van"};
  var catCls = {cit:"cat-cit",suv:"cat-suv",ber:"cat-ber",van:"cat-van"};
  var catBadge = document.getElementById("vvCat");
  catBadge.textContent = catMap[cat]||cat;
  catBadge.className = "vv-cat-badge " + (cat==="cit"?"cat-cit":cat==="suv"?"cat-suv":cat==="ber"?"tgo":"tgo");
  catBadge.style.cssText = "font-size:.6rem;font-weight:600;letter-spacing:1.5px;text-transform:uppercase;padding:3px 9px;border-radius:4px;background:rgba(59,130,246,.1);color:#93c5fd;border:1px solid rgba(59,130,246,.2)";

  buildGallery(name);

  // Specs
  var specs = SPECS[name] || buildAutoSpecs(name, cat);
  var sg = document.getElementById("specsGrid");
  sg.innerHTML = Object.keys(specs).map(function(k){
    return '<div class="spec-item"><p class="spec-label">'+k+'</p><p class="spec-value">'+specs[k]+'</p></div>';
  }).join("");
}

function buildAutoSpecs(name, cat) {
  var catSizes = {
    cit:{L:"3,8–4,1m",l:"1,7–1,8m",co:"300–380L",pl:"5"},
    suv:{L:"4,2–4,7m",l:"1,8–1,9m",co:"400–650L",pl:"5–7"},
    ber:{L:"4,3–4,8m",l:"1,8–1,9m",co:"370–520L",pl:"5"},
    van:{L:"4,3–4,8m",l:"1,8–2,0m",co:"500–1000L",pl:"5–7"}
  };
  var s = catSizes[cat]||catSizes.ber;
  return {Longueur:s.L,Largeur:s.l,Places:s.pl,Coffre:s.co,Catégorie:cat==="cit"?"Citadine":cat==="suv"?"SUV":cat==="van"?"Van":"Berline"};
}

function buildGallery(name) {
  var gs = document.getElementById("gallerySlide");
  gs.querySelectorAll(".g-slide").forEach(function(s){s.remove()});
  var views = ["Front","Side","Rear","Interior"];
  var labels = ["Vue avant","Profil côté","Vue arrière","Habitacle"];
  gTotal = views.length;
  gIdx = 0;

  views.forEach(function(v,i){
    var slide = document.createElement("div");
    slide.className = "g-slide" + (i===0?" active":"");

    // Try real photo from Unsplash with car+name keywords
    var seed = Math.abs(hashStr(name+i)) % 800 + 100;
    var kws  = ["car+front+exterior+road","car+side+view+outdoor","car+rear+view","car+interior+seats+dashboard"];
    var imgUrl = "https://source.unsplash.com/900x450/?" + kws[i] + "&sig=" + seed;

    var img = document.createElement("img");
    img.alt = name + " " + labels[i];
    img.style.cssText = "width:100%;height:100%;object-fit:cover;position:absolute;inset:0;";
    var fb = document.createElement("div");
    fb.className = "g-fallback";
    fb.innerHTML = '<span class="gf-emoji">🚗</span>'
      + '<span class="gf-name">'+name+'</span>'
      + '<span class="gf-view">'+labels[i]+'</span>';
    img.onload = function(){fb.style.display="none"};
    img.onerror = function(){img.style.display="none";fb.style.display="flex"};
    img.src = imgUrl;

    slide.style.position = "relative";
    slide.appendChild(img);
    slide.appendChild(fb);

    var prevBtn = gs.querySelector(".g-prev");
    gs.insertBefore(slide, prevBtn);
  });

  var dots = document.getElementById("gDots");
  dots.innerHTML = views.map(function(v,i){
    return '<div class="g-dot'+(i===0?" active":"") + '" onclick="goSlide('+i+')"></div>';
  }).join("");

  clearInterval(window._gt);
  window._gt = setInterval(function(){gNav(1)},4200);
}

function hashStr(s){var h=0;for(var i=0;i<s.length;i++){h=((h<<5)-h)+s.charCodeAt(i);h|=0}return h}

function gNav(dir){
  var slides = document.querySelectorAll("#gallerySlide .g-slide");
  var dots   = document.querySelectorAll("#gDots .g-dot");
  if(!slides.length)return;
  slides[gIdx].classList.remove("active");
  if(dots[gIdx])dots[gIdx].classList.remove("active");
  gIdx=(gIdx+dir+gTotal)%gTotal;
  slides[gIdx].classList.add("active");
  if(dots[gIdx])dots[gIdx].classList.add("active");
}

function goSlide(i){
  var slides=document.querySelectorAll("#gallerySlide .g-slide");
  var dots=document.querySelectorAll("#gDots .g-dot");
  if(!slides.length)return;
  slides[gIdx].classList.remove("active");
  if(dots[gIdx])dots[gIdx].classList.remove("active");
  gIdx=i;
  slides[gIdx].classList.add("active");
  if(dots[gIdx])dots[gIdx].classList.add("active");
}

function setMode(m){ /* only gallery for now */ }

function toggleSpecs(){
  specOpen = !specOpen;
  var sp = document.getElementById("vvSpecs");
  sp.classList.toggle("show", specOpen);
  document.getElementById("btnSpecs").classList.toggle("active", specOpen);
}

// ══════════════════════════════════════════════
// PILLS & CARDS
// ══════════════════════════════════════════════
function setPill(type){
  carType = type;
  ["cit","suv","ber","van"].forEach(function(t){
    document.getElementById("p-"+t).className = "type-pill" + (t===type?" a-"+type:"");
  });
  renderCards();
}

function pHtml(f,t){
  var p=P[f][t]||P[f].cit, nn=N[f][t]||N[f].cit;
  if(PROMO) return '<span class="pold">'+nn+'€</span><span class="pnew">'+p+'€</span>';
  return p+"€";
}

function renderCards(){
  var t=carType;
  var lblMap={cit:"Citadine",suv:"SUV / Crossover",ber:"Berline / Break",van:"Monospace / Van"};
  var lbl=lblMap[t]||"Citadine";
  ["basic","confort","premium"].forEach(function(f){
    var short={basic:"b",confort:"c",premium:"p"}[f];
    document.getElementById(short+"-lbl").textContent=lbl;
    document.getElementById(short+"-val").innerHTML=pHtml(f,t);
    document.getElementById(short+"-tags").innerHTML=
      (DEMO[t]||DEMO.cit)[f].map(function(m){return'<span class="m-tag">'+m+'</span>'}).join("");
  });
  var op=document.getElementById("optP");
  if(PROMO) op.innerHTML='+5€ <span style="text-decoration:line-through;font-size:1rem;opacity:.36">+10€</span>';
  else op.textContent="+10€";
  refreshFp();updSum();
}

function pick(f){pickF(f);goTab("rdv")}

function pickF(f){
  selF=f;
  ["b","c","p"].forEach(function(id){document.getElementById("fc-"+id).className="fc2"});
  var map={basic:"b",confort:"c",premium:"p"};
  document.getElementById("fc-"+map[f]).classList.add("s-"+f);
  updSum();
}

function refreshFp(){
  var t=carType;
  ["basic","confort","premium"].forEach(function(f){
    var short={basic:"b",confort:"c",premium:"p"}[f];
    document.getElementById("fp-"+short).innerHTML=
      "Cit. <strong>"+P[f].cit+"€</strong> · SUV <strong>"+P[f].suv+"€</strong>";
  });
}

function togOpt(){
  optOn=!optOn;
  document.getElementById("oTog").classList.toggle("on",optOn);
  updSum();
}

function updSum(){
  refreshFp();
  var sb=document.getElementById("sumBox");
  if(!selF){sb.style.display="none";return}
  var vt=document.getElementById("r-vt").value||"cit";
  if(!["cit","suv","ber","van"].includes(vt))vt="cit";
  var base=P[selF][vt]||P[selF].cit;
  var total=base+(optOn?P.opt:0);
  var lblMap={cit:"Citadine",suv:"SUV",ber:"Berline/Break",van:"Van"};
  var fLbl=selF.charAt(0).toUpperCase()+selF.slice(1);
  sb.style.display="flex";
  document.getElementById("sumL").textContent=fLbl+" · "+(lblMap[vt]||"Citadine")+(optOn?" + Désinfection":"");
  document.getElementById("sumV").textContent=total+"€";
}

// ══════════════════════════════════════════════
// FORM SUBMIT — Formspree
// ══════════════════════════════════════════════
async function submitRDV(){
  var btn=document.getElementById("subBtn");
  var aOk=document.getElementById("aOk");
  var aErr=document.getElementById("aErr");
  aOk.classList.remove("show");aErr.classList.remove("show");

  var pn=document.getElementById("r-pn").value.trim();
  var nm=document.getElementById("r-nm").value.trim();
  var em=document.getElementById("r-em").value.trim();
  var tl=document.getElementById("r-tl").value.trim();
  var vh=document.getElementById("r-veh").value.trim();
  var vt=document.getElementById("r-vt").value;
  var dt=document.getElementById("r-dt").value;
  var hr=document.getElementById("r-hr").value;
  var msg=document.getElementById("r-msg").value.trim();

  if(!pn||!nm||!em||!tl||!vh||!vt||!selF||!dt||!hr){
    aErr.textContent="Veuillez remplir tous les champs obligatoires et choisir une formule.";
    aErr.classList.add("show");return;
  }
  var lblMap={cit:"Citadine",suv:"SUV / Crossover",ber:"Berline / Break",van:"Monospace / Van"};
  var vLbl=lblMap[vt]||vt;
  var base=P[selF][vt]||P[selF].cit;
  var total=base+(optOn?P.opt:0);
  var fLbl=selF.charAt(0).toUpperCase()+selF.slice(1);

  btn.disabled=true;btn.textContent="Envoi…";

  try{
    var res=await fetch(FS,{
      method:"POST",
      headers:{"Content-Type":"application/json","Accept":"application/json"},
      body:JSON.stringify({
        _replyto:em,
        _subject:"[SpeedClean Auto] RDV - "+pn+" "+nm+" - "+dt+" a "+hr,
        Nom_Prenom:pn+" "+nm,
        Telephone:tl,
        Email_client:em,
        Vehicule:vLbl+" - "+vh,
        Formule:fLbl,
        Option_Parfum:optOn?"Oui (+"+P.opt+"euros)":"Non",
        Total_estime:total+"euros",
        Date_RDV:dt,
        Heure_RDV:hr,
        Adresse_Message:msg||"Non renseigne"
      })
    });
    if(res.ok){
      aOk.textContent="Demande envoyée ! Confirmation sous 24h pour le RDV du "+dt+" à "+hr+".";
      aOk.classList.add("show");
      ["r-pn","r-nm","r-em","r-tl","r-veh","r-dt","r-msg"].forEach(function(id){document.getElementById(id).value=""});
      document.getElementById("r-vt").value="";document.getElementById("r-hr").value="";
      document.getElementById("detType").style.display="none";
      document.getElementById("manFg").style.display="block";
      selF=null;optOn=false;vehSel=null;
      document.getElementById("oTog").classList.remove("on");
      ["b","c","p"].forEach(function(f){document.getElementById("fc-"+f).className="fc2"});
      document.getElementById("sumBox").style.display="none";
    }else throw new Error("err");
  }catch(e){
    aErr.textContent="Erreur. Appelez directement le 07 72 35 53 54";
    aErr.classList.add("show");
  }
  btn.disabled=false;btn.textContent="Envoyer ma demande de rendez-vous";
}

// ══════════════════════════════════════════════
// BOUTIQUE
// ══════════════════════════════════════════════
function orderP(name){
  goTab("rdv");
  document.getElementById("r-msg").value="Interesse par le produit : "+name;
  setTimeout(function(){document.getElementById("r-msg").scrollIntoView({behavior:"smooth",block:"center"})},400);
}

// ══════════════════════════════════════════════
// CLOSE DROPDOWNS
// ══════════════════════════════════════════════
document.addEventListener("click",function(e){
  if(!e.target.closest(".search-row"))document.getElementById("mDrop").classList.remove("open");
  if(!e.target.closest(".veh-wrap2"))document.getElementById("vDrop").classList.remove("open");
});

// ══════════════════════════════════════════════
// INIT
// ══════════════════════════════════════════════
document.addEventListener("DOMContentLoaded",function(){
  var d=new Date();d.setDate(d.getDate()+1);
  document.getElementById("r-dt").min=d.toISOString().split("T")[0];
  if(!PROMO)document.getElementById("promoBar").style.display="none";
  setPill("cit");
  var obs=new IntersectionObserver(function(es){es.forEach(function(e){if(e.isIntersecting)e.target.classList.add("in")})},{threshold:.1});
  document.querySelectorAll("[data-a]").forEach(function(el){obs.observe(el)});
});
</script>
</body>
</html>
