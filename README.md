html = """<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Surat Hari Guru - Bu Titik</title>
<style>
body {
    margin: 0;
    font-family: Georgia, serif;
    background: linear-gradient(135deg, #fff0d9, #f8c9c9);
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}
.container {
    width: 85%;
    max-width: 450px;
    padding: 30px 20px;
}
h1 { color: #a13c52; }
.envelope {
    font-size: 100px;
    cursor: pointer;
    transition: transform .3s;
}
.envelope:hover { transform: scale(1.1); }
button {
    background: #a13c52;
    color: white;
    border: none;
    padding: 13px 25px;
    border-radius: 25px;
    cursor: pointer;
    font-size: 16px;
}
.letter {
    display: none;
    background: #fffdf5;
    padding: 25px;
    border-radius: 15px;
    box-shadow: 0 5px 20px #0002;
    line-height: 1.8;
    color: #543b3b;
    animation: muncul 1s;
}
@keyframes muncul {
    from {opacity:0; transform:translateY(20px);}
    to {opacity:1; transform:translateY(0);}
}
.footer { color: #a13c52; font-weight: bold; }
</style>
</head>
<body>
<div class="container">
    <h1>🌷 Selamat Hari Guru 🌷</h1>
    <p>Ada sebuah surat spesial untuk Bu Titik.</p>

    <div class="envelope" onclick="bukaSurat()">💌</div>
    <p>Klik amplop untuk membuka surat</p>

    <button onclick="bukaSurat()">Buka Surat</button>

    <div class="letter" id="surat">
        <h2>Untuk Bu Titik ❤️</h2>
        <p>
        Terima kasih, Bu Titik, atas segala ilmu,
        kesabaran, bimbingan, dan kasih sayang
        yang telah Ibu berikan kepada kami.
        </p>
        <p>
        Terima kasih karena selalu membimbing kami
        untuk menjadi pribadi yang lebih baik.
        Jasa dan kebaikan Ibu akan selalu kami kenang.
        </p>
        <h2>Terima Kasih, Bu Titik! 🌹</h2>
        <p class="footer">
        Selamat Hari Guru! ❤️
        </p>
    </div>
</div>

<script>
function bukaSurat() {
    document.getElementById("surat").style.display = "block";
}
</script>
</body>
</html>
"""

with open("surat_hari_guru.html", "w", encoding="utf-8") as file:
    file.write(html)

print("Surat berhasil dibuat!")
print("Nama file: surat_hari_guru.html")
```

