<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Responsive product grid with header and sidebar using CSS Grid.">
  <title>Store – Header, Sidebar & Product Grid</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
    }

    body {
      font-family: system-ui, sans-serif;
      background: #f6f7fb;
    }

    .page {
      display: grid;
      grid-template-columns: 240px 1fr;
      grid-template-areas: "header header" "sidebar main" "footer footer";
      min-height: 100vh;
    }

    header {
      grid-area: header;
      background: #14213d;
      color: #fff;
      padding: 1rem 1.5rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    header input {
      padding: .5rem .8rem;
      border-radius: 6px;
      border: 0;
      width: min(260px, 40vw);
    }

    aside {
      grid-area: sidebar;
      background: #fff;
      padding: 1.5rem;
      border-right: 1px solid #ddd;
    }

    aside h2 {
      font-size: 1rem;
      margin-bottom: .5rem;
    }

    aside ul {
      list-style: none;
      padding: 0;
      margin-bottom: 1.5rem;
    }

    aside li {
      padding: .3rem 0;
    }

    main {
      grid-area: main;
      padding: 1.5rem;
    }

    .products {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 1.25rem;
    }

    .product {
      background: #fff;
      border-radius: 10px;
      padding: 1rem;
      box-shadow: 0 2px 8px rgba(0, 0, 0, .07);
    }

    .product img {
      width: 100%;
      aspect-ratio: 1;
      object-fit: cover;
      border-radius: 8px;
    }

    .product h3 {
      font-size: 1rem;
      margin: .6rem 0 .2rem;
    }

    .product p {
      color: #0a8754;
      font-weight: 700;
    }

    footer {
      grid-area: footer;
      background: #14213d;
      color: #ccc;
      text-align: center;
      padding: 1rem;
    }

    @media (max-width: 720px) {
      .page {
        grid-template-columns: 1fr;
        grid-template-areas: "header" "sidebar" "main" "footer";
      }

      aside {
        border-right: 0;
        border-bottom: 1px solid #ddd;
      }
    }
  </style>
</head>

<body>
  <div class="page">
    <header><strong>ShopGrid</strong><input type="search" placeholder="Search products" aria-label="Search products">
    </header>
    <aside>
      <h2>Categories</h2>
      <ul>
        <li>Electronics</li>
        <li>Clothing</li>
        <li>Home</li>
        <li>Beauty Products</li>
      </ul>
      <h2>Price</h2>
      <ul>
        <li>Under ₹500</li>
        <li>₹500 – ₹2000</li>
        <li>Above ₹2000</li>
      </ul>
    </aside>
    <main>
      <h1 style="margin-bottom:1rem">All Products</h1>
      <div class="products">
        <article class="product"><img src="https://assets.ajio.com/medias/sys_master/root/20250331/WUxY/67e9c4b455340d4b4f9c6c47/-473Wx593H-701393955-black-MODEL.jpg" alt="Pair of sneakers">
          <h3>heels</h3>
          <p>₹1,999</p>
        </article>
        <article class="product"><img src="https://static.cilory.com/796431-thickbox_default/women-s-frayed-hem-long-denim-skirt.jpg.webp" alt="denim jeans">
          <h3>Denim Skirt</h3>
          <p>₹1,299</p>
        </article>
        <article class="product"><img src="https://www.giftoo.in/cdn/shop/files/download_21__upscayl_2x_ultrasharp.png?v=1744010944" alt="cute girly headphones">
          <h3>Headphones</h3>
          <p>₹2,999</p>
        </article>
        <article class="product"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdLSepLaFyNJfhI_oVwwd06cINcIXYIYKBA1s1Ry4m_Q0bRXevmjzaToE&s=10" alt="Digital camera">
          <h3>DSLR Camera</h3>
          <p>₹19,999</p>
        </article>
        <article class="product"><img src="https://picsum.photos/id/180/300/300" alt="Laptop on a table">
          <h3>Laptop</h3>
          <p>₹54,999</p>
        </article>
        <article class="product"><img src="https://etimg.etb2bimg.com/thumb/msid-120051117,width-1200,resizemode-4/.jpg" alt="beauty products">
          <h3>Makeup Products</h3>
          <p>₹849</p>
        </article>
      </div>
    </main>
    <footer>&copy; 2026 ShopGrid</footer>
  </div>
</body>

</html>
