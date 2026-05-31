# -kad-doa-selamat
<!DOCTYPE html>
<html lang="ms">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Jemputan Doa Selamat</title>
<style>
body{
    font-family: Arial, sans-serif;
    background:#f4f4f4;
    margin:0;
    padding:20px;
}
.card{
    max-width:800px;
    margin:auto;
    background:white;
    padding:20px;
    border-radius:15px;
    box-shadow:0 0 10px rgba(0,0,0,0.2);
}
h1,h2{
    text-align:center;
    color:#2c3e50;
}
.section{
    margin-top:20px;
}
input,button{
    width:100%;
    padding:10px;
    margin-top:10px;
}
button{
    background:#27ae60;
    color:white;
    border:none;
    cursor:pointer;
}
button:hover{
    background:#219150;
}
ul{
    padding-left:20px;
}
</style>
</head>
<body>
<div class="card">
<h1>Majlis Doa Selamat</h1>
<p style="text-align:center">
Dengan segala hormatnya menjemput tuan/puan ke majlis doa selamat kami.
</p>
<div class="section">
<h2>Maklumat Majlis</h2>
<p><b>Tarikh:</b> 15 Jun 2026</p>
<p><b>Masa:</b> 7.30 Malam</p>
<p><b>Tempat:</b> No. 123, Taman Harmoni, Kuala Lumpur</p>
</div>
<div class="section">
<h2>Atur Cara</h2>
<ul>
<li>7.30 PM - Ketibaan Tetamu</li>
<li>8.00 PM - Bacaan Yasin</li>
<li>8.30 PM - Doa Selamat</li>
<li>9.00 PM - Jamuan Makan</li>
</ul>
</div>
<div class="section">
<h2>Lokasi</h2>
<iframe
src="https://maps.google.com/maps?q=Kuala%20Lumpur&t=&z=13&ie=UTF8&iwloc=&output=embed"
width="100%"
height="300"
style="border:0;">
</iframe>
</div>
<div class="section">
<h2>Pengesahan Kehadiran (RSVP)</h2>
<input type="text" id="nama" placeholder="Nama">
<button onclick="simpanKehadiran()">
Sahkan Kehadiran
</button>
<h3>Senarai Kehadiran</h3>
<ul id="senarai"></ul>
</div>
</div>
<script>
function simpanKehadiran(){
let nama = document.getElementById("nama").value;
if(nama===""){
    alert("Sila masukkan nama");
    return;
}
let li = document.createElement("li");
li.textContent = nama;
document.getElementById("senarai").appendChild(li);
document.getElementById("nama").value="";
}
</script>
</body>
</html>