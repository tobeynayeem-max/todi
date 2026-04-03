# todi
AI powered freelance marketplace like Fiverr
<!DOCTYPE html>
<html>
<head>
  <title>Todi</title>
  <style>
    body {font-family: Arial; text-align:center; background:#f2f2f2;}
    h1 {color: green;}
  </style>
</head>
<body>

<h1>Welcome to Todi 🚀</h1>
<p>AI Powered Freelance Marketplace</p>

<button onclick="alert('Service coming soon!')">Order Service</button>

</body>
</html>
<!DOCTYPE html>
<html>
<head>
  <title>Todi - Freelance Marketplace</title>
  <style>
    body {margin:0;font-family:Arial;background:#f5f5f5;}
    header {
      background:#111;color:white;padding:15px;
      display:flex;justify-content:space-between;
    }
    .menu a {color:white;margin:10px;text-decoration:none;}
    .hero {
      text-align:center;padding:50px;
      background:linear-gradient(to right,green,blue);
      color:white;
    }
    input {
      padding:10px;width:60%;border:none;
    }
    .services {
      display:flex;flex-wrap:wrap;justify-content:center;
    }
    .card {
      background:white;padding:20px;margin:15px;
      border-radius:10px;width:250px;text-align:center;
      box-shadow:0 0 10px rgba(0,0,0,0.1);
    }
    button {
      padding:10px;background:green;color:white;
      border:none;border-radius:5px;
    }
    #chatbox {
      position:fixed;bottom:10px;right:10px;
      width:250px;background:white;padding:10px;
      border-radius:10px;box-shadow:0 0 10px gray;
    }
  </style>
</head>
<body>

<header>
  <h2>Todi</h2>
  <div class="menu">
    <a href="#">Home</a>
    <a href="#">Services</a>
    <a href="#">Login</a>
  </div>
</header>

<div class="hero">
  <h1>Find the perfect service</h1>
  <input type="text" placeholder="Search services...">
</div>

<div class="services">

  <div class="card">
    <h3>Video Editing</h3>
    <p>Professional video editing</p>
    <button onclick="order('Video Editing')">Order</button>
  </div>

  <div class="card">
    <h3>Logo Design</h3>
    <p>Creative logo design</p>
    <button onclick="order('Logo Design')">Order</button>
  </div>

  <div class="card">
    <h3>AI Content Writing</h3>
    <p>Fast AI writing</p>
    <button onclick="order('AI Writing')">Order</button>
  </div>

</div>

<!-- Chat Box -->
<div id="chatbox">
  <b>AI Helper</b><br>
  <input id="msg" placeholder="Type message">
  <button onclick="reply()">Send</button>
  <p id="chat"></p>
</div>

<script>
function order(service){
  alert("Order placed for " + service);
}

function reply(){
  let msg = document.getElementById("msg").value;
  document.getElementById("chat").innerHTML = "AI: Thanks! I will help you.";
}
</script>

</body>
</html>
