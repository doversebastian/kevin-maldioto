# kevin-maldioto
<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Kevin pagame MALDITO</title>
  <style>
    :root{
      --bg1:#0f172a; --bg2:#1e293b;
      --c1:#22d3ee; --c2:#a78bfa; --c3:#f472b6;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      display:grid;
      place-items:center;
      background:
        radial-gradient(1000px 600px at 20% 20%, var(--bg2) 0 40%, var(--bg1) 100%);
      color:#e5e7eb;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Inter, Arial, sans-serif;
    }
    .wrap{ text-align:center; padding:1rem }
    .badge{
      display:inline-flex; gap:.5rem; align-items:center;
      padding:.5rem .8rem; border:1px solid rgba(255,255,255,.15);
      border-radius:999px; background:rgba(255,255,255,.06); backdrop-filter:blur(6px);
      font-size:clamp(.85rem,2vw,1rem);
    }
    h1{
      margin:.75rem 0 0;
      font-size:clamp(2rem,8vw,5rem);
      line-height:1.05; font-weight:800; letter-spacing:.02em;
      background:linear-gradient(90deg,var(--c1),var(--c2),var(--c3));
      -webkit-background-clip:text; background-clip:text; color:transparent;
      text-shadow:0 0 18px rgba(167,139,250,.25);
      animation: shimmer 6s linear infinite;
    }
    .sub{ opacity:.85; margin-top:.4rem; font-size:clamp(1rem,2.5vw,1.2rem) }

    /* Imagen */
    .foto{
      margin:1.25rem auto 0;
      width:clamp(220px, 40vw, 460px);
      max-width:100%;
      height:auto;
      border-radius:1.25rem;
      box-shadow:0 20px 45px rgba(0,0,0,.35);
      outline:1px solid rgba(255,255,255,.12);
      display:block;
    }

    /* Botón subir */
    .uploader{
      margin-top:1rem;
      display:inline-flex; align-items:center; gap:.6rem;
      padding:.6rem .9rem; border-radius:.8rem; border:1px solid rgba(255,255,255,.15);
      background:rgba(255,255,255,.06); cursor:pointer;
    }
    .uploader input{ display:none; }
    .uploader span{ font-size:.95rem; }
    @keyframes shimmer { 
      0%{ filter:hue-rotate(0deg) } 
      100%{ filter:hue-rotate(360deg) } 
    }
  </style>
</head>
<body>
  <main class="wrap">
    <div class="badge">💸 Recordatorio</div>
    <h1>Kevin pagame </h1>
    <p class="sub"</p>

    <!-- 👇 Usa tu imagen local cambiando el src -->
    <img id="foto" class="foto" src="img/kevin.jpg" alt="Kevin, paga Visual Studio">

    <!-- 👇 O súbela al vuelo sin rutas -->
    <label class="uploader">
      <input id="picker" type="file" accept="image/*">
      📷 <span>Subir foto</span>
    </label>
  </main>

  <script>
    const picker = document.getElementById('picker');
    const img = document.getElementById('foto');
    picker.addEventListener('change', e => {
      const file = e.target.files?.[0];
      if (!file) return;
      const url = URL.createObjectURL(file);
      img.src = url;
      img.alt = file.name;
    });
  </script>
</body>
</html>
<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Kevin pagame MALDITO</title>
  <style>
    :root{
      --bg1:#0f172a; --bg2:#1e293b;
      --c1:#22d3ee; --c2:#a78bfa; --c3:#f472b6;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      display:grid;
      place-items:center;
      background:
        radial-gradient(1000px 600px at 20% 20%, var(--bg2) 0 40%, var(--bg1) 100%);
      color:#e5e7eb;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Inter, Arial, sans-serif;
    }
    .wrap{ text-align:center; padding:1rem }
    .badge{
      display:inline-flex; gap:.5rem; align-items:center;
      padding:.5rem .8rem; border:1px solid rgba(255,255,255,.15);
      border-radius:999px; background:rgba(255,255,255,.06); backdrop-filter:blur(6px);
      font-size:clamp(.85rem,2vw,1rem);
    }
    h1{
      margin:.75rem 0 0;
      font-size:clamp(2rem,8vw,5rem);
      line-height:1.05; font-weight:800; letter-spacing:.02em;
      background:linear-gradient(90deg,var(--c1),var(--c2),var(--c3));
      -webkit-background-clip:text; background-clip:text; color:transparent;
      text-shadow:0 0 18px rgba(167,139,250,.25);
      animation: shimmer 6s linear infinite;
    }
    .sub{ opacity:.85; margin-top:.4rem; font-size:clamp(1rem,2.5vw,1.2rem) }

    /* Imagen */
    .foto{
      margin:1.25rem auto 0;
      width:clamp(220px, 40vw, 460px);
      max-width:100%;
      height:auto;
      border-radius:1.25rem;
      box-shadow:0 20px 45px rgba(0,0,0,.35);
      outline:1px solid rgba(255,255,255,.12);
      display:block;
    }

    /* Botón subir */
    .uploader{
      margin-top:1rem;
      display:inline-flex; align-items:center; gap:.6rem;
      padding:.6rem .9rem; border-radius:.8rem; border:1px solid rgba(255,255,255,.15);
      background:rgba(255,255,255,.06); cursor:pointer;
    }
    .uploader input{ display:none; }
    .uploader span{ font-size:.95rem; }
    @keyframes shimmer { 
      0%{ filter:hue-rotate(0deg) } 
      100%{ filter:hue-rotate(360deg) } 
    }
  </style>
</head>
<body>
  <main class="wrap">
    <div class="badge">💸 Recordatorio</div>
    <h1>Kevin pagame </h1>
    <p class="sub"</p>

    <!-- 👇 Usa tu imagen local cambiando el src -->
    <img id="foto" class="foto" src="img/kevin.jpg" alt="Kevin, paga Visual Studio">

    <!-- 👇 O súbela al vuelo sin rutas -->
    <label class="uploader">
      <input id="picker" type="file" accept="image/*">
      📷 <span>Subir foto</span>
    </label>
  </main>

  <script>
    const picker = document.getElementById('picker');
    const img = document.getElementById('foto');
    picker.addEventListener('change', e => {
      const file = e.target.files?.[0];
      if (!file) return;
      const url = URL.createObjectURL(file);
      img.src = url;
      img.alt = file.name;
    });
  </script>
</body>
</html>
