<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Post 2 - ERD: Attribute, Entitas, Relasi</title>
  <style>
    :root{
      --pink:#ff8fb1;
      --ungu:#8b5cf6;
      --abu:#8d7792;
      --hitam:#0b0b0b;
      --biru:#4da6ff;
      --glass: rgba(255,255,255,0.6);
      --card-shadow: 0 8px 24px rgba(11,11,11,0.12);
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }

    *{box-sizing:border-box}
    html,body{height:100%;margin:0;background:linear-gradient(180deg,#8268ac,#000000);color:var(--hitam)}

    .container{max-width:980px;margin:28px auto;padding:20px}
    
    header{display:flex;align-items:center;gap:18px;padding:18px;border-radius:18px;background:linear-gradient(90deg,rgba(238, 230, 255, 0.829),rgba(144, 89, 154, 0.708));box-shadow:var(--card-shadow)}

    .avatar{
      width:100px;height:100px;border-radius:18px;overflow:hidden;flex:0 0 100px;background:linear-gradient(135deg,var(--pink),var(--ungu));display:grid;place-items:center;border:4px solid rgba(255,255,255,0.6);
    }
    .avatar img{width:100%;height:100%;object-fit:cover;display:block}
    .profile-info h1{margin:0;font-size:1.25rem;color:#371b5e}
    .profile-info p{margin:6px 0 0;color:#371b5e}
    .badges{margin-top:8px;display:flex;gap:8px;color:#371b5e}
    .badge{background:#e6e6e9;padding:6px 10px;border-radius:999px;font-size:12px}


    /* Navbar */
    .navbar {
      background: linear-gradient(90deg, #a855f7, #ec4899);
      color: white;
      padding: 12px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-radius: 0 0 12px 12px;
    }
    .navbar .logo { font-weight: bold; font-size: 18px; }
    .navbar ul { list-style: none; display: flex; gap: 16px; margin: 0; padding: 0; }
    .navbar ul li a { color: white; text-decoration: none; font-weight: 600; }
    .navbar ul li a:hover { text-decoration: underline; }

    /* Hero Video */
    .hero {
      text-align: center;
      margin-top: 20px;
    }
    .hero iframe {
      width: 100%;
      max-width: 720px;
      height: 405px;
      border-radius: 12px;
      border: none;
      box-shadow: var(--card-shadow);
    }

    /* Konten */
    .post {
      background:linear-gradient(180deg,rgba(255, 255, 255, 0.8),rgba(208, 195, 220, 0.7));
      border-radius:14px;
      box-shadow:var(--card-shadow);
      padding:20px;
      margin-top:20px;
    }
    .post h1 { color:#8a36ff; margin-top:0; }
    .post p { line-height:1.6; color:#222; }
    .post ul { margin:10px 0 10px 20px; }

    footer{margin-top:20px;text-align:center;color:#ccc;font-size:13px}
  </style>
</head>
<body>
  <!-- Navbar -->
  <nav class="navbar">
    <div class="logo">🌸 My Blog</div>
    <ul>
      <li><a href="index.html">Home</a></li>
      <li><a href="profile.html">Profile</a></li>
      <li><a href="blog.html">Tugas Blog</a></li>
    </ul>
  </nav>

    <div class="container">
    <header>
      <div class="avatar" id="avatar">
        <div class="avatar" id="avatar">
        <img src="foto1.jpg" alt="Foto Profil" class="profile-img">
      </div>
    </div>
      <div class="profile-info">
          <h1>KAISHA KAMILA PUSPITO</h1>
          <p>Teknik Informatika UBP Karawang</p>
          <div class="badges">
            <span class="badge">NIM : 24416255201028</span>
            <span class="badge">if24.kaishapuspito@mhs.ubpkarawang.ac.id</span>
            <span class="badge">Basis Data</span>
          </div>
      </div>
    </header>


  <!-- Hero Video -->
  <div class="hero">
    <iframe src="https://www.youtube.com/embed/x_DNoLEnW3U?si=M3lwcgRAyqyZW2Tr" 
      title="YouTube video" allowfullscreen></iframe>
  </div>

  <div class="container">
    <div class="post">
      <h1>Post 2: Apa itu Attribute, Entitas, dan Relasi dalam ERD?</h1>
      <p>Dalam <em>Entity Relationship Diagram (ERD)</em>, ada tiga komponen utama yang digunakan untuk memodelkan data:</p>

      <ul>
        <li><strong>Entitas</strong> → objek nyata atau abstrak yang informasinya ingin kita simpan.  
          <br>Contoh: <em>Mahasiswa, Dosen, Mata Kuliah</em>.</li>
        <li><strong>Atribut</strong> → karakteristik atau properti dari sebuah entitas.  
          <br>Contoh: entitas Mahasiswa punya atribut <em>NIM, Nama, Tanggal Lahir</em>.</li>
        <li><strong>Relasi</strong> → hubungan antar entitas.  
          <br>Contoh: Mahasiswa <em>mengambil</em> Mata Kuliah, Dosen <em>mengajar</em> Mata Kuliah.</li>
      </ul>

      <p>ERD membantu kita menggambarkan struktur data secara konseptual sehingga lebih mudah dipahami sebelum diimplementasikan menjadi tabel dalam basis data.</p>
    </div>

    <footer>
      © 2025 Blog Basis Data | Kaisha | <a href="https://www.ubpkarawang.ac.id" target="_blank" style="color:#fff">UBP Karawang</a>
    </footer>
  </div>
</body>
</html>
