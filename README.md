<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Member - IPKOLINDO</title>

<link rel="stylesheet" href="style.css">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>

<body>

<!-- ================= HEADER ================= -->
<header>
        <div class="logo">
            <img src="lpkolindo.png" alt="Logo">
            <div class="logo-text">
                <h3>IPKOLINDO</h3>
                <span>Ikatan Pelatih Kolintang Indonesia</span>
            </div>
        </div>
        <nav>
            <a href="home.html">Home</a>
            <a href="profile.html">Profile</a>
            <a href="member.html" class="active">Member</a>
            <a href="news.html">News</a>
            <a href="kontak.html">Contact</a>
        </nav>
    </header>


<!-- ================= MEMBER ================= -->
<section class="member-section">
   
<h2>Daftar Nama Pelatih Kolintang</h2>


<!-- SEARCH -->
<input type="text" id="searchInput" placeholder="Cari nama / domisili...">

<!-- TABLE -->
 
<div class="table-box">
  <div class="table-wrapper">

    <table id="pelatihTable">
  <thead>
    <tr>
      <th style="width: 50px;">No</th> <th onclick="sortTable(0)">Nama Pelatih ⬍</th>
      <th onclick="sortTable(1)">Domisili ⬍</th>
      <th>Aksi</th>
    </tr>
  </thead>
  <tbody id="pelatihBody">
    </tbody>
</table>

      <tbody id="pelatihBody">
        <!-- DATA DIISI OTOMATIS DARI JS -->
      </tbody>

    </table>

  </div>
</div>

</section>

<div id="pelatihModal" class="popup">
    <div class="popup-content">
        <span class="close" onclick="closeModal()">&times;</span>
        <img id="modalImg" src="" alt="Foto Pelatih">
        <h3 id="modalNama" style="margin-bottom: 5px; color: #2c5aa0;"></h3>
        <p id="modalDomisili" style="font-weight: bold; color: #666; margin-bottom: 15px;"></p>
        <hr style="margin-bottom: 15px; opacity: 0.3;">
        <div style="text-align: left; font-size: 14px; line-height: 1.6;">
            <strong>Biodata:</strong>
            <p id="modalBiodata" style="margin-bottom: 10px;"></p>
            <strong>Prestasi:</strong>
            <p id="modalPrestasi"></p>
        </div>
    </div>
</div>
<!-- ================= FOOTER ================= -->
<footer>
<p>© 2025 IPKOLINDO</p>
</footer>


<!-- ================= JS ================= -->
<script src="js_member.js"></script>

</body>
</html>
