<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Review Buku Modern</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* Reset dan General */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f5f5f5;
            color: #333;
            line-height: 1.6;
            transition: background-color 0.3s, color 0.3s;
        }

        body.dark-mode {
            background-color: #1a1a2e;
            color: #ddd;
        }

        /* Navbar */
        nav {
            background: #4e54c8;
            color: white;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 1rem;
        }

        nav ul li a:hover {
            color: #f1c40f;
        }

        nav .dark-mode-toggle {
            cursor: pointer;
        }

        /* Header */
        header {
            background: linear-gradient(45deg, #4e54c8, #8f94fb);
            color: white;
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        header p {
            font-size: 1rem;
        }

        /* Search Bar */
        .search-container {
            margin: 20px auto;
            max-width: 600px;
            display: flex;
            gap: 10px;
        }

        .search-container input {
            flex: 1;
            padding: 10px;
            font-size: 1rem;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .search-container button {
            padding: 10px 20px;
            font-size: 1rem;
            background-color: #4e54c8;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .search-container button:hover {
            background-color: #8f94fb;
        }

        /* Container */
        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 0 15px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        /* Card */
        .card {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
        }

        .card img {
            width: 100%;
            height: auto;
            /* Menjaga proporsi gambar */
            aspect-ratio: 2 / 3;
            /* Untuk ukuran 1080x1920 */
        }

        .card-content {
            padding: 15px;
        }

        .card-content h2 {
            font-size: 1.5rem;
            margin-bottom: 10px;
            color: #4e54c8;
        }

        .card-content p {
            font-size: 0.9rem;
            margin-bottom: 10px;
            color: #666;
        }

        .rating {
            margin-top: 10px;
            display: flex;
            align-items: center;
            font-size: 1rem;
            color: #f1c40f;
        }

        .rating span {
            margin-left: 5px;
            font-size: 0.9rem;
            color: #333;
        }

        /* Footer */
        footer {
            text-align: center;
            background: #4e54c8;
            color: white;
            padding: 10px 0;
            margin-top: 20px;
            font-size: 0.9rem;
        }

        label {
            border: 1px solid;
            padding: 5px;
            background-color: #333;
            color: whitesmoke;
            border: none;
            border-radius: 5px;
            margin-left: 60%;
        }
    </style>
</head>

<body>
    
    <!-- Navbar -->
    <nav>
        <div class="logo">Riutrive</div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#buku">Buku</a></li>
            <li><a href="#kontak">Kontak</a></li>
        </ul>
        <div class="dark-mode-toggle">
            <i class="fas fa-moon"></i>
        </div>
    </nav>

    <!-- Header -->
    <header id="home">
        <h1>Selamat Datang di Riutrive</h1>
        <p>Temukan ulasan buku terbaik dan menarik untuk inspirasi membaca Anda dari unitrive!</p>
    </header>
    

    <!-- Search Bar -->
    <div class="search-container">
        <input type="text" id="searchBar" placeholder="Cari berdasarkan judul, penulis, atau deskripsi...">
        <button onclick="searchBooks()">Cari</button>
    </div>

   

    <div class="container" id="bookContainer">
        <!-- Card 1 -->
        <div class="card">
            <a href="halaman selanjutnya.html">
                <img src="images/Selamat Tinggal.png" alt="Cover Buku Dunia Sophie"></a>
                <div class="card-content">
                <h2>Selamat Tinggal</h2>
                <p><strong>Penulis:</strong> Tere Liye</p>
                <p>Buku ini bercerita tentang Sintong Tinggal, mahasiswa yang lulus setelah 6 tahun dengan skripsi
                    tentang Sutan Pane. Ia bekerja paruh waktu di toko buku bajakan dan menyadari dampaknya terhadap
                    penulis. Pertemuannya dengan Jess dan Bunga, mahasiswa fakultas ekonomi, di toko buku bajakan
                    membuka jalan bagi hubungan dan konflik yang menarik.</p>
                <a href="halaman selanjutnya.html">
                    <label for="tombol">Selengkapnya</label></a>
                <div class="rating">
                    ⭐⭐⭐⭐<span>(4.5/5)</span>
                </div>
            </div>
        </div>

        <!-- Card 2 -->
        <div class="card">
            <a href="Hal 2 Laut Bercerita.html">
                 <img src="images/Laut Bercerita jernih.png" alt="Cover Buku Laskar Pelangi"></a>
                <div class="card-content">
                <h2>Laut Bercerita</h2>
                <p><strong>Penulis:</strong> Leila S. Chudori</p>
                <p>Laut Bercerita, novel dari Leila S. Chudori, bertutur tentang kisah keluarga yang kehilangan,
                    sekumpulan sahabat yang merasakan kekosongan di dada, sekelompok orang yang gemar menyiksa dan
                    lancar berkhianat, sejumlah keluarga yang mencari kejelasan makam anaknya, dan tentang cinta yang
                    tak akan luntur.</p>
                <a href="Hal 2 Laut Bercerita.html">
                    <label for="tombol">Selengkapnya</label></a>
                <div class="rating">
                    ⭐⭐⭐⭐⭐<span>(5/5)</span>
                </div>
            </div>
        </div>

        <!-- Card 3 -->
        <div class="card">
            <a href="Hal 2 Home Sweet Loan.html">
            <img src="images/Home_Sweet_Loan_cov.png" alt="Cover Buku The Alchemist"></a>
            <div class="card-content">
                <h2>Home Sweet Loan</h2>
                <p><strong>Penulis:</strong> Christian Simamora</p>
                <p> Home Sweet Loan adalah novel karya Christian Simamora yang menceritakan perjuangan seorang wanita muda bernama Jasmine dalam menghadapi realitas pahit kehidupan urban.
                    Jasmine, seorang pekerja kantoran, terjebak dalam dilema besar: mengejar impiannya memiliki rumah sendiri di Jakarta atau terus berkutat dengan gaya hidup konsumtif yang tidak ada habisnya.
                </p>
                <a href="Hal 2 Home Sweet Loan.html">
                    <label for="tombol">Selengkapnya</label></a>
                <div class="rating">
                    ⭐⭐⭐⭐<span>(4.2/5)</span>
                </div>
            </div>
        </div>
        <!-- Card 4 -->
        <div class="card">
            <a href="halaman selanjutnya.html">
                <img src="images/Hello_Cello.png" alt="Cover Buku Dunia Sophie"></a>
                <div class="card-content">
                <h2>Hello Cello</h2>
                <p><strong>Penulis:</strong> Nadia Ristivani</p>
                <p>Novel ini menggambarkan perjalanan Cello dalam mencari makna hidup, menghadapi trauma masa lalu, serta hubungannya dengan orang-orang di sekitarnya, termasuk keluarga dan teman-temannya.
                </p>
                
                
                
                <a href="halaman selanjutnya.html">
                <label for="tombol">Selengkapnya</label></a>
                
                
                    <div class="rating">
                   ⭐⭐⭐⭐<span>(4.4/5)</span>
                </div>
            
            </div>
        </div>
        <!-- Card 5 -->
        <div class="card">
            <a href="halaman selanjutnya.html">
                <img src="images/Hello cello again.png"alt="Cover Buku Dunia Sophie"></a>
                <div class="card-content">
                <h2>Hello Cello Again</h2>
                <p><strong>Penulis:</strong> Tere Liye</p>
                <p>Buku ini bercerita tentang Sintong Tinggal, mahasiswa yang lulus setelah 6 tahun dengan skripsi
                    tentang Sutan Pane. Ia bekerja paruh waktu di toko buku bajakan dan menyadari dampaknya terhadap
                    penulis. Pertemuannya dengan Jess dan Bunga, mahasiswa fakultas ekonomi, di toko buku bajakan
                    membuka jalan bagi hubungan dan konflik yang menarik.</p>
                <a href="halaman selanjutnya.html">
                    <label for="tombol">Selengkapnya</label></a>
                <div class="rating">
                    ⭐⭐⭐⭐<span>(4.5/5)</span>
                </div>
            </div>
        </div>
        <!-- Card 6 -->
        <div class="card">
            <a href="halaman selanjutnya.html">
                <img src="images/Azzamine.png" alt="Cover Buku Dunia Sophie"></a>
                <div class="card-content">
                <h2>Azzamine</h2>
                <p><strong>Penulis:</strong> Shopie Aulia</p>
                <p>Buku ini bercerita tentang Sintong Tinggal, mahasiswa yang lulus setelah 6 tahun dengan skripsi
                    tentang Sutan Pane. Ia bekerja paruh waktu di toko buku bajakan dan menyadari dampaknya terhadap
                    penulis. Pertemuannya dengan Jess dan Bunga, mahasiswa fakultas ekonomi, di toko buku bajakan
                    membuka jalan bagi hubungan dan konflik yang menarik.</p>
                <a href="halaman selanjutnya.html">
                    <label for="tombol">Selengkapnya</label></a>
                <div class="rating">
                    ⭐⭐⭐⭐<span>(4.5/5)</span>
                </div>
            </div>
        </div>

        <!-- Card 7 -->
        <div class="card">
            <a href="halaman selanjutnya.html">
                <img src="images/Teluk alaska.png" alt="Cover Buku Dunia Sophie"></a>
                <div class="card-content">
                <h2>Teluk Alaska</h2>
                <p><strong>Penulis:</strong> Shopie Aulia</p>
                <p>Buku ini bercerita tentang Sintong Tinggal, mahasiswa yang lulus setelah 6 tahun dengan skripsi
                    tentang Sutan Pane. Ia bekerja paruh waktu di toko buku bajakan dan menyadari dampaknya terhadap
                    penulis. Pertemuannya dengan Jess dan Bunga, mahasiswa fakultas ekonomi, di toko buku bajakan
                    membuka jalan bagi hubungan dan konflik yang menarik.</p>
                <a href="halaman selanjutnya.html">
                    <label for="tombol">Selengkapnya</label></a>
                <div class="rating">
                    ⭐⭐⭐⭐<span>(4.5/5)</span>
                </div>
            </div>
        </div>
    </div>

    <script>
        function searchBooks() {
            const searchTerm = document.getElementById("searchBar").value.toLowerCase();
            const cards = document.querySelectorAll(".card");

            cards.forEach(card => {
                const title = card.querySelector("h2").textContent.toLowerCase();
                const author = card.querySelector("p strong").textContent.toLowerCase();
                const description = card.querySelector("p").textContent.toLowerCase();

                if (title.includes(searchTerm) || author.includes(searchTerm) || description.includes(searchTerm)) {
                    card.style.display = "block";
                } else {
                    card.style.display = "none";
                }
            });
        }
    </script>


    <script>
        // Dark Mode Toggle
        const toggle = document.querySelector('.dark-mode-toggle');
        toggle.addEventListener('click', () => {
            document.body.classList.toggle('dark-mode');
            toggle.innerHTML = document.body.classList.contains('dark-mode') ? '<i class="fas fa-sun"></i>' : '<i class="fas fa-moon"></i>';
        });
    </script>
</body>
    <footer>
        <p>&copy; 2024 Review Buku Modern. Dibuat dengan semangat membaca.</p>
    </footer>
</body>

</html>


</html>
