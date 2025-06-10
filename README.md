# Afotechnig-data-site
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>AFOTECHNIG | Data Sales</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      background-color: #fff;
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      color: #333;
    }

    header {
      background: #4CAF50;
      padding: 20px;
      text-align: center;
      color: white;
    }

    .brand {
      font-size: 30px;
      font-weight: bold;
    }

    .brand span {
      color: #4CAF50;
      background: white;
      padding: 3px 6px;
      border-radius: 4px;
    }

    .container {
      max-width: 500px;
      margin: 40px auto;
      padding: 20px;
      background: #f9f9f9;
      border-radius: 8px;
      box-shadow: 0 0 10px #eee;
    }

    h2 {
      color: #4CAF50;
      text-align: center;
    }

    label {
      display: block;
      margin-top: 15px;
      margin-bottom: 5px;
      font-weight: bold;
    }

    select, input {
      width: 100%;
      padding: 10px;
      font-size: 16px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      width: 100%;
      padding: 12px;
      background: #4CAF50;
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    button:hover {
      background: #45a049;
    }

    footer {
      text-align: center;
      margin-top: 50px;
      font-size: 14px;
      color: #777;
    }
  </style>
</head>
<body>

  <header>
    <div class="brand"><span>AFO</span>TECHNIG</div>
    <p>Affordable Data | Fast Delivery | Trusted</p>
  </header>

  <div class="container">
    <h2>Buy Data</h2>

    <form>
      <label for="network">Choose Network</label>
      <select id="network" required>
        <option value="">-- Select Network --</option>
        <option value="MTN">MTN</option>
        <option value="Airtel">Airtel</option>
        <option value="Glo">Glo</option>
        <option value="9mobile">9mobile</option>
      </select>

      <label for="plan">Choose Plan</label>
      <select id="plan" required>
        <option value="">-- Select Data Plan --</option>
        <option value="500MB">500MB – ₦100</option>
        <option value="1GB">1GB – ₦250</option>
        <option value="2GB">2GB – ₦450</option>
        <option value="5GB">5GB – ₦1,000</option>
      </select>

      <label for="phone">Phone Number</label>
      <input type="tel" id="phone" placeholder="Enter phone number" required>

      <label for="pin">Transaction PIN</label>
      <input type="password" id="pin" placeholder="Enter your 4-digit PIN" required>

      <button type="submit">Buy Data</button>
    </form>
  </div>

  <footer>
    &copy; 2025 AFOTECHNIG. All rights reserved.
  </footer>

</body>
</html>
