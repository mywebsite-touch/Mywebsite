# <!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ফ্রিতে ফেক লগইন পেজ</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #89f7fe, #66a6ff);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .container {
      background: #fff;
      padding: 40px 50px;
      border-radius: 15px;
      box-shadow: 0 8px 25px rgba(0,0,0,0.2);
      text-align: center;
      width: 100%;
      max-width: 400px;
    }
    h1 {
      margin-bottom: 20px;
      color: #333;
    }
    input[type="text"], input[type="password"] {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 1em;
    }
    button {
      width: 100%;
      padding: 12px;
      background: #66a6ff;
      border: none;
      border-radius: 8px;
      color: #fff;
      font-size: 1em;
      cursor: pointer;
      transition: 0.3s;
    }
    button:hover {
      background: #89f7fe;
    }
    .footer {
      margin-top: 15px;
      font-size: 0.9em;
      color: #555;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Login</h1>
    <form onsubmit="fakeLogin(event)">
      <input type="text" placeholder="Username" required>
      <input type="password" placeholder="Password" required>
      <button type="submit">Login</button>
    </form>
    <div class="footer">© 2025 Safe Practice Demo</div>
  </div>

  <script>
    function fakeLogin(event) {
      event.preventDefault(); // ফর্ম সাবমিট ব্লক
      alert("ধন্যবাদ! এটি শুধুই শেখার জন্য। আপনার ডেটা কোথাও যাবে না।");
    }
  </script>
</body>
</html>
