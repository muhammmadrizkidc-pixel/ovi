!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>WARUNG MBA OVI
  </title>BERDIRI SEJAK KEMARIN KARENA LELAH

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Poppins',sans-serif;
    }

    body{
      background:#f8f5f2;
      color:#333;
    }

    header{
      background:rgba(0,0,0,0.7);
      backdrop-filter:blur(10px);
      position:fixed;
      width:100%;
      top:0;
      z-index:1000;
      padding:20px 50px;
      display:flex;
      justify-content:space-between;
      align-items:center;
    }

    header h1{
      color:#fff;
      font-size:30px;
      letter-spacing:2px;
    }

    nav a{
      color:#fff;
      text-decoration:none;
      margin-left:25px;
      font-weight:500;
      transition:0.3s;
    }

    nav a:hover{
      color:#ffb347;
    }

    .hero{
      height:100vh;
      background:
      linear-gradient(rgba(0,0,0,0.5),rgba(0,0,0,0.5)),
      url('https://images.unsplash.com/photo-1504674900247-0877df9cc836?q=80&w=1400') center/cover;
      display:flex;
      justify-content:center;
      align-items:center;
      text-align:center;
      color:white;
      padding:20px;
    }

    .hero-content h2{
      font-size:60px;
      margin-bottom:20px;
    }

    .hero-content p{
      font-size:20px;
      margin-bottom:30px;
    }

    .hero-content button{
      padding:15px 35px;
      border:none;
      border-radius:40px;
      background:#ffb347;
      color:#fff;
      font-size:18px;
      cursor:pointer;
      transition:0.3s;
    }

    .hero-content button:hover{
      background:#ff9800;
      transform:scale(1.05);
    }

    .products{
      padding:100px 60px;
    }

    .section-title{
      text-align:center;
      font-size:40px;
      margin-bottom:50px;
      color:#222;
    }

    .product-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:30px;
    }

    .card{
      background:white;
      border-radius:20px;
      overflow:hidden;
      box-shadow:0 8px 20px rgba(0,0,0,0.1);
      transition:0.3s;
    }

    .card:hover{
      transform:translateY(-10px);
    }

    .card img{
      width:100%;
      height:220px;
      object-fit:cover;
    }

    .card-body{
      padding:25px;
    }

    .card-body h3{
      margin-bottom:10px;
      font-size:24px;
    }

    .price{
      color:#ff9800;
      font-size:22px;
      font-weight:bold;
      margin-bottom:20px;
    }

    .card-body button{
      width:100%;
      padding:12px;
      border:none;
      border-radius:10px;
      background:#222;
      color:white;
      font-size:16px;
      cursor:pointer;
      transition:0.3s;
    }

    .card-body button:hover{
      background:#ff9800;
    }

    .cart{
      position:fixed;
      bottom:20px;
      right:20px;
      background:#222;
      color:white;
      padding:15px 20px;
      border-radius:50px;
      font-weight:bold;
      box-shadow:0 5px 15px rgba(0,0,0,0.3);
      z-index:1000;
    }

    .music-btn{
      position:fixed;
      bottom:90px;
      right:20px;
      background:#ff9800;
      color:white;
      border:none;
      padding:15px;
      border-radius:50%;
      font-size:20px;
      cursor:pointer;
      box-shadow:0 5px 15px rgba(0,0,0,0.3);
    }

    footer{
      background:#111;
      color:white;
      text-align:center;
      padding:30px;
      margin-top:50px;
    }

    @media(max-width:768px){

      header{
        padding:20px;
      }

      .hero-content h2{
        font-size:38px;
      }

      .hero-content p{
        font-size:16px;
      }

      .products{
        padding:80px 20px;
      }
    }
  </style>
</head>
<body>

  <!-- Musik Elegan -->
  <audio id="bgMusic" loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_c8c8e57d8c.mp3?filename=luxury-lounge-112191.mp3" type="audio/mp3">
  </audio>70


  <header>
    <h1>WARUNG MBA OVI</h1>

    <nav>
      <a href="#">Home</a>
      <a href="#">Menu</a>
      <a href="#">About</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-content">
      <h2>WARUNG MBA OVI</h2>
      <p>Nikmati makanan premium dengan suasana mewah harga lebih murah</p>
      <button>Lihat Menu</button>
    </div>
  </section>

  <section class="products">

    <h2 class="section-title">Menu Favorit</h2>

    <div class="product-grid">

      <div class="card">
        <img src="https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?q=80&w=800">
        <div class="card-body">
          <h3>Pizza Italian</h3>
          <div class="price">Rp 85.000</div>
          <button onclick="addToCart()">Tambah ke Keranjang</button>
        </div>
      </div>

      <div class="card">
        <img src="https://images.unsplash.com/photo-1550547660-d9450f859349?q=80&w=800">
        <div class="card-body">
          <h3>Burger Premium</h3>
          <div class="price">Rp 55.000</div>
          <button onclick="addToCart()">Tambah ke Keranjang</button>
        </div>
      </div>

      <div class="card">
        <img src="https://images.unsplash.com/photo-1604908176997-4310f7f1c6d4?q=80&w=800">
        <div class="card-body">
          <h3>Chicken Crispy</h3>
          <div class="price">Rp 40.000</div>
          <button onclick="addToCart()">Tambah ke Keranjang</button>
        </div>
      </div>

    </div>

  </section>

  <div class="cart">
    🛒 Cart: <span id="cart-count">0</span>
  </div>

  <!-- Tombol Musik -->
  <button class="music-btn" onclick="toggleMusic()">
    🎵
  </button>

  <footer>
    © 2026 WARUNG MBA OVI
  </footer>

  <script>

    let cart = 0;

    function addToCart(){
      cart++;
      document.getElementById('cart-count').innerText = cart;

      alert("Produk berhasil ditambahkan!");
    }

    const music = document.getElementById("bgMusic");

    let isPlaying = false;

    function toggleMusic(){

      if(isPlaying){
        music.pause();
        isPlaying = false;
      }else{
        music.play();
        isPlaying = true;
      }
    }

    // Auto play saat user klik layar pertama kali
    document.body.addEventListener('click', function () {
      if(!isPlaying){
        music.play();
        isPlaying = true;
      }
    }, { once:true });

  </script>

</body>
</html>
