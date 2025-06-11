
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>AFOTECHNIG – Fast & Affordable Data</title>
  <style>
    /* Basic Resets */
    * { margin:0; padding:0; box-sizing:border-box; }
    body, html { height:100%; font-family:Arial,sans-serif; color:#333; }
    a { text-decoration:none; color:inherit; }

    /* Hero Section */
    .hero {
      position:relative; height:100vh; width:100%; overflow:hidden;
      background:#fff;
    }
    .slides {
      position:absolute; width:400%; height:100%; display:flex;
      animation: slideBg 20s infinite;
    }
    .slide {
      flex:1; background-size:cover; background-position:center;
    }
    .slide1 { background-image:url('https://via.placeholder.com/1600x900?text=Fast+Data'); }
    .slide2 { background-image:url('https://via.placeholder.com/1600x900?text=Secure+Payment'); }
    .slide3 { background-image:url('https://via.placeholder.com/1600x900?text=Trusted+Service'); }
    .slide4 { background-image:url('https://via.placeholder.com/1600x900?text=24/7+Support'); }

    @keyframes slideBg {
      0%,20%{transform:translateX(0);}
      25%,45%{transform:translateX(-100%);}
      50%,70%{transform:translateX(-200%);}
      75%,95%{transform:translateX(-300%);}
      100%{transform:translateX(0);}
    }

    .overlay {
      position:absolute; top:0; left:0; width:100%; height:100%;
      background:rgba(255,255,255,0.6);
      display:flex; flex-direction:column;
      justify-content:center; align-items:center; text-align:center;
      backdrop-filter:blur(2px); padding:0 20px;
    }

    .overlay h1 {
      font-size:3rem; color:#4CAF50; margin-bottom:10px;
      animation: fadeInDown 1s ease-out;
    }
    .overlay p {
      font-size:1.2rem; max-width:600px;
      animation: fadeInUp 1s ease-out;
    }

    .btn-group {
      margin-top:20px; display:flex; gap:15px;
      animation: zoomIn 1s ease-out;
    }
    .btn {
      padding:15px 30px; border:none; border-radius:30px;
      font-size:1rem; font-weight:bold; cursor:pointer;
      background:#4CAF50; color:white;
      transition:background 0.3s;
    }
    .btn:hover { background:#388E3C; }

    /* Sign Up/In Forms */
    .form-container {
      margin-top:40px; background:rgba(255,255,255,0.9);
      padding:20px; border-radius:10px;
      box-shadow:0 2px 10px rgba(0,0,0,0.1);
      display:flex; gap:20px; flex-wrap:wrap;
      justify-content:center;
      animation: fadeIn 1s ease-out;
    }
    .form-container form {
      display:flex; flex-direction:column; gap:10px;
      min-width:250px; width:300px;
    }
    .form-container input {
      padding:10px; font-size:1rem;
      border:1px solid #ccc; border-radius:5px;
      outline:none; width:100%;
    }

    /* Footer */
    footer {
      position:absolute; bottom:10px; width:100%;
      text-align:center; color:#555; font-size:0.9rem;
    }

    /* Animations */
    @keyframes fadeInDown {
      from { opacity:0; transform:translateY(-20px); }
      to { opacity:1; transform:none; }
    }
    @keyframes fadeInUp {
      from { opacity:0; transform:translateY(20px); }
      to { opacity:1; transform:none; }
    }
    @keyframes zoomIn {
      from { opacity:0; transform:scale(0.5); }
      to { opacity:1; transform:none; }
    }
    @keyframes fadeIn {
      from { opacity:0; }
      to { opacity:1; }
    }
  </style>
</head>
<body>
  <section class="hero">
    <div class="slides">
      <div class="slide slide1"></div>
      <div class="slide slide2"></div>
      <div class="slide slide3"></div>
      <div class="slide slide4"></div>
    </div>
    <div class="overlay">
      <h1><span>AFO</span>TECHNIG</h1>
      <p>Fast • Secure • Affordable Data Bundles for MTN, Glo, Airtel & 9mobile — powered by professional service in 2025!</p>
      <div class="btn-group">
        <button class="btn" onclick="scrollToForm()">Sign Up</button>
        <button class="btn" onclick="scrollToForm()">Sign In</button>
      </div>
      <div id="formAnchor" class="form-container">
        <!-- Sign Up Form -->
        <form id="signUp">
          <input type="text" placeholder="Full Name" required>
          <input type="email" placeholder="Email Address" required>
          <button class="btn" type="submit">Create Account</button>
        </form>
        <!-- Sign In Form -->
        <form id="signIn">
          <input type="email" placeholder="Email Address" required>
          <input type="password" placeholder="Password" required>
          <button class="btn" type="submit">Log In</button>
        </form>
      </div>
      <footer>© 2025 AFOTECHNIG</footer>
    </div>
  </section>

  <script>
    function scrollToForm(){
      document.getElementById('formAnchor').scrollIntoView({ behavior: 'smooth' });
    }
  </script>
</body>
</html>
