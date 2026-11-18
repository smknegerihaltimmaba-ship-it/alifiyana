<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PT ANTAM Tbk - UBPN Maluku Utara | Buli, Halmahera Timur</title>
    
    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Konfigurasi Warna Korporat ANTAM -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        antam: {
                            navy: '#0B1F3A',      // Biru Tua Korporat
                            blue: '#163A6C',      // Biru Sekunder
                            gold: '#D4AF37',      // Emas Korporat
                            goldLight: '#F3D060', // Emas Terang (Hover/Highlight)
                            dark: '#1E293B',      // Abu-abu Gelap
                            light: '#F8FAFC',     // Putih Keabu-abuan
                        }
                    }
                }
            }
        }
    </script>
</head>
<body class="font-sans text-slate-800 bg-antam-light antialiased selection:bg-antam-gold selection:text-antam-navy">

    <!-- 1. NAVBAR RESPONSIF -->
    <header id="navbar" class="fixed top-0 left-0 right-0 z-50 bg-antam-navy/95 backdrop-blur-md text-white shadow-lg transition-all duration-300 border-b border-white/10">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logo & Judul -->
                <a href="#beranda" class="flex items-center space-x-3 group">
                    <div class="w-11 h-11 rounded-xl bg-gradient-to-br from-antam-gold to-yellow-600 flex items-center justify-center text-antam-navy font-extrabold text-xl shadow-md group-hover:scale-105 transition-transform">
                        <i class="fa-solid fa-gem"></i>
                    </div>
                    <div>
                        <div class="flex items-center space-x-2">
                            <span class="font-extrabold text-xl tracking-wider text-white">ANTAM</span>
                            <span class="text-[10px] font-bold uppercase px-2 py-0.5 rounded-full bg-antam-gold/20 text-antam-gold border border-antam-gold/40">MIND ID</span>
                        </div>
                        <p class="text-xs text-slate-300 font-medium tracking-wide">UBPN Maluku Utara • Buli</p>
                    </div>
                </a>

                <!-- Desktop Navigation -->
                <nav class="hidden lg:flex items-center space-x-7 text-sm font-medium">
                    <a href="#beranda" class="text-slate-200 hover:text-antam-gold transition-colors py-2">Beranda</a>
                    <a href="#tentang" class="text-slate-200 hover:text-antam-gold transition-colors py-2">Tentang Kami</a>
                    <a href="#operasi" class="text-slate-200 hover:text-antam-gold transition-colors py-2">Operasi & Komoditas</a>
                    <a href="#hilirisasi" class="text-slate-200 hover:text-antam-gold transition-colors py-2">Hilirisasi P3FH</a>
                    <a href="#lingkungan-csr" class="text-slate-200 hover:text-antam-gold transition-colors py-2">Lingkungan & CSR</a>
                    <a href="#lokasi" class="px-4 py-2.5 rounded-xl bg-antam-gold text-antam-navy font-semibold hover:bg-antam-goldLight transition-all shadow-md">
                        Lokasi & Kontak
                    </a>
                </nav>

                <!-- Mobile Menu Button -->
                <button id="mobile-menu-btn" aria-label="Buka Menu" class="lg:hidden p-2.5 rounded-xl text-slate-200 hover:text-white hover:bg-white/10 focus:outline-none transition-colors">
                    <i class="fa-solid fa-bars text-xl" id="menu-icon"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Navigation Drawer -->
        <div id="mobile-menu" class="hidden lg:hidden bg-antam-navy border-t border-white/10 px-4 pt-3 pb-6 space-y-2 shadow-2xl">
            <a href="#beranda" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-200 hover:bg-white/10 hover:text-antam-gold transition-colors">Beranda</a>
            <a href="#tentang" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-200 hover:bg-white/10 hover:text-antam-gold transition-colors">Tentang Kami</a>
            <a href="#operasi" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-200 hover:bg-white/10 hover:text-antam-gold transition-colors">Operasi & Komoditas</a>
            <a href="#hilirisasi" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-200 hover:bg-white/10 hover:text-antam-gold transition-colors">Hilirisasi P3FH</a>
            <a href="#lingkungan-csr" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-200 hover:bg-white/10 hover:text-antam-gold transition-colors">Lingkungan & CSR</a>
            <a href="#lokasi" class="mobile-link block px-4 py-3 mt-2 rounded-xl text-base font-semibold bg-antam-gold text-antam-navy text-center shadow-md">Lokasi & Kontak</a>
        </div>
    </header>

    <!-- 2. HERO SECTION -->
    <section id="beranda" class="relative pt-28 pb-20 lg:pt-40 lg:pb-32 bg-antam-navy text-white overflow-hidden">
        <!-- Latar Belakang Dekoratif & Pola Tambang -->
        <div class="absolute inset-0 z-0 opacity-20">
            <img src="https://images.unsplash.com/photo-1578319439584-104c94d37305?auto=format&fit=crop&w=1920&q=80" 
                 onerror="this.onerror=null; this.src='https://placehold.co/1920x1080/0B1F3A/163A6C?text=ANTAM+UBPN+Maluku+Utara';" 
                 alt="Operasional Pertambangan Nikel" 
                 class="w-full h-full object-cover">
        </div>
        <div class="absolute inset-0 z-0 bg-gradient-to-r from-antam-navy via-antam-navy/95 to-antam-blue/80"></div>
        
        <!-- Aksen Cahaya Emas -->
        <div class="absolute -top-24 -right-24 w-96 h-96 bg-antam-gold/15 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute bottom-0 left-10 w-72 h-72 bg-blue-500/10 rounded-full blur-3xl pointer-events-none"></div>

        <div class="relative z-10 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <div class="lg:col-span-8 space-y-6">
                    <div class="inline-flex items-center space-x-2 px-4 py-2 rounded-full bg-white/10 border border-white/15 backdrop-blur-sm">
                        <span class="w-2.5 h-2.5 rounded-full bg-antam-gold animate-pulse"></span>
                        <span class="text-xs sm:text-sm font-medium text-antam-goldLight tracking-wide">Anggota MIND ID • BUMN Industri Pertambangan</span>
                    </div>
                    
                    <h1 class="text-3xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight leading-tight">
                        Mengoptimalkan Potensi Nikel <span class="text-transparent bg-clip-text bg-gradient-to-r from-antam-gold to-yellow-300">Halmahera Timur</span> untuk Masa Depan Bangsa
                    </h1>
                    
                    <p class="text-base sm:text-lg text-slate-300 max-w-2xl leading-relaxed">
                        <strong>Unit Bisnis Pertambangan Nikel (UBPN) Maluku Utara</strong> di Buli, Kecamatan Maba merupakan tulang punggung strategis PT Aneka Tambang Tbk dalam penyediaan bijih nikel berkualitas tinggi dan hilirisasi mineral berkelanjutan di kawasan Timur Indonesia.
                    </p>
                    
                    <div class="flex flex-col sm:flex-row gap-4 pt-2">
                        <a href="#operasi" class="inline-flex items-center justify-center px-7 py-4 rounded-xl bg-antam-gold text-antam-navy font-bold text-base hover:bg-antam-goldLight transition-all shadow-lg shadow-antam-gold/20">
                            <span>Jelajahi Operasi Kami</span>
                            <i class="fa-solid fa-arrow-right ml-2.5"></i>
                        </a>
                        <a href="#hilirisasi" class="inline-flex items-center justify-center px-7 py-4 rounded-xl bg-white/10 text-white font-semibold text-base hover:bg-white/20 border border-white/20 transition-all backdrop-blur-sm">
                            <i class="fa-solid fa-industry mr-2.5 text-antam-gold"></i>
                            <span>Proyek Hilirisasi P3FH</span>
                        </a>
                    </div>
                </div>

                <!-- Kartu Ringkasan Statistik Cepat -->
                <div class="lg:col-span-4">
                    <div class="bg-white/10 backdrop-blur-md border border-white/15 rounded-2xl p-6 sm:p-8 shadow-2xl space-y-6">
                        <div class="border-b border-white/10 pb-4">
                            <p class="text-xs uppercase tracking-widest text-antam-gold font-semibold">Profil Singkat Unit</p>
                            <h2 class="text-xl font-bold text-white mt-1">UBPN Maluku Utara</h2>
                        </div>
                        
                        <div class="grid grid-cols-2 gap-4">
                            <div class="bg-antam-navy/60 p-4 rounded-xl border border-white/5">
                                <p class="text-2xl sm:text-3xl font-extrabold text-antam-gold">13.500</p>
                                <p class="text-xs text-slate-300 mt-1">Kapasitas TNi/Tahun (Proyek P3FH)</p>
                            </div>
                            <div class="bg-antam-navy/60 p-4 rounded-xl border border-white/5">
                                <p class="text-2xl sm:text-3xl font-extrabold text-white">4 Blok</p>
                                <p class="text-xs text-slate-300 mt-1">Area Tambang Utama Halmahera Timur</p>
                            </div>
                        </div>

                        <div class="space-y-3 text-sm text-slate-200">
                            <div class="flex items-start space-x-3">
                                <i class="fa-solid fa-location-dot text-antam-gold mt-1"></i>
                                <span>Kecamatan Maba (Buli), Kab. Halmahera Timur, Maluku Utara</span>
                            </div>
                            <div class="flex items-start space-x-3">
                                <i class="fa-solid fa-layer-group text-antam-gold mt-1"></i>
                                <span>Komoditas Utama: Bijih Nikel Saprolite & Limonite</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 3. TENTANG KAMI & SEJARAH SINGKAT -->
    <section id="tentang" class="py-20 lg:py-28 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <!-- Visual & Timeline Card -->
                <div class="lg:col-span-6 space-y-6">
                    <div class="relative rounded-2xl overflow-hidden shadow-xl border border-slate-200">
                        <img src="https://images.unsplash.com/photo-1518709268805-4e9042af9f23?auto=format&fit=crop&w=1200&q=80" 
                             onerror="this.onerror=null; this.src='https://placehold.co/800x500/0B1F3A/D4AF37?text=Sejarah+ANTAM+Buli';" 
                             alt="Kawasan Industri dan Pertambangan Buli" 
                             class="w-full h-72 sm:h-80 object-cover">
                        <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-antam-navy via-antam-navy/80 to-transparent p-6 text-white">
                            <p class="text-xs font-semibold uppercase tracking-wider text-antam-gold">Transformasi Berkelanjutan</p>
                            <p class="text-base sm:text-lg font-bold mt-1">Estafet Produksi dari Pulau Gebe ke Daratan Halmahera Timur</p>
                        </div>
                    </div>

                    <!-- Tonggak Sejarah (Timeline) -->
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-4">
                        <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200">
                            <span class="text-xs font-bold text-antam-blue bg-blue-100 px-2.5 py-1 rounded-lg">Era 1970-an</span>
                            <h4 class="font-bold text-slate-900 mt-2 text-sm">Eksplorasi Awal</h4>
                            <p class="text-xs text-slate-600 mt-1">Pemetaan geologi dan potensi cadangan nikel di kawasan Buli dan Pulau Gee.</p>
                        </div>
                        <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200">
                            <span class="text-xs font-bold text-amber-800 bg-amber-100 px-2.5 py-1 rounded-lg">Tahun 2004</span>
                            <h4 class="font-bold text-slate-900 mt-2 text-sm">Transisi Pulau Gebe</h4>
                            <p class="text-xs text-slate-600 mt-1">Buli resmi menjadi pusat produksi utama menggantikan tambang Pulau Gebe yang purna operasi.</p>
                        </div>
                        <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200">
                            <span class="text-xs font-bold text-emerald-800 bg-emerald-100 px-2.5 py-1 rounded-lg">Era MIND ID</span>
                            <h4 class="font-bold text-slate-900 mt-2 text-sm">Hilirisasi Terintegrasi</h4>
                            <p class="text-xs text-slate-600 mt-1">Bagian dari Holding BUMN Pertambangan dengan pengembangan Pabrik Feronikel Haltim.</p>
                        </div>
                    </div>
                </div>

                <!-- Deskripsi Tentang Kami -->
                <div class="lg:col-span-6 space-y-6">
                    <div class="inline-flex items-center space-x-2 text-antam-blue font-bold text-sm uppercase tracking-wider">
                        <span class="w-8 h-0.5 bg-antam-gold"></span>
                        <span>Tentang Kami & Sejarah</span>
                    </div>
                    
                    <h2 class="text-3xl sm:text-4xl font-extrabold text-antam-navy leading-tight">
                        Pilar Utama Produksi Bijih Nikel ANTAM di Kawasan Timur Indonesia
                    </h2>
                    
                    <p class="text-slate-600 leading-relaxed">
                        <strong>PT Aneka Tambang Tbk (ANTAM) – Unit Bisnis Pertambangan Nikel (UBPN) Maluku Utara</strong> merupakan unit operasional strategis yang berpusat di Buli, Kecamatan Maba, Kabupaten Halmahera Timur. Sebagai bagian dari <strong>MIND ID (Mining Industry Indonesia)</strong>, UBPN Maluku Utara memegang mandat mengelola sumber daya mineral nikel negara secara profesional, efisien, dan bernilai tambah tinggi.
                    </p>
                    
                    <p class="text-slate-600 leading-relaxed">
                        Keberadaan UBPN Maluku Utara di Buli merupakan kelanjutan historis dari kesuksesan operasi pertambangan nikel ANTAM di Pulau Gebe (1979–2004). Sejak berakhirnya masa tambang di Pulau Gebe pada tahun 2004, wilayah Buli dan sekitarnya berkembang pesat menjadi pusat produksi bijih nikel andalan yang memasok kebutuhan pabrik feronikel internal ANTAM maupun pasar domestik.
                    </p>

                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 pt-2">
                        <div class="flex items-start space-x-3 p-4 rounded-2xl bg-antam-light border border-slate-200/80">
                            <div class="w-10 h-10 rounded-xl bg-antam-navy text-antam-gold flex items-center justify-center shrink-0">
                                <i class="fa-solid fa-shield-halved"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-antam-navy text-sm">Tata Kelola Terbaik</h3>
                                <p class="text-xs text-slate-600 mt-1">Menerapkan standar keselamatan kerja (K3) dan kepatuhan regulasi pertambangan nasional.</p>
                            </div>
                        </div>
                        <div class="flex items-start space-x-3 p-4 rounded-2xl bg-antam-light border border-slate-200/80">
                            <div class="w-10 h-10 rounded-xl bg-antam-navy text-antam-gold flex items-center justify-center shrink-0">
                                <i class="fa-solid fa-handshake-angle"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-antam-navy text-sm">Sinergi BUMN (MIND ID)</h3>
                                <p class="text-xs text-slate-600 mt-1">Mendukung ekosistem rantai pasok baterai kendaraan listrik dan industri baja nasional.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 4. OPERASI & KOMODITAS -->
    <section id="operasi" class="py-20 lg:py-28 bg-slate-100 border-y border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16 space-y-4">
                <div class="inline-flex items-center space-x-2 text-antam-blue font-bold text-sm uppercase tracking-wider">
                    <span class="w-8 h-0.5 bg-antam-gold"></span>
                    <span>Operasi & Komoditas</span>
                    <span class="w-8 h-0.5 bg-antam-gold"></span>
                </div>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-antam-navy">
                    Rantai Operasi Pertambangan Terintegrasi
                </h2>
                <p class="text-slate-600">
                    Mengelola cadangan bijih nikel unggulan di Halmahera Timur dengan metode penambangan modern dan fasilitas logistik maritim yang andal.
                </p>
            </div>

            <!-- Grid Kartu Komoditas & Aktivitas Utama -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-14">
                <!-- Kartu 1: Saprolite -->
                <div class="bg-white rounded-2xl p-6 shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-200/80 group">
                    <div class="w-12 h-12 rounded-xl bg-amber-50 text-amber-600 flex items-center justify-center text-xl mb-5 group-hover:bg-antam-navy group-hover:text-antam-gold transition-colors">
                        <i class="fa-solid fa-fire-flame-curved"></i>
                    </div>
                    <span class="text-xs font-bold uppercase tracking-wider text-amber-700 bg-amber-100/80 px-2.5 py-1 rounded-md">Kadar Tinggi</span>
                    <h3 class="text-xl font-bold text-antam-navy mt-3">Bijih Nikel Saprolite</h3>
                    <p class="text-sm text-slate-600 mt-2 leading-relaxed">
                        Bijih nikel kadar tinggi yang menjadi bahan baku utama proses pirometalurgi untuk menghasilkan produk feronikel berkualitas ekspor.
                    </p>
                </div>

                <!-- Kartu 2: Limonite -->
                <div class="bg-white rounded-2xl p-6 shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-200/80 group">
                    <div class="w-12 h-12 rounded-xl bg-blue-50 text-antam-blue flex items-center justify-center text-xl mb-5 group-hover:bg-antam-navy group-hover:text-antam-gold transition-colors">
                        <i class="fa-solid fa-battery-full"></i>
                    </div>
                    <span class="text-xs font-bold uppercase tracking-wider text-blue-700 bg-blue-100/80 px-2.5 py-1 rounded-md">Kadar Rendah</span>
                    <h3 class="text-xl font-bold text-antam-navy mt-3">Bijih Nikel Limonite</h3>
                    <p class="text-sm text-slate-600 mt-2 leading-relaxed">
                        Bijih nikel laterit lapisan atas yang potensial untuk pengolahan hidrometalurgi (HPAL) sebagai bahan baku prekursor baterai EV.
                    </p>
                </div>

                <!-- Kartu 3: Open-Pit Mining -->
                <div class="bg-white rounded-2xl p-6 shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-200/80 group">
                    <div class="w-12 h-12 rounded-xl bg-slate-100 text-slate-700 flex items-center justify-center text-xl mb-5 group-hover:bg-antam-navy group-hover:text-antam-gold transition-colors">
                        <i class="fa-solid fa-truck-monster"></i>
                    </div>
                    <span class="text-xs font-bold uppercase tracking-wider text-slate-700 bg-slate-200/80 px-2.5 py-1 rounded-md">Metode Tambang</span>
                    <h3 class="text-xl font-bold text-antam-navy mt-3">Open-Pit Mining</h3>
                    <p class="text-sm text-slate-600 mt-2 leading-relaxed">
                        Sistem penambangan terbuka berjenjang (*benching*) yang didukung pemetaan geologi presisi, *grade control* ketat, serta armada alat berat modern.
                    </p>
                </div>

                <!-- Kartu 4: Fasilitas Jetty -->
                <div class="bg-white rounded-2xl p-6 shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-200/80 group">
                    <div class="w-12 h-12 rounded-xl bg-teal-50 text-teal-700 flex items-center justify-center text-xl mb-5 group-hover:bg-antam-navy group-hover:text-antam-gold transition-colors">
                        <i class="fa-solid fa-ship"></i>
                    </div>
                    <span class="text-xs font-bold uppercase tracking-wider text-teal-700 bg-teal-100/80 px-2.5 py-1 rounded-md">Logistik Maritim</span>
                    <h3 class="text-xl font-bold text-antam-navy mt-3">Fasilitas Jetty Khusus</h3>
                    <p class="text-sm text-slate-600 mt-2 leading-relaxed">
                        Dermaga pemuatan khusus (*ore loading jetty*) di Teluk Buli untuk efisiensi proses *barging* dan *transshipment* menuju kapal induk (*mother vessel*).
                    </p>
                </div>
            </div>

            <!-- Panel Interaktif Wilayah Konsesi / Blok Tambang -->
            <div class="bg-white rounded-3xl p-6 sm:p-10 shadow-md border border-slate-200">
                <div class="flex flex-col lg:flex-row lg:items-center justify-between gap-6 border-b border-slate-100 pb-6 mb-6">
                    <div>
                        <span class="text-xs font-bold uppercase tracking-widest text-antam-gold">Wilayah Izin Usaha Pertambangan (IUP)</span>
                        <h3 class="text-2xl font-bold text-antam-navy mt-1">Blok Operasi Utama Halmahera Timur</h3>
                    </div>
                    <!-- Tab Buttons -->
                    <div class="flex flex-wrap gap-2" id="blok-tabs">
                        <button data-blok="tanjung-buli" class="blok-btn active px-4 py-2.5 rounded-xl text-sm font-semibold bg-antam-navy text-white transition-all cursor-pointer">
                            Blok Tanjung Buli
                        </button>
                        <button data-blok="mornopo" class="blok-btn px-4 py-2.5 rounded-xl text-sm font-semibold bg-slate-100 text-slate-700 hover:bg-slate-200 transition-all cursor-pointer">
                            Blok Mornopo
                        </button>
                        <button data-blok="sangaji" class="blok-btn px-4 py-2.5 rounded-xl text-sm font-semibold bg-slate-100 text-slate-700 hover:bg-slate-200 transition-all cursor-pointer">
                            Blok Sangaji
                        </button>
                        <button data-blok="pakal" class="blok-btn px-4 py-2.5 rounded-xl text-sm font-semibold bg-slate-100 text-slate-700 hover:bg-slate-200 transition-all cursor-pointer">
                            Pulau Pakal
                        </button>
                    </div>
                </div>

                <!-- Konten Dinamis Blok Tambang -->
                <div id="blok-content" class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                    <div class="lg:col-span-7 space-y-4">
                        <div class="inline-flex items-center space-x-2 px-3 py-1 rounded-full bg-antam-gold/15 text-antam-navy text-xs font-bold">
                            <i class="fa-solid fa-map-pin text-antam-gold"></i>
                            <span id="blok-tag">Zona Inti & Pusat Administrasi</span>
                        </div>
                        <h4 id="blok-title" class="text-2xl font-bold text-antam-navy">Blok Tanjung Buli</h4>
                        <p id="blok-desc" class="text-slate-600 leading-relaxed">
                            Merupakan kawasan operasional utama sekaligus pusat perkantoran, laboratorium preparasi sampel, workshop alat berat, serta fasilitas pelabuhan khusus (jetty) UBPN Maluku Utara. Memiliki akses langsung ke pesisir Teluk Buli untuk kelancaran distribusi komoditas.
                        </p>
                        <div class="grid grid-cols-2 sm:grid-cols-3 gap-4 pt-2">
                            <div class="p-3.5 rounded-xl bg-slate-50 border border-slate-200">
                                <p class="text-xs text-slate-500">Fokus Aktivitas</p>
                                <p id="blok-fokus" class="font-bold text-antam-navy text-sm mt-0.5">Penambangan & Jetty</p>
                            </div>
                            <div class="p-3.5 rounded-xl bg-slate-50 border border-slate-200">
                                <p class="text-xs text-slate-500">Tipe Endapan</p>
                                <p id="blok-endapan" class="font-bold text-antam-navy text-sm mt-0.5">Saprolite & Limonite</p>
                            </div>
                            <div class="p-3.5 rounded-xl bg-slate-50 border border-slate-200 col-span-2 sm:col-span-1">
                                <p class="text-xs text-slate-500">Infrastruktur</p>
                                <p id="blok-infra" class="font-bold text-antam-navy text-sm mt-0.5">Kantor Pusat & Lab</p>
                            </div>
                        </div>
                    </div>
                    <div class="lg:col-span-5">
                        <div class="bg-gradient-to-br from-antam-navy to-antam-blue rounded-2xl p-6 text-white space-y-4 shadow-lg">
                            <div class="flex items-center justify-between">
                                <span class="text-xs uppercase tracking-wider text-antam-gold font-semibold">Standar Operasional</span>
                                <i class="fa-solid fa-circle-check text-antam-gold text-lg"></i>
                            </div>
                            <h5 class="text-lg font-bold">Pengendalian Kualitas & Lingkungan</h5>
                            <ul class="space-y-2.5 text-sm text-slate-200">
                                <li class="flex items-start space-x-2.5">
                                    <i class="fa-solid fa-check text-antam-gold mt-1"></i>
                                    <span>Analisis kadar bijih akurat di laboratorium terakreditasi.</span>
                                </li>
                                <li class="flex items-start space-x-2.5">
                                    <i class="fa-solid fa-check text-antam-gold mt-1"></i>
                                    <span>Pengelolaan jalan angkut (*hauling road*) berstandar K3.</span>
                                </li>
                                <li class="flex items-start space-x-2.5">
                                    <i class="fa-solid fa-check text-antam-gold mt-1"></i>
                                    <span>Sistem *settling pond* berlapis sebelum air dilepas ke perairan.</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 5. PROYEK HILIRISASI STRATEGIS (P3FH) -->
    <section id="hilirisasi" class="py-20 lg:py-28 bg-antam-navy text-white relative overflow-hidden">
        <!-- Elemen Dekoratif -->
        <div class="absolute top-0 right-0 w-1/2 h-full bg-gradient-to-l from-antam-blue/40 to-transparent pointer-events-none"></div>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <div class="lg:col-span-7 space-y-6">
                    <div class="inline-flex items-center space-x-2 px-3.5 py-1.5 rounded-full bg-antam-gold/20 border border-antam-gold/40 text-antam-gold text-xs font-bold uppercase tracking-wider">
                        <i class="fa-solid fa-bolt"></i>
                        <span>Proyek Strategis Nasional</span>
                    </div>
                    
                    <h2 class="text-3xl sm:text-4xl lg:text-5xl font-extrabold leading-tight">
                        Pabrik Feronikel Haltim <span class="text-antam-gold">(P3FH)</span>
                    </h2>
                    
                    <p class="text-slate-300 text-base sm:text-lg leading-relaxed">
                        Wujud nyata komitmen ANTAM dalam mendukung program hilirisasi mineral Pemerintah Republik Indonesia. P3FH dirancang untuk mengolah bijih nikel saprolite dari tambang Buli menjadi logam feronikel bernilai tambah tinggi langsung di Halmahera Timur.
                    </p>

                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-5 pt-2">
                        <div class="p-5 rounded-2xl bg-white/5 border border-white/10 backdrop-blur-sm">
                            <div class="flex items-center space-x-3 text-antam-gold mb-2">
                                <i class="fa-solid fa-gauge-high text-xl"></i>
                                <span class="text-xs font-bold uppercase tracking-wider">Kapasitas Produksi</span>
                            </div>
                            <p class="text-3xl font-extrabold text-white">13.500 <span class="text-base font-medium text-antam-gold">TNi / Tahun</span></p>
                            <p class="text-xs text-slate-300 mt-1">Ton Nikel dalam Feronikel untuk pasar industri baja nirkarat global.</p>
                        </div>

                        <div class="p-5 rounded-2xl bg-white/5 border border-white/10 backdrop-blur-sm">
                            <div class="flex items-center space-x-3 text-antam-gold mb-2">
                                <i class="fa-solid fa-industry text-xl"></i>
                                <span class="text-xs font-bold uppercase tracking-wider">Integrasi Hulu-Hilir</span>
                            </div>
                            <p class="text-xl font-bold text-white mt-1">Efisiensi Rantai Pasok</p>
                            <p class="text-xs text-slate-300 mt-1">Memangkas biaya logistik bijih mentah sekaligus menciptakan pusat pertumbuhan ekonomi baru di Maluku Utara.</p>
                        </div>
                    </div>
                </div>

                <!-- Visual & Highlight Teknis P3FH -->
                <div class="lg:col-span-5">
                    <div class="bg-white text-slate-800 rounded-3xl p-6 sm:p-8 shadow-2xl space-y-6">
                        <div class="flex items-center justify-between border-b border-slate-100 pb-4">
                            <div>
                                <p class="text-xs font-bold text-antam-blue uppercase tracking-wider">Nilai Tambah Mineral</p>
                                <h3 class="text-xl font-extrabold text-antam-navy mt-0.5">Keunggulan Strategis P3FH</h3>
                            </div>
                            <div class="w-12 h-12 rounded-2xl bg-antam-navy text-antam-gold flex items-center justify-center text-xl">
                                <i class="fa-solid fa-fire-burner"></i>
                            </div>
                        </div>

                        <div class="space-y-4">
                            <div class="flex items-start space-x-4">
                                <div class="w-8 h-8 rounded-lg bg-amber-100 text-amber-700 font-bold flex items-center justify-center shrink-0 text-sm">1</div>
                                <div>
                                    <h4 class="font-bold text-antam-navy text-sm">Teknologi Rotary Kiln-Electric Furnace (RKEF)</h4>
                                    <p class="text-xs text-slate-600 mt-1">Proses peleburan modern yang terbukti andal dalam memproduksi feronikel berstandar internasional.</p>
                                </div>
                            </div>

                            <div class="flex items-start space-x-4">
                                <div class="w-8 h-8 rounded-lg bg-amber-100 text-amber-700 font-bold flex items-center justify-center shrink-0 text-sm">2</div>
                                <div>
                                    <h4 class="font-bold text-antam-navy text-sm">Penyerapan Tenaga Kerja Lokal</h4>
                                    <p class="text-xs text-slate-600 mt-1">Membuka peluang karier serta transfer teknologi metalurgi bagi putra-putri terbaik Maluku Utara.</p>
                                </div>
                            </div>

                            <div class="flex items-start space-x-4">
                                <div class="w-8 h-8 rounded-lg bg-amber-100 text-amber-700 font-bold flex items-center justify-center shrink-0 text-sm">3</div>
                                <div>
                                    <h4 class="font-bold text-antam-navy text-sm">Kontribusi Devisa & Pendapatan Daerah</h4>
                                    <p class="text-xs text-slate-600 mt-1">Meningkatkan nilai ekspor non-migas nasional dan mendorong efek berganda (*multiplier effect*) ekonomi daerah.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 6. KOMITMEN LINGKUNGAN & CSR -->
    <section id="lingkungan-csr" class="py-20 lg:py-28 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16 space-y-4">
                <div class="inline-flex items-center space-x-2 text-emerald-700 font-bold text-sm uppercase tracking-wider">
                    <span class="w-8 h-0.5 bg-emerald-600"></span>
                    <span>Keberlanjutan & Sosial</span>
                    <span class="w-8 h-0.5 bg-emerald-600"></span>
                </div>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-antam-navy">
                    Komitmen Lingkungan & Pemberdayaan Masyarakat
                </h2>
                <p class="text-slate-600">
                    Menjalankan kaidah pertambangan yang baik (<em>Good Mining Practice</em>) serta tumbuh harmonis bersama masyarakat lingkar tambang (Ring 1) di Halmahera Timur.
                </p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-10">
                <!-- Kolom Kiri: Pengelolaan Lingkungan -->
                <div class="bg-emerald-50/60 border border-emerald-200/80 rounded-3xl p-6 sm:p-8 space-y-6">
                    <div class="flex items-center space-x-4">
                        <div class="w-14 h-14 rounded-2xl bg-emerald-700 text-white flex items-center justify-center text-2xl shadow-md">
                            <i class="fa-solid fa-seedling"></i>
                        </div>
                        <div>
                            <span class="text-xs font-bold uppercase tracking-wider text-emerald-700">Good Mining Practice</span>
                            <h3 class="text-2xl font-bold text-antam-navy">Pengelolaan Lingkungan Hidup</h3>
                        </div>
                    </div>

                    <p class="text-sm text-slate-700 leading-relaxed">
                        UBPN Maluku Utara memastikan setiap tahapan operasi pertambangan selaras dengan kelestarian ekosistem darat dan pesisir Teluk Buli melalui program lingkungan terukur:
                    </p>

                    <div class="space-y-4">
                        <div class="bg-white p-4 rounded-2xl border border-emerald-100 shadow-sm flex items-start space-x-4">
                            <div class="w-10 h-10 rounded-xl bg-emerald-100 text-emerald-700 flex items-center justify-center shrink-0 mt-0.5">
                                <i class="fa-solid fa-tree"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-antam-navy text-sm">Reklamasi & Revegetasi Pascatambang</h4>
                                <p class="text-xs text-slate-600 mt-1">Penataan kembali lahan bekas tambang dan penanaman spesies pohon lokal endemik Halmahera serta tanaman penutup tanah (*cover crop*).</p>
                            </div>
                        </div>

                        <div class="bg-white p-4 rounded-2xl border border-emerald-100 shadow-sm flex items-start space-x-4">
                            <div class="w-10 h-10 rounded-xl bg-emerald-100 text-emerald-700 flex items-center justify-center shrink-0 mt-0.5">
                                <i class="fa-solid fa-water"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-antam-navy text-sm">Pengelolaan Air Limpasan (Settling Pond)</h4>
                                <p class="text-xs text-slate-600 mt-1">Pembangunan kolam pengendapan sedimen berlapis dengan kontrol kualitas air harian sesuai baku mutu lingkungan sebelum dialirkan ke perairan.</p>
                            </div>
                        </div>

                        <div class="bg-white p-4 rounded-2xl border border-emerald-100 shadow-sm flex items-start space-x-4">
                            <div class="w-10 h-10 rounded-xl bg-emerald-100 text-emerald-700 flex items-center justify-center shrink-0 mt-0.5">
                                <i class="fa-solid fa-microscope"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-antam-navy text-sm">Pemantauan Ekosistem Udara & Laut</h4>
                                <p class="text-xs text-slate-600 mt-1">Penyiraman jalan tambang rutin untuk menekan debu serta pemantauan berkala kualitas air laut dan terumbu karang di Teluk Buli.</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Kolom Kanan: Program CSR / PPM -->
                <div class="bg-amber-50/50 border border-amber-200/80 rounded-3xl p-6 sm:p-8 space-y-6">
                    <div class="flex items-center space-x-4">
                        <div class="w-14 h-14 rounded-2xl bg-antam-navy text-antam-gold flex items-center justify-center text-2xl shadow-md">
                            <i class="fa-solid fa-people-carry-box"></i>
                        </div>
                        <div>
                            <span class="text-xs font-bold uppercase tracking-wider text-amber-800">Tanggung Jawab Sosial (PPM / CSR)</span>
                            <h3 class="text-2xl font-bold text-antam-navy">Pemberdayaan Masyarakat Ring 1</h3>
                        </div>
                    </div>

                    <p class="text-sm text-slate-700 leading-relaxed">
                        Melalui program Pengembangan dan Pemberdayaan Masyarakat (PPM), ANTAM berkomitmen meningkatkan kemandirian dan kesejahteraan masyarakat di sekitar wilayah operasi Buli:
                    </p>

                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div class="bg-white p-4 rounded-2xl border border-amber-100 shadow-sm">
                            <div class="w-10 h-10 rounded-xl bg-blue-50 text-antam-blue flex items-center justify-center mb-3">
                                <i class="fa-solid fa-graduation-cap"></i>
                            </div>
                            <h4 class="font-bold text-antam-navy text-sm">Pendidikan & Beasiswa</h4>
                            <p class="text-xs text-slate-600 mt-1">Program beasiswa pelajar/mahasiswa Halmahera Timur, renovasi fasilitas sekolah, dan pelatihan kompetensi guru.</p>
                        </div>

                        <div class="bg-white p-4 rounded-2xl border border-amber-100 shadow-sm">
                            <div class="w-10 h-10 rounded-xl bg-rose-50 text-rose-600 flex items-center justify-center mb-3">
                                <i class="fa-solid fa-heart-pulse"></i>
                            </div>
                            <h4 class="font-bold text-antam-navy text-sm">Kesehatan Masyarakat</h4>
                            <p class="text-xs text-slate-600 mt-1">Layanan pengobatan gratis, dukungan posyandu, pencegahan stunting, serta peningkatan sanitasi air bersih desa.</p>
                        </div>

                        <div class="bg-white p-4 rounded-2xl border border-amber-100 shadow-sm">
                            <div class="w-10 h-10 rounded-xl bg-amber-50 text-amber-700 flex items-center justify-center mb-3">
                                <i class="fa-solid fa-store"></i>
                            </div>
                            <h4 class="font-bold text-antam-navy text-sm">Ekonomi Lokal & UMKM</h4>
                            <p class="text-xs text-slate-600 mt-1">Pembinaan UMKM lokal, pemberdayaan kelompok tani, peternak, serta dukungan sarana tangkap nelayan Teluk Buli.</p>
                        </div>

                        <div class="bg-white p-4 rounded-2xl border border-amber-100 shadow-sm">
                            <div class="w-10 h-10 rounded-xl bg-purple-50 text-purple-700 flex items-center justify-center mb-3">
                                <i class="fa-solid fa-landmark"></i>
                            </div>
                            <h4 class="font-bold text-antam-navy text-sm">Sosial & Pelestarian Budaya</h4>
                            <p class="text-xs text-slate-600 mt-1">Dukungan sarana ibadah, pembangunan infrastruktur desa, serta pelestarian kearifan lokal masyarakat Maba.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 7. INFORMASI LOKASI, AKSESIBILITAS & KONTAK -->
    <section id="lokasi" class="py-20 lg:py-28 bg-slate-100 border-t border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-10">
                <!-- Info Lokasi & Aksesibilitas -->
                <div class="lg:col-span-6 space-y-6">
                    <div class="inline-flex items-center space-x-2 text-antam-blue font-bold text-sm uppercase tracking-wider">
                        <span class="w-8 h-0.5 bg-antam-gold"></span>
                        <span>Lokasi & Aksesibilitas</span>
                    </div>
                    
                    <h2 class="text-3xl sm:text-4xl font-extrabold text-antam-navy">
                        Terhubung Strategis di Jantung Halmahera Timur
                    </h2>
                    
                    <p class="text-slate-600 leading-relaxed">
                        Kantor operasional dan kawasan tambang UBPN Maluku Utara berlokasi di <strong>Buli, Kecamatan Maba, Kabupaten Halmahera Timur, Provinsi Maluku Utara</strong>. Kawasan ini didukung infrastruktur transportasi udara dan laut yang memadai.
                    </p>

                    <div class="space-y-4 pt-2">
                        <div class="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm flex items-start space-x-4">
                            <div class="w-12 h-12 rounded-xl bg-antam-navy text-antam-gold flex items-center justify-center text-xl shrink-0">
                                <i class="fa-solid fa-plane-arrival"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-antam-navy">Akses Jalur Udara — Bandara Buli (PGQ)</h3>
                                <p class="text-sm text-slate-600 mt-1">
                                    Dapat dijangkau melalui penerbangan perintis maupun reguler menuju Bandar Udara Buli (Maba) dari Kota Ternate (Bandara Sultan Babullah) maupun Manado (Bandara Sam Ratulangi).
                                </p>
                            </div>
                        </div>

                        <div class="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm flex items-start space-x-4">
                            <div class="w-12 h-12 rounded-xl bg-antam-navy text-antam-gold flex items-center justify-center text-xl shrink-0">
                                <i class="fa-solid fa-anchor"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-antam-navy">Akses Jalur Laut — Pelabuhan Buli & Jetty Khusus</h3>
                                <p class="text-sm text-slate-600 mt-1">
                                    Didukung Pelabuhan Umum Buli untuk transportasi penumpang dan logistik regional, serta dermaga khusus (jetty) ANTAM di pesisir Teluk Buli untuk pengapalan komoditas mineral.
                                </p>
                            </div>
                        </div>

                        <div class="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm flex items-start space-x-4">
                            <div class="w-12 h-12 rounded-xl bg-antam-navy text-antam-gold flex items-center justify-center text-xl shrink-0">
                                <i class="fa-solid fa-road"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-antam-navy">Akses Jalur Darat Lintas Halmahera</h3>
                                <p class="text-sm text-slate-600 mt-1">
                                    Terhubung melalui jaringan jalan lintas Halmahera dari Pelabuhan Penyeberangan Sofifi (Tidore Kepulauan) menuju Maba / Buli, Halmahera Timur.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Kartu Kontak & Formulir Pesan -->
                <div class="lg:col-span-6">
                    <div class="bg-white rounded-3xl p-6 sm:p-10 shadow-lg border border-slate-200 space-y-6">
                        <div>
                            <span class="text-xs font-bold uppercase tracking-wider text-antam-gold">Hubungi Kami</span>
                            <h3 class="text-2xl font-bold text-antam-navy mt-1">Informasi & Korespondensi Unit</h3>
                            <p class="text-sm text-slate-600 mt-1">Sampaikan pertanyaan terkait informasi perusahaan, kemitraan, atau program CSR UBPN Maluku Utara.</p>
                        </div>

                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 bg-slate-50 p-4 rounded-2xl border border-slate-200/80 text-sm">
                            <div>
                                <p class="text-xs text-slate-500 font-medium">Alamat Operasional</p>
                                <p class="font-semibold text-antam-navy mt-0.5">Jl. Raya Buli, Kec. Maba, Kab. Halmahera Timur, Maluku Utara 97862</p>
                            </div>
                            <div>
                                <p class="text-xs text-slate-500 font-medium">Kantor Pusat Korporat</p>
                                <p class="font-semibold text-antam-navy mt-0.5">Gedung Aneka Tambang, Jl. Letjen TB Simatupang No.1, Jakarta Selatan</p>
                            </div>
                        </div>

                        <form id="contact-form" class="space-y-4">
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                <div>
                                    <label for="nama" class="block text-xs font-semibold text-slate-700 mb-1.5">Nama Lengkap</label>
                                    <input type="text" id="nama" required placeholder="Masukkan nama Anda" class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm focus:outline-none focus:ring-2 focus:ring-antam-gold focus:border-antam-navy transition-all">
                                </div>
                                <div>
                                    <label for="email" class="block text-xs font-semibold text-slate-700 mb-1.5">Alamat Email</label>
                                    <input type="email" id="email" required placeholder="nama@email.com" class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm focus:outline-none focus:ring-2 focus:ring-antam-gold focus:border-antam-navy transition-all">
                                </div>
                            </div>

                            <div>
                                <label for="kategori" class="block text-xs font-semibold text-slate-700 mb-1.5">Keperluan / Topik</label>
                                <select id="kategori" class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm bg-white focus:outline-none focus:ring-2 focus:ring-antam-gold focus:border-antam-navy transition-all">
                                    <option value="Informasi Umum">Informasi Umum Perusahaan</option>
                                    <option value="Program CSR / PPM">Program CSR & Kemitraan Masyarakat</option>
                                    <option value="Karier & Magang">Informasi Karier & Kerja Praktik</option>
                                    <option value="Pengadaan / Vendor">Informasi Kemitraan & Vendor</option>
                                </select>
                            </div>

                            <div>
                                <label for="pesan" class="block text-xs font-semibold text-slate-700 mb-1.5">Pesan Anda</label>
                                <textarea id="pesan" rows="3" required placeholder="Tuliskan pesan atau pertanyaan Anda..." class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm focus:outline-none focus:ring-2 focus:ring-antam-gold focus:border-antam-navy transition-all"></textarea>
                            </div>

                            <button type="submit" class="w-full py-3.5 px-6 rounded-xl bg-antam-navy text-white font-bold text-sm hover:bg-antam-blue transition-all shadow-md flex items-center justify-center space-x-2 cursor-pointer">
                                <span>Kirim Pesan</span>
                                <i class="fa-solid fa-paper-plane text-antam-gold"></i>
                            </button>
                        </form>

                        <!-- Kotak Notifikasi Pengganti alert() -->
                        <div id="form-feedback" class="hidden p-4 rounded-xl bg-emerald-50 border border-emerald-200 text-emerald-800 text-sm flex items-start space-x-3">
                            <i class="fa-solid fa-circle-check text-emerald-600 text-lg mt-0.5"></i>
                            <div>
                                <p class="font-bold">Pesan Berhasil Dicatat</p>
                                <p class="text-xs mt-0.5" id="feedback-text">Terima kasih telah menghubungi PT ANTAM Tbk - UBPN Maluku Utara.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER PROFESIONAL -->
    <footer class="bg-antam-navy text-slate-300 pt-16 pb-10 border-t border-white/10">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-12 gap-10 pb-12 border-b border-white/10">
                <!-- Brand & Deskripsi -->
                <div class="lg:col-span-5 space-y-4">
                    <div class="flex items-center space-x-3">
                        <div class="w-10 h-10 rounded-xl bg-antam-gold flex items-center justify-center text-antam-navy font-extrabold text-lg">
                            <i class="fa-solid fa-gem"></i>
                        </div>
                        <div>
                            <span class="font-extrabold text-xl tracking-wider text-white">PT ANTAM Tbk</span>
                            <p class="text-xs text-antam-gold font-medium">UBPN Maluku Utara • Anggota MIND ID</p>
                        </div>
                    </div>
                    <p class="text-sm text-slate-400 leading-relaxed max-w-md">
                        Unit Bisnis Pertambangan Nikel Maluku Utara berkomitmen mengelola sumber daya mineral secara berkelanjutan, berstandar keselamatan tinggi, serta memberi nilai tambah bagi masyarakat Halmahera Timur dan Indonesia.
                    </p>
                    <div class="flex items-center space-x-3 pt-2">
                        <a href="https://www.antam.com" target="_blank" rel="noopener noreferrer" aria-label="Situs Resmi ANTAM" class="w-9 h-9 rounded-lg bg-white/10 hover:bg-antam-gold hover:text-antam-navy flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-globe"></i>
                        </a>
                        <a href="#lokasi" aria-label="Lokasi Buli" class="w-9 h-9 rounded-lg bg-white/10 hover:bg-antam-gold hover:text-antam-navy flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-location-dot"></i>
                        </a>
                        <a href="#lingkungan-csr" aria-label="Keberlanjutan" class="w-9 h-9 rounded-lg bg-white/10 hover:bg-antam-gold hover:text-antam-navy flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-leaf"></i>
                        </a>
                    </div>
                </div>

                <!-- Navigasi Cepat -->
                <div class="lg:col-span-3 space-y-3">
                    <h4 class="text-sm font-bold uppercase tracking-wider text-white">Navigasi Profil</h4>
                    <ul class="space-y-2.5 text-sm text-slate-400">
                        <li><a href="#beranda" class="hover:text-antam-gold transition-colors">Beranda</a></li>
                        <li><a href="#tentang" class="hover:text-antam-gold transition-colors">Tentang & Sejarah</a></li>
                        <li><a href="#operasi" class="hover:text-antam-gold transition-colors">Operasi & Komoditas</a></li>
                        <li><a href="#hilirisasi" class="hover:text-antam-gold transition-colors">Proyek Hilirisasi P3FH</a></li>
                        <li><a href="#lingkungan-csr" class="hover:text-antam-gold transition-colors">Lingkungan & CSR</a></li>
                    </ul>
                </div>

                <!-- Wilayah Operasi -->
                <div class="lg:col-span-4 space-y-3">
                    <h4 class="text-sm font-bold uppercase tracking-wider text-white">Wilayah Operasi Utama</h4>
                    <ul class="space-y-2.5 text-sm text-slate-400">
                        <li class="flex items-center space-x-2">
                            <i class="fa-solid fa-angle-right text-antam-gold text-xs"></i>
                            <span>Blok Tanjung Buli (Kec. Maba)</span>
                        </li>
                        <li class="flex items-center space-x-2">
                            <i class="fa-solid fa-angle-right text-antam-gold text-xs"></i>
                            <span>Blok Mornopo (Halmahera Timur)</span>
                        </li>
                        <li class="flex items-center space-x-2">
                            <i class="fa-solid fa-angle-right text-antam-gold text-xs"></i>
                            <span>Blok Sangaji (Halmahera Timur)</span>
                        </li>
                        <li class="flex items-center space-x-2">
                            <i class="fa-solid fa-angle-right text-antam-gold text-xs"></i>
                            <span>Pulau Pakal (Teluk Buli)</span>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="pt-8 flex flex-col sm:flex-row justify-between items-center gap-4 text-xs text-slate-400">
                <p>&copy; 2026 PT Aneka Tambang Tbk – Unit Bisnis Pertambangan Nikel Maluku Utara. Hak Cipta Dilindungi.</p>
                <p class="text-slate-500">Buli, Kabupaten Halmahera Timur • Provinsi Maluku Utara</p>
            </div>
        </div>
    </footer>

    <!-- JAVASCRIPT INTERAKTIF -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // 1. Toggle Mobile Menu
            const mobileMenuBtn = document.getElementById('mobile-menu-btn');
            const mobileMenu = document.getElementById('mobile-menu');
            const menuIcon = document.getElementById('menu-icon');
            const mobileLinks = document.querySelectorAll('.mobile-link');

            mobileMenuBtn.addEventListener('click', () => {
                const isHidden = mobileMenu.classList.toggle('hidden');
                menuIcon.className = isHidden ? 'fa-solid fa-bars text-xl' : 'fa-solid fa-xmark text-xl';
            });

            mobileLinks.forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                    menuIcon.className = 'fa-solid fa-bars text-xl';
                });
            });

            // 2. Data & Interaksi Tab Blok Pertambangan
            const blokData = {
                'tanjung-buli': {
                    tag: 'Zona Inti & Pusat Administrasi',
                    title: 'Blok Tanjung Buli',
                    desc: 'Merupakan kawasan operasional utama sekaligus pusat perkantoran, laboratorium preparasi sampel, workshop alat berat, serta fasilitas pelabuhan khusus (jetty) UBPN Maluku Utara. Memiliki akses langsung ke pesisir Teluk Buli untuk kelancaran distribusi komoditas.',
                    fokus: 'Penambangan & Jetty',
                    endapan: 'Saprolite & Limonite',
                    infra: 'Kantor Pusat & Lab'
                },
                'mornopo': {
                    tag: 'Zona Eksplorasi & Produksi',
                    title: 'Blok Mornopo',
                    desc: 'Salah satu blok konsesi strategis dengan cadangan bijih nikel laterit yang signifikan di daratan Halmahera Timur. Dikelola dengan perencanaan tambang jangka panjang dan infrastruktur jalan angkut (hauling road) terpadu menuju area stockpile.',
                    fokus: 'Open-Pit Mining',
                    endapan: 'Saprolite Kadar Tinggi',
                    infra: 'Hauling Road & Stockpile'
                },
                'sangaji': {
                    tag: 'Zona Cadangan Strategis',
                    title: 'Blok Sangaji',
                    desc: 'Kawasan penambangan potensial di wilayah Maba yang mendukung keberlanjutan pasokan bijih nikel bagi kebutuhan industri domestik maupun pasokan bahan baku Pabrik Feronikel Haltim (P3FH).',
                    fokus: 'Produksi & Konservasi',
                    endapan: 'Saprolite & Limonite',
                    infra: 'Settling Pond & Nursery'
                },
                'pakal': {
                    tag: 'Zona Pulau Kecil Terkelola',
                    title: 'Pulau Pakal',
                    desc: 'Blok operasi kepulauan di kawasan Teluk Buli yang dioperasikan dengan pengawasan lingkungan maritim ketat serta fasilitas pemuatan tongkang langsung untuk menjaga efisiensi rantai pasok.',
                    fokus: 'Tambang & Barging',
                    endapan: 'Nikel Laterit Unggulan',
                    infra: 'Jetty Pemasok Tongkang'
                }
            };

            const blokButtons = document.querySelectorAll('.blok-btn');
            const blokTag = document.getElementById('blok-tag');
            const blokTitle = document.getElementById('blok-title');
            const blokDesc = document.getElementById('blok-desc');
            const blokFokus = document.getElementById('blok-fokus');
            const blokEndapan = document.getElementById('blok-endapan');
            const blokInfra = document.getElementById('blok-infra');

            blokButtons.forEach(btn => {
                btn.addEventListener('click', () => {
                    // Reset style semua tombol
                    blokButtons.forEach(b => {
                        b.classList.remove('bg-antam-navy', 'text-white');
                        b.classList.add('bg-slate-100', 'text-slate-700');
                    });

                    // Aktifkan tombol terpilih
                    btn.classList.remove('bg-slate-100', 'text-slate-700');
                    btn.classList.add('bg-antam-navy', 'text-white');

                    // Update konten
                    const key = btn.getAttribute('data-blok');
                    const data = blokData[key];
                    if (data) {
                        blokTag.textContent = data.tag;
                        blokTitle.textContent = data.title;
                        blokDesc.textContent = data.desc;
                        blokFokus.textContent = data.fokus;
                        blokEndapan.textContent = data.endapan;
                        blokInfra.textContent = data.infra;
                    }
                });
            });

            // 3. Penanganan Form Kontak (Tanpa alert)
            const contactForm = document.getElementById('contact-form');
            const formFeedback = document.getElementById('form-feedback');
            const feedbackText = document.getElementById('feedback-text');

            contactForm.addEventListener('submit', (e) => {
                e.preventDefault();
                const nama = document.getElementById('nama').value.trim();
                const kategori = document.getElementById('kategori').value;

                feedbackText.textContent = `Terima kasih, ${nama}. Pesan Anda terkait "${kategori}" telah tercatat untuk tim Humas & CSR UBPN Maluku Utara.`;
                formFeedback.classList.remove('hidden');
                contactForm.reset();

                setTimeout(() => {
                    formFeedback.classList.add('hidden');
                }, 7000);
            });
        });
    </script>
</body>
</html>
