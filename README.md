
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tu Empresa — Higiene profesional para restaurantes</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600;700&family=IBM+Plex+Mono:wght@500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#12211D;
    --teal:#0B5351;
    --teal-dark:#082F2E;
    --lime:#C7DC3F;
    --lime-dark:#9EB730;
    --steel:#7E9490;
    --panel:#E7ECE7;
    --cream:#F5F7F3;
    --white:#FFFFFF;
    --danger:#C24444;
    --success:#3E8E5A;
    --line: rgba(18,33,29,0.12);
    --radius: 16px;
    --radius-sm: 10px;
    --shadow-sm: 0 4px 14px -6px rgba(11,83,81,0.18);
    --shadow: 0 10px 30px -12px rgba(11,83,81,0.25);
    --shadow-lg: 0 30px 60px -20px rgba(0,0,0,0.35);
    --font-display:'Space Grotesk', sans-serif;
    --font-body:'Inter', sans-serif;
    --font-mono:'IBM Plex Mono', monospace;
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  @media (prefers-reduced-motion: reduce){
    html{scroll-behavior:auto;}
    *{animation-duration:0.001ms !important; transition-duration:0.001ms !important;}
  }
  body{
    font-family:var(--font-body);
    color:var(--ink);
    background:var(--cream);
    line-height:1.55;
    -webkit-font-smoothing:antialiased;
    overflow-x:hidden;
  }
  body.lock{ overflow:hidden; }
  a{color:inherit; text-decoration:none;}
  ul{list-style:none;}
  img,svg{display:block; max-width:100%;}
  button{ font-family:inherit; }
  ::selection{ background:var(--lime); color:var(--teal-dark); }
  ::-webkit-scrollbar{ width:10px; height:10px; }
  ::-webkit-scrollbar-track{ background:transparent; }
  ::-webkit-scrollbar-thumb{ background:var(--steel); border-radius:999px; }
  :focus-visible{
    outline:3px solid var(--teal);
    outline-offset:3px;
    border-radius:4px;
  }
  .wrap{
    max-width:1200px;
    margin:0 auto;
    padding:0 28px;
  }
  h1,h2,h3,h4{
    font-family:var(--font-display);
    font-weight:600;
    letter-spacing:-0.01em;
    line-height:1.12;
  }
  .eyebrow{
    font-family:var(--font-mono);
    font-size:0.72rem;
    letter-spacing:0.14em;
    text-transform:uppercase;
    color:var(--teal);
    font-weight:600;
  }
  .btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    gap:8px;
    font-family:var(--font-body);
    font-weight:600;
    font-size:0.95rem;
    padding:13px 24px;
    border-radius:999px;
    border:1.5px solid transparent;
    cursor:pointer;
    transition:transform .18s ease, background .18s ease, color .18s ease, border-color .18s ease, box-shadow .18s ease;
    white-space:nowrap;
  }
  .btn-primary{ background:var(--lime); color:var(--teal-dark); }
  .btn-primary:hover{ transform:translateY(-2px); background:#d5e857; box-shadow:0 12px 24px -8px rgba(199,220,63,0.5); }
  .btn-primary:disabled{ opacity:.45; cursor:not-allowed; transform:none; box-shadow:none; }
  .btn-ghost{ background:transparent; color:var(--white); border-color:rgba(255,255,255,0.4); }
  .btn-ghost:hover{ border-color:var(--white); transform:translateY(-2px); }
  .btn-outline{ background:transparent; color:var(--teal); border-color:var(--teal); }
  .btn-outline:hover{ background:var(--teal); color:var(--white); transform:translateY(-2px); }
  .btn-dark{ background:var(--teal-dark); color:var(--white); }
  .btn-dark:hover{ background:var(--ink); transform:translateY(-2px); }
  .btn-sm{ padding:8px 16px; font-size:0.82rem; }
  .btn-block{ width:100%; }
  .btn:disabled{ opacity:.5; cursor:not-allowed; transform:none !important; box-shadow:none !important; }
  /* ---------- Header ---------- */
  header{
    position:sticky; top:0; z-index:60;
    background:rgba(245,247,243,0.9);
    backdrop-filter:blur(10px);
    border-bottom:1px solid var(--line);
  }
  .nav{
    display:flex; align-items:center; justify-content:space-between;
    padding:16px 28px;
    max-width:1200px; margin:0 auto;
    gap:20px;
  }
  .logo{
    display:flex; align-items:center; gap:10px;
    font-family:var(--font-display); font-weight:700; font-size:1.3rem; letter-spacing:-0.02em;
  }
  .logo .dot{ width:11px;height:11px;border-radius:50%; background:var(--lime); box-shadow:0 0 0 4px rgba(199,220,63,0.25); }
  .nav-links{ display:flex; gap:30px; font-size:0.92rem; font-weight:500; margin-left:auto; }
  .nav-links a{ position:relative; padding:4px 0; color:var(--ink); }
  .nav-links a::after{ content:''; position:absolute; left:0; bottom:-2px; width:0; height:2px; background:var(--teal); transition:width .2s ease; }
  .nav-links a:hover::after{ width:100%; }
  .nav-cta{ display:flex; align-items:center; gap:10px; }
  .cart-btn{
    position:relative;
    display:flex; align-items:center; gap:8px;
    background:var(--teal-dark); color:var(--white);
    border:none; border-radius:999px;
    padding:10px 16px 10px 12px;
    cursor:pointer;
    transition:transform .18s ease, background .18s ease;
  }
  .cart-btn:hover{ transform:translateY(-2px); background:var(--ink); }
  .cart-btn svg{ width:19px; height:19px; }
  .cart-count{
    position:absolute; top:-7px; right:-7px;
    background:var(--lime); color:var(--teal-dark);
    font-family:var(--font-mono); font-size:0.68rem; font-weight:700;
    min-width:19px; height:19px; border-radius:999px;
    display:flex; align-items:center; justify-content:center;
    padding:0 4px;
    transition:transform .15s ease;
  }
  .cart-count.bump{ transform:scale(1.3); }
  .cart-count[data-empty="true"]{ opacity:0; transform:scale(0.4); }
  .account-btn{
    display:flex; align-items:center; gap:8px;
    background:var(--panel); color:var(--teal-dark);
    border:1.5px solid transparent; border-radius:999px;
    padding:9px 15px; font-size:0.85rem; font-weight:600; cursor:pointer;
    transition:all .18s ease; max-width:190px;
  }
  .account-btn:hover{ background:var(--white); border-color:var(--teal); }
  .account-btn svg{ width:16px; height:16px; flex-shrink:0; }
  .account-btn span{ overflow:hidden; text-overflow:ellipsis; white-space:nowrap; }
  .nav-toggle{
    display:none; background:none; border:1px solid var(--line); border-radius:8px;
    width:40px; height:40px; align-items:center; justify-content:center; cursor:pointer;
  }
  .nav-toggle svg{ width:20px; height:20px; }
  .mobile-menu{
    display:none; flex-direction:column; gap:2px;
    background:var(--white); border-bottom:1px solid var(--line);
    padding:8px 28px 18px;
  }
  .mobile-menu.open{ display:flex; }
  .mobile-menu a{ padding:12px 4px; font-size:0.95rem; font-weight:500; border-bottom:1px solid var(--line); }
  .mobile-menu a:last-child{ border-bottom:none; }
  /* ---------- Hero ---------- */
  .hero{
    background:linear-gradient(160deg,var(--teal-dark) 0%, var(--teal) 68%);
    color:var(--white); position:relative; overflow:hidden;
  }
  .hero::before{
    content:''; position:absolute; inset:0; z-index:0; opacity:0.5;
    background-image:radial-gradient(circle, rgba(255,255,255,0.07) 1px, transparent 1.3px);
    background-size:24px 24px;
  }
  .hero::after{
    content:''; position:absolute; top:-120px; right:-160px; width:520px; height:520px;
    background:radial-gradient(circle, rgba(199,220,63,0.16), transparent 70%); z-index:1;
  }
  .hero .wrap{
    display:grid; grid-template-columns:1.05fr 0.95fr; gap:48px; align-items:center;
    padding-top:80px; padding-bottom:80px; position:relative; z-index:2;
  }
  .hero-eyebrow{
    font-family:var(--font-mono); font-size:0.75rem; letter-spacing:0.16em; text-transform:uppercase;
    color:var(--lime); font-weight:600; margin-bottom:18px; display:flex; align-items:center; gap:10px;
  }
  .hero-eyebrow::before{ content:''; width:26px; height:1.5px; background:var(--lime); }
  .hero h1{ font-size:clamp(2.1rem, 4vw, 3.3rem); max-width:12ch; margin-bottom:20px; }
  .hero h1 em{ font-style:normal; color:var(--lime); }
  .hero > .wrap > .hero-copy > p{ font-size:1.06rem; color:rgba(255,255,255,0.82); max-width:46ch; margin-bottom:30px; }
  .hero-actions{ display:flex; gap:16px; flex-wrap:wrap; margin-bottom:36px;}
  .hero-meta{ display:flex; gap:28px; flex-wrap:wrap; padding-top:24px; border-top:1px solid rgba(255,255,255,0.18); }
  .hero-meta div{ display:flex; flex-direction:column; gap:2px; }
  .hero-meta strong{ font-family:var(--font-display); font-size:1.3rem; color:var(--lime); }
  .hero-meta span{ font-size:0.76rem; color:rgba(255,255,255,0.7); }
  .hero-art{ position:relative; }
  .hero-art svg{ width:100%; height:auto; filter:drop-shadow(0 30px 40px rgba(0,0,0,0.28)); animation:float 6s ease-in-out infinite; }
  @keyframes float{ 0%,100%{ transform:translateY(0); } 50%{ transform:translateY(-10px); } }
  /* ---------- Trust strip ---------- */
  .trust{ background:var(--white); border-bottom:1px solid var(--line); }
  .trust .wrap{ display:grid; grid-template-columns:repeat(4,1fr); gap:0; padding-top:32px; padding-bottom:32px; }
  .trust-item{ padding:0 22px; border-left:1px solid var(--line); }
  .trust-item:first-child{ border-left:none; padding-left:0; }
  .trust-item strong{ display:block; font-family:var(--font-display); font-size:1.4rem; color:var(--teal); margin-bottom:4px; }
  .trust-item span{ font-size:0.83rem; color:var(--steel); }
  /* ---------- Category pill nav ---------- */
  .cat-nav-wrap{
    position:sticky; top:73px; z-index:40;
    background:rgba(245,247,243,0.95); backdrop-filter:blur(8px);
    border-bottom:1px solid var(--line);
  }
  .cat-nav{
    display:flex; gap:10px; overflow-x:auto; padding:14px 28px;
    max-width:1200px; margin:0 auto;
    scrollbar-width:none;
  }
  .cat-nav::-webkit-scrollbar{ display:none; }
  .cat-pill{
    flex-shrink:0;
    font-size:0.84rem; font-weight:600; color:var(--steel);
    background:var(--white); border:1px solid var(--line);
    padding:9px 16px; border-radius:999px; cursor:pointer;
    transition:all .18s ease;
  }
  .cat-pill:hover{ border-color:var(--teal); color:var(--teal); }
  .cat-pill.active{ background:var(--teal-dark); border-color:var(--teal-dark); color:var(--lime); }
  /* ---------- Section heading ---------- */
  .section{ padding:88px 0; }
  .section-head{ display:flex; justify-content:space-between; align-items:flex-end; gap:24px; margin-bottom:46px; flex-wrap:wrap; }
  .section-head h2{ font-size:clamp(1.6rem, 3vw, 2.2rem); max-width:16ch; margin-top:10px; }
  .section-head p{ max-width:38ch; color:var(--steel); font-size:0.96rem; }
  /* ---------- Catalog ---------- */
  .catalog{ background:var(--cream); padding-top:52px; }
  .cat-group{ padding-top:36px; scroll-margin-top:150px; }
  .cat-group:first-child{ padding-top:0; }
  .cat-group + .cat-group{ border-top:1px solid var(--line); margin-top:52px; }
  .cat-group-head{ display:flex; align-items:flex-start; gap:16px; margin-bottom:28px; }
  .cat-group-icon{
    width:50px; height:50px; border-radius:12px; background:var(--panel);
    display:flex; align-items:center; justify-content:center; color:var(--teal); flex-shrink:0;
  }
  .cat-group-icon svg{ width:26px; height:26px; }
  .cat-group-head h3{ font-size:1.3rem; margin-bottom:4px; }
  .cat-group-head p{ color:var(--steel); font-size:0.92rem; max-width:56ch; }
  .grid{ display:grid; grid-template-columns:repeat(auto-fill, minmax(250px,1fr)); gap:22px; }
.card{
display:flex;
    flex-direction:column;
    height:100%;
    background:#fff;
    border-radius:18px;
    overflow:hidden;
    transition:.3s;
    border:1px solid rgba(0,0,0,.08);
}
.card:hover{
    transform:translateY(-6px);
}
  .card:hover{ transform:translateY(-4px); box-shadow:var(--shadow); }
  .card.in-cart{ border-color:var(--lime); box-shadow:0 0 0 3px rgba(199,220,63,0.18); }
/* --- Casilla de imagen del producto --- */
  /* Cada producto tiene "img" en el arreglo PRODUCTS. Si la imagen no carga,
     se muestra automáticamente el ícono de respaldo — nada se rompe. */
  .card-media{
    position:relative;
    width:100%;
    height:280px;
    background:#fff;
    display:flex;
    align-items:center;
    justify-content:center;
    overflow:hidden;
    border-bottom:1px solid rgba(0,0,0,.06);
}
  /* Ícono de respaldo, como un sello circular centrado */
  .card-media-fallback{
    position:absolute; inset:0;
    display:flex; align-items:center; justify-content:center;
    color:var(--steel);
  }
  .card-media-fallback::before{
    content:'';
    position:absolute;
    width:56px; height:56px;
    border-radius:50%;
    background:rgba(255,255,255,0.65);
    box-shadow:0 4px 14px -6px rgba(11,83,81,0.2);
  }
  .card-media-fallback svg{
    position:relative; z-index:1;
    width:26px; height:26px;
  }
  /* La foto se ve completa (sin recortes de tapas/etiquetas), centrada y con margen */
  .card-media img{
    width:100%;
    height:100%;
   object-fit:cover;
    object-position:center;
    padding:18px;
    transition:.35s;
    filter:drop-shadow(0 12px 18px rgba(0,0,0,.15));
}
  .card-media img.loaded{
    opacity:1;
    transform:scale(1);
  }
  .card:hover .card-media img{
    transform:scale(1.05);
}
  /* Degradado inferior sutil para que la etiqueta de referencia siempre se lea bien */
  .card-media::after{
    content:'';
    position:absolute; inset:0;
    background:linear-gradient(to top, rgba(8,20,18,0.22) 0%, transparent 34%);
    z-index:1;
    pointer-events:none;
  }
  .card-media .card-ref{
    position:absolute; top:10px; left:10px; z-index:2;
    background:rgba(8,20,18,0.72); color:var(--lime);
    font-family:var(--font-mono); font-size:0.65rem; letter-spacing:0.03em;
    padding:4px 9px; border-radius:6px;
    backdrop-filter:blur(2px);
  }
  .card-content{
   display:flex;
    flex-direction:column;
    flex:1;
    padding:20px;
}
  .card h4{ font-family:var(--font-display); font-size:1.02rem; font-weight:600; line-height:1.25; }
  .card-pres{
    font-family:var(--font-mono); font-size:0.72rem; color:var(--teal);
    background:var(--panel); display:inline-block; padding:3px 9px; border-radius:999px; align-self:flex-start;
  }
  .card-bottom{ margin-top:auto; display:flex; align-items:center; justify-content:flex-end; gap:10px; }
  .stepper{ display:flex; align-items:center; gap:0; border:1.5px solid var(--line); border-radius:999px; overflow:hidden; }
  .stepper button{
    width:32px; height:32px; border:none; background:var(--panel); color:var(--teal-dark);
    font-size:1.05rem; font-weight:700; cursor:pointer; display:flex; align-items:center; justify-content:center;
    transition:background .15s ease;
  }
  .stepper button:hover{ background:var(--lime); }
  .stepper button:disabled{ opacity:.4; cursor:not-allowed; }
  .stepper .qty{ width:34px; text-align:center; font-family:var(--font-mono); font-weight:600; font-size:0.9rem; }
  /* ---------- Why us ---------- */
  .why{ background:var(--white); border-top:1px solid var(--line); border-bottom:1px solid var(--line);}
  .why .wrap{ display:grid; grid-template-columns:0.9fr 1.1fr; gap:64px; align-items:center; }
  .why-visual{ background:var(--panel); border-radius:var(--radius); padding:36px; aspect-ratio:1/1; display:flex; align-items:center; justify-content:center; }
  .why-visual svg{ width:100%; height:100%; }
  .why-list{ display:flex; flex-direction:column; gap:24px; margin-top:26px; }
  .why-list li{ display:flex; gap:16px; }
  .why-num{ font-family:var(--font-mono); font-size:0.8rem; color:var(--teal); background:var(--panel); width:34px; height:34px; border-radius:8px; display:flex; align-items:center; justify-content:center; flex-shrink:0; }
  .why-list h4{ font-size:1.0rem; margin-bottom:4px; }
  .why-list p{ color:var(--steel); font-size:0.9rem; max-width:44ch; }
  /* ---------- Final CTA ---------- */
  .final-cta{ background:linear-gradient(160deg,var(--teal-dark) 0%, var(--teal) 75%); color:var(--white); }
  .final-cta .wrap{ text-align:center; display:flex; flex-direction:column; align-items:center; gap:18px; }
  .final-cta h2{ color:var(--white); font-size:clamp(1.6rem,3vw,2.2rem); max-width:22ch; }
  .final-cta p{ color:rgba(255,255,255,0.78); max-width:48ch; }
  .final-actions{ display:flex; gap:16px; flex-wrap:wrap; justify-content:center; margin-top:10px; }
  .final-direct{ margin-top:18px; font-size:0.88rem; color:rgba(255,255,255,0.65); }
  .final-direct a{ color:var(--lime); font-weight:600; }
  /* ---------- Footer ---------- */
  footer{ background:var(--ink); color:rgba(255,255,255,0.7); }
  footer .wrap{ display:grid; grid-template-columns:1.3fr 1fr 1fr 1fr; gap:40px; padding-top:60px; padding-bottom:32px; }
  .footer-brand .logo{ color:var(--white); margin-bottom:14px; }
  .footer-brand p{ font-size:0.87rem; max-width:32ch; color:rgba(255,255,255,0.55); }
  footer h5{ font-family:var(--font-mono); font-size:0.72rem; letter-spacing:0.1em; text-transform:uppercase; color:rgba(255,255,255,0.45); margin-bottom:16px; }
  footer ul{ display:flex; flex-direction:column; gap:10px; font-size:0.87rem; }
  footer ul a:hover{ color:var(--lime); }
  .footer-bottom{ border-top:1px solid rgba(255,255,255,0.1); padding:20px 28px; max-width:1200px; margin:0 auto; display:flex; justify-content:space-between; font-size:0.78rem; color:rgba(255,255,255,0.4); flex-wrap:wrap; gap:10px; }
  /* ---------- Overlay ---------- */
  .overlay{
    position:fixed; inset:0; background:rgba(8,20,18,0.55);
    opacity:0; visibility:hidden; transition:opacity .25s ease, visibility .25s ease;
    z-index:80;
  }
  .overlay.show{ opacity:1; visibility:visible; }
  /* ---------- Cart drawer ---------- */
  .cart-drawer{
    position:fixed; top:0; right:0; height:100%; width:min(420px,92vw);
    background:var(--white); z-index:90;
    display:flex; flex-direction:column;
    transform:translateX(100%); transition:transform .3s ease;
    box-shadow:-20px 0 50px rgba(0,0,0,0.2);
  }
  .cart-drawer.open{ transform:translateX(0); }
  .cart-head{ display:flex; align-items:center; justify-content:space-between; padding:22px 22px 18px; border-bottom:1px solid var(--line); }
  .cart-head h3{ font-size:1.1rem; }
  .cart-close{ background:var(--panel); border:none; width:34px; height:34px; border-radius:999px; cursor:pointer; display:flex; align-items:center; justify-content:center; }
  .cart-close svg{ width:16px; height:16px; }
  .cart-items{ flex:1; overflow-y:auto; padding:16px 22px; display:flex; flex-direction:column; gap:14px; }
  .cart-empty{ text-align:center; color:var(--steel); font-size:0.9rem; padding:60px 10px; display:flex; flex-direction:column; align-items:center; gap:14px; }
  .cart-empty svg{ width:44px; height:44px; color:var(--panel); }
  .cart-row{ display:flex; gap:12px; align-items:flex-start; border-bottom:1px solid var(--line); padding-bottom:14px; }
.cart-row-media{ width:46px; height:46px; border-radius:10px; overflow:hidden; position:relative; background:linear-gradient(135deg,var(--panel),var(--cream)); flex-shrink:0; }
  .cart-row-media img{ position:absolute; inset:6px; object-fit:contain; opacity:0; transition:opacity .3s ease; }
  .cart-row-media img.loaded{ opacity:1; }
  .cart-row-media .card-media-fallback svg{ width:16px; height:16px; }
  .cart-row-info{ flex:1; }
  .cart-row-info h5{ font-family:var(--font-display); font-size:0.9rem; font-weight:600; line-height:1.3; }
  .cart-row-info span{ font-family:var(--font-mono); font-size:0.7rem; color:var(--steel); }
  .cart-row-actions{ display:flex; align-items:center; gap:8px; margin-top:8px; }
  .cart-row-remove{ background:none; border:none; color:var(--danger); font-size:0.75rem; cursor:pointer; text-decoration:underline; margin-top:8px; }
  .cart-foot{ padding:18px 22px 24px; border-top:1px solid var(--line); display:flex; flex-direction:column; gap:10px; }
  .cart-summary{ display:flex; justify-content:space-between; font-size:0.9rem; color:var(--steel); }
  .cart-summary strong{ color:var(--ink); font-family:var(--font-mono); }
  /* ---------- Modal (checkout + auth) ---------- */
  .modal{
    position:fixed; top:50%; left:50%; transform:translate(-50%,-48%);
    width:min(520px,92vw); max-height:88vh; overflow-y:auto;
    background:var(--white); border-radius:18px; z-index:95;
    opacity:0; visibility:hidden; transition:opacity .25s ease, transform .25s ease, visibility .25s ease;
    box-shadow:var(--shadow-lg);
  }
  .modal.show{ opacity:1; visibility:visible; transform:translate(-50%,-50%); }
  .modal-head{ display:flex; align-items:flex-start; justify-content:space-between; gap:14px; padding:26px 26px 6px; }
  .modal-head h3{ font-size:1.25rem; margin-bottom:6px; }
  .modal-head p{ font-size:0.88rem; color:var(--steel); }
  .modal-close{ background:var(--panel); border:none; width:32px; height:32px; border-radius:999px; cursor:pointer; display:flex; align-items:center; justify-content:center; flex-shrink:0; }
  .modal-close svg{ width:15px; height:15px; }
  .modal-body{ padding:16px 26px 26px; }
  .modal-summary{
    background:var(--cream); border:1px solid var(--line); border-radius:10px; padding:12px 14px; margin-bottom:18px;
    font-size:0.82rem; color:var(--steel); max-height:130px; overflow-y:auto;
  }
  .modal-summary div{ display:flex; justify-content:space-between; padding:4px 0; color:var(--ink); }
  .modal-summary div span:last-child{ font-family:var(--font-mono); color:var(--teal); flex-shrink:0; margin-left:10px; }
  .field{ display:flex; flex-direction:column; gap:6px; margin-bottom:15px; }
  .field label{ font-size:0.8rem; font-weight:600; color:var(--teal-dark); }
  .field label .opt{ color:var(--steel); font-weight:400; }
  .field input, .field select, .field textarea{
    font-family:var(--font-body); font-size:0.92rem; padding:11px 13px;
    border:1.5px solid var(--line); border-radius:9px; background:var(--cream); color:var(--ink);
    transition:border-color .18s ease;
  }
  .field input:focus, .field select:focus, .field textarea:focus{ border-color:var(--teal); outline:none; }
  .form-row{ display:grid; grid-template-columns:1fr 1fr; gap:14px; }
  .modal-note{ font-size:0.76rem; color:var(--steel); margin-top:12px; text-align:center; }
  .wa-icon{ width:18px; height:18px; }
  /* ---------- Auth modal specific ---------- */
  .auth-tabs{ display:flex; gap:6px; background:var(--panel); border-radius:999px; padding:4px; margin-bottom:20px; }
  .auth-tab{ flex:1; text-align:center; padding:9px 0; border-radius:999px; font-size:0.85rem; font-weight:600; color:var(--steel); cursor:pointer; border:none; background:none; transition:all .18s ease; }
  .auth-tab.active{ background:var(--white); color:var(--teal-dark); box-shadow:var(--shadow-sm); }
  .auth-panel{ display:none; }
  .auth-panel.active{ display:block; }
  .auth-error{ background:rgba(194,68,68,0.08); border:1px solid rgba(194,68,68,0.3); color:var(--danger); font-size:0.82rem; padding:10px 12px; border-radius:9px; margin-bottom:14px; display:none; }
  .auth-error.show{ display:block; }
  .auth-disabled-note{ background:rgba(199,220,63,0.16); border:1px solid rgba(199,220,63,0.45); color:var(--teal-dark); font-size:0.78rem; padding:11px 13px; border-radius:9px; margin-bottom:18px; display:none; line-height:1.5; }
  .auth-disabled-note.show{ display:block; }
  .auth-success{ text-align:center; padding:10px 0 4px; }
  .auth-success svg{ width:44px; height:44px; color:var(--success); margin:0 auto 14px; }
  /* ---------- Toast ---------- */
  .toast{
    position:fixed; bottom:24px; left:50%; transform:translateX(-50%) translateY(20px);
    background:var(--teal-dark); color:var(--white); padding:13px 22px; border-radius:999px;
    font-size:0.85rem; font-weight:500; display:flex; align-items:center; gap:8px;
    opacity:0; visibility:hidden; transition:all .25s ease; z-index:100;
    box-shadow:0 15px 30px -10px rgba(0,0,0,0.4);
    max-width:90vw;
  }
  .toast.show{ opacity:1; visibility:visible; transform:translateX(-50%) translateY(0); }
  .toast svg{ width:16px; height:16px; color:var(--lime); flex-shrink:0; }
  /* ---------- Responsive ---------- */
  @media (max-width: 900px){
    .hero .wrap{ grid-template-columns:1fr; padding-top:52px; padding-bottom:52px; }
    .hero-art{ order:-1; max-width:340px; margin:0 auto; }
    .trust .wrap{ grid-template-columns:repeat(2,1fr); row-gap:22px; }
    .trust-item{ border-left:none !important; padding-left:0 !important; }
    .why .wrap{ grid-template-columns:1fr; }
    .why-visual{ max-width:300px; margin:0 auto; }
    footer .wrap{ grid-template-columns:1fr 1fr; }
    .cat-nav-wrap{ top:65px; }
  }
  @media (max-width: 640px){
    .nav-links{ display:none; }
    .nav-toggle{ display:flex; }
    .account-btn span{ display:none; }
    .account-btn{ padding:9px; }
    .form-row{ grid-template-columns:1fr; }
    footer .wrap{ grid-template-columns:1fr; }
    .section{ padding:60px 0; }
    .nav{ padding:14px 20px; }
    .wrap{ padding:0 20px; }
  }
</style>
</head>
<body>
<header>
  <nav class="nav">
    <a href="#" class="logo"><span class="dot"></span>Tu Empresa</a>
    <ul class="nav-links">
      <li><a href="#catalogo">Catálogo</a></li>
      <li><a href="#nosotros">Por qué nosotros</a></li>
      <li><a href="#contacto">Contacto</a></li>
    </ul>
    <div class="nav-cta">
      <button class="account-btn" id="accountBtn" onclick="openAuth()" aria-label="Iniciar sesión">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="8" r="4"/><path d="M4 20c0-4 4-6 8-6s8 2 8 6"/></svg>
        <span id="accountBtnLabel">Iniciar sesión</span>
      </button>
      <button class="cart-btn" onclick="openCart()" aria-label="Ver pedido">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M6 6h15l-1.5 9h-12L6 6Z"/><path d="M6 6 4.5 3H2"/><circle cx="9" cy="20" r="1.3" fill="currentColor" stroke="none"/><circle cx="17" cy="20" r="1.3" fill="currentColor" stroke="none"/></svg>
        <span>Mi pedido</span>
        <span class="cart-count" id="cartCount" data-empty="true">0</span>
      </button>
      <button class="nav-toggle" onclick="toggleMobileMenu()" aria-label="Abrir menú">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M4 7h16M4 12h16M4 17h16"/></svg>
      </button>
    </div>
  </nav>
  <div class="mobile-menu" id="mobileMenu">
    <a href="#catalogo" onclick="toggleMobileMenu()">Catálogo</a>
    <a href="#nosotros" onclick="toggleMobileMenu()">Por qué nosotros</a>
    <a href="#contacto" onclick="toggleMobileMenu()">Contacto</a>
  </div>
</header>

<section class="hero">
  <div class="wrap">
    <div class="hero-copy">
      <div class="hero-eyebrow">Suministro para HORECA</div>
      <h1>Higiene profesional para cocinas que <em>no se detienen</em>.</h1>
      <p>Surtimos a restaurantes, cocinas industriales y cadenas de alimentos con productos de limpieza y desinfección pensados para el ritmo de un servicio real — no para el hogar.</p>
      <div class="hero-actions">
        <a href="#catalogo" class="btn btn-primary">Ver catálogo completo</a>
        <button class="btn btn-ghost" onclick="openCart()">Armar mi pedido</button>
      </div>
      <div class="hero-meta">
        <div><strong>+150</strong><span>cocinas comerciales surtidas</span></div>
        <div><strong>24–48h</strong><span>tiempo de entrega</span></div>
        <div><strong>6</strong><span>líneas de producto especializadas</span></div>
      </div>
    </div>
    <div class="hero-art">
      <svg viewBox="0 0 420 460" xmlns="http://www.w3.org/2000/svg">
        <defs>
          <linearGradient id="bottleGrad" x1="0" y1="0" x2="1" y2="1">
            <stop offset="0" stop-color="#C7DC3F"/><stop offset="1" stop-color="#93B02C"/>
          </linearGradient>
          <linearGradient id="drumGrad" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0" stop-color="#F5F7F3"/><stop offset="1" stop-color="#CFDAD3"/>
          </linearGradient>
        </defs>
        <ellipse cx="210" cy="430" rx="160" ry="18" fill="#03201F" opacity="0.35"/>
        <rect x="70" y="230" width="150" height="180" rx="16" fill="url(#drumGrad)"/>
        <rect x="70" y="230" width="150" height="34" rx="16" fill="#0B5351" opacity="0.15"/>
        <rect x="86" y="300" width="118" height="26" rx="4" fill="#0B5351"/>
        <text x="145" y="318" font-family="IBM Plex Mono, monospace" font-size="12" fill="#C7DC3F" text-anchor="middle" font-weight="600">DES-02</text>
        <rect x="86" y="345" width="70" height="8" rx="4" fill="#7E9490" opacity="0.5"/>
        <rect x="86" y="362" width="95" height="8" rx="4" fill="#7E9490" opacity="0.5"/>
        <g>
          <rect x="230" y="150" width="118" height="230" rx="18" fill="#FFFFFF"/>
          <rect x="230" y="150" width="118" height="230" rx="18" fill="#0B5351" opacity="0.06"/>
          <rect x="252" y="180" width="74" height="150" rx="10" fill="url(#bottleGrad)"/>
          <rect x="264" y="196" width="50" height="18" rx="3" fill="#082F2E"/>
          <text x="289" y="209" font-family="IBM Plex Mono, monospace" font-size="9" fill="#C7DC3F" text-anchor="middle" font-weight="600">DEG-01</text>
          <rect x="270" y="110" width="42" height="46" rx="8" fill="#082F2E"/>
          <rect x="278" y="70" width="8" height="46" rx="4" fill="#082F2E"/>
          <circle cx="282" cy="66" r="8" fill="#C7DC3F"/>
        </g>
        <g>
          <rect x="20" y="290" width="70" height="120" rx="12" fill="#0B5351"/>
          <rect x="34" y="270" width="42" height="26" rx="6" fill="#0B5351"/>
          <rect x="48" y="255" width="14" height="20" rx="4" fill="#082F2E"/>
          <rect x="32" y="330" width="46" height="18" rx="4" fill="#F5F7F3" opacity="0.9"/>
          <text x="55" y="343" font-family="IBM Plex Mono, monospace" font-size="8" fill="#0B5351" text-anchor="middle" font-weight="600">LOZ-03</text>
        </g>
        <circle cx="340" cy="120" r="4" fill="#C7DC3F" opacity="0.8"/>
        <circle cx="360" cy="150" r="2.5" fill="#C7DC3F" opacity="0.6"/>
        <circle cx="40" cy="240" r="3" fill="#C7DC3F" opacity="0.6"/>
      </svg>
    </div>
  </div>
</section>

<section class="trust">
  <div class="wrap">
    <div class="trust-item"><strong>24–48 h</strong><span>Entrega a tu restaurante</span></div>
    <div class="trust-item"><strong>+150</strong><span>Cocinas comerciales surtidas</span></div>
    <div class="trust-item"><strong>100%</strong><span>Insumos con ficha técnica y de seguridad</span></div>
    <div class="trust-item"><strong>A tu medida</strong><span>Asesoría en dilución, uso y almacenamiento</span></div>
  </div>
</section>

<div class="cat-nav-wrap">
  <div class="cat-nav" id="catNav">
    <button class="cat-pill" data-target="cat-deg">Desengrasantes</button>
    <button class="cat-pill" data-target="cat-des">Desinfectantes</button>
    <button class="cat-pill" data-target="cat-loz">Loza y utensilios</button>
    <button class="cat-pill" data-target="cat-hig">Higiene de manos</button>
    <button class="cat-pill" data-target="cat-pis">Pisos y superficies</button>
    <button class="cat-pill" data-target="cat-eqp">Equipos y accesorios</button>
  </div>
</div>

<section class="section catalog" id="catalogo">
  <div class="wrap">
    <div class="section-head">
      <div>
        <span class="eyebrow">Catálogo</span>
        <h2>Selecciona lo que necesita tu cocina</h2>
      </div>
      <p>No manejamos precios en línea: agrega los productos que necesitas a tu pedido y lo enviamos directo a tu asesor por WhatsApp para cotizarlo.</p>
    </div>
    <!-- DESENGRASANTES -->
    <div class="cat-group" id="cat-deg">
      <div class="cat-group-head">
        <div class="cat-group-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M8 3h8l1 4H7l1-4Z"/><path d="M6 7h12l1 13a1 1 0 0 1-1 1H6a1 1 0 0 1-1-1L6 7Z"/><path d="M9 12h6"/><path d="M9 16h6"/></svg>
        </div>
        <div>
          <h3>Desengrasantes de cocina</h3>
          <p>Fórmulas de alto poder para grasa quemada en parrillas, campanas, hornos y freidoras.</p>
        </div>
      </div>
      <div class="grid" data-grid="cat-deg"></div>
    </div>
    <!-- DESINFECTANTES -->
    <div class="cat-group" id="cat-des">
      <div class="cat-group-head">
        <div class="cat-group-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2s6 6.5 6 11a6 6 0 1 1-12 0c0-4.5 6-11 6-11Z"/><path d="M9.5 15.5a2.5 2.5 0 0 0 3 2.4"/></svg>
        </div>
        <div>
          <h3>Desinfectantes y sanitizantes</h3>
          <p>Elimina bacterias y virus en superficies de contacto con alimentos, dentro de la normativa sanitaria vigente.</p>
        </div>
      </div>
      <div class="grid" data-grid="cat-des"></div>
    </div>
    <!-- LOZA -->
    <div class="cat-group" id="cat-loz">
      <div class="cat-group-head">
        <div class="cat-group-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="13" r="7"/><path d="M9 13a3 3 0 0 0 3 3"/><path d="M12 3v3"/></svg>
        </div>
        <div>
          <h3>Detergentes para loza y utensilios</h3>
          <p>Desengrasa y abrillanta vajilla, ollas y utensilios, en lavado manual o en máquina industrial.</p>
        </div>
      </div>
      <div class="grid" data-grid="cat-loz"></div>
    </div>
    <!-- HIGIENE -->
    <div class="cat-group" id="cat-hig">
      <div class="cat-group-head">
        <div class="cat-group-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M7 11V7a5 5 0 0 1 10 0v4"/><path d="M5 11h14l-1.2 8.4a2 2 0 0 1-2 1.6H8.2a2 2 0 0 1-2-1.6L5 11Z"/></svg>
        </div>
        <div>
          <h3>Higiene de manos y papel</h3>
          <p>Jabones antibacteriales, gel y línea de papel institucional para baños, vestidores y cocina.</p>
        </div>
      </div>
      <div class="grid" data-grid="cat-hig"></div>
    </div>
    <!-- PISOS -->
    <div class="cat-group" id="cat-pis">
      <div class="cat-group-head">
        <div class="cat-group-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M3 17h18"/><path d="M3 21h18"/><path d="M8 17c0-5 2-9 4-13 2 4 4 8 4 13"/></svg>
        </div>
        <div>
          <h3>Limpieza de pisos y superficies</h3>
          <p>Desinfectantes y desengrasantes para pisos antiderrapantes, resistentes a grasa, agua y tránsito constante.</p>
        </div>
      </div>
      <div class="grid" data-grid="cat-pis"></div>
    </div>
    <!-- EQUIPOS -->
    <div class="cat-group" id="cat-eqp">
      <div class="cat-group-head">
        <div class="cat-group-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M14 3l7 7-8.5 8.5L4 20l1.5-8.5L14 3Z"/><path d="M12 8l4 4"/></svg>
        </div>
        <div>
          <h3>Equipos y accesorios</h3>
          <p>Trapeadores, cubetas, dispensadores, cepillos y carros de limpieza para uso profesional rudo.</p>
        </div>
      </div>
      <div class="grid" data-grid="cat-eqp"></div>
    </div>

  </div>
</section>

<section class="section why" id="nosotros">
  <div class="wrap">
    <div class="why-visual">
      <svg viewBox="0 0 300 300" xmlns="http://www.w3.org/2000/svg">
        <circle cx="150" cy="150" r="130" fill="#0B5351" opacity="0.06"/>
        <circle cx="150" cy="150" r="95" fill="#0B5351" opacity="0.08"/>
        <rect x="105" y="70" width="90" height="150" rx="14" fill="#0B5351"/>
        <rect x="120" y="100" width="60" height="10" rx="5" fill="#C7DC3F"/>
        <rect x="120" y="120" width="44" height="8" rx="4" fill="#F5F7F3" opacity="0.7"/>
        <rect x="120" y="136" width="52" height="8" rx="4" fill="#F5F7F3" opacity="0.7"/>
        <rect x="120" y="152" width="38" height="8" rx="4" fill="#F5F7F3" opacity="0.7"/>
        <circle cx="150" cy="190" r="14" fill="#C7DC3F"/>
        <path d="M144 190l4 4 8-8" stroke="#082F2E" stroke-width="2.4" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
        <rect x="60" y="200" width="34" height="50" rx="8" fill="#7E9490"/>
        <rect x="206" y="180" width="34" height="70" rx="8" fill="#7E9490"/>
      </svg>
    </div>
    <div class="why-copy">
      <span class="eyebrow">Por qué nosotros</span>
      <h2 style="margin-top:10px; max-width:18ch;">Diseñado para cocinas que trabajan a diario, no para el hogar</h2>
      <ul class="why-list">
        <li><span class="why-num">01</span><div><h4>Formulado para el ritmo de una cocina real</h4><p>Concentraciones y rendimiento pensados para servicio diario, no para uso doméstico ocasional.</p></div></li>
        <li><span class="why-num">02</span><div><h4>Cumplimiento con normativa sanitaria</h4><p>Cada línea cuenta con ficha técnica y de seguridad disponible para tus auditorías e inspecciones.</p></div></li>
        <li><span class="why-num">03</span><div><h4>Reposición programada</h4><p>Coordinamos entregas recurrentes para que nunca te falte insumo en plena operación.</p></div></li>
      </ul>
    </div>
  </div>
</section>

<section class="section final-cta" id="contacto">
  <div class="wrap">
    <span class="eyebrow" style="color:var(--lime)">Tu pedido</span>
    <h2>Agrega lo que necesitas y lo enviamos directo por WhatsApp</h2>
    <p>Selecciona los productos del catálogo, ábrelo desde el botón "Mi pedido" y en un minuto tu solicitud llega ordenada a tu asesor — sin llamadas, sin esperar cotización por correo.</p>
    <div class="final-actions">
      <button class="btn btn-primary" onclick="openCart()">Ver mi pedido</button>
      <a href="#catalogo" class="btn btn-ghost">Seguir viendo el catálogo</a>
    </div>
    <p class="final-direct">¿Prefieres hablar directo? Escríbenos a <a href="https://wa.me/529930000000" target="_blank" rel="noopener">WhatsApp</a> o al correo <a href="mailto:ventas@tuempresa.mx">ventas@tuempresa.mx</a></p>
  </div>
</section>

<footer>
  <div class="wrap">
    <div class="footer-brand">
      <a href="#" class="logo"><span class="dot"></span>Tu Empresa</a>
      <p>Suministro de productos de limpieza e higiene para restaurantes, cocinas industriales y cadenas de alimentos.</p>
    </div>
    <div>
      <h5>Catálogo</h5>
      <ul>
        <li><a href="#cat-deg">Desengrasantes</a></li>
        <li><a href="#cat-des">Desinfectantes</a></li>
        <li><a href="#cat-loz">Loza y utensilios</a></li>
        <li><a href="#cat-hig">Higiene de manos</a></li>
      </ul>
    </div>
    <div>
      <h5>Empresa</h5>
      <ul>
        <li><a href="#nosotros">Por qué nosotros</a></li>
        <li><a href="#contacto">Contacto</a></li>
        <li><a href="#">Aviso de privacidad</a></li>
      </ul>
    </div>
    <div>
      <h5>Contacto directo</h5>
      <ul>
        <li>ventas@tuempresa.mx</li>
        <li>+52 993 000 0000</li>
        <li>Tabasco, México</li>
      </ul>
    </div>
  </div>
  <div class="footer-bottom">
    <span>© 2026 Tu Empresa. Todos los derechos reservados.</span>
    <span>Higiene profesional para restaurantes</span>
  </div>
</footer>

<!-- Overlay -->
<div class="overlay" id="overlay" onclick="closeAll()"></div>

<!-- Cart drawer -->
<aside class="cart-drawer" id="cartDrawer" aria-label="Mi pedido">
  <div class="cart-head">
    <h3>Mi pedido</h3>
    <button class="cart-close" onclick="closeCart()" aria-label="Cerrar"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg></button>
  </div>
  <div class="cart-items" id="cartItems"></div>
  <div class="cart-foot">
    <div class="cart-summary">
      <span>Productos distintos</span>
      <strong id="cartLinesCount">0</strong>
    </div>
    <div class="cart-summary">
      <span>Piezas / envases en total</span>
      <strong id="cartUnitsCount">0</strong>
    </div>
    <button class="btn btn-primary btn-block" id="checkoutBtn" onclick="openCheckout()" disabled>Enviar pedido por WhatsApp</button>
  </div>
</aside>

<!-- Checkout modal -->
<div class="modal" id="checkoutModal" role="dialog" aria-label="Datos para tu pedido">
  <div class="modal-head">
    <div>
      <h3>Un último paso</h3>
      <p>Con estos datos armamos tu pedido y lo mandamos directo a WhatsApp.</p>
    </div>
    <button class="modal-close" onclick="closeCheckout()" aria-label="Cerrar"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg></button>
  </div>
  <div class="modal-body">
    <div class="modal-summary" id="modalSummary"></div>
    <form id="checkoutForm" onsubmit="return sendOrder(event)">
      <div class="field">
        <label for="negocio">Nombre del negocio / restaurante</label>
        <input id="negocio" type="text" placeholder="Ej. Restaurante El Buen Sabor" required>
      </div>
      <div class="form-row">
        <div class="field">
          <label for="contacto2">Nombre de quien solicita</label>
          <input id="contacto2" type="text" placeholder="Tu nombre" required>
        </div>
        <div class="field">
          <label for="telefono">Teléfono</label>
          <input id="telefono" type="tel" placeholder="10 dígitos" required>
        </div>
      </div>
      <div class="field">
        <label for="direccion">Dirección o sucursal <span class="opt">(opcional)</span></label>
        <input id="direccion" type="text" placeholder="Dirección de entrega o nombre de sucursal">
      </div>
      <div class="field">
        <label for="notas">Notas adicionales <span class="opt">(opcional)</span></label>
        <textarea id="notas" rows="2" placeholder="Horario de entrega, referencias, etc."></textarea>
      </div>
      <button type="submit" class="btn btn-primary btn-block" id="sendOrderBtn">
        <svg class="wa-icon" viewBox="0 0 24 24" fill="currentColor"><path d="M17.5 14.4c-.3-.1-1.7-.8-2-.9-.3-.1-.5-.1-.7.1-.2.3-.7.9-.9 1-.2.2-.4.2-.7.1-.3-.1-1.3-.5-2.4-1.5-.9-.8-1.5-1.8-1.7-2.1-.2-.3 0-.5.1-.6.1-.1.3-.4.4-.5.1-.2.2-.3.1-.6-.1-.3-.7-1.7-.9-2.1-.2-.4-.4-.4-.6-.4h-.5c-.2 0-.5.1-.7.4-.2.3-.9 1-.9 2.3 0 1.3 1 2.6 1.1 2.8.1.2 1.9 2.9 4.6 4 2.7 1.1 2.7.7 3.2.7.5-.1 1.7-.7 1.9-1.4.2-.7.2-1.3.2-1.4 0-.1-.1-.2-.3-.3Z"/><path d="M12 2a10 10 0 0 0-8.6 15.1L2 22l5-1.3A10 10 0 1 0 12 2Zm0 18.2c-1.6 0-3.1-.4-4.5-1.2l-.3-.2-3 .8.8-2.9-.2-.3A8.2 8.2 0 1 1 20.2 12 8.2 8.2 0 0 1 12 20.2Z"/></svg>
        Enviar pedido por WhatsApp
      </button>
      <p class="modal-note">Se abrirá WhatsApp con tu pedido ya redactado, listo para enviar.</p>
    </form>
  </div>
</div>

<!-- Auth modal (login / registro) -->
<div class="modal" id="authModal" role="dialog" aria-label="Iniciar sesión o crear cuenta">
  <div class="modal-head">
    <div>
      <h3 id="authTitle">Tu cuenta</h3>
      <p>Regístrate una vez y tus datos se autocompletan en cada pedido.</p>
    </div>
    <button class="modal-close" onclick="closeAuth()" aria-label="Cerrar"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg></button>
  </div>
  <div class="modal-body">
    <div class="auth-disabled-note" id="authDisabledNote">
      ⚠️ El registro con Firebase todavía no está configurado en esta página. Puedes seguir armando tu pedido y enviarlo por WhatsApp sin iniciar sesión.
    </div>
    <!-- Vista: usuario ya conectado -->
    <div id="authLoggedInView" style="display:none;">
      <div class="auth-success">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6 9 17l-5-5"/></svg>
        <p style="margin-bottom:4px;"><strong id="loggedInName">—</strong></p>
        <p style="color:var(--steel); font-size:0.88rem;" id="loggedInEmail">—</p>
      </div>
      <button type="button" class="btn btn-outline btn-block" style="margin-top:18px;" onclick="handleLogout()">Cerrar sesión</button>
    </div>
    <!-- Vista: login / registro -->
    <div id="authFormsView">
      <div class="auth-tabs">
        <button type="button" class="auth-tab active" id="tabLogin" onclick="switchAuthTab('login')">Iniciar sesión</button>
        <button type="button" class="auth-tab" id="tabRegister" onclick="switchAuthTab('register')">Crear cuenta</button>
      </div>
      <div class="auth-error" id="authError"></div>
      <!-- Panel: login -->
      <div class="auth-panel active" id="panelLogin">
        <form id="loginForm" onsubmit="return handleLogin(event)">
          <div class="field">
            <label for="loginEmail">Correo</label>
            <input id="loginEmail" type="email" placeholder="tucorreo@ejemplo.com" required>
          </div>
          <div class="field">
            <label for="loginPassword">Contraseña</label>
            <input id="loginPassword" type="password" placeholder="Tu contraseña" required minlength="6">
          </div>
          <button type="submit" class="btn btn-primary btn-block" id="loginBtn">Iniciar sesión</button>
        </form>
      </div>
      <!-- Panel: registro -->
      <div class="auth-panel" id="panelRegister">
        <form id="registerForm" onsubmit="return handleRegister(event)">
          <div class="field">
            <label for="regNegocio">Nombre del negocio</label>
            <input id="regNegocio" type="text" placeholder="Ej. Restaurante El Buen Sabor" required>
          </div>
          <div class="form-row">
            <div class="field">
              <label for="regContacto">Nombre de contacto</label>
              <input id="regContacto" type="text" placeholder="Tu nombre" required>
            </div>
            <div class="field">
              <label for="regTelefono">Teléfono</label>
              <input id="regTelefono" type="tel" placeholder="10 dígitos" required>
            </div>
          </div>
          <div class="field">
            <label for="regEmail">Correo</label>
            <input id="regEmail" type="email" placeholder="tucorreo@ejemplo.com" required>
          </div>
          <div class="form-row">
            <div class="field">
              <label for="regPassword">Contraseña</label>
              <input id="regPassword" type="password" placeholder="Mínimo 6 caracteres" required minlength="6">
            </div>
            <div class="field">
              <label for="regPassword2">Confirmar</label>
              <input id="regPassword2" type="password" placeholder="Repite la contraseña" required minlength="6">
            </div>
          </div>
          <button type="submit" class="btn btn-primary btn-block" id="registerBtn">Crear cuenta</button>
        </form>
      </div>
    </div>

  </div>
</div>

<!-- Toast -->
<div class="toast" id="toast"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6 9 17l-5-5"/></svg><span id="toastMsg">Agregado a tu pedido</span></div>

<!-- ================= FIREBASE SDK (compat) =================
     Si no vas a usar el login por ahora, puedes dejar estas líneas tal cual:
     la página seguirá funcionando normal (catálogo + WhatsApp) sin registro. -->
<script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-auth-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore-compat.js"></script>

<script>
  /* ======================================================================
     CONFIGURACIÓN — edita solo estos dos bloques
     ====================================================================== */

  // 1) Tu número de WhatsApp de negocio.
  //    Formato: código de país + número, SIN espacios, signos ni "+".
  //    Ejemplo México: 52 993 123 4567  ->  "529931234567"
  const WHATSAPP_NUMBER = "529613267670";

  // 2) Tu configuración de Firebase (Firebase Console > Configuración del proyecto > SDK de Firebase).
  //    Mientras dejes "TU_API_KEY" tal cual, el registro/login queda desactivado
  //    de forma segura y el resto de la página funciona normal.
  const firebaseConfig = {
    apiKey: "TU_API_KEY",
    authDomain: "TU_PROYECTO.firebaseapp.com",
    projectId: "TU_PROYECTO",
    storageBucket: "TU_PROYECTO.appspot.com",
    messagingSenderId: "TU_ID_MENSAJERIA",
    appId: "TU_APP_ID"
  };

  /* ====================================================================== */

  const ICONS = {
    deg: '<path d="M8 3h8l1 4H7l1-4Z"/><path d="M6 7h12l1 13a1 1 0 0 1-1 1H6a1 1 0 0 1-1-1L6 7Z"/><path d="M9 12h6"/><path d="M9 16h6"/>',
    des: '<path d="M12 2s6 6.5 6 11a6 6 0 1 1-12 0c0-4.5 6-11 6-11Z"/><path d="M9.5 15.5a2.5 2.5 0 0 0 3 2.4"/>',
    loz: '<circle cx="12" cy="13" r="7"/><path d="M9 13a3 3 0 0 0 3 3"/><path d="M12 3v3"/>',
    hig: '<path d="M7 11V7a5 5 0 0 1 10 0v4"/><path d="M5 11h14l-1.2 8.4a2 2 0 0 1-2 1.6H8.2a2 2 0 0 1-2-1.6L5 11Z"/>',
    pis: '<path d="M3 17h18"/><path d="M3 21h18"/><path d="M8 17c0-5 2-9 4-13 2 4 4 8 4 13"/>',
    eqp: '<path d="M14 3l7 7-8.5 8.5L4 20l1.5-8.5L14 3Z"/><path d="M12 8l4 4"/>'
  };

  // Cada producto tiene "img": la ruta de tu foto.
  // Guarda tus fotos en una carpeta "images" junto a este archivo HTML,
  // con estos mismos nombres, y se mostrarán automáticamente.
  // Si la foto no existe todavía, se muestra el ícono de respaldo — nada se rompe.
  const PRODUCTS = [
    { id:'deg-1', cat:'cat-deg', icon:'deg', ref:'REF. DEG-01', name:'Desengrasante industrial para parrilla', pres:'Bidón 5L', img:'data:image/webp;base64,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'},
    { id:'deg-2', cat:'cat-deg', icon:'deg', ref:'REF. DEG-02', name:'Desengrasante para campanas y extractores', pres:'Bidón 5L', img:'data:image/webp;base64,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'},
    { id:'deg-3', cat:'cat-deg', icon:'deg', ref:'REF. DEG-03', name:'Desincrustante para hornos y planchas', pres:'Botella 1L', img:'https://encrypted-tbn0.gstatic.com/shopping?q=tbn:ANd9GcR2Fvg18gB5Ic29cItgFd8vmbqe-J59gB8BLEI9CHvyGABfZHgz-FGlislx5xs730MbUiWRcAHmQhfOiHpOws5oi0t1pWR0AAXW1lCO06gyumzCSnLRF3U6iZUh'},

    { id:'des-1', cat:'cat-des', icon:'des', ref:'REF. DES-01', name:'Sanitizante de superficies sin enjuague', pres:'Botella 1L', img:'https://encrypted-tbn3.gstatic.com/shopping?q=tbn:ANd9GcTwAFSS44gBrPP4cewVeFBKMXY3hCOHRyeBN19fLM72S3ijGcZieSfuFAo_hzQGEbOIcnrfBq8M_GVLi3gDNElqVcpb3rVjop8grmcephgJpVNs6vlUViHZW93rjQY773OA1gcX5No&usqp=CAc'},
    { id:'des-2', cat:'cat-des', icon:'des', ref:'REF. DES-02', name:'Desinfectante de amplio espectro', pres:'Bidón 5L', img: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSaXDsR8Y0Q5fU6EyTPZzCbC1pi83adQoTZrPyHUkyzsQ&s=10'},
    { id:'des-3', cat:'cat-des', icon:'des', ref:'REF. DES-03', name:'Gel antibacterial para manos', pres:'Bidón 3.8L', img:'https://encrypted-tbn3.gstatic.com/shopping?q=tbn:ANd9GcS6MEPDl_MdawUDoY9e2yYiQo5s10j6urwvY7yZmzeDx6WiQ9EZd24LKtxXSYeGZnif-F7IritoLGopYz9IzrpWNOeoHhDwlwRGPsmVax9K6lQn_L3RCf67E4gOsxaFsLMwQUSklw&usqp=CAc'},

    { id:'loz-1', cat:'cat-loz', icon:'loz', ref:'REF. LOZ-01', name:'Detergente líquido para trastes', pres:'Bidón 5L', img:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcReV0yxcT30ebye5iiLBJcm_Q6hp7PbNnziBdX_pCScuA&s'},
    { id:'loz-2', cat:'cat-loz', icon:'loz', ref:'REF. LOZ-02', name:'Detergente en polvo para lavaloza industrial', pres:'Saco 10kg',  img:'https://http2.mlstatic.com/D_NQ_NP_795052-MLA99346972152_112025-O.webp'},
    { id:'loz-3', cat:'cat-loz', icon:'loz', ref:'REF. LOZ-03', name:'Abrillantador para lavaloza industrial', pres:'Bidón 5L', img:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQEWsJJr09phqKc3qrLoYIEo33BNfHG1HqnS8jxxcuTdg&s=10'},

    { id:'hig-1', cat:'cat-hig', icon:'hig', ref:'REF. HIG-01', name:'Jabón antibacterial para manos', pres:'Botella 1L', img:'data:image/webp;base64,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'},
    { id:'hig-2', cat:'cat-hig', icon:'hig', ref:'REF. HIG-02', name:'Papel higiénico institucional', pres:'Paquete 12 rollos', img:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSKPNnedzPaJDCpmpXq19eq_vgeh0jLgEv91pHNyH6dzA&s=10'},
    { id:'hig-3', cat:'cat-hig', icon:'hig', ref:'REF. HIG-03', name:'Toalla interdoblada para manos', pres:'Paquete 3000 hojas', img:' https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzpgPLUsH8KVJ7tDs4duQodINS9ujV3tfvh1tVEkIUgQ&s=10'},

    { id:'pis-1', cat:'cat-pis', icon:'pis', ref:'REF. PIS-01', name:'Desengrasante para pisos de cocina', pres:'Bidón 5L', img:'https://encrypted-tbn0.gstatic.com/shopping?q=tbn:ANd9GcSYZNkSWMlDO7DXBOU0ZYtGGSaEijVcCy5ANs8k_iWjiTDKkukpavswgAoHZStW33DR4DQuy3WsnYqB0C0lUPTQvdRVlau87QZBgI6wY7g6KzFMmuq4szD8qnGfz79BdYU_6iRHy3A&usqp=CAc'},
    { id:'pis-2', cat:'cat-pis', icon:'pis', ref:'REF. PIS-02', name:'Limpiador multiusos para superficies', pres:'Botella 1L', img:'https://encrypted-tbn2.gstatic.com/shopping?q=tbn:ANd9GcTEOqm8fyAA7dDwk8StJvwUohhBAFNosUwyDWsLTrCNXMemLjpnzT33aFoAamirxBYH3nKQ7ZiBd6rA-Ytq66i3Y7WjP1t0fpDJ1pLnr_GhJhNEbxlBGEy4-rBxPf0sAHViWX4r7A&usqp=CAc'},
    { id:'pis-3', cat:'cat-pis', icon:'pis', ref:'REF. PIS-03', name:'Aromatizante de ambientes', pres:'Botella 1L', img:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS8BFJdSPfZtuWsiPy_8407vxsKaG2aYxfB2n58vVoWxg&s=10'},

    { id:'eqp-1', cat:'cat-eqp', icon:'eqp', ref:'REF. EQP-01', name:'Trapeador industrial de microfibra', pres:'Pieza', img:'data:image/webp;base64,UklGRiQVAABXRUJQVlA4IBgVAACwSQCdASrGANAAPk0kjkUioiETy5z0KATEpu3V+rBVEXVV955r1dfun9o+3HjrTDd7PMB84PQj+bfYJ/TL9UOtp5l/PF9O3+o9SD+xf5T1//Vx9Bvy6fZv/cv92PagukH4V+dfl19R+2nJY6u8x/5X9/v1H9h9uPZHwBfxz+Tf2X8uOHuAF+Xf0f/c/2L1V5qGQB5a/9XwmfPvYA8TP/0/3Pnc+pP/h/pPgG/mn9k/4nrkev394fZZ/bT/6FdZk6x/Xt7ItiJnr+WwzBCz0FjYwvEweVcm7QYG9qgc0HlXJv2XJyDHOx8126FVKJPTxaDlcHuXERfbqA1swbwtTxPyg2/zlub4n++YpN5o5mEZTE6j2H0ic0e1gHRQCKFsW3SGtwDHjyLgXoaneft/+02k5+P1ShRXQlnmPdAeSbbHpKQhbeCFOM0kFfBQIdXxZx/0n9l1fM9KmnsaKPTK9/gdrmNzXXjLglhgDSrZlr7vbaK89c1sPx7HOIo2yOAZm8Lz/yV3Mzyd/WP//79TXeZ4TWMFwOjFPf36jfvQY0kmAjk6vrs/9/U51l/Sec/yHNeIrccz3PGt5Sg9hn/LvF+1GKyILj/sdUhnZbETHpOFzWv4wK9urMuNFlvgNV3uiPjensv4P/IJLmLgU1UhGShVZAND4g0aaqEgJyiRcY6rXKEnjuS3uMH/y+9OHvlr/QWekPKkXOcmm/ZezdHf4moVeFMdMWmgjXeobpzmGbqaGKC0gmlWJdfV2RLRmDyrg/E5jAlt1lx6vnWsiYPKuTftPvX8thXAAP79gQKc8mbodO42pTqveGyfnTkl2H/ZEXCm5XKR8lDEMIHD8igpV5G6UmpgWFqf/+Vf/iDsp2Bx/4ef+MHSo9BQxOTsOY+vG4+fWJiCOMdzWWj4uRN7LPF5urBt1hVckeqX1uZABMrVGrE/jPb2x2Ao/6/H/HNSFMiFCZeLyx9PYCoDla2Oq/A8YeUTtAGfZCUxJ4RPIW35foN5Jmz2iAOsiqfml8sXhnQniwh4i68yIxHcACBvHSl88+nG936ZiRBhS0s2pyYZhujWeSXq7/JwkrHW8gsG96eL989iREugl/3Ywu/Sae7pNK/vRiwT/iC+ad9s2/MEAEKN06f5PsM3Uc4amvtdJ447neAtjI8JRi6FTzsgZPmqeKRa8+PUf8k5zaFy07/CFO3ThHMatCFY5auGXaPAH/m0UygVXrhEYksxoN+3tY6o+w+IP/9/gcqjN5DGFog3DQOHDomb95o5T1t+tBYqxHa4dFlyN8p31/uGD5sSycHwykoT1hu4bPGP7PybSBKEDBaaEX7jgbo49Bu7BCu9uJIbgdZchuhL+ZGDL+ycVxzuSik2m1zDixAbpMcO80T7LliPSMy026lkzYvS0JAJa6OmqMHQGci6gA8slBf/F9eLLZEcwa2zrzIT2JW9EC9Av4H/69KeUVU4ynDHonAxhX58T0AIvosDMuWBQ6Ojrqa2iGQqFro/E7w48HQJIGnskoViFQa+j7zu4vyl/0XifgLSKgJ9jND7CCxLT2bup8bQyK9Qy1M5j4GTrHi5srw2EOzHZ+bATDhX8jW066HvS620fe4bSSJcmQKM2Rto1tZo1lNeOOyp5f0OSE8i7+FwDAoiF0l8wr7avgnBEm3/e/YVl1BPKeieFP59bx/bX96dmyPSoveI5DL9t1WaKxQqf0p2ciQEAhPbX1h8DCufmgvT2qBtTRGlC1dNtL1BC081UVUikHYjA0xtNSmb6fy3rJjw4iGHD38BYIfnoiKsMQHd4BpNfnL8/gAVjY/z/XmpHZ3/khSZDZJy0oxVku8dsu3/8qrAGKLu9r/O6Etmjyp+zBvgDOHpVsUrjskA9rKTnpiVh8LRk/vj8+YVfEaVznKoyzzRzvHY/PKMwwa/2XkUukeFjrZAP3AKAMpOwjVSwT3QYuky4SiUYWBhK0qbWYP/aT0Pm1xELoI9cD2Gv78iNZvbSRpkmcDMNFfbZrRfIrWIhv9187Hke+UC7ogGQL8fiu+md2Y+dBT+xuZFNv5AuWNPtElazzMGwkBi5Y2fOa8QwlElEX4zi4k3zVrycHykwlEMg2qwz8M3sTRkP6imNhx7bYK9b0MA6EXxtD4HwyBljAJcBHPpyRtCdA3OLB1/5Hw+y39eP/5oTu1xFdhWu5C4bu/8519Scy5YZCdhN3aG0KNIF7EH+AiFeuLTEAJRofwUIqaM0epZEgT6fP4xvtS0FszkiPUoLQ5/lwin8BWkPee+eM8O64XaGg8rvat1+qp57ZBbwomkV9Klo9oPC7Mj8ZwVupvOYMKGw3IM8iTv2YQ+K//jIFpz1Dr4Wu9Y373KjC3FTrl1T5UBLoHW883q/+yB4IWErdO2cK5pq83Wrng3hcF61b6DtcTNdI7QRWW+aKuCgc/JDBc2qc5QUdXLJKOX2tX4gUef/yvlMV5SvXvCMLaJcVeheUKCjGh8X+zIQPQLrlYPeqau87WahT7sMft1U3RMMjSxXXWol6vPlmjI+3dVk0N74k6Uh5cs1zsWmacwkg7SvK1kFGkxEzWKsujnnWb5Cx9m2V/eLHNlL7J4eeG+2wxGyYbFsJImVAAhD24EiBp2x2phOjxudERVtm3SqJ2G1XIXWkOFcte6vVs/O9jFFzoxjjwLgkzqUvfOCE0pt1Ee7I3Y3UdutmUH0ffaI3/EZmBsvFYu+8p1D/+rbtm1HYvrjqpuAOdt+SS0MOefrGpyECpLunFGpvi7rYzOtZi7o00l+INe7Xby/M5cl+VSWFuAW4jZS+YkBulLP3FeiMWIpo4tfSY99IIDATgnp7vDPw7k7Vnvw0zIhScFdLAwNgd/mgYJopeZBqvw+CaNPdODKH5nXO0TozdH4+RCQDdNudCSM2I+WYbVfchA7KHV6Iwe34LfmEAkeqU4iMVoOscWq31A5QMPYyNCkoj3kjNfl3owmyaVS1nEGP5T/TEs6vV04xugRXlTyn+UOASbf+dfXi/1eD1MrE9rIed0s+L56kme6pTcUkisZEwGFJ7HGHfP0fEYYwzRZ5+Zrp65SqJKVDj8gwGII0/lEtN7ZTlGvWktsgPo2fWLoTiDdoiVtOXDoMLAdzsm1N18KCxyCIEWtCKEt1y2/9rZX+3DDRD2//7eljiN1xp3LxFusweKl9DpkvepgOcQkTgq8DUO50yNNytaH+DFf0mGNr6vi8EXGiB6HBZbBJtg1Azn9ytOboWw96LEuJAFZcDf4XO0jTfCU8egm6agSB+W6zugrNFuN2vDWLB32QcWe6cuzZBLH5se9x+iH/QU7XRLwx2/5MSmD3RltBrYOiItjDfTumA5d9RR/D6kAxnzoKGaSh56qGYs7KNbFOTx3Rytnm9jCd9l06lqNxPmCLPq2QZvgPouAmF0mqeVsnOTiPh/roIp7EoqrbV5q8uuCx1nt4eyukkgdmcLL+NhSLln1Dbc5QUNA8az1gBvp4vkfNadbJuduLatipXeSBePe8VtNPwImfPJYRF5eJZrFVsH8eejzr3jfJ1gFlEo7m1AvQWURIJCRG1i3qmyyGghbFHagKN7USmd4DDVncNnqh4rAJpBh1DKivlG85JjuNZ2CJJDeJKQY5jKCFK9KJ7VT/Uv6fbAoEc8A8lBwqnWDyctAI1liq0YPKoLobi9gctAT1VF/1gIKjQZju+6GRBKk8a3cLN+H4oy7/ZtNsA1sx6WNb/TKR2E3EKdks6gf/B512f5vbm/2RILvngHYbBMgQ9orQhMdH2GATVgDSiTTq+P4aaOlfWkvcT0HPZdT6ZAAC+oAVJ2cpccHgscgItJirk7e8LB1L7/3/wyfWfBSS9gNi/2IJw7Hdv4ozfbRb3vTEbMQLSZ0IOgfYK/y5ogUQ303jZWax605fLYbFzBgJmcHmV0QeqCd0wfcfjEEM9iq5VQZ+nzmKtEADBj3zzFur+0qPeK5oh2Lla2FDB85f7RjBjMlHsNkhWRtO4SwGC7QEDBmGZQ6q1AT/87DFbpBMHM3aNtbGnDe2CVCF//8KLOZTfU47+Qtkmi9UzygF37xPzMMCx0i54KcHciclDN5l5jTgQUM66dFQj7z6f4DpAmzseM5t9a6jVqbZsymaJyHbSGbxKV/3/5cSPKtCQSZxXXBsvK3Qaw3p8LEYikVVOXNaoHUAJifluhSK34CVEYU9wZdJ3XoVRJLaYD3EmnAHoZJGfN0ugQtbivpgMieTpZA0fFZIrSy/vCjH44/zIdhvwW4Wb/yEBXOoJsUhl+WxMaUxrI+3/88b5ukYV8Wj36qxMX0kH/iiNCe9a8/qwUuR5FUODs67lLKZ97GgDOxaH26O12l+9Q44beeZjAudxVPcciu+L3godf/6oX3MODWKpYwlQ3ROhWBmr7xPuCRQpvspLXdJL+PWw+k8jTwWFguR3YMBfEw8Hmvha2KzkDA+HjYWdk7HJ/nRVCstd1Ua3Q+HcUfvrQfBGrWGVQw4/6WnnFT/ot9EwMUhLD6Y1Vfe9JupIymgcaqmRe4ug4RVExrw6RcPmpbEPtHcjA/341tFVtNtG5gOnbIGsbjo89SnscC35vK/MJZoASC0thXBbuitxZIr8ZL0vswpmk92BaDdNAbEbXvjtC6iynHvWStlB0KH2Hyy7R+ZgFuM8puzHywC9J6eBqi8puipmK6iZ72sIrk8uwX/nAyJkg9wOE1bu043lj2V73OpRwU4ArbOjEUxGs8zFXkM50IkslFWlJT9JTm7dHRNhjH6e39BDOVeFsDBNbP0rtiQ4/HaxwyNnKDtXTDudUsAtP5E0TvGYv6XzAEOINTpRXsJSldWgAAmUuh/TDIy9WzDiW6VvTsOQkvx9IH5GvBQPhmQY1cXTWRvZQ384aILHgFYHNON5tnMYtMIcfE/StE5zU/5/Kd8FChRcYmDqj7PyGtWrJpoGT2rFZIAvMVj89qH6vYPgOutA5pHqL1ZHB5f+Bwa8AEXABaZmVYozSt4w1SLGsm11aCqrpKs8CJ1IdDWEduLm/lK5JlZjVRpqZo6pmmr+/qgdgv8uy3MagWNuCsBlWSykGhbW6Kqdow8DarXKiwm8NypUML8lCe7j0RtC/1ZMihBl9P0fGt3n565lcHkUF+eBK2rBEY95zCC7V4k66XuUk1Oc4aCDWkRF/hsHKFWIN+qfHZCUi7o/QlolXBFpiUQJjFmwhLUO3bG9QwHMY7yNN7VjMgLHm3+MFaaqZSzT1lT+4Wm/YtFo3Uqs0bo74eGAk64n5+NjjU5KycN/vbfHJw3VpRrW24hCjtrnLFeJoEV0QWpCUKk1YYoJ85GQzpzGBQyw+K+GySlPCuJf6MXCTNzEvHHOTZd590mgNH8zax1HgdBcwQkEaQ5oP60ebtjKzbIMo/KSsE+ESw6rvoexwuzsHPUucts9nE9Jw663GzajKL8YPGYu7/CUekFG9usZ8kc8SqRBjgmfGIaAAmtK5RsU4/XS2exzEISw84z4QtGl/WFixKYk81Ebho0su6FZISgKUE4tsob22rYeyc/QTdvupOnWCLVZ9e57ove9wrGf5LDwGcFZUPWOtRDExErZBulLqzNkL7PbXIDm6hiNg+zmN+H7FatnDFSquGTih4LUPTdlIfOkSseAlxXpHk0Mp/ZvSL+hBeqvzyae1I38xddQmksK+d+zYLEALWX4C8/oXOJtkBx2aQ87DgBicR0LHXjMMr4fWe+wHjKAABWu/y5/4P7r/g53A0rmloHX7KS7pidE3nDoER6sxpB+MahD0ZjU0t7gpsVGD7NXKiW9X7W73cZ9bMqUs4R9q9h0uO/+DkA05XS5SWHkxTExBZ0dhAzs/TU91S26fbi84Uhh54/eToNHXXsXQihqBg/4Jbkro8JkyHdW+u9NN+J8qV/uJ1aQNNy1S+bQVSa7UZk2OUkI6kHWVmNF+9ZTZkcg3/bYswoaxP2f6uU5YcmF6TyMYm0YBfPdbsFhZhG5JKKg3AeFG8Po+daPj2K0KApfEdfC4OGwQ5VAHQq8fG03l1nbqhKV0NytrfoHwCekVxaFOVyEF5Yq+qAkOT9o1hUjyu1x+B/CCrO1oKp8K04BaBnbf6wNC2nNYYmNIEboOLaPXZj0jeOvkoNblWxo35Q7h6R/EuGPPD9wIJ/9f5QKN2syaJCeJ/BwcttGuyLVr4wq4GnIVwXxeHcJHEfZU20eveSVr5xoavFEa6zW+LOLMiXGz+XQjMn9UkOvngwcDVPamZBcsuC0gsUxkFeWGY4Yblq/owAbw/Hhae/LW2ZU/1byKZ8kzsw9atVAJQtc4vo58wZGtBCkTpk38wtur9S6Pq986n4qbVAigR/vCRDw3DTfn27ZcCw8Yby7MamWQYSstqdPmaj4feNEli/yCxAwCIoMbK9g9ya17uUeFXxsDFLwUzVk1opM84mVTsahZeII+OIsKNSGNMAPIMGEMpLudRpCYa4meeZp9UdABOAqEUcAxvaBO8nXQ24M4XzuaFJj1ImUWWj13LWbYP9p7vKTM/wMj34kkBb6KPbix947Dqe5Q8t7d4992bf/7/qwLkbNa/m0DIIZ5WEp/fketaXO5nhmAxUq51fWX/fhdh6/QTZZbWsQMq4MVjLmHXVTKkteHO/UldPtrrczMH548eVreLW022d1j+zPuD8/qXo7cR053qzinECKkhjFVsu329m+RnkHOQbD1EFmk1mUG+nbitobpEikmqCd7Z73C05zmzRYy/8l8YFTjnwUpvO23Z5qPXVUIzLRPG30p7qaxOCUsUZLPI3M8AIvznbxe4+sEhTEpzb1iYlM4MSKPOyhOH81H5t+HBu2EuiAEQj+uL4vUPdpKIO8o71T/8ma9yfWWEaV5U2994zj4q/czpBAE1gF7fbRnGjTQrouX7p+FA/Jp8/KkRFTTDRz6dWj46lMJfNtE0Ss+q31KfTsHX77cjlgnMBIeM07Au0Rp23/nCJTxzk9AE69LecOkXYcQwk/lVsJiKEaamypLpThBIt9KY6nIikAKZEzkd8BB6SgmZNKVTfF4F4w3ux0d1m/+VIov3EqjhXo1LKoPMqRqjRrS5OpeK8G5Lg1IzXh2fVm+93wJTxQyT8/rbpqL1bEMux1vevkqJHG/g33gLbyu7Lk9XTqlFRsKVv7br1KZK99K3skaXxWpvT7cAo6YMsD8jGSCKXWuPNxJb4AiUWfsZqBGW4AAAAAAAAA='},
    { id:'eqp-2', cat:'cat-eqp', icon:'eqp', ref:'REF. EQP-02', name:'Cubeta con exprimidor de trapeador', pres:'Pieza', img:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSlpHYTY4D0yVBPcXC33JY4SWI8Spi_6GnU1dl6KeeAzg&s=10'},
    { id:'eqp-3', cat:'cat-eqp', icon:'eqp', ref:'REF. EQP-03', name:'Dispensador de jabón para pared', pres:'Pieza', img:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR4bExPpBdWBcqWaFTjinKRhfaF0xUzkQ_jWgiDbC0jmg&s=10'}
  ];

  let cart = {};        // id -> qty
  let currentUser = null; // { uid, email, negocio, contacto, telefono } | null

  /* ---------------------------------------------------------------------
     RENDER DE CATÁLOGO
     --------------------------------------------------------------------- */
  function renderCatalog(){
    const groups = {};
    PRODUCTS.forEach(p=>{
      if(!groups[p.cat]) groups[p.cat] = [];
      groups[p.cat].push(p);
    });
    Object.keys(groups).forEach(catId=>{
      const gridEl = document.querySelector(`[data-grid="${catId}"]`);
      if(!gridEl) return;
      gridEl.innerHTML = groups[catId].map(p => cardHTML(p)).join('');
    });
  }

 function mediaHTML(p, fallbackSize){
    return `
      <div class="card-media-fallback">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">${ICONS[p.icon] || ''}</svg>
      </div>
      <img src="${p.img}" alt="${p.name}" loading="lazy" onload="this.classList.add('loaded')" onerror="this.remove()">
    `;
  }

  function cardHTML(p){
    return `
    <div class="card" id="card-${p.id}">
      <div class="card-media">
        ${mediaHTML(p)}
        <span class="card-ref">${p.ref}</span>
      </div>
      <div class="card-content">
        <h4>${p.name}</h4>
        <span class="card-pres">${p.pres}</span>
        <div class="card-bottom">
          <div class="stepper">
            <button type="button" aria-label="Quitar uno" onclick="changeQty('${p.id}', -1)">−</button>
            <span class="qty" id="qty-${p.id}">0</span>
            <button type="button" aria-label="Agregar uno" onclick="changeQty('${p.id}', 1)">+</button>
          </div>
        </div>
      </div>
    </div>`;
  }

  /* ---------------------------------------------------------------------
     CARRITO
     --------------------------------------------------------------------- */
  function changeQty(id, delta){
    const current = cart[id] || 0;
    const next = Math.max(0, current + delta);
    cart[id] = next;
    if(next === 0) delete cart[id];

    const qtyEl = document.getElementById(`qty-${id}`);
    if(qtyEl) qtyEl.textContent = next;
    const cardEl = document.getElementById(`card-${id}`);
    if(cardEl) cardEl.classList.toggle('in-cart', next > 0);

    updateCartBadge();
    renderCartDrawer();
    if(delta > 0) showToast('Agregado a tu pedido');
  }

  function setQty(id, value){
    const next = Math.max(0, value);
    cart[id] = next;
    if(next === 0) delete cart[id];
    const qtyEl = document.getElementById(`qty-${id}`);
    if(qtyEl) qtyEl.textContent = next;
    const cardEl = document.getElementById(`card-${id}`);
    if(cardEl) cardEl.classList.toggle('in-cart', next > 0);
    updateCartBadge();
    renderCartDrawer();
  }

  function totalUnits(){ return Object.values(cart).reduce((a,b)=>a+b,0); }
  function totalLines(){ return Object.keys(cart).length; }

  function updateCartBadge(){
    const el = document.getElementById('cartCount');
    if(!el) return;
    const units = totalUnits();
    el.textContent = units;
    el.dataset.empty = units === 0 ? 'true' : 'false';
    el.classList.remove('bump');
    requestAnimationFrame(()=> el.classList.add('bump'));
  }

  function renderCartDrawer(){
    const wrap = document.getElementById('cartItems');
    if(!wrap) return;
    const ids = Object.keys(cart);
    document.getElementById('cartLinesCount').textContent = totalLines();
    document.getElementById('cartUnitsCount').textContent = totalUnits();
    document.getElementById('checkoutBtn').disabled = ids.length === 0;

    if(ids.length === 0){
      wrap.innerHTML = `
        <div class="cart-empty">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M6 6h15l-1.5 9h-12L6 6Z"/><path d="M6 6 4.5 3H2"/></svg>
          <span>Tu pedido está vacío.<br>Agrega productos desde el catálogo.</span>
        </div>`;
      return;
    }

    wrap.innerHTML = ids.map(id=>{
      const p = PRODUCTS.find(x=>x.id===id);
      if(!p) return '';
      const qty = cart[id];
      return `
      <div class="cart-row">
        <div class="cart-row-media">${mediaHTML(p)}</div>
        <div class="cart-row-info">
          <h5>${p.name}</h5>
          <span>${p.pres}</span>
          <div class="cart-row-actions">
            <div class="stepper">
              <button type="button" onclick="changeQty('${p.id}', -1)">−</button>
              <span class="qty">${qty}</span>
              <button type="button" onclick="changeQty('${p.id}', 1)">+</button>
            </div>
          </div>
          <button type="button" class="cart-row-remove" onclick="setQty('${p.id}', 0)">Quitar</button>
        </div>
      </div>`;
    }).join('');
  }

  /* ---------------------------------------------------------------------
     OVERLAY / DRAWER / MODALES
     --------------------------------------------------------------------- */
  function openCart(){
    document.getElementById('overlay').classList.add('show');
    document.getElementById('cartDrawer').classList.add('open');
    document.body.classList.add('lock');
  }
  function closeCart(){
    document.getElementById('cartDrawer').classList.remove('open');
    if(!document.getElementById('checkoutModal').classList.contains('show') &&
       !document.getElementById('authModal').classList.contains('show')){
      document.getElementById('overlay').classList.remove('show');
      document.body.classList.remove('lock');
    }
  }
  function openCheckout(){
    if(totalLines() === 0) return;
    renderModalSummary();
    if(currentUser){
      const negocioEl = document.getElementById('negocio');
      const contactoEl = document.getElementById('contacto2');
      const telEl = document.getElementById('telefono');
      if(negocioEl && !negocioEl.value) negocioEl.value = currentUser.negocio || '';
      if(contactoEl && !contactoEl.value) contactoEl.value = currentUser.contacto || '';
      if(telEl && !telEl.value) telEl.value = currentUser.telefono || '';
    }
    document.getElementById('cartDrawer').classList.remove('open');
    document.getElementById('overlay').classList.add('show');
    document.getElementById('checkoutModal').classList.add('show');
    document.body.classList.add('lock');
  }
  function closeCheckout(){
    document.getElementById('checkoutModal').classList.remove('show');
    document.getElementById('overlay').classList.remove('show');
    document.body.classList.remove('lock');
  }
  function openAuth(){
    clearAuthError();
    document.getElementById('overlay').classList.add('show');
    document.getElementById('authModal').classList.add('show');
    document.body.classList.add('lock');
  }
  function closeAuth(){
    document.getElementById('authModal').classList.remove('show');
    document.getElementById('overlay').classList.remove('show');
    document.body.classList.remove('lock');
  }
  function closeAll(){
    closeCart();
    closeCheckout();
    closeAuth();
    document.getElementById('overlay').classList.remove('show');
    document.body.classList.remove('lock');
  }

  function renderModalSummary(){
    const ids = Object.keys(cart);
    const el = document.getElementById('modalSummary');
    if(!el) return;
    el.innerHTML = ids.map(id=>{
      const p = PRODUCTS.find(x=>x.id===id);
      if(!p) return '';
      return `<div><span>${p.name} (${p.pres})</span><span>x${cart[id]}</span></div>`;
    }).join('');
  }

  function showToast(msg){
    const t = document.getElementById('toast');
    if(!t) return;
    document.getElementById('toastMsg').textContent = msg;
    t.classList.add('show');
    clearTimeout(window._toastTimer);
    window._toastTimer = setTimeout(()=> t.classList.remove('show'), 2400);
  }

  function toggleMobileMenu(){
    const el = document.getElementById('mobileMenu');
    if(el) el.classList.toggle('open');
  }

  /* ---------------------------------------------------------------------
     ENVÍO DE PEDIDO POR WHATSAPP
     --------------------------------------------------------------------- */
  function sendOrder(e){
    e.preventDefault();
    try{
      const negocio = document.getElementById('negocio').value.trim();
      const contacto = document.getElementById('contacto2').value.trim();
      const telefono = document.getElementById('telefono').value.trim();
      const direccion = document.getElementById('direccion').value.trim();
      const notas = document.getElementById('notas').value.trim();

      if(!negocio || !contacto || !telefono || totalLines() === 0) return false;

      const lines = [];
      lines.push('📄 *Nuevo pedido*');
      lines.push('');
      lines.push(`🏬 Negocio: ${negocio}`);
      lines.push(`👤 Solicita: ${contacto}`);
      lines.push(`📞 Teléfono: ${telefono}`);
      if(direccion) lines.push(`📍 Dirección / sucursal: ${direccion}`);
      lines.push('');
      lines.push('🛒 *Productos solicitados:*');
      Object.keys(cart).forEach((id, i)=>{
        const p = PRODUCTS.find(x=>x.id===id);
        if(!p) return;
        lines.push(`${i+1}. ${p.name} (${p.pres}) — cantidad: ${cart[id]}`);
      });
      lines.push('');
      if(notas) lines.push(`📄 Notas: ${notas}`);
      lines.push('');
      lines.push('Quedo al pendiente de la cotización, gracias.');

      const message = lines.join('\n');
      const url = `https://wa.me/${WHATSAPP_NUMBER}?text=${encodeURIComponent(message)}`;
      window.open(url, '_blank');
      closeCheckout();
      showToast('Pedido listo — revisa WhatsApp para enviarlo');
    } catch(err){
      console.error('No se pudo generar el pedido:', err);
      showToast('Hubo un problema al armar el pedido, intenta de nuevo');
    }
    return false;
  }

  /* ---------------------------------------------------------------------
     CATEGORÍAS: NAV + SCROLLSPY
     --------------------------------------------------------------------- */
  function initCatNav(){
    const pills = Array.from(document.querySelectorAll('.cat-pill'));
    pills.forEach(pill=>{
      pill.addEventListener('click', ()=>{
        const target = document.getElementById(pill.dataset.target);
        if(target){
          const offset = 150;
          window.scrollTo({ top: target.getBoundingClientRect().top + window.scrollY - offset, behavior:'smooth' });
        }
      });
    });
    const groups = pills.map(p=>document.getElementById(p.dataset.target)).filter(Boolean);
    if(!('IntersectionObserver' in window) || groups.length === 0) return;
    const observer = new IntersectionObserver((entries)=>{
      entries.forEach(entry=>{
        if(entry.isIntersecting){
          const idx = groups.indexOf(entry.target);
          pills.forEach(p=>p.classList.remove('active'));
          if(idx>-1 && pills[idx]) pills[idx].classList.add('active');
        }
      });
    }, { rootMargin:'-160px 0px -60% 0px', threshold:0 });
    groups.forEach(g=> observer.observe(g));
  }

  /* =======================================================================
     FIREBASE — AUTENTICACIÓN Y PERFIL DE CLIENTE
     Todo va protegido con try/catch: si Firebase no está configurado o
     falla la conexión, la página sigue funcionando normal sin login.
     ======================================================================= */
  let firebaseReady = false;
  let fbAuth = null;
  let fbDb = null;

  function initFirebase(){
    try{
      const isConfigured = firebaseConfig && firebaseConfig.apiKey && firebaseConfig.apiKey !== 'TU_API_KEY';
      if(!isConfigured || typeof firebase === 'undefined'){
        firebaseReady = false;
        return;
      }
      firebase.initializeApp(firebaseConfig);
      fbAuth = firebase.auth();
      fbDb = firebase.firestore();
      firebaseReady = true;

      fbAuth.onAuthStateChanged(async (user)=>{
        if(user){
          let profile = {};
          try{
            const doc = await fbDb.collection('clientes').doc(user.uid).get();
            if(doc.exists) profile = doc.data();
          } catch(err){
            console.error('No se pudo leer el perfil del cliente:', err);
          }
          currentUser = {
            uid: user.uid,
            email: user.email || '',
            negocio: profile.negocio || '',
            contacto: profile.contacto || '',
            telefono: profile.telefono || ''
          };
        } else {
          currentUser = null;
        }
        updateAccountUI();
      });
    } catch(err){
      console.error('Firebase no se pudo inicializar:', err);
      firebaseReady = false;
    }
  }

  function updateAccountUI(){
    const btn = document.getElementById('accountBtn');
    const label = document.getElementById('accountBtnLabel');
    const loggedInView = document.getElementById('authLoggedInView');
    const formsView = document.getElementById('authFormsView');
    if(!btn || !label) return;

    if(currentUser){
      label.textContent = currentUser.negocio || currentUser.email || 'Mi cuenta';
      btn.onclick = openAuth;
      if(loggedInView) loggedInView.style.display = 'block';
      if(formsView) formsView.style.display = 'none';
      const nameEl = document.getElementById('loggedInName');
      const emailEl = document.getElementById('loggedInEmail');
      if(nameEl) nameEl.textContent = currentUser.negocio || 'Cliente';
      if(emailEl) emailEl.textContent = currentUser.email || '';
    } else {
      label.textContent = 'Iniciar sesión';
      btn.onclick = openAuth;
      if(loggedInView) loggedInView.style.display = 'none';
      if(formsView) formsView.style.display = 'block';
    }
  }

  function switchAuthTab(tab){
    const tabLogin = document.getElementById('tabLogin');
    const tabRegister = document.getElementById('tabRegister');
    const panelLogin = document.getElementById('panelLogin');
    const panelRegister = document.getElementById('panelRegister');
    if(!tabLogin || !tabRegister || !panelLogin || !panelRegister) return;
    clearAuthError();
    if(tab === 'register'){
      tabRegister.classList.add('active'); tabLogin.classList.remove('active');
      panelRegister.classList.add('active'); panelLogin.classList.remove('active');
    } else {
      tabLogin.classList.add('active'); tabRegister.classList.remove('active');
      panelLogin.classList.add('active'); panelRegister.classList.remove('active');
    }
  }

  function showAuthError(msg){
    const el = document.getElementById('authError');
    if(!el) return;
    el.textContent = msg;
    el.classList.add('show');
  }
  function clearAuthError(){
    const el = document.getElementById('authError');
    if(!el) return;
    el.textContent = '';
    el.classList.remove('show');
  }

  function mapFirebaseError(err){
    const code = err && err.code ? err.code : '';
    const map = {
      'auth/email-already-in-use': 'Ese correo ya tiene una cuenta registrada.',
      'auth/invalid-email': 'El correo no es válido.',
      'auth/weak-password': 'La contraseña debe tener al menos 6 caracteres.',
      'auth/user-not-found': 'No encontramos una cuenta con ese correo.',
      'auth/wrong-password': 'La contraseña es incorrecta.',
      'auth/invalid-credential': 'Correo o contraseña incorrectos.',
      'auth/too-many-requests': 'Demasiados intentos. Espera un momento e inténtalo de nuevo.',
      'auth/network-request-failed': 'Problema de conexión. Revisa tu internet e intenta de nuevo.'
    };
    return map[code] || (err && err.message) || 'Ocurrió un error inesperado. Intenta de nuevo.';
  }

  async function handleLogin(e){
    e.preventDefault();
    clearAuthError();

    if(!firebaseReady){
      showAuthError('El registro con Firebase todavía no está configurado en esta página.');
      return false;
    }

    const emailEl = document.getElementById('loginEmail');
    const passEl = document.getElementById('loginPassword');
    const btn = document.getElementById('loginBtn');
    if(!emailEl || !passEl) return false;

    const email = emailEl.value.trim();
    const password = passEl.value;

    if(!email || !password){
      showAuthError('Completa correo y contraseña.');
      return false;
    }

    try{
      if(btn){ btn.disabled = true; btn.textContent = 'Entrando...'; }
      await fbAuth.signInWithEmailAndPassword(email, password);
      showToast('Sesión iniciada');
      closeAuth();
    } catch(err){
      console.error('Error de inicio de sesión:', err);
      showAuthError(mapFirebaseError(err));
    } finally {
      if(btn){ btn.disabled = false; btn.textContent = 'Iniciar sesión'; }
    }
    return false;
  }

  async function handleRegister(e){
    e.preventDefault();
    clearAuthError();

    if(!firebaseReady){
      showAuthError('El registro con Firebase todavía no está configurado en esta página.');
      return false;
    }

    const negocioEl = document.getElementById('regNegocio');
    const contactoEl = document.getElementById('regContacto');
    const telefonoEl = document.getElementById('regTelefono');
    const emailEl = document.getElementById('regEmail');
    const passEl = document.getElementById('regPassword');
    const pass2El = document.getElementById('regPassword2');
    const btn = document.getElementById('registerBtn');
    if(!negocioEl || !contactoEl || !telefonoEl || !emailEl || !passEl || !pass2El) return false;

    const negocio = negocioEl.value.trim();
    const contacto = contactoEl.value.trim();
    const telefono = telefonoEl.value.trim();
    const email = emailEl.value.trim();
    const password = passEl.value;
    const password2 = pass2El.value;

    if(!negocio || !contacto || !telefono || !email || !password || !password2){
      showAuthError('Completa todos los campos.');
      return false;
    }
    if(password.length < 6){
      showAuthError('La contraseña debe tener al menos 6 caracteres.');
      return false;
    }
    if(password !== password2){
      showAuthError('Las contraseñas no coinciden.');
      return false;
    }

    try{
      if(btn){ btn.disabled = true; btn.textContent = 'Creando cuenta...'; }
      const cred = await fbAuth.createUserWithEmailAndPassword(email, password);
      try{
        await fbDb.collection('clientes').doc(cred.user.uid).set({
          negocio, contacto, telefono, email,
          creadoEn: firebase.firestore.FieldValue.serverTimestamp()
        });
      } catch(err){
        console.error('La cuenta se creó pero no se pudo guardar el perfil:', err);
      }
      showToast('Cuenta creada, ¡bienvenido!');
      closeAuth();
    } catch(err){
      console.error('Error de registro:', err);
      showAuthError(mapFirebaseError(err));
    } finally {
      if(btn){ btn.disabled = false; btn.textContent = 'Crear cuenta'; }
    }
    return false;
  }

  async function handleLogout(){
    try{
      if(firebaseReady && fbAuth){
        await fbAuth.signOut();
      } else {
        currentUser = null;
        updateAccountUI();
      }
      showToast('Sesión cerrada');
      closeAuth();
    } catch(err){
      console.error('Error al cerrar sesión:', err);
      showToast('No se pudo cerrar sesión, intenta de nuevo');
    }
  }

  /* ---------------------------------------------------------------------
     INICIALIZACIÓN
     --------------------------------------------------------------------- */
  document.addEventListener('DOMContentLoaded', function(){
    try{ renderCatalog(); } catch(err){ console.error('Error al renderizar el catálogo:', err); }
    try{ initCatNav(); } catch(err){ console.error('Error al iniciar la navegación de categorías:', err); }
    try{ initFirebase(); } catch(err){ console.error('Error al iniciar Firebase:', err); }

    const note = document.getElementById('authDisabledNote');
    if(note){
      // Se muestra el aviso solo si Firebase de verdad no quedó listo.
      setTimeout(()=>{ if(!firebaseReady) note.classList.add('show'); }, 0);
    }
    updateAccountUI();
  });
</script>

</body>
</html>
