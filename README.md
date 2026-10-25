# Wester-Eagleticketing-
WESTERN EAGLE ENTERTAINMENT MINISTRY ticketing system 

<!DOCTYPE html>
<html lang="sw">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Western Eagle Ticketing</title>
<style>
body{margin:0;font-family:Arial,sans-serif;background:#f2f5f9;color:#172033}
header{background:#102b55;color:white;text-align:center;padding:30px 15px}
main{max-width:650px;margin:30px auto;padding:0 15px}
.card{background:white;padding:24px;border-radius:12px;box-shadow:0 3px 15px #0001}
label{display:block;margin-top:16px;font-weight:bold}
input,select{box-sizing:border-box;width:100%;padding:12px;margin-top:7px;border:1px solid #ccd3df;border-radius:6px}
button{width:100%;padding:14px;margin-top:22px;background:#e4a629;border:0;border-radius:6px;font-weight:bold;font-size:16px;cursor:pointer}
footer{text-align:center;padding:25px;color:#566176}
</style>
</head>
<body>
<header>
<h1>WESTERN EAGLE</h1>
<p>ENTERTAINMENT MINISTRY</p>
<h2>MFUMO WA TIKETI</h2>
</header>
<main>
<section class="card">
<h2>Omba Tiketi</h2>
<p>Jaza taarifa zako kuomba tiketi ya tukio.</p>
<form id="ticketForm">
<label for="name">Jina kamili</label>
<input id="name" required>
<label for="phone">Namba ya simu</label>
<input id="phone" type="tel" required>
<label for="event">Jina la tukio</label>
<input id="event" required>
<label for="date">Tarehe ya tukio</label>
<input id="date" type="date" required>
<label for="quantity">Idadi ya tiketi</label>
<select id="quantity">
<option>1</option><option>2</option><option>3</option><option>4</option><option>5</option>
</select>
<button type="submit">Wasilisha Ombi</button>
</form>
<p id="message" role="status"></p>
</section>
</main>
<footer>© Western Eagle Entertainment Ministry</footer>
<script>
document.getElementById("ticketForm").addEventListener("submit",function(e){
e.preventDefault();
document.getElementById("message").textContent="Muonekano wa maombi umefanya kazi. Tiketi haijahifadhiwa wala kuthibitishwa bado.";
});
</script>
</body>
</html>
