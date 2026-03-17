<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Welcome - Adeel Ali</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(-45deg, #0f2027, #203a43, #2c5364, #00c6ff);
      background-size: 400% 400%;
      animation: gradientBG 10s ease infinite;
      overflow: hidden;
      color: white;
    }

    @keyframes gradientBG {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .container {
      text-align: center;
      backdrop-filter: blur(15px);
      background: rgba(255, 255, 255, 0.1);
      padding: 50px;
      border-radius: 20px;
      box-shadow: 0 0 40px rgba(0,0,0,0.3);
      animation: fadeIn 2s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }

    h1 {
      font-size: 45px;
      margin-bottom: 10px;
      animation: slideDown 1.5s ease;
    }

    h2 {
      font-weight: 300;
      margin-bottom: 20px;
      animation: slideUp 1.5s ease;
    }

    @keyframes slideDown {
      from { opacity: 0; transform: translateY(-40px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes slideUp {
      from { opacity: 0; transform: translateY(40px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .btn {
      margin-top: 20px;
      padding: 12px 30px;
      border: none;
      border-radius: 30px;
      background: #00c6ff;
      color: black;
      font-size: 16px;
      cursor: pointer;
      transition: 0.3s;
    }

    .btn:hover {
      background: white;
      transform: scale(1.1);
    }

    .loader {
      margin-top: 20px;
      font-size: 14px;
      opacity: 0.8;
    }

  </style>
</head>
<body>

  <div class="container">
    <h1>Hi, I'm Syed Anees</h1>
    <h2>Rigger 3 & EOT Crane Operator</h2>

    <button class="btn" onclick="goToSite()">Enter Website</button>

    <div class="loader">Redirecting automatically...</div>
  </div>

  <script>
    function goToSite() {
      window.location.href = "home.html";
    }

    // Auto redirect after 4 seconds
    setTimeout(() => {
      window.location.href = "home.html";
    }, 4000);
  </script>

</body>
</html>
