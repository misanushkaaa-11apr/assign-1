<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Demonstration of CSS selector types.">
  <title>CSS Selector Types</title>
  <style>
  * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      background: #eef2f7;
      color: #222;
      padding: 2px;
      line-height: 1.6;
    }

    h1 {
      margin-bottom: 1px;
      color: #1d3557;
    }

    .card {
      background: #fff;
      padding: 10px;
      margin-bottom: 10px;
      border-radius: 8px;
      box-shadow: 0 1px 4px rgba(0, 0, 0, .15);
    }

    .highlight {
      background: #ffe066;
      padding: 2px;
    }

    #special {
      border-left: 6px solid #e63946;
    }

    h2,
    h3 {
      color: #457b9d;
      margin-bottom: 5px;
    }

  </style>
</head>

<body>
  <h1>Selector Playground</h1>

  <div class="card">
    <h2>Class & Element</h2>
    <p>This bold line is styled by the <mark>adjacent sibling</mark> selector.</p>
    <p>This is a normal paragraph styled by the element selector.</p>
  </div>

  <div class="card" id="special">
    <h3>ID selector</h3>
    <p>Only one element on the page may own this id, giving it a red left border.</p>
  </div>

  <div class="card">
    <h3>Descendant, child & pseudo-class</h3>
    <ul>
      <li>Odd item (nth-child)</li>
      <li>Even item</li>
      <li>Odd item with <a href="https://developer.mozilla.org/" target="_blank" rel="noopener">MDN (attribute
          selector)</a></li>
    </ul>
    <p><input type="text" placeholder="Click me – :focus"></p>
  </div>
</body>

</html>
