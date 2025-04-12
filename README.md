<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Under the Rooftop Sky</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Roboto&display=swap" rel="stylesheet">
  <style>
    body, html {
      margin: 0;
      padding: 0;
      font-family: 'Roboto', sans-serif;
      background-color: #1e1e2f;
      color: #fff;
      overflow: hidden;
    }
    .gate {
      position: fixed;
      top: 0; left: 0;
      width: 100vw;
      height: 100vh;
      background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1503264116251-35a269479413?auto=format&fit=crop&w=1470&q=80') center/cover no-repeat;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      z-index: 10;
      transition: opacity 1s ease;
    }
    .gate h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3em;
      margin-bottom: 0.5em;
    }
    .gate p {
      font-size: 1.2em;
      margin-bottom: 1.5em;
    }
    .enter-btn {
      padding: 0.8em 2em;
      font-size: 1em;
      border: none;
      background-color: #ff6f61;
      color: white;
      border-radius: 10px;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    .enter-btn:hover {
      background-color: #ff4e42;
    }
    .content {
      display: none;
      height: 100vh;
    }
    iframe {
      width: 100%;
      height: 100%;
      border: none;
    }
  </style>
</head>
<body>
  <div class="gate" id="gate">
    <h1>Under the Rooftop Sky</h1>
    <p>A Love Story Written in the Stars</p>
    <button class="enter-btn" onclick="enterSite()">Enter the Story</button>
  </div>

  <div class="content" id="content">
    <iframe src="Untitled%20design_20250412_123322_0000.pdf#toolbar=0" allowfullscreen></iframe>
  </div>

  <script>
    function enterSite() {
      document.getElementById('gate').style.opacity = 0;
      setTimeout(() => {
        document.getElementById('gate').style.display = 'none';
        document.getElementById('content').style.display = 'block';
      }, 1000);
    }
  </script>
</body>
</html>
