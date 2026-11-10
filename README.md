# las-aceitunas.com
<!DOCTYPE html>
<html lang="es-AR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Luz & Meme — Dupla creativa</title>
<meta name="description" content="Luz & Meme, dupla creativa publicitaria. Copy y arte. Ideas con carozo.">
<meta property="og:title" content="Luz & Meme — Dupla creativa">
<meta property="og:description" content="Ideas con carozo. Portfolio de nuestra dupla creativa.">
<meta property="og:image" content="assets/img/og.jpg">
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Cellipse cx='50' cy='56' rx='32' ry='40' fill='%235E6B2C'/%3E%3Cellipse cx='50' cy='22' rx='13' ry='8' fill='%23D9472B'/%3E%3C/svg%3E">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400..900;1,9..144,400..900&family=DM+Sans:wght@400;500;700&display=swap" rel="stylesheet">
<style>
  :root{
    --crema:#F3ECDB; --papel:#FBF7EE;
    --oliva:#5E6B2C; --oliva-osc:#3B4320; --oliva-clara:#B5BE7A;
    --bordo:#6E1F30; --bordo-osc:#3E1019; --morron:#D9472B;
    --tinta:#221D19; --gris:#6F675C; --linea:rgba(34,29,25,.15);
    --serif:"Fraunces",Georgia,serif; --sans:"DM Sans",system-ui,-apple-system,sans-serif;
    --radio:22px;
  }
  *{box-sizing:border-box;margin:0;padding:0}
  html{scroll-behavior:smooth}
  body{font-family:var(--sans);background:var(--crema);color:var(--tinta);line-height:1.6;-webkit-font-smoothing:antialiased;overflow-x:clip}
  body::before{content:"";position:fixed;inset:0;pointer-events:none;z-index:100;opacity:.08;mix-blend-mode:multiply;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='160' height='160'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='.9' numOctaves='3'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E")}
  img,video,iframe{display:block;max-width:100%}
  a{color:inherit}
  ::selection{background:var(--oliva);color:var(--crema)}
  h1,h2,h3,h4{font-family:var(--serif);font-weight:800;line-height:1.02;letter-spacing:-.01em}
  h1 em,h2 em{font-style:italic;font-weight:700;color:var(--bordo)}
  .eyebrow{font-size:.78rem;letter-spacing:.22em;text-transform:uppercase;font-weight:700;color:var(--oliva)}

  /* NAV */
  nav{position:sticky;top:0;z-index:20;display:flex;justify-content:space-between;align-items:center;padding:16px 6vw;background:rgba(243,236,219,.88);backdrop-filter:blur(10px);-webkit-backdrop-filter:blur(10px);border-bottom:1px solid var(--linea)}
  .logo{font-family:var(--serif);font-weight:800;font-style:italic;font-size:1.4rem;background:none;border:0;cursor:pointer;color:var(--bordo);display:flex;align-items:center;gap:8px}
  .logo svg{width:20px;aspect-ratio:100/130;transform:rotate(-15deg)}
  .logo.giro{animation:giro .5s ease}
  @keyframes giro{50%{transform:rotateX(90deg)}}
  .amp{color:var(--oliva)}
  nav ul{display:flex;gap:28px;list-style:none}
  nav ul a{text-decoration:none;font-size:.95rem;font-weight:500}
  nav ul a:hover{color:var(--bordo)}

  /* HERO */
  .hero{min-height:calc(100vh - 70px);display:grid;grid-template-columns:1.25fr .75fr;align-items:center;gap:4vw;padding:60px 6vw 90px}
  .hero h1{font-size:clamp(3.2rem,10vw,8.5rem);margin:18px 0 26px;color:var(--oliva-osc)}
  .lead{font-size:clamp(1.05rem,1.6vw,1.25rem);max-width:42ch;color:var(--gris)}
  .lead strong{color:var(--tinta)}
  .ctas{display:flex;flex-wrap:wrap;gap:12px;margin-top:34px}
  .btn{display:inline-flex;align-items:center;gap:8px;padding:14px 26px;border-radius:999px;background:var(--bordo);color:var(--crema);text-decoration:none;font:inherit;font-weight:700;border:2px solid var(--bordo);cursor:pointer;transition:transform .2s,background .2s,color .2s}
  .btn:hover{transform:translateY(-2px);background:var(--bordo-osc);border-color:var(--bordo-osc)}
  .btn-linea{background:transparent;color:var(--bordo)}
  .btn-linea:hover{background:var(--bordo);color:var(--crema)}
  .frasco{position:relative;aspect-ratio:1;width:100%;max-width:440px;justify-self:center}
  .frasco .o{position:absolute;width:44%;aspect-ratio:100/130;filter:drop-shadow(0 18px 22px rgba(34,29,25,.25))}
  .frasco .o1{left:14%;top:20%;rotate:-18deg;animation:flotar 6s ease-in-out infinite}
  .frasco .o2{right:12%;top:30%;rotate:22deg;animation:flotar 6s ease-in-out -3s infinite}
  @keyframes flotar{50%{translate:0 -14px}}
  .sello{position:absolute;inset:0;width:100%;height:100%;animation:girar 24s linear infinite}
  .sello text{font-family:var(--sans);font-weight:700;font-size:6.4px;fill:var(--bordo)}
  @keyframes girar{to{transform:rotate(360deg)}}

  /* CINTA */
  .cinta{background:var(--bordo);color:var(--crema);overflow:hidden;padding:14px 0;border-block:2px solid var(--tinta);transform:rotate(-1.2deg);margin:0 -2vw}
  .cinta-track{display:flex;width:max-content;animation:cinta 30s linear infinite}
  .cinta span{font-family:var(--serif);font-style:italic;font-weight:700;font-size:clamp(1.2rem,2.4vw,1.9rem);padding-right:.6em;white-space:nowrap}
  .cinta i{color:var(--oliva-clara);font-style:normal}
  @keyframes cinta{to{transform:translateX(-50%)}}

  /* SECCIONES */
  section{padding:120px 6vw}
  .sec-head{display:flex;flex-wrap:wrap;justify-content:space-between;align-items:flex-end;gap:24px;margin-bottom:48px}
  h2{font-size:clamp(2.4rem,6vw,4.6rem);color:var(--oliva-osc);margin-top:12px}
  .sec-head p{max-width:44ch;color:var(--gris);font-size:1.05rem}

  /* NOSOTRAS */
  .nosotras{display:grid;grid-template-columns:repeat(auto-fit,minmax(min(100%,320px),1fr));gap:28px}
  .persona{border-radius:var(--radio);padding:34px;color:var(--crema);min-height:420px;display:flex;flex-direction:column;position:relative;overflow:hidden}
  .persona.verde{background:var(--oliva)}
  .persona.negra{background:var(--bordo-osc)}
  .persona .foto{width:112px;height:112px;border-radius:50%;object-fit:cover;border:3px solid var(--crema);margin-bottom:22px}
  .persona .foto-oliva{width:74px;aspect-ratio:100/130;margin-bottom:22px;rotate:-14deg}
  .persona small{letter-spacing:.2em;text-transform:uppercase;font-weight:700;font-size:.75rem;opacity:.75}
  .persona h3{font-size:clamp(2rem,4vw,2.6rem);margin:6px 0 14px}
  .persona p{opacity:.9;flex:1}
  .persona .links{display:flex;flex-wrap:wrap;gap:10px;margin-top:24px}
  .pill{display:inline-flex;align-items:center;gap:6px;padding:9px 18px;border-radius:999px;border:1.5px solid currentColor;text-decoration:none;font-weight:700;font-size:.88rem;transition:.2s}
  .persona .pill:hover{background:var(--crema);color:var(--tinta)}
  .pill.falta{border-style:dashed;opacity:.55;pointer-events:none}
  .pendiente{font-style:italic;opacity:.6;border-bottom:1px dashed currentColor}

  /* IDEAS */
  .filtros{display:flex;flex-wrap:wrap;gap:10px;margin-bottom:36px}
  .filtros button{font:inherit;font-weight:600;font-size:.92rem;padding:9px 20px;border-radius:999px;border:1.5px solid var(--oliva-osc);background:transparent;color:var(--oliva-osc);cursor:pointer;transition:.2s}
  .filtros button:hover{background:rgba(94,107,44,.12)}
  .filtros button.activo{background:var(--oliva-osc);color:var(--crema)}
  .grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(min(100%,320px),1fr));gap:28px}
  .card{background:var(--papel);border:1.5px solid var(--tinta);border-radius:var(--radio);overflow:hidden;cursor:pointer;display:flex;flex-direction:column;transition:transform .25s,box-shadow .25s}
  .card:hover,.card:focus-visible{transform:translate(-4px,-4px);box-shadow:6px 6px 0 var(--bordo);outline:none}
  .portada{aspect-ratio:4/3;position:relative;overflow:hidden}
  .portada img{width:100%;height:100%;object-fit:cover}
  .portada.generada{display:flex;align-items:flex-end;padding:22px}
  .portada-titulo{font-family:var(--serif);font-weight:800;font-style:italic;font-size:clamp(1.7rem,3vw,2.3rem);line-height:1;position:relative;z-index:1;max-width:78%}
  .portada-oliva{position:absolute;width:36%;aspect-ratio:100/130;right:-3%;top:-6%;rotate:24deg;transition:transform .5s}
  .card:hover .portada-oliva{transform:rotate(-14deg) translateY(10px)}
  .card-body{padding:20px 22px 24px;border-top:1.5px solid var(--tinta);flex:1}
  .tag{font-size:.72rem;letter-spacing:.18em;text-transform:uppercase;font-weight:700;color:var(--bordo)}
  .card h3{font-size:1.5rem;margin:8px 0 6px}
  .card p{color:var(--gris);font-size:.95rem}
  .premio{display:inline-block;margin-top:14px;font-size:.78rem;font-weight:700;padding:5px 12px;border-radius:999px;background:var(--oliva-clara);color:var(--oliva-osc)}

  /* MODAL */
  .modal{position:fixed;inset:0;z-index:50;background:rgba(34,29,25,.72);display:none;align-items:flex-start;justify-content:center;padding:4vh 16px;overflow-y:auto}
  .modal.abierto{display:flex}
  .modal-box{background:var(--crema);border-radius:28px;max-width:960px;width:100%;position:relative;overflow:hidden;animation:subir .35s ease}
  @keyframes subir{from{opacity:0;transform:translateY(30px)}}
  .modal .portada{aspect-ratio:16/7}
  .modal .portada.generada{padding:clamp(22px,4vw,44px)}
  .modal .portada-titulo{font-size:clamp(2.2rem,6vw,4.2rem)}
  .modal .portada-oliva{width:20%}
  .cerrar{position:absolute;top:16px;right:16px;z-index:2;width:44px;height:44px;border-radius:50%;border:none;background:var(--crema);color:var(--tinta);font-size:1.5rem;cursor:pointer;box-shadow:0 4px 14px rgba(0,0,0,.2)}
  .modal-body{padding:clamp(24px,5vw,56px)}
  .modal-body h3{font-size:clamp(2rem,5vw,3.4rem);color:var(--oliva-osc);margin:10px 0 20px}
  .meta{display:flex;flex-wrap:wrap;gap:12px 40px;padding:18px 0;border-block:1.5px solid var(--linea);margin-bottom:28px}
  .meta dt{font-size:.7rem;letter-spacing:.18em;text-transform:uppercase;font-weight:700;color:var(--bordo)}
  .meta dd{font-weight:600}
  .desc{font-size:1.15rem;max-width:62ch;margin-bottom:30px}
  .concepto{font-family:var(--serif);font-style:italic;font-size:clamp(1.4rem,3vw,2rem);color:var(--bordo);line-height:1.2;padding-left:20px;border-left:4px solid var(--oliva);margin-bottom:40px}
  .concepto small{display:block;font-family:var(--sans);font-style:normal;font-size:.7rem;letter-spacing:.18em;text-transform:uppercase;font-weight:700;color:var(--oliva);margin-bottom:6px}
  .bloques{display:grid;grid-template-columns:repeat(auto-fit,minmax(min(100%,220px),1fr));gap:18px;margin-bottom:40px}
  .bloque{background:var(--papel);border-radius:18px;padding:22px}
  .bloque h4{font-size:1.2rem;color:var(--bordo);margin-bottom:8px}
  .sub-titulo{font-size:1.6rem;color:var(--oliva-osc);margin-bottom:16px}
  .titulares{display:grid;gap:14px;margin-bottom:40px}
  .titulares blockquote{background:var(--bordo);color:var(--crema);border-radius:18px;padding:26px 28px;font-family:var(--serif);font-size:clamp(1.1rem,2.2vw,1.45rem);line-height:1.35}
  .titulares blockquote.vacio{background:transparent;color:var(--gris);border:2px dashed rgba(34,29,25,.3);font-style:italic;font-size:1rem}
  .galeria{display:grid;grid-template-columns:repeat(auto-fit,minmax(min(100%,260px),1fr));gap:18px;margin-bottom:40px}
  .media{grid-column:1/-1}
  .media.medio,.media.vertical{grid-column:auto}
  .media img,.media video{width:100%;border-radius:16px}
  .media iframe{width:100%;aspect-ratio:16/9;border:0;border-radius:16px;background:var(--tinta)}
  .media.vertical img,.media.vertical video,.media.vertical iframe{aspect-ratio:9/16;width:min(100%,380px);margin:0 auto;object-fit:cover}
  .media figcaption{font-size:.85rem;color:var(--gris);margin-top:8px;text-align:center}
  .hueco{border:2px dashed rgba(34,29,25,.3);border-radius:16px;min-height:200px;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:4px;color:var(--gris);font-weight:600;text-align:center;padding:20px}
  .media.vertical .hueco{aspect-ratio:9/16;min-height:0;width:min(100%,300px);margin:0 auto}
  .hueco small{font-weight:400;text-transform:uppercase;letter-spacing:.15em;font-size:.7rem}
  .extra{margin-bottom:40px}
  .extra p{max-width:62ch}
  .links-proy{display:flex;flex-wrap:wrap;gap:10px;margin-bottom:40px}
  .links-proy .pill{color:var(--bordo)}
  .links-proy .pill:hover{background:var(--bordo);color:var(--crema)}
  .navegar{display:flex;justify-content:space-between;gap:12px;border-top:1.5px solid var(--linea);padding-top:24px}
  .navegar button{background:none;border:none;font-family:var(--serif);font-weight:700;font-style:italic;font-size:1.15rem;color:var(--oliva-osc);cursor:pointer;text-align:left}
  .navegar button:last-child{text-align:right}
  .navegar button:hover{color:var(--bordo)}

  /* CONTACTO */
  #contacto{background:var(--oliva-osc);color:var(--crema);border-radius:36px 36px 0 0}
  #contacto h2{color:var(--crema)}
  #contacto h2 em{color:var(--oliva-clara)}
  #contacto .eyebrow{color:var(--oliva-clara)}
  .contacto{display:grid;grid-template-columns:1fr 1fr;gap:6vw;align-items:start}
  .contacto .sub{opacity:.8;margin:18px 0 30px;max-width:40ch}
  .mail-grande{font-family:var(--serif);font-style:italic;font-weight:700;font-size:clamp(1.3rem,2.8vw,2rem);word-break:break-all;text-decoration:none;border-bottom:2px solid var(--oliva-clara)}
  .redes{display:flex;flex-wrap:wrap;gap:10px;margin-top:28px}
  .redes .pill:hover{background:var(--crema);color:var(--oliva-osc)}
  form{display:grid;gap:14px}
  input,textarea{font:inherit;background:rgba(243,236,219,.08);border:1.5px solid rgba(243,236,219,.3);color:var(--crema);padding:14px 18px;border-radius:14px}
  input::placeholder,textarea::placeholder{color:rgba(243,236,219,.55)}
  input:focus,textarea:focus{outline:none;border-color:var(--oliva-clara)}
  textarea{min-height:140px;resize:vertical}
  #contacto .btn{background:var(--crema);color:var(--oliva-osc);border-color:var(--crema);justify-self:start}
  .estado{font-size:.9rem;min-height:1.4em}
  footer{background:var(--oliva-osc);color:rgba(243,236,219,.7);padding:28px 6vw 34px;display:flex;justify-content:space-between;flex-wrap:wrap;gap:12px;font-size:.88rem;border-top:1px solid rgba(243,236,219,.15)}

  @media (max-width:820px){
    nav ul{gap:16px}
    nav ul a{font-size:.85rem}
    .hero{grid-template-columns:1fr;min-height:auto;padding-top:40px}
    .frasco{max-width:300px}
    .contacto{grid-template-columns:1fr}
    section{padding:84px 6vw}
  }
  @media (max-width:420px){ nav ul li:first-child{display:none} }
  @media (prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}}
</style>
</head>
<body>

<!-- Aceitunas (se reutilizan en todo el sitio) -->
<svg width="0" height="0" style="position:absolute" aria-hidden="true">
  <defs>
    <symbol id="oliva-verde" viewBox="0 0 100 130">
      <ellipse cx="50" cy="68" rx="42" ry="56" fill="#6E7B33"/>
      <ellipse cx="34" cy="56" rx="9" ry="20" fill="#B5BE7A" opacity=".5" transform="rotate(-18 34 56)"/>
      <ellipse cx="50" cy="20" rx="18" ry="10" fill="#D9472B"/>
      <ellipse cx="50" cy="18" rx="10" ry="5" fill="#B0311B"/>
    </symbol>
    <symbol id="oliva-negra" viewBox="0 0 100 130">
      <ellipse cx="50" cy="68" rx="42" ry="56" fill="#3E1019"/>
      <ellipse cx="34" cy="56" rx="8" ry="18" fill="#8A3A4C" opacity=".6" transform="rotate(-18 34 56)"/>
      <ellipse cx="50" cy="20" rx="12" ry="7" fill="#1A060B"/>
    </symbol>
  </defs>
</svg>

<nav>
  <button class="logo" id="logo" title="Tocá para cambiar el orden">
    <svg><use href="#oliva-verde"/></svg><span data-nombres=" & "></span>
  </button>
  <ul>
    <li><a href="#nosotras">Nosotras</a></li>
    <li><a href="#ideas">Ideas</a></li>
    <li><a href="#contacto">Contacto</a></li>
  </ul>
</nav>

<header class="hero">
  <div>
    <p class="eyebrow">Dupla creativa · Copy & Arte</p>
    <h1>Ideas con <em>carozo</em>.</h1>
    <p class="lead">Somos <strong data-nombres=" y "></strong>, dupla creativa publicitaria. Buscamos ideas simples, con sabor y con algo adentro: de las que se quedan en la cabeza.</p>
    <div class="ctas">
      <a class="btn" href="#ideas">Ver ideas</a>
      <a class="btn btn-linea" href="#nosotras">Conocernos</a>
    </div>
  </div>
  <div class="frasco" aria-hidden="true">
    <svg class="sello" viewBox="0 0 100 100">
      <path id="circulo" d="M50,50 m-44,0 a44,44 0 1,1 88,0 a44,44 0 1,1 -88,0" fill="none"/>
      <text><textPath href="#circulo" textLength="272" lengthAdjust="spacing">DOS ACEITUNAS ✦ UN MISMO FRASCO ✦ COPY & ARTE ✦</textPath></text>
    </svg>
    <svg class="o o1"><use href="#oliva-verde"/></svg>
    <svg class="o o2"><use href="#oliva-negra"/></svg>
  </div>
</header>

<div class="cinta" aria-hidden="true">
  <div class="cinta-track">
    <span>Copy <i>✦</i> Arte <i>✦</i> Ideas con carozo <i>✦</i> Verdes y negras <i>✦</i> Copy <i>✦</i> Arte <i>✦</i> Ideas con carozo <i>✦</i> Verdes y negras <i>✦</i></span>
    <span>Copy <i>✦</i> Arte <i>✦</i> Ideas con carozo <i>✦</i> Verdes y negras <i>✦</i> Copy <i>✦</i> Arte <i>✦</i> Ideas con carozo <i>✦</i> Verdes y negras <i>✦</i></span>
  </div>
</div>

<section id="nosotras">
  <div class="sec-head">
    <div>
      <p class="eyebrow">Nosotras</p>
      <h2>Una verde, <em>una negra.</em></h2>
    </div>
    <p>Distintas, pero del mismo frasco. Pensamos el copy y el arte al mismo tiempo: cada idea nace de una charla, no de un brief partido en dos.</p>
  </div>
  <div class="nosotras" id="nosotrasGrid"></div>
</section>

<section id="ideas">
  <div class="sec-head">
    <div>
      <p class="eyebrow">Portfolio</p>
      <h2>Ideas <em>seleccionadas</em></h2>
    </div>
    <p>Campañas, activaciones y productos. Tocá una idea para ver el caso completo.</p>
  </div>
  <div class="filtros" id="filtros"></div>
  <div class="grid" id="grid"></div>
</section>

<section id="contacto">
  <div class="contacto">
    <div>
      <p class="eyebrow">Contacto</p>
      <h2>¿Un vermú y <em>lo charlamos?</em></h2>
      <p class="sub">Contanos la marca, el desafío y los plazos. Las aceitunas las ponemos nosotras.</p>
      <a class="mail-grande" id="mail" href="#"></a>
      <div class="redes" id="redes"></div>
    </div>
    <form id="form">
      <input name="nombre" type="text" placeholder="Tu nombre" required>
      <input name="email" type="email" placeholder="Tu email" required>
      <input name="marca" type="text" placeholder="Empresa / marca">
      <textarea name="mensaje" placeholder="Contanos sobre el proyecto"></textarea>
      <button class="btn" type="submit">Enviar mensaje</button>
      <p class="estado" id="estado" role="status"></p>
    </form>
  </div>
</section>

<footer>
  <span>© <span id="anio"></span> <span data-nombres=" & "></span> · Dupla creativa</span>
  <span>Hecho con aceitunas 🫒</span>
</footer>

<div class="modal" id="modal" role="dialog" aria-modal="true" aria-labelledby="mTitulo">
  <div class="modal-box">
    <button class="cerrar" id="cerrar" aria-label="Cerrar">×</button>
    <div id="modalContenido"></div>
  </div>
</div>

<script>
// =====================================================================
//  ✏️  EDITÁ ACÁ — todo el contenido del sitio está en este bloque
// =====================================================================

const DUPLA = {
  email: "luzymeme@ejemplo.com",
  instagram: "",   // ej: "https://instagram.com/luzymeme"
  behance: "",     // ej: "https://behance.net/..."
  formspree: "",   // ej: "https://formspree.io/f/abcdwxyz" — si queda vacío, el formulario abre el mail
  // true = muestra recuadros punteados "Completar" donde falta info (útil mientras arman).
  // Pónganlo en false cuando publiquen: lo vacío simplemente no se muestra.
  mostrarPendientes: true
};

const NOSOTRAS = [
  {
    nombre: "Luz Apellido",
    rol: "Copywriter",            // cámbienlo si es al revés
    oliva: "verde",               // "verde" o "negra" (color de la tarjeta)
    foto: "",                     // ej: "assets/img/luz.jpg"
    bio: "",                      // 2 o 3 líneas: de dónde venís, qué te gusta, dónde estudiaste/trabajaste
    linkedin: "",                 // ej: "https://www.linkedin.com/in/..."
    cv: ""                        // ej: "assets/cv/luz.pdf"
  },
  {
    nombre: "Meme Apellido",
    rol: "Directora de Arte",
    oliva: "negra",
    foto: "",
    bio: "",
    linkedin: "",
    cv: ""
  }
];

/*  CÓMO ARMAR UN PROYECTO
    tema:     color de la portada si no hay imagen → "oliva" | "bordo" | "negra" | "crema" | "clara"
    portada:  imagen de portada, ej "assets/img/alma-mora/portada.jpg" (vacío = portada generada)
    media:    lista de piezas. tipo: "imagen" | "video" (mp4 propio) | "youtube" | "vimeo" | "drive"
              src: ruta o link. texto: epígrafe.
              formato: "vertical" para piezas 9:16. ancho: "medio" para poner dos imágenes lado a lado.
    titulares: lista de titulares (se muestran como citas grandes).
    extras:   secciones libres { titulo, texto }.
    links:    botones { texto, url } (PDF del board, nota de prensa, etc.)
    Cualquier campo vacío ("") no se muestra (o se marca como pendiente). */

const PROYECTOS = [
  {
    id: "loading-logo",
    titulo: "Loading logo...",
    marca: "Junior Achievement",
    categoria: "Digital",
    anio: "",
    premio: "Presentada a Premios Obrar",
    tema: "oliva",
    portada: "",
    bajada: "Un welcome kit para quienes buscan su primer empleo.",
    descripcion: "Un «welcome kit» que les enviamos a jóvenes en busca de su primer empleo para que lo suban a su LinkedIn y empiecen a generar redes.",
    concepto: "",
    reto: "",
    idea: "",
    resultado: "",
    titulares: [],
    media: [
      { tipo: "imagen",  src: "", texto: "Board" },
      { tipo: "youtube", src: "", texto: "Videocaso" }
    ],
    extras: [],
    links: [ { texto: "Board en PDF", url: "" } ]
  },
  {
    id: "alma-mora",
    titulo: "Alma Mora",
    marca: "Alma Mora",
    categoria: "Gráfica",
    anio: "",
    premio: "",
    tema: "bordo",
    portada: "",
    bajada: "Un concepto, muchos titulares largos.",
    descripcion: "Serie de gráficas con distintos titulares bajo un mismo concepto de campaña, respetando el concepto de marca.",
    concepto: "",
    reto: "",
    idea: "",
    resultado: "",
    titulares: ["", "", ""],
    media: [
      { tipo: "imagen", src: "", texto: "Gráfica 1", ancho: "medio" },
      { tipo: "imagen", src: "", texto: "Gráfica 2", ancho: "medio" },
      { tipo: "imagen", src: "", texto: "Gráfica 3", ancho: "medio" }
    ],
    extras: [],
    links: []
  },
  {
    id: "coppola",
    titulo: "Coppola",
    marca: "Coppola (serie)",
    categoria: "Activación",
    anio: "",
    premio: "",
    tema: "negra",
    portada: "",
    bajada: "Activaciones para el lanzamiento de la nueva temporada.",
    descripcion: "Activaciones para el lanzamiento de la nueva temporada de la serie Coppola.",
    concepto: "",
    reto: "",
    idea: "",
    resultado: "",
    titulares: [],
    media: [
      { tipo: "imagen",  src: "", texto: "Board / key visual" },
      { tipo: "youtube", src: "", texto: "Videocaso o render de la activación" }
    ],
    extras: [],
    links: []
  },
  {
    id: "shorta",
    titulo: "Shorta",
    marca: "Shorta",
    categoria: "Vía pública",
    anio: "",
    premio: "",
    tema: "crema",
    portada: "",
    bajada: "Vía pública para una app de series verticales.",
    descripcion: "Piezas de vía pública —gráficas y videos— para Shorta, la app de series verticales. Además, una idea de film.",
    concepto: "",
    reto: "",
    idea: "",
    resultado: "",
    titulares: [],
    media: [
      { tipo: "imagen", src: "", texto: "Gráfica vía pública", ancho: "medio" },
      { tipo: "video",  src: "", texto: "Video vertical", formato: "vertical" }
    ],
    extras: [ { titulo: "Idea de film", texto: "" } ],
    links: []
  },
  {
    id: "hojas-rivadavia",
    titulo: "Hojas Rivadavia",
    marca: "Hojas Rivadavia",
    categoria: "Producto",
    anio: "",
    premio: "",
    tema: "clara",
    portada: "",
    bajada: "Una idea de producto para la marca.",
    descripcion: "",
    concepto: "",
    reto: "",
    idea: "",
    resultado: "",
    titulares: [],
    media: [ { tipo: "imagen", src: "", texto: "Producto / mockup" } ],
    extras: [],
    links: []
  }
];

// =====================================================================
//  De acá para abajo no hace falta tocar nada
// =====================================================================

const $ = s => document.querySelector(s);
const esc = s => String(s ?? "").replace(/[&<>"']/g, c => ({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]));
const pend = (t = "Completar") => DUPLA.mostrarPendientes ? `<span class="pendiente">${esc(t)}</span>` : "";

/* --- Luz & Meme o Meme & Luz: al azar en cada visita, y se invierte tocando el logo --- */
let orden = Math.random() < .5 ? ["Luz", "Meme"] : ["Meme", "Luz"];
function pintarNombres(){
  document.querySelectorAll("[data-nombres]").forEach(el => {
    el.innerHTML = `${orden[0]}<span class="amp">${esc(el.dataset.nombres)}</span>${orden[1]}`;
  });
  document.title = `${orden[0]} & ${orden[1]} — Dupla creativa`;
}
$("#logo").addEventListener("click", () => {
  const l = $("#logo");
  l.classList.remove("giro"); void l.offsetWidth; l.classList.add("giro");
  setTimeout(() => { orden.reverse(); pintarNombres(); }, 250);
});

/* --- Nosotras --- */
function linkPill(texto, url){
  if (url) return `<a class="pill" href="${esc(url)}" target="_blank" rel="noopener">${esc(texto)} ↗</a>`;
  return DUPLA.mostrarPendientes ? `<span class="pill falta">${esc(texto)} (falta link)</span>` : "";
}
$("#nosotrasGrid").innerHTML = NOSOTRAS.map(p => `
  <article class="persona ${p.oliva === "negra" ? "negra" : "verde"}">
    ${p.foto ? `<img class="foto" src="${esc(p.foto)}" alt="${esc(p.nombre)}">`
             : `<svg class="foto-oliva"><use href="#oliva-${p.oliva === "negra" ? "verde" : "negra"}"/></svg>`}
    <small>${esc(p.rol)}</small>
    <h3>${esc(p.nombre)}</h3>
    <p>${p.bio ? esc(p.bio) : pend("Bio corta: de dónde venís, qué te gusta hacer, dónde estudiaste o trabajaste.")}</p>
    <div class="links">${linkPill("LinkedIn", p.linkedin)}${linkPill("CV", p.cv)}</div>
  </article>`).join("");

/* --- Portadas --- */
const TEMAS = {
  oliva: { bg: "var(--oliva)",      fg: "var(--crema)",      ol: "oliva-negra" },
  bordo: { bg: "var(--bordo)",      fg: "var(--crema)",      ol: "oliva-verde" },
  negra: { bg: "var(--tinta)",      fg: "var(--oliva-clara)",ol: "oliva-verde" },
  crema: { bg: "#E6DABE",           fg: "var(--bordo)",      ol: "oliva-verde" },
  clara: { bg: "var(--oliva-clara)",fg: "var(--oliva-osc)",  ol: "oliva-negra" }
};
function portada(p){
  const t = TEMAS[p.tema] || TEMAS.oliva;
  if (p.portada) return `<div class="portada" style="background:${t.bg}"><img src="${esc(p.portada)}" alt="${esc(p.titulo)}" loading="lazy"></div>`;
  return `<div class="portada generada" style="background:${t.bg};color:${t.fg}">
            <span class="portada-titulo">${esc(p.titulo)}</span>
            <svg class="portada-oliva"><use href="#${t.ol}"/></svg>
          </div>`;
}

/* --- Filtros y grilla --- */
const cats = ["Todas", ...new Set(PROYECTOS.map(p => p.categoria).filter(Boolean))];
let actual = "Todas";
function pintarFiltros(){
  $("#filtros").innerHTML = cats.map(c => `<button class="${c === actual ? "activo" : ""}" data-cat="${esc(c)}">${esc(c)}</button>`).join("");
}
$("#filtros").addEventListener("click", e => {
  const b = e.target.closest("button"); if (!b) return;
  actual = b.dataset.cat; pintarFiltros(); pintarGrilla();
});
function pintarGrilla(){
  $("#grid").innerHTML = PROYECTOS
    .filter(p => actual === "Todas" || p.categoria === actual)
    .map(p => `
      <article class="card" tabindex="0" role="button" data-id="${esc(p.id)}" aria-label="Ver ${esc(p.titulo)}">
        ${portada(p)}
        <div class="card-body">
          <div class="tag">${esc(p.categoria)}${p.marca && p.marca !== p.titulo ? " · " + esc(p.marca) : ""}</div>
          <h3>${esc(p.titulo)}</h3>
          <p>${esc(p.bajada)}</p>
          ${p.premio ? `<span class="premio">★ ${esc(p.premio)}</span>` : ""}
        </div>
      </article>`).join("");
}
$("#grid").addEventListener("click", e => { const c = e.target.closest(".card"); if (c) abrir(c.dataset.id); });
$("#grid").addEventListener("keydown", e => {
  const c = e.target.closest(".card");
  if (c && (e.key === "Enter" || e.key === " ")) { e.preventDefault(); abrir(c.dataset.id); }
});

/* --- Piezas (imágenes y videos) --- */
const ytId    = u => (String(u).match(/(?:youtu\.be\/|v=|embed\/|shorts\/)([\w-]{11})/) || [, u])[1];
const vimeoId = u => (String(u).match(/vimeo\.com\/(?:video\/)?(\d+)/) || [, u])[1];
const driveId = u => (String(u).match(/\/d\/([\w-]+)/) || [, u])[1];
const NOMBRE_TIPO = { imagen: "imagen", video: "video", youtube: "video de YouTube", vimeo: "video de Vimeo", drive: "archivo de Drive" };

function pieza(m){
  const cls = ["media", m.formato === "vertical" ? "vertical" : "", m.ancho === "medio" ? "medio" : ""].join(" ");
  const pie = m.texto ? `<figcaption>${esc(m.texto)}</figcaption>` : "";
  if (!m.src) return DUPLA.mostrarPendientes
    ? `<figure class="${cls}"><div class="hueco">＋ ${esc(m.texto || "Agregar pieza")}<small>${esc(NOMBRE_TIPO[m.tipo] || m.tipo)}</small></div></figure>` : "";
  const titulo = esc(m.texto || "Video");
  let el = "";
  switch (m.tipo) {
    case "imagen":  el = `<img src="${esc(m.src)}" alt="${esc(m.texto || "")}" loading="lazy">`; break;
    case "video":   el = `<video src="${esc(m.src)}" controls playsinline preload="metadata"${m.poster ? ` poster="${esc(m.poster)}"` : ""}></video>`; break;
    case "youtube": el = `<iframe src="https://www.youtube-nocookie.com/embed/${esc(ytId(m.src))}" title="${titulo}" allow="autoplay; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>`; break;
    case "vimeo":   el = `<iframe src="https://player.vimeo.com/video/${esc(vimeoId(m.src))}" title="${titulo}" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen loading="lazy"></iframe>`; break;
    case "drive":   el = `<iframe src="https://drive.google.com/file/d/${esc(driveId(m.src))}/preview" title="${titulo}" allow="autoplay" allowfullscreen loading="lazy"></iframe>`; break;
  }
  return `<figure class="${cls}">${el}${pie}</figure>`;
}

/* --- Detalle del proyecto --- */
function bloque(titulo, txt){
  if (!txt && !DUPLA.mostrarPendientes) return "";
  return `<div class="bloque"><h4>${titulo}</h4><p>${txt ? esc(txt) : pend()}</p></div>`;
}
function abrir(id){
  const i = PROYECTOS.findIndex(p => p.id === id);
  if (i < 0) return;
  const p = PROYECTOS[i];
  const ant = PROYECTOS[(i - 1 + PROYECTOS.length) % PROYECTOS.length];
  const sig = PROYECTOS[(i + 1) % PROYECTOS.length];

  const meta = [["Marca", p.marca], ["Categoría", p.categoria], ["Año", p.anio], ["Reconocimiento", p.premio]]
    .filter(([, v]) => v).map(([k, v]) => `<div><dt>${k}</dt><dd>${esc(v)}</dd></div>`).join("");

  const titulares = (p.titulares || []).map((t, n) => t
    ? `<blockquote>${esc(t)}</blockquote>`
    : (DUPLA.mostrarPendientes ? `<blockquote class="vacio">Titular ${n + 1} — completar</blockquote>` : "")).join("");

  const bloques = bloque("El reto", p.reto) + bloque("La idea", p.idea) + bloque("Resultado", p.resultado);
  const piezas = (p.media || []).map(pieza).join("");
  const extras = (p.extras || []).map(x => (x.texto || DUPLA.mostrarPendientes)
    ? `<div class="extra"><h4 class="sub-titulo">${esc(x.titulo)}</h4><p>${x.texto ? esc(x.texto) : pend()}</p></div>` : "").join("");
  const links = (p.links || []).map(l => l.url
    ? `<a class="pill" href="${esc(l.url)}" target="_blank" rel="noopener">${esc(l.texto)} ↗</a>`
    : (DUPLA.mostrarPendientes ? `<span class="pill falta">${esc(l.texto)} (falta link)</span>` : "")).join("");

  $("#modalContenido").innerHTML = `
    ${portada(p)}
    <div class="modal-body">
      <div class="tag">${esc(p.categoria)}</div>
      <h3 id="mTitulo">${esc(p.titulo)}</h3>
      ${meta ? `<dl class="meta">${meta}</dl>` : ""}
      ${p.descripcion ? `<p class="desc">${esc(p.descripcion)}</p>` : (DUPLA.mostrarPendientes ? `<p class="desc">${pend("Descripción del proyecto")}</p>` : "")}
      ${p.concepto ? `<p class="concepto"><small>Concepto</small>${esc(p.concepto)}</p>`
                   : (DUPLA.mostrarPendientes ? `<p class="concepto"><small>Concepto</small>${pend("El concepto en una frase")}</p>` : "")}
      ${bloques ? `<div class="bloques">${bloques}</div>` : ""}
      ${titulares ? `<h4 class="sub-titulo">Titulares</h4><div class="titulares">${titulares}</div>` : ""}
      ${piezas ? `<div class="galeria">${piezas}</div>` : ""}
      ${extras}
      ${links ? `<div class="links-proy">${links}</div>` : ""}
      <div class="navegar">
        <button data-ir="${esc(ant.id)}">← ${esc(ant.titulo)}</button>
        <button data-ir="${esc(sig.id)}">${esc(sig.titulo)} →</button>
      </div>
    </div>`;

  $("#modal").classList.add("abierto");
  $("#modal").scrollTop = 0;
  document.body.style.overflow = "hidden";
  history.replaceState(null, "", "#idea/" + p.id);   // link directo a cada caso
  $("#cerrar").focus();
}
function cerrar(){
  $("#modal").classList.remove("abierto");
  document.body.style.overflow = "";
  $("#modalContenido").innerHTML = "";   // corta videos que estén sonando
  history.replaceState(null, "", "#ideas");
}
$("#cerrar").addEventListener("click", cerrar);
$("#modal").addEventListener("click", e => {
  if (e.target.id === "modal") cerrar();
  const b = e.target.closest("[data-ir]"); if (b) abrir(b.dataset.ir);
});
document.addEventListener("keydown", e => { if (e.key === "Escape" && $("#modal").classList.contains("abierto")) cerrar(); });

/* --- Contacto --- */
$("#mail").textContent = DUPLA.email;
$("#mail").href = "mailto:" + DUPLA.email;
$("#redes").innerHTML = [["Instagram", DUPLA.instagram], ["Behance", DUPLA.behance]]
  .filter(([, u]) => u).map(([t, u]) => `<a class="pill" href="${esc(u)}" target="_blank" rel="noopener">${t} ↗</a>`).join("");

$("#form").addEventListener("submit", async e => {
  e.preventDefault();
  const f = e.target, d = new FormData(f), estado = $("#estado");
  if (DUPLA.formspree) {
    estado.textContent = "Enviando…";
    try {
      const r = await fetch(DUPLA.formspree, { method: "POST", body: d, headers: { Accept: "application/json" } });
      estado.textContent = r.ok ? "¡Gracias! Te respondemos pronto." : "Ups, algo falló. Escribinos al mail.";
      if (r.ok) f.reset();
    } catch { estado.textContent = "Ups, algo falló. Escribinos al mail."; }
  } else {
    const asunto = encodeURIComponent("Proyecto" + (d.get("marca") ? " — " + d.get("marca") : ""));
    const cuerpo = encodeURIComponent(`${d.get("mensaje") || ""}\n\n${d.get("nombre")} · ${d.get("email")}`);
    location.href = `mailto:${DUPLA.email}?subject=${asunto}&body=${cuerpo}`;
  }
});

/* --- Arranque --- */
$("#anio").textContent = new Date().getFullYear();
pintarNombres();
pintarFiltros();
pintarGrilla();
const deHash = location.hash.match(/^#idea\/(.+)$/);
if (deHash) abrir(decodeURIComponent(deHash[1]));
</script>
</body>
</html>
