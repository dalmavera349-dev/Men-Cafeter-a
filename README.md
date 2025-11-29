<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>LODEVIC - Menú</title>
  <style>
    :root{
      --cream:#f7efe6;
      --brown:#6b3f24;
      --accent:#b67a44;
      --paper:#fffefc;
      --max-width:900px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: 'Georgia', serif;
      background:linear-gradient(180deg, #f3efe9 0%, #fff 100%);
      color:var(--brown);
      display:flex;
      justify-content:center;
      padding:24px;
    }
    .menu-wrap{
      width:100%;
      max-width:var(--max-width);
      background:var(--paper);
      border-radius:10px;
      box-shadow:0 6px 18px rgba(0,0,0,0.08);
      padding:28px;
      position:relative;
      overflow:hidden;
    }
    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
    }
    .brand{
      font-family: 'Georgia', serif;
      color:var(--brown);
    }
    .brand h1{
      margin:0;
      font-size:40px;
      letter-spacing:2px;
    }
    .brand p{margin:2px 0 0 0; color:#5b4031}

    .hero-img{
      width:120px;
      height:80px;
      background-image:url('images/croissant.png');
      background-size:cover;
      background-position:center;
      border-radius:6px;
    }

    .columns{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:18px;
      margin-top:18px;
    }

    .section{
      background:rgba(255,255,255,0.95);
      padding:14px 16px;
      border-radius:8px;
    }
    .section h2{
      margin:0 0 10px 0;
      font-size:20px;
      color:var(--accent);
      text-decoration: underline;
    }

    ul.menu-list{
      list-style:none;
      margin:0;
      padding:0;
    }
    ul.menu-list li{
      display:flex;
      justify-content:space-between;
      padding:6px 0;
      border-bottom:1px dashed rgba(0,0,0,0.03);
      font-size:15px;
    }
    ul.menu-list li:last-child{border-bottom:0}
    .item-name{max-width:70%}
    .price{white-space:nowrap; font-weight:700}

    /* Iced single box */
    .iced-box{
      margin-top:18px;
      padding:12px;
      border-radius:8px;
      background:linear-gradient(180deg,#fff,#fbf6f1);
      box-shadow:inset 0 1px 0 rgba(255,255,255,0.6);
    }

    /* Right column image */
    .drink-img{
      width:120px;
      height:160px;
      background-image:url('images/iced-coffee.png');
      background-size:cover;
      background-position:center;
      border-radius:8px;
      margin-top:8px;
    }

    footer{
      margin-top:18px;
      text-align:center;
      color:#6a4f3a;
      font-size:13px;
    }

    /* Responsive */
    @media (max-width:700px){
      .columns{grid-template-columns:1fr}
      .hero-img{display:none}
      .brand h1{font-size:28px}
    }
  </style>
</head>
<body>
  <div class="menu-wrap">
    <header>
      <div class="brand">
        <h1>LODEVIC</h1>
        <p>CAFE ESPRESS</p>
      </div>
      <div class="hero-img" aria-hidden="true"></div>
    </header>

    <div class="columns">
      <!-- LEFT COLUMN -->
      <div class="section">
        <h2>Café Caliente</h2>
        <ul class="menu-list">
          <li><span class="item-name">Cafe Americano</span><span class="price">15.000</span></li>
          <li><span class="item-name">Latte</span><span class="price">18.000</span></li>
          <li><span class="item-name">Capuccino</span><span class="price">20.000</span></li>
          <li><span class="item-name">Mocca</span><span class="price">20.000</span></li>
          <li><span class="item-name">Latte vainilla</span><span class="price">18.000</span></li>
          <li><span class="item-name">Latte caramell</span><span class="price">18.000</span></li>
          <li><span class="item-name">Latte Lodevic</span><span class="price">18.000</span></li>
          <li><span class="item-name">Cocido Negro</span><span class="price">8.000</span></li>
          <li><span class="item-name">Cocido con Leche</span><span class="price">12.000</span></li>
        </ul>

        <div class="iced-box">
          <h2 style="text-decoration:none; margin-bottom:8px;">Iced</h2>
          <ul class="menu-list">
            <li><span class="item-name">Iceed Americano</span><span class="price">15.000</span></li>
            <li><span class="item-name">Iceed latte</span><span class="price">18.000</span></li>
            <li><span class="item-name">Iceed Mocca</span><span class="price">20.000</span></li>
            <li><span class="item-name">Coffee with orange</span><span class="price">18.000</span></li>
          </ul>
        </div>
      </div>

      <!-- RIGHT COLUMN -->
      <div class="section">
        <h2>Para Acompañar</h2>
        <ul class="menu-list">
          <li><span class="item-name">Cookies Limon</span><span class="price">16.000</span></li>
          <li><span class="item-name">Cookiefrola</span><span class="price">15.000</span></li>
          <li><span class="item-name">Cookiered velve</span><span class="price">18.000</span></li>
          <li><span class="item-name">Cookies tradicional</span><span class="price">15.000</span></li>
          <li><span class="item-name">Cookies Nutela</span><span class="price">20.000</span></li>
          <li><span class="item-name">Pastafrola</span><span class="price">16.000</span></li>
          <li><span class="item-name">Muffins Limon</span><span class="price">16.000</span></li>
          <li><span class="item-name">Muffins Arandanos</span><span class="price">18.000</span></li>
          <li><span class="item-name">Muffins Chocolate</span><span class="price">18.000</span></li>
          <li><span class="item-name">Chipa</span><span class="price">5.000</span></li>
          <li><span class="item-name">Mbeju</span><span class="price">10.000</span></li>
          <li><span class="item-name">Mbeju con queso</span><span class="price">15.000</span></li>
          <li><span class="item-name">Tapioca con jamon y queso</span><span class="price">12.000</span></li>
          <li><span class="item-name">Mixto de pan arabe</span><span class="price">15.000</span></li>
          <li><span class="item-name">Mixto Jamon y Queso</span><span class="price">10.000</span></li>
          <li><span class="item-name">Huevo revuelto + tostada</span><span class="price">15.000</span></li>
        </ul>

        <div class="drink-img" aria-hidden="true"></div>
      </div>
    </div>

    <footer>
      © 2025 LODEVIC CAFE ESPRESS — Menú Digital
    </footer>
  </div>
</body>
</html>
