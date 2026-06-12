# whatsyourzodiac-website
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PANMIÉRE</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<header>
<h1>PANMIÉRE</h1>
<p>Luxury Zodiac Candles</p>

<nav>
<a href="#shop">Shop</a>
<a href="#quiz">Zodiac Quiz</a>
<a href="#about">About</a>
<a href="#contact">Contact</a>
</nav>
</header>

<section class="hero">
<h2>Find the Scent Written in Your Stars</h2>
<button>Shop Collection</button>
</section>

<section id="shop">
<h2>Zodiac Collection</h2>
<div class="card">Aries Candle</div>
<div class="card">Taurus Candle</div>
<div class="card">Gemini Candle</div>
</section>

<section id="about">
<h2>About Panmiére</h2>
<p>Luxury fragrances inspired by the zodiac.</p>
</section>

<section id="contact">
<h2>Contact</h2>
<p>hello@panmiere.com</p>
</section>

</body>
</html>
body{
    margin:0;
    background:#000;
    color:#D4AF37;
    font-family:Georgia,serif;
}

header{
    text-align:center;
    padding:30px;
}

nav a{
    color:#D4AF37;
    text-decoration:none;
    margin:10px;
}

.hero{
    padding:120px 20px;
    text-align:center;
}

section{
    padding:60px 20px;
    text-align:center;
}

.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.card{
    border:1px solid #D4AF37;
    padding:20px;
    border-radius:10px;
}

button{
    background:#D4AF37;
    color:black;
    border:none;
    padding:12px 20px;
    margin-top:10px;
    cursor:pointer;
}

input,textarea,select{
    width:80%;
    max-width:500px;
    margin:10px;
    padding:12px;
}

footer{
    text-align:center;
    padding:20px;
}
function recommend(){

let scent =
document.getElementById("scent").value;

let result = "";

if(scent==="Floral"){
result="Pisces - Lavender Dream";
}
else if(scent==="Fresh"){
result="Aquarius - Ocean Mist";
}
else if(scent==="Woody"){
result="Capricorn - Oak Reserve";
}
else{
result="Aries - Cinnamon Ember";
}

document.getElementById("result").innerHTML =
"Recommended Candle: " + result;
}
