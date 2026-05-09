# DEMarket-tienda
DEMarket Suministros &amp; Retail
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DEMarket | Suministros y Retail</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --primario: #1a1a1a;
            --acento: #00b894;
            --fondo: #ffffff;
            --gris-claro: #f4f4f4;
            --secundario: #666666;
        }

        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            background-color: var(--fondo);
            color: var(--primario);
        }

        /* Cabecera */
        header {
            position: sticky;
            top: 0;
            background: white;
            z-index: 1000;
            border-bottom: 1px solid #eee;
        }

        .promo-bar {
            background: var(--primario);
            color: white;
            font-size: 11px;
            text-align: center;
            padding: 5px 0;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .nav-main {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
        }

        .logo {
            font-weight: 800;
            font-size: 20px;
            letter-spacing: -0.5px;
            text-transform: uppercase;
        }

        /* Banner Principal */
        .hero {
            padding: 30px 20px;
            background: var(--gris-claro);
            text-align: center;
            border-bottom: 1px solid #eee;
        }

        /* Cuadrícula de Productos */
        .container {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 12px;
            padding: 12px;
        }

        .card {
            background: white;
            border: 1px solid #eaeaea;
            border-radius: 12px;
            overflow: hidden;
            position: relative;
        }

        .card img {
            width: 100%;
            aspect-ratio: 1 / 1;
            object-fit: cover;
        }

        .info {
            padding: 12px;
        }

        .product-title {
            font-size: 13px;
            color: var(--secundario);
            margin-bottom: 5px;
            display: block;
            height: 32px;
            overflow: hidden;
        }

        .product-price {
            font-size: 16px;
            font-weight: 700;
        }

        .btn-add {
            width: 100%;
            background: var(--primario);
            color: white;
            border: none;
            padding: 10px;
            border-radius: 8px;
            font-weight: 600;
            margin-top: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>

<header>
    <div class="promo-bar">Envíos gratis en pedidos mayores a $50 🚚</div>
    <div class="nav-main">
        <div class="logo">DE<span style="color: var(--acento);">MARKET</span></div>
        <div id="cart-icon">🛒 <span id="cart-count">0</span></div>
    </div>
</header>

<section class="hero">
    <h2 style="margin:0; font-size: 18px;">📦 Especialistas en Empaques</h2>
    <p style="margin:5px 0 0; font-size: 14px; color: var(--secundario);">Fabricación de cajas y distribución mayorista.</p>
</section>

<div class="container">
    <!-- Producto 1 -->
    <div class="card">
        <img src="https://via.placeholder.com/300x300/f4f4f4/000000?text=Caja+Repostería" alt="Caja">
        <div class="info">
            <span class="product-title">Caja para Tortas 20x20x10 (Unidad)</span>
            <span class="product-price">$1.20</span>
            <button class="btn-add">Añadir</button>
        </div>
    </div>

    <!-- Producto 2 -->
    <div class="card">
        <img src="https://via.placeholder.com/300x300/f4f4f4/000000?text=Envase+PT-1" alt="Envase">
        <div class="info">
            <span class="product-title">Envase Plástico PT-1 (Bulto 100u)</span>
            <span class="product-price">$15.50</span>
            <button class="btn-add">Añadir</button>
        </div>
    </div>
</div>

</body>
</html>
