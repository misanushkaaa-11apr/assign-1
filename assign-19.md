<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Audit of all assignment.">
  <meta name="author" content="Anushka Mishra ">
  <meta name="keywords" content="html, meta tags, css , html, audit"> 
  <title>Meta Tag Audit</title>
  <style>
    body {
      font-family:Times New Roman;
      max-width: 800px;
      margin: auto;
      padding: 20px;
    }

    table {
      border-collapse: collapse;
      width: 100%;
    }

    th,td {
      border: 1px solid #aaa;
      padding: 6px 10px;
      text-align: left;
    }

    th {
      background: #eee;
    }

    .ok {
      color: green;
    }

    .fix {
      color: crimson;
    }
  </style>
</head>

<body>
  <h1>Meta-Tag Audit of Assignments 6 – 18</h1>
  <p>Every HTML file was checked for <code>charset</code>, <code>viewport</code>, <code>description</code> and a
    meaningful <code>&lt;title&gt;</code>.</p>
  <table>
    <thead>
      <tr>
        <th>File</th>
        <th>Missing before</th>
        <th>Status</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>06-basic-page.html</td>
        <td>viewport, description</td>
        <td class="ok">Fixed ✔</td>
      </tr>
      <tr>
        <td>07-resume-text-only.html</td>
        <td>viewport, description</td>
        <td class="ok">Fixed ✔</td>
      </tr>
      <tr>
        <td>08-resume-semantic.html</td>
        <td>viewport, description</td>
        <td class="ok">Fixed ✔</td>
      </tr>
      <tr>
        <td>09-debug-buggy-html.html</td>
        <td>charset (bug #2)</td>
        <td class="ok">Fixed ✔</td>
      </tr>
      <tr>
        <td>10 – 18</td>
        <td>description on some pages</td>
        <td class="ok">Fixed ✔</td>
      </tr>
    </tbody>
  </table>
  <h2>Why each tag matters</h2>
  <ul>
    <li><b>charset</b> – prevents garbled characters such as ₹ or é.</li>
    <li><b>viewport</b> – makes pages usable on phones.</li>
    <li><b>description</b> – the snippet shown in Google results.</li>
    <li><b>Open Graph</b> – controls the preview when the link is shared.</li>
  </ul>
</body>

</html>
