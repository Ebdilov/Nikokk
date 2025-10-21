# Nikokk
<!doctype html>
<html lang="az">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>ElectroShop — Elektronika Mağazası</title>

  <style>
    /* Sade, modern stil — asanlıqla dəyişdir */
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#94a3b8;
      --accent:#06b6d4;
      --glass: rgba(255,255,255,0.03);
      --radius:12px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      color-scheme: dark;
    }

    html,body{
      height:100%;
      margin:0;
      background:linear-gradient(180deg,#071022 0%, #06121a 100%);
      color:#e6eef6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .container{
      max-width:980px;
      margin:28px auto;
      padding:20px;
      backdrop-filter: blur(6px);
    }

    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
    }

    .brand{
      display:flex;
      gap:12px;
      align-items:center;
    }

    .logo{
      width:56px;
      height:56px;
      border-radius:10px;
      background:linear-gradient(135deg,#0ea5a4,#2563eb);
      display:flex;
      align-items:center;
      justify-content:center;
      font-weight:700;
      color:white;
      font-size:18px;
      box-shadow:0 6px 18px rgba(2,6,23,0.6);
    }

    h1{ margin:0; font-size:20px; letter-spacing:0.2px; }
    p.lead{ color:var(--muted); margin:2px 0 0; font-size:13px; }

    nav{
      display:flex;
      gap:12px;
      align-items:center;
    }

    nav a{
      color:var(--muted);
      text-decoration:none;
      font-size:14px;
      padding:8px 10px;
      border-radius:8px;
    }

    nav a.cta{
      background:var(--accent);
      color:#022;
      font-weight:600;
    }

    /* Product grid */
    .grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:18px;
      margin-top:20px;
    }

    .card{
      background:var(--card);
      border-radius:var(--radius);
      padding:14px;
      box-shadow: 0 6px 20px rgba(2,6,23,0.6);
      display:flex;
      flex-direction:column;
      gap:10px;
    }

    .imgwrap{
      width:100%;
      aspect-ratio:16/10;
      border-radius:10px;
      overflow:hidden;
      background:var(--glass);
      display:flex;
      align-items:center;
      justify-content:center;
    }

    .imgwrap img{ width:100%; height:100%; object-fit:cover; }

    h2.prod-title{ font-size:16px; margin:0; }
    p.meta{ margin:0; color:var(--muted); font-size:13px; }

    .price-row{
      display:flex;
      align-items:center;
      gap:10px;
      justify-content:space-between;
      margin-top:6px;
    }

    .price{
      font-weight:700;
      font-size:16px;
    }

    .old-price{ color:var(--muted); text-decoration:line-through; font-size:13px; }

    .badges{ display:flex; gap:8px; align-items:center; }
    .badge{
      background:rgba(255,255,255,0.05);
      padding:4px 8px;
      border-radius:999px;
      font-size:12px;
      color:var(--muted);
    }

    .buy{
      margin-top:8px;
      display:inline-block;
      padding:8px 12px;
      border-radius:10px;
      background:linear-gradient(90deg,var(--accent),#34d399);
      color:#022;
      font-weight:600;
      text-decoration:none;
      text-align:center;
    }

    hr{ border:none; height:1px; background:rgba(255,255,255,0.03); margin:22px 0; }

    footer{
      text-align:center;
      color:var(--muted);
      font-size:13px;
      margin-top:18px;
    }

    /* Responsive tweaks */
    @media (max-width:420px){
      header{ flex-direction:column; align-items:flex-start; gap:12px; }
      .brand p.lead{ font-size:12px; }
    }
  </style>
</head>
<body>
  <div class="container">

    <header>
      <div class="brand">
        <div class="logo">E</div>
        <div>
          <h1>ElectroShop</h1>
          <p class="lead">Sürətli çatdırılma · Rəsmi zəmanət · Endirimlər</p>
        </div>
      </div>

      <nav>
        <a href="#phones">Telefonlar</a>
        <a href="#laptops">Noutbuklar</a>
        <a href="#audio">Audio</a>
        <a href="#watches">Smart Saatlar</a>
        <a class="cta" href="#contact">Sifariş et</a>
      </nav>
    </header>

    <hr />

    <main>
      <section id="featured">
        <h2 style="margin:0 0 10px 0;">Üst məhsullar</h2>

        <div class="grid">
          <!-- Məhsul 1 -->
          <article class="card">
            <div class="imgwrap">
              <img src="https://via.placeholder.com/800x500?text=Smartphone" alt="Smartphone">
            </div>
            <h2 class="prod-title">SmartPhone X12</h2>
            <p class="meta">İlkin: Marka A · 128GB · 8GB RAM</p>
            <div class="price-row">
              <div>
                <div class="price">$499.00</div>
                <div class="old-price">$599.00</div>
              </div>
              <div class="badges">
                <span class="badge">Yeni</span>
                <span class="badge">Populyar</span>
              </div>
            </div>
            <a class="buy" href="#buy-phone">Sifariş et</a>
          </article>

          <!-- Məhsul 2 -->
          <article class="card">
            <div class="imgwrap">
              <img src="https://via.placeholder.com/800x500?text=Laptop" alt="Laptop">
            </div>
            <h2 class="prod-title">UltraBook Pro 15"</h2>
            <p class="meta">İlkin: Marka B · i7 · 16GB RAM · 512GB SSD</p>
            <div class="price-row">
              <div>
                <div class="price">$1,149.00</div>
                <div class="old-price">$1,299.00</div>
              </div>
              <div class="badges">
                <span class="badge">7% endirim</span>
              </div>
            </div>
            <a class="buy" href="#buy-laptop">Sifariş et</a>
          </article>

          <!-- Məhsul 3 -->
          <article class="card">
            <div class="imgwrap">
              <img src="https://via.placeholder.com/800x500?text=Headphones" alt="Headphones">
            </div>
            <h2 class="prod-title">SoundBeat Q HR</h2>
            <p class="meta">Simli / Simsiz · ANC · 30 saat batareya</p>
            <div class="price-row">
              <div>
                <div class="price">$89.00</div>
                <div class="old-price">$120.00</div>
              </div>
              <div class="badges">
                <span class="badge">Endirimdə</span>
              </div>
            </div>
            <a class="buy" href="#buy-audio">Sifariş et</a>
          </article>

          <!-- Məhsul 4 -->
          <article class="card">
            <div class="imgwrap">
              <img src="https://via.placeholder.com/800x500?text=Smartwatch" alt="Smartwatch">
            </div>
            <h2 class="prod-title">TimePro S3</h2>
            <p class="meta">Yuxarı səviyyə sağlamlıq izləmə · Suya davamlı</p>
            <div class="price-row">
              <div>
                <div class="price">$149.00</div>
                <div class="old-price">$179.00</div>
              </div>
              <div class="badges">
                <span class="badge">Məhdud stok</span>
              </div>
            </div>
            <a class="buy" href="#buy-watch">Sifariş et</a>
          </article>
        </div>
      </section>

      <hr />

      <section id="about" style="margin-top:10px;">
        <h2 style="margin:0 0 8px 0;">Haqqımızda</h2>
        <p style="color:var(--muted); margin:0;">
          ElectroShop — Azərbaycanda sürətli və etibarlı elektronika satışı. Rəsmi zəmanət, çatdırılma və 30 günlük qaytarma şərtləri.
        </p>
      </section>

      <hr />

      <section id="contact">
        <h2 style="margin:0 0 8px 0;">Əlaqə / Sifariş</h2>
        <p class="meta">Telefon: +994 50 000 00 00 · E-poçt: info@electroshop.az</p>
      </section>
    </main>

    <footer>
      <p>&copy; 2025 ElectroShop — Bütün hüquqlar qorunur.</p>
    </footer>

  </div>
</body>
</html>
