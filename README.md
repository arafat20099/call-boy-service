<!DOCTYPE html>
<html>
<head>
  <title>Registration Form</title>

  <!-- Premium font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;800&display=swap" rel="stylesheet">

  <style>
    body {
      margin:0;
      padding:0;
      background: #000;
      font-family: 'Poppins', sans-serif;
      color:white;
      display:flex;
      justify-content:center;
      align-items:center;
      height:100vh;
    }

    .container {
      background:#111;
      padding:25px;
      width:400px;
      border-radius:12px;
      box-shadow:0 0 20px rgba(0,0,0,0.7);
    }

    h2 {
      text-align:center;
      margin-bottom:20px;
    }

    label {
      display:block;
      margin-top:12px;
      font-size:14px;
    }

    input, select, textarea {
      width:100%;
      padding:10px;
      margin-top:5px;
      border-radius:6px;
      border:1px solid #333;
      background:#000;
      color:white;
    }

    textarea {
      resize:none;
    }

    button {
      width:100%;
      padding:12px;
      margin-top:15px;
      background:#ff0055;
      border:none;
      border-radius:6px;
      color:white;
      font-weight:bold;
      font-size:16px;
      cursor:pointer;
    }

    button:hover {
      background:#ff3366;
    }

    .success {
      text-align:center;
      margin-top:10px;
      color:#0f0;
      font-weight:bold;
    }

    .footer {
      text-align:center;
      font-size:12px;
      margin-top:15px;
    }
  </style>
</head>

<body>

<div class="container">

<h2>Premium Registration</h2>

<form id="regForm">

<label>Full Name</label>
<input type="text" required>

<label>Age</label>
<input type="number" required>

<label>Location</label>
<input type="text" required>

<label>Experience</label>
<input type="text">

<label>Available Time</label>
<input type="text">

<label>Payment Method</label>
<select>
<option>Bkash</option>
<option>Nagad</option>
<option>Binance</option>
<option>Bybit</option>
</select>

<label>Select Package</label>
<select>
<option>3 Months</option>
<option>8 Months VIP</option>
<option>1.5 Year VIP</option>
<option>Lifetime Premium</option>
</select>

<label>Message</label>
<textarea rows="3"></textarea>

<button type="submit">Submit Registration</button>

</form>

<div class="success" id="successMsg"></div>

<div class="footer">
Contact Telegram:
<a href="https://t.me/ariyan9087" target="_blank">@ariyan9087</a>
</div>

</div>

<script>
const form = document.getElementById("regForm");

form.addEventListener("submit", function(e){
  e.preventDefault();

  document.getElementById("successMsg").innerText =
  "Registration successful! Redirecting...";

  setTimeout(function(){
    window.location.href = "https://t.me/luxury_bd_agency_vip";
  },2000);
});
</script>

</body>
</html>
