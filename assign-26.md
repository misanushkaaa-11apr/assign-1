<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="box model">
  <title>Box Model</title>
  <style>
    body {
      font-family: system-ui, sans-serif;
      max-width: 860px;
      margin: 0 auto;
      padding: 1.5rem;
      line-height: 1.5;
    }
    .my-box {
      width: 200px;
      height: 80px;
      padding: 20px;
      border: 10px solid #1d3557;
      margin: 30px;
      background: #a8dadc;
      display: grid;
      place-items: center;
      font-weight: bold;
    }
    .layer {
      display: grid;
      place-items: center;
      position: relative;
      text-align: center;
      font-size: .8rem;
    }
    .l-margin {
      background: #f9cb9c;
      padding: 36px;
    }
    .l-border {
      background: #ffe599;
      padding: 22px;
    }
    .l-padding {
      background: #b6d7a8;
      padding: 36px;
    }
    .l-content {
      background: #9fc5e8;
      padding: 28px 40px;
    }
    .tag {
      position: absolute;
      top: 3px;
      left: 8px;
      font-weight: bold;
    }

    .demo {
      display: flex;
      gap: 2rem;
      flex-wrap: wrap;
      align-items: flex-start;
    }

    table {
      border-collapse: collapse;
    }

    th,
    td {
      border: 1px solid #999;
      padding: .35rem .7rem;
    }

    code {
      background: #eee;
      padding: 0 .25rem;
    }
  </style>
</head>

<body>
    <h1>Box Model of <code>.my-box</code></h1>
  <div class="demo">
    <div class="my-box">Hello</div>

    <!-- Annotated diagram -->
    <div class="layer l-margin"><span class="tag">margin 30px</span>
      <div class="layer l-border"><span class="tag">border 10px</span>
        <div class="layer l-padding"><span class="tag">padding 20px</span>
          <div class="layer l-content">content<br>250 × 80</div>
        </div>
      </div>
    </div>
  </div>

    <h2>Box Model Calculation</h2>

    <table>
        <tr>
            <th>Property</th>
            <th>Calculation</th>
            <th>Total</th>
        </tr>
        <tr>
            <td>Width</td>
            <td>200 + 40 + 20</td>
            <td>260px</td>
        </tr>
        <tr>
            <td>Height</td>
            <td>80 + 40 + 20</td>
            <td>140px</td>
        </tr>
    </table>

    <h2>Box Sizing</h2>

    <p>
        By default, CSS uses content-box. The padding and border
        are added to the given width and height.
    </p>

    <p>
        With box-sizing: border-box, the given width and height
        include the padding and border.
    </p>

</body>
</html>
