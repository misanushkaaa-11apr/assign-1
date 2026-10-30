grid-auto-fit-products.html

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Responsive product grid that reflows with auto-fit and minmax.">
  <title>Auto-Reflowing Product Grid</title>
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: system-ui, sans-serif;
      background: #f5f6fa;
      padding: 2rem 1rem;
    }

    h1 {
      text-align: center;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 1.25rem;
      max-width: 1200px;
      margin: 1.5rem auto;
    }

    .card {
      background: #fff;
      border-radius: 12px;
      padding: 1rem;
      box-shadow: 0 2px 8px rgba(0, 0, 0, .08);
      text-align: center;
    }

    .card img {
      width: 100%;
      aspect-ratio: 4/3;
      object-fit: cover;
      border-radius: 8px;
    }

    .card h2 {
      font-size: 1.05rem;
      margin: .75rem 0 .25rem;
    }

    .price {
      color: #0a8754;
      font-weight: 700;
    }

    .note {
      text-align: center;
      color: #666;
    }
  </style>
</head>

<body>
  <h1>Our Products</h1>
  <div class="grid">
    <div class="card"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRqC-HTIvzv70YLi1WohnpfMzEZ1XFnzz9Ss4K3gc4WEKlG_62XTpeOP7mM&s=10" alt="Coffee beans">
      <h2>Coffee Beans</h2>
      <p class="price">₹399</p>
    </div>
    <div class="card"><img src="https://foodal.com/wp-content/uploads/2015/03/Make-Strawberry-Season-Last-All-Year.jpg" alt="fresh strawberries">
      <h2>Strawberries</h2>
      <p class="price">₹199</p>
    </div>
    <div class="card"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcShrQIG3Bzl2Xk24VSDvz-VJZhVeuH7qWZlVxrZhVSy6Lzo48t2WLyJoNw-&s=10" alt="home spices">
      <h2>Spices</h2>
      <p class="price">₹149</p>
    </div>
    <div class="card"><img src="https://picsum.photos/id/312/400/300" alt="Glass jar of honey">
      <h2>Honey Jar</h2>
      <p class="price">₹329</p>
    </div>
    <div class="card"><img src="https://picsum.photos/id/429/400/300" alt="Cup of tea beside a book">
      <h2>Green Tea</h2>
      <p class="price">₹259</p>
    </div>
    <div class="card"><img src="https://picsum.photos/id/493/400/300" alt="Assorted spices in bowls">
      <h2>Spice Box</h2>
      <p class="price">₹599</p>
    </div>
  </div>
</body>

</html>
