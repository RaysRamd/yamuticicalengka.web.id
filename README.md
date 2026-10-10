<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yamu'ti Cicalengka - Berbagi Kebaikan</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome untuk Ikon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#800000', // Maroon (Merah Hati)
                        secondary: '#dc2626', // Merah (untuk aksen dan tombol sekunder)
                        dark: '#3f000f', // Maroon sangat gelap hampir hitam
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    animation: {
                        'bounce-slow': 'bounce 2s infinite',
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom scrollbar untuk tampilan yang lebih mulus */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        ::-webkit-scrollbar-thumb {
            background: #800000;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #5e0000;
        }
        /* Efek transisi halus */
        .transition-all-ease {
            transition: all 0.3s ease-in-out;
        }
        
        /* Typing Indicator Animation */
        .typing-dot {
            animation: typing 1.4s infinite ease-in-out both;
        }
        .typing-dot:nth-child(1) { animation-delay: -0.32s; }
        .typing-dot:nth-child(2) { animation-delay: -0.16s; }
        @keyframes typing {
            0%, 80%, 100% { transform: scale(0); }
            40% { transform: scale(1); }
        }
    </style>
</head>
<body class="font-sans text-gray-700 bg-gray-50 overflow-x-hidden">

    <!-- Navbar -->
    <nav class="bg-white shadow-md fixed w-full z-40 top-0 transition-all-ease" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20">
                <div class="flex items-center">
                    <!-- Logo -->
                    <a href="#" class="flex-shrink-0 flex items-center gap-2">
                        <img src="https://cdn.phototourl.com/member/2026-10-03-d82bd2ed-cb64-4aa8-8488-a2c3ed74d69a.png" alt="Logo Yamu'ti Cicalengka" class="h-14 w-auto rounded-full object-cover shadow-sm">
                        <span class="font-bold text-xl text-dark hidden sm:block">Yamu'ti Cicalengka</span>
                    </a>
                </div>
                
                <!-- Desktop Menu -->
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#beranda" class="text-primary font-semibold hover:text-secondary transition-colors">Beranda</a>
                    <a href="#tentang" class="text-gray-600 hover:text-primary transition-colors">Tentang Kami</a>
                    <a href="#program" class="text-gray-600 hover:text-primary transition-colors">Program</a>
                    <a href="#dokumentasi" class="text-gray-600 hover:text-primary transition-colors">Dokumentasi</a>
                    <a href="#kontak" class="text-gray-600 hover:text-primary transition-colors">Kontak</a>
                    <a href="#donasi" class="bg-primary text-white px-6 py-2 rounded-full font-semibold hover:bg-red-800 transition-colors shadow-lg hover:shadow-xl transform hover:-translate-y-0.5">Donasi Sekarang</a>
                </div>

                <!-- Mobile menu button -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-btn" class="text-gray-600 hover:text-primary focus:outline-none">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu (Hidden by default) -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100 absolute w-full shadow-lg z-40">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#beranda" class="block px-3 py-2 rounded-md text-base font-medium text-primary bg-red-50">Beranda</a>
                <a href="#tentang" class="block px-3 py-2 rounded-md text-base font-medium text-gray-600 hover:text-primary hover:bg-gray-50">Tentang Kami</a>
                <a href="#program" class="block px-3 py-2 rounded-md text-base font-medium text-gray-600 hover:text-primary hover:bg-gray-50">Program</a>
                <a href="#dokumentasi" class="block px-3 py-2 rounded-md text-base font-medium text-gray-600 hover:text-primary hover:bg-gray-50">Dokumentasi</a>
                <a href="#kontak" class="block px-3 py-2 rounded-md text-base font-medium text-gray-600 hover:text-primary hover:bg-gray-50">Kontak</a>
                <a href="#donasi" class="block w-full text-center mt-4 bg-primary text-white px-3 py-3 rounded-md font-bold hover:bg-red-800">Donasi Sekarang</a>
            </div>
        </div>
    </nav>

    <!-- Spacer untuk navbar fixed -->
    <div class="h-20"></div>

    <!-- Hero Section -->
    <section id="beranda" class="relative bg-dark overflow-hidden">
        <div class="absolute inset-0 bg-dark">
            <!-- Background Images Slideshow -->
            <img src="https://lh3.googleusercontent.com/d/11074FnQ-zVdln18eN0dbBGMIJdcgODQ1" alt="Kegiatan 1" class="hero-slide absolute inset-0 w-full h-full object-cover opacity-50 transition-opacity duration-[1500ms] ease-in-out">
            <img src="https://lh3.googleusercontent.com/d/1P-ZCbjswds5W0KysQKJsrb_iSgW7-wHO" alt="Kegiatan 2" class="hero-slide absolute inset-0 w-full h-full object-cover opacity-0 transition-opacity duration-[1500ms] ease-in-out">
            <img src="https://lh3.googleusercontent.com/d/1vDE7R4dF0T-ke65-UOkZdxQCceJwJ6Tu" alt="Kegiatan 3" class="hero-slide absolute inset-0 w-full h-full object-cover opacity-0 transition-opacity duration-[1500ms] ease-in-out">
            <img src="https://lh3.googleusercontent.com/d/10wtR6P1th5gGeXpB32eOLRbdG_HaQ8_B" alt="Kegiatan 4" class="hero-slide absolute inset-0 w-full h-full object-cover opacity-0 transition-opacity duration-[1500ms] ease-in-out">
            <img src="https://lh3.googleusercontent.com/d/1tOja0-KTrnHAcbtIeNk_rbWaof4S0pjf" alt="Kegiatan 5" class="hero-slide absolute inset-0 w-full h-full object-cover opacity-0 transition-opacity duration-[1500ms] ease-in-out">
            
            <!-- Overlay -->
            <div class="absolute inset-0 bg-gradient-to-r from-dark via-dark/70 to-transparent z-10"></div>
        </div>
        
        <!-- Slide Indicators -->
        <div class="absolute bottom-8 left-0 right-0 z-30 flex justify-center gap-3">
            <button class="slide-dot w-3 h-3 rounded-full bg-white opacity-100 transition-opacity focus:outline-none shadow-md" onclick="goToSlide(0)" aria-label="Slide 1"></button>
            <button class="slide-dot w-3 h-3 rounded-full bg-white opacity-50 hover:opacity-100 transition-opacity focus:outline-none shadow-md" onclick="goToSlide(1)" aria-label="Slide 2"></button>
            <button class="slide-dot w-3 h-3 rounded-full bg-white opacity-50 hover:opacity-100 transition-opacity focus:outline-none shadow-md" onclick="goToSlide(2)" aria-label="Slide 3"></button>
            <button class="slide-dot w-3 h-3 rounded-full bg-white opacity-50 hover:opacity-100 transition-opacity focus:outline-none shadow-md" onclick="goToSlide(3)" aria-label="Slide 4"></button>
            <button class="slide-dot w-3 h-3 rounded-full bg-white opacity-50 hover:opacity-100 transition-opacity focus:outline-none shadow-md" onclick="goToSlide(4)" aria-label="Slide 5"></button>
        </div>

        <div class="relative z-20 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-24 lg:py-32 flex flex-col justify-center min-h-[80vh]">
            <div class="md:w-2/3 lg:w-1/2">
                <span class="text-secondary font-semibold tracking-wider uppercase text-sm mb-4 block">Bersama Membangun Asa</span>
                <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white leading-tight mb-6">
                    Langkah Kecil Anda,<br>
                    <span class="text-red-400">Harapan Besar</span> Bagi Mereka
                </h1>
                <p class="text-lg text-gray-300 mb-8 max-w-xl leading-relaxed">
                    Kami berdedikasi untuk memberikan pengasuhan, pendidikan, dan kesejahteraan bagi anak-anak yatim dan kaum dhuafa di wilayah Cicalengka. Bergabunglah menjadi jalan kebaikan bagi mereka.
                </p>
                <div class="flex flex-col sm:flex-row gap-4">
                    <a href="#donasi" class="bg-primary hover:bg-[#5e0000] text-white text-center px-8 py-3 rounded-full font-semibold transition-all shadow-lg hover:shadow-xl flex items-center justify-center gap-2 border border-red-900">
                        <i class="fa-solid fa-heart"></i> Bantu Sekarang
                    </a>
                    <a href="#tentang" class="bg-transparent border-2 border-white text-white hover:bg-white hover:text-dark text-center px-8 py-3 rounded-full font-semibold transition-all flex items-center justify-center gap-2">
                        Pelajari Lebih Lanjut
                    </a>
                </div>
            </div>
            
            <!-- Quick Stats -->
            <div class="mt-16 grid grid-cols-2 gap-6 border-t border-gray-700/50 pt-8 max-w-2xl">
                <div>
                    <h3 class="text-3xl font-bold text-white">50</h3>
                    <p class="text-gray-400 text-sm mt-1">Yatim Binaan</p>
                </div>
                <div>
                    <h3 class="text-3xl font-bold text-white">50</h3>
                    <p class="text-gray-400 text-sm mt-1">Dhuafa Terbantu</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Tentang Yayasan Section -->
    <section id="tentang" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col lg:flex-row gap-12 items-center">
                <!-- Gambar -->
                <div class="lg:w-1/2 relative w-full">
                    <div class="relative rounded-2xl overflow-hidden shadow-2xl border-4 border-white">
                        <img src="https://lh3.googleusercontent.com/d/1crcN8AJi62rA3xjd8Re6BEUTdS7K5oLO" alt="Kegiatan Yamu'ti Cicalengka" class="w-full h-auto object-cover hover:scale-105 transition-transform duration-700">
                    </div>
                    <!-- Badge absolute -->
                    <div class="absolute -bottom-6 -right-6 bg-white p-6 rounded-xl shadow-xl flex items-center gap-4 border-l-4 border-primary hidden md:flex z-10">
                        <div class="bg-primary/10 p-3 rounded-full text-primary">
                            <i class="fa-solid fa-medal text-2xl"></i>
                        </div>
                        <div>
                            <p class="font-bold text-dark text-xl">8 Tahun</p>
                            <p class="text-gray-500 text-sm">Berbagi Kebaikan</p>
                        </div>
                    </div>
                </div>
        
                <!-- Konten -->
        <div class="lg:w-1/2 w-full mt-8 lg:mt-0">
            <div class="inline-block px-4 py-1.5 bg-primary/10 text-primary font-semibold rounded-full text-sm mb-4">
                Tentang Kami
            </div>
            <h2 class="text-3xl md:text-4xl font-bold text-dark mb-6">Merangkul Harapan,<br>Menebar Kebahagiaan Bagi Sesama</h2>
            <p class="text-gray-600 mb-6 leading-relaxed">
                Yamu'ti Cicalengka adalah lembaga sosial yang berfokus pada penyantunan dan pemberdayaan anak yatim, piatu, serta kaum dhuafa yang membutuhkan perlindungan dan harapan baru.
            </p>
            <p class="text-gray-600 mb-8 leading-relaxed">
                Kami percaya bahwa setiap anak yatim memiliki potensi besar yang perlu didukung melalui pendidikan agama, pendidikan formal, dan pemenuhan kebutuhan dasar agar mereka kelak tumbuh menjadi generasi yang mandiri dan berakhlak mulia.
            </p>
            
            <ul class="space-y-4 mb-8">
                        <li class="flex items-start gap-3">
                            <div class="mt-1 text-primary"><i class="fa-solid fa-circle-check"></i></div>
                            <span class="text-gray-700 font-medium">Pengelolaan dana zakat, infaq, dan sedekah (ZIS) yang amanah.</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <div class="mt-1 text-primary"><i class="fa-solid fa-circle-check"></i></div>
                            <span class="text-gray-700 font-medium">Pendidikan karakter dan tahfidz quran bagi anak asuh.</span>
                        </li>
                        <li class="flex items-start gap-3">
                    <div class="mt-1 text-primary"><i class="fa-solid fa-circle-check"></i></div>
                    <span class="text-gray-700 font-medium">Bantuan logistik bulanan untuk keluarga dhuafa dan janda.</span>
                </li>
            </ul>
        </div>
    </div>

    <!-- Visi & Misi Block -->
    <div class="mt-16 grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Visi -->
        <div class="bg-red-50 rounded-2xl p-8 border-t-4 border-primary shadow-sm hover:shadow-md transition-shadow flex flex-col justify-center">
            <div class="w-12 h-12 bg-primary rounded-full flex items-center justify-center text-white text-xl mb-6 shadow-md">
                <i class="fa-regular fa-eye"></i>
            </div>
            <h3 class="text-2xl font-bold text-dark mb-4">Visi Kami</h3>
            <p class="text-primary font-bold text-lg italic leading-relaxed">
                “Menjadi lembaga sosial terpercaya yang membina yatim, dhuafa, dan masyarakat luas melalui sinergi saling belajar, berbagi manfaat, dan memberdayakan.”
            </p>
        </div>

        <!-- Misi -->
        <div class="md:col-span-2 bg-white rounded-2xl p-8 border border-gray-100 shadow-lg hover:shadow-xl transition-shadow">
            <div class="flex items-center gap-4 mb-6">
                <div class="w-12 h-12 bg-dark rounded-full flex items-center justify-center text-white text-xl shadow-md flex-shrink-0">
                    <i class="fa-solid fa-bullseye"></i>
                </div>
                <h3 class="text-2xl font-bold text-dark">Misi Kami</h3>
            </div>
            <p class="text-gray-600 mb-6 font-medium">Visi tersebut direalisasikan melalui misi Yamu'ti Cicalengka sebagai berikut:</p>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                <div class="flex items-start gap-4 p-4 rounded-xl border border-gray-50 hover:bg-red-50 transition-colors group cursor-default">
                    <span class="text-secondary/30 group-hover:text-primary font-black text-2xl transition-colors mt-1">01</span>
                    <div>
                        <h4 class="text-primary font-bold text-sm mb-1 leading-tight">Transformasi Pendidikan dan Karakter (Belajar & Mengajari)</h4>
                        <p class="text-gray-700 text-sm leading-relaxed">Mewujudkan sistem pembinaan berbasis edukasi, pelatihan vokasi, dan pengembangan potensi diri yang inklusif bagi anak yatim dan dhuafa guna mencetak generasi mandiri dan berintegritas.</p>
                    </div>
                </div>
                <div class="flex items-start gap-4 p-4 rounded-xl border border-gray-50 hover:bg-red-50 transition-colors group cursor-default">
                    <span class="text-secondary/30 group-hover:text-primary font-black text-2xl transition-colors mt-1">02</span>
                    <div>
                        <h4 class="text-primary font-bold text-sm mb-1 leading-tight">Penguatan Kesadaran dan Kepedulian Sosial (Mengingat & Mengingatkan)</h4>
                        <p class="text-gray-700 text-sm leading-relaxed">Menggerakkan partisipasi publik melalui dakwah sosial dan edukasi kedermawanan untuk terus saling mengingatkan dalam kebaikan dan keadilan sosial.</p>
                    </div>
                </div>
                <div class="flex items-start gap-4 p-4 rounded-xl border border-gray-50 hover:bg-red-50 transition-colors group cursor-default">
                    <span class="text-secondary/30 group-hover:text-primary font-black text-2xl transition-colors mt-1">03</span>
                    <div>
                        <h4 class="text-primary font-bold text-sm mb-1 leading-tight">Pemberdayaan Ekonomi dan Kemandirian Umat (Memberi & Menerima Manfaat)</h4>
                        <p class="text-gray-700 text-sm leading-relaxed">Mengelola penyaluran dana hibah, zakat, infak, dan sedekah secara tepat guna, produktif, dan berbasis dampak (impact-driven) demi mengangkat martabat serta kesejahteraan para penerima manfaat.</p>
                    </div>
                </div>
                <div class="flex items-start gap-4 p-4 rounded-xl border border-gray-50 hover:bg-red-50 transition-colors group cursor-default">
                    <span class="text-secondary/30 group-hover:text-primary font-black text-2xl transition-colors mt-1">04</span>
                    <div>
                        <h4 class="text-primary font-bold text-sm mb-1 leading-tight">Sinergi dan Kemitraan Strategis (Memberi & Menerima Faedah)</h4>
                        <p class="text-gray-700 text-sm leading-relaxed">Membangun kolaborasi lintas sektor yang adaptif, inovatif, dan berdaya guna tinggi untuk memperluas jangkauan kebermanfaatan bagi masyarakat luas.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
</section>

<!-- Program Section -->
<section id="program" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-primary font-semibold uppercase tracking-wider text-sm">Apa Yang Kami Lakukan</span>
                <h2 class="text-3xl md:text-4xl font-bold text-dark mt-2 mb-4">Program Kepedulian Kami</h2>
                <p class="text-gray-600">Berbagai inisiatif dan kegiatan rutin yang kami selenggarakan untuk menebar kebermanfaatan bagi masyarakat luas.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Program 1: Jum'at Berkah -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-xl transition-shadow group border-b-4 border-primary flex flex-col">
                    <div class="relative h-48 overflow-hidden flex-shrink-0">
                        <img src="https://images.unsplash.com/photo-1593113565214-8ca7ebcc49a8?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Jum'at Berkah" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute top-4 right-4 bg-white/90 px-3 py-1 rounded-full text-sm font-semibold text-primary">Sosial</div>
                    </div>
                    <div class="p-6 flex flex-col flex-1">
                        <h3 class="text-xl font-bold text-dark mb-3">Jum'at Berkah</h3>
                        <p class="text-gray-600 mb-6 flex-1">Berbagi kebahagiaan melalui penyaluran paket makanan dan sembako setiap hari Jumat untuk kaum dhuafa dan masyarakat membutuhkan.</p>
                        <a href="#donasi" class="block w-full text-center bg-red-50 text-primary border border-primary hover:bg-primary hover:text-white py-2 rounded-lg font-semibold transition-colors mt-auto">Dukung Program</a>
                    </div>
                </div>

                <!-- Program 2: Magrib Mengaji -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-xl transition-shadow group border-b-4 border-primary flex flex-col">
                    <div class="relative h-48 overflow-hidden flex-shrink-0">
                        <img src="https://images.unsplash.com/photo-1609599006353-e629aaab31ce?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Magrib Mengaji" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute top-4 right-4 bg-white/90 px-3 py-1 rounded-full text-sm font-semibold text-primary">Pendidikan</div>
                    </div>
                    <div class="p-6 flex flex-col flex-1">
                        <h3 class="text-xl font-bold text-dark mb-3">Magrib Mengaji</h3>
                        <p class="text-gray-600 mb-6 flex-1">Program pembinaan baca tulis Al-Quran dan pemahaman nilai-nilai agama Islam bagi anak-anak binaan setelah waktu Magrib.</p>
                        <a href="#donasi" class="block w-full text-center bg-red-50 text-primary border border-primary hover:bg-primary hover:text-white py-2 rounded-lg font-semibold transition-colors mt-auto">Dukung Program</a>
                    </div>
                </div>

                <!-- Program 3: YAMUGREEN -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-xl transition-shadow group border-b-4 border-primary flex flex-col">
                    <div class="relative h-48 overflow-hidden flex-shrink-0">
                        <img src="https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="YAMUGREEN" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute top-4 right-4 bg-white/90 px-3 py-1 rounded-full text-sm font-semibold text-primary">Lingkungan</div>
                    </div>
                    <div class="p-6 flex flex-col flex-1">
                        <h3 class="text-xl font-bold text-dark mb-3">YAMUGREEN</h3>
                        <p class="text-gray-600 mb-6 flex-1">Inisiatif pelestarian lingkungan dan penghijauan sebagai wujud nyata kepedulian lembaga terhadap kelestarian alam sekitar.</p>
                        <a href="#donasi" class="block w-full text-center bg-red-50 text-primary border border-primary hover:bg-primary hover:text-white py-2 rounded-lg font-semibold transition-colors mt-auto">Dukung Program</a>
                    </div>
                </div>
                
                <!-- Program 4: Puncak MPLS -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-xl transition-shadow group border-b-4 border-primary flex flex-col">
                    <div class="relative h-48 overflow-hidden flex-shrink-0">
                        <img src="https://images.unsplash.com/photo-1577896851231-70ef18881754?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Puncak MPLS" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute top-4 right-4 bg-white/90 px-3 py-1 rounded-full text-sm font-semibold text-primary">Sosial</div>
                    </div>
                    <div class="p-6 flex flex-col flex-1">
                        <h3 class="text-xl font-bold text-dark mb-3">Puncak MPLS <span class="text-sm block font-normal text-primary mt-1">(Mengetuk Pintu Langit dengan Shodaqoh)</span></h3>
                        <p class="text-gray-600 mb-6 flex-1">Program sedekah spesial dan doa bersama anak yatim sebagai ikhtiar spiritual untuk mengetuk pintu rahmat dan keberkahan dari Allah SWT.</p>
                        <a href="#donasi" class="block w-full text-center bg-red-50 text-primary border border-primary hover:bg-primary hover:text-white py-2 rounded-lg font-semibold transition-colors mt-auto">Dukung Program</a>
                    </div>
                </div>
                
                <!-- Program 5: SILABUS -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-xl transition-shadow group border-b-4 border-primary flex flex-col">
                    <div class="relative h-48 overflow-hidden flex-shrink-0">
                        <img src="https://lh3.googleusercontent.com/d/1-mp3lAgb3e_7XzDHAtMxdBu7QCexE7wj" alt="SILABUS" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute top-4 right-4 bg-white/90 px-3 py-1 rounded-full text-sm font-semibold text-primary">Sosial</div>
                    </div>
                    <div class="p-6 flex flex-col flex-1">
                        <h3 class="text-xl font-bold text-dark mb-3">SILABUS <span class="text-sm block font-normal text-primary mt-1">(Silahturahmi Berbagi Untuk Sesama)</span></h3>
                        <p class="text-gray-600 mb-6 flex-1">Kegiatan silaturahmi rutin yang dirangkaikan dengan aksi berbagi kebahagiaan dan kepedulian bagi sesama yang membutuhkan.</p>
                        <a href="#donasi" class="block w-full text-center bg-red-50 text-primary border border-primary hover:bg-primary hover:text-white py-2 rounded-lg font-semibold transition-colors mt-auto">Dukung Program</a>
                    </div>
                </div>

                <!-- Program 6: Tabungan Kurban -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-xl transition-shadow group border-b-4 border-primary flex flex-col">
                    <div class="relative h-48 overflow-hidden flex-shrink-0">
                        <img src="https://images.unsplash.com/photo-1553729459-efe14ef6055d?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Tabungan Kurban" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute top-4 right-4 bg-white/90 px-3 py-1 rounded-full text-sm font-semibold text-primary">Ibadah</div>
                    </div>
                    <div class="p-6 flex flex-col flex-1">
                        <h3 class="text-xl font-bold text-dark mb-3">Tabungan Kurban</h3>
                        <p class="text-gray-600 mb-6 flex-1">Fasilitas perencanaan ibadah kurban yang mudah dan terjangkau agar kelak daging kurban dapat disalurkan tepat sasaran kepada dhuafa.</p>
                        <a href="#donasi" class="block w-full text-center bg-red-50 text-primary border border-primary hover:bg-primary hover:text-white py-2 rounded-lg font-semibold transition-colors mt-auto">Dukung Program</a>
                    </div>
                </div>
                
                <!-- Program 7: Sedekah Subuh -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-xl transition-shadow group border-b-4 border-primary flex flex-col">
                    <div class="relative h-48 overflow-hidden flex-shrink-0">
                        <img src="https://lh3.googleusercontent.com/d/1nh67mXhO5ii4W0pZwGDaQ85CKKFoitYg" alt="Sedekah Subuh" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute top-4 right-4 bg-white/90 px-3 py-1 rounded-full text-sm font-semibold text-primary">Sosial</div>
                    </div>
                    <div class="p-6 flex flex-col flex-1">
                        <h3 class="text-xl font-bold text-dark mb-3">Sedekah Subuh</h3>
                        <p class="text-gray-600 mb-6 flex-1">Mengawali hari dengan kebaikan melalui rutinitas sedekah harian di waktu subuh untuk meraih keberkahan hidup yang berlipat ganda.</p>
                        <a href="#donasi" class="block w-full text-center bg-red-50 text-primary border border-primary hover:bg-primary hover:text-white py-2 rounded-lg font-semibold transition-colors mt-auto">Dukung Program</a>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- CTA Banner -->
    <section class="py-16 bg-primary relative overflow-hidden">
        <!-- Dekorasi background -->
        <div class="absolute top-0 right-0 -mr-20 -mt-20 w-64 h-64 rounded-full border-4 border-white opacity-20"></div>
        <div class="absolute bottom-0 left-0 -ml-10 -mb-10 w-40 h-40 rounded-full bg-white opacity-10"></div>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="flex flex-col md:flex-row items-center justify-between gap-8 text-center md:text-left">
                <div class="md:w-2/3">
                    <h2 class="text-3xl font-bold text-white mb-4">Sedekah Jumat, Berkah Berlipat Ganda.</h2>
                    <p class="text-red-100 text-lg">Sisihkan sebagian rezeki Anda untuk membahagiakan anak yatim dan dhuafa. Mari raih keberkahan bersama kami.</p>
                </div>
                <div>
                    <a href="#donasi" class="inline-block bg-white text-primary px-8 py-4 rounded-full font-bold shadow-lg hover:bg-gray-100 transform hover:-translate-y-1 transition-all border-2 border-white hover:border-gray-200">Salurkan Sedekah</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Dokumentasi Section -->
    <section id="dokumentasi" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-end mb-12">
                <div class="max-w-2xl">
                    <span class="text-primary font-semibold uppercase tracking-wider text-sm">Galeri Kegiatan</span>
                    <h2 class="text-3xl font-bold text-dark mt-2">Dokumentasi Program Kami</h2>
                </div>
                <div class="hidden md:block">
                    <a href="#" class="text-primary font-medium hover:underline flex items-center gap-2">Lihat Semua Galeri <i class="fa-solid fa-arrow-right text-sm"></i></a>
                </div>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Item 1 -->
                <div class="relative group rounded-xl overflow-hidden shadow-md cursor-pointer h-64">
                    <img src="https://images.unsplash.com/photo-1488521787991-ed7bbaae773c?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Santunan Yatim" class="w-full h-full object-cover transform group-hover:scale-110 transition-transform duration-700">
                    <div class="absolute inset-0 bg-gradient-to-t from-dark/90 via-dark/20 to-transparent opacity-80 group-hover:opacity-100 transition-opacity duration-300"></div>
                    <div class="absolute bottom-0 left-0 right-0 p-5 translate-y-4 group-hover:translate-y-0 transition-transform duration-300">
                        <span class="text-secondary text-xs font-bold uppercase tracking-wider mb-1 block">Santunan</span>
                        <h3 class="text-white text-lg font-bold leading-tight">Khitanan Massal & Santunan Yatim</h3>
                    </div>
                </div>

                <!-- Item 2 -->
                <div class="relative group rounded-xl overflow-hidden shadow-md cursor-pointer h-64">
                    <img src="https://images.unsplash.com/photo-1593113565214-8ca7ebcc49a8?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Distribusi Sembako" class="w-full h-full object-cover transform group-hover:scale-110 transition-transform duration-700">
                    <div class="absolute inset-0 bg-gradient-to-t from-dark/90 via-dark/20 to-transparent opacity-80 group-hover:opacity-100 transition-opacity duration-300"></div>
                    <div class="absolute bottom-0 left-0 right-0 p-5 translate-y-4 group-hover:translate-y-0 transition-transform duration-300">
                        <span class="text-secondary text-xs font-bold uppercase tracking-wider mb-1 block">Logistik</span>
                        <h3 class="text-white text-lg font-bold leading-tight">Penyaluran 5 Ton Beras untuk Dhuafa</h3>
                    </div>
                </div>

                <!-- Item 3 -->
                <div class="relative group rounded-xl overflow-hidden shadow-md cursor-pointer h-64">
                    <img src="https://images.unsplash.com/photo-1594708767771-a7502209ff51?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Bantuan Bencana" class="w-full h-full object-cover transform group-hover:scale-110 transition-transform duration-700">
                    <div class="absolute inset-0 bg-gradient-to-t from-dark/90 via-dark/20 to-transparent opacity-80 group-hover:opacity-100 transition-opacity duration-300"></div>
                    <div class="absolute bottom-0 left-0 right-0 p-5 translate-y-4 group-hover:translate-y-0 transition-transform duration-300">
                        <span class="text-secondary text-xs font-bold uppercase tracking-wider mb-1 block">Tanggap Bencana</span>
                        <h3 class="text-white text-lg font-bold leading-tight">Bantuan Sembako Korban Banjir</h3>
                    </div>
                </div>
                
                <!-- Item 4 -->
                <div class="relative group rounded-xl overflow-hidden shadow-md cursor-pointer h-64 hidden sm:block">
                    <img src="https://images.unsplash.com/photo-1511895426328-dc8714191300?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Pendidikan" class="w-full h-full object-cover transform group-hover:scale-110 transition-transform duration-700">
                    <div class="absolute inset-0 bg-gradient-to-t from-dark/90 via-dark/20 to-transparent opacity-80 group-hover:opacity-100 transition-opacity duration-300"></div>
                    <div class="absolute bottom-0 left-0 right-0 p-5 translate-y-4 group-hover:translate-y-0 transition-transform duration-300">
                        <span class="text-secondary text-xs font-bold uppercase tracking-wider mb-1 block">Pendidikan</span>
                        <h3 class="text-white text-lg font-bold leading-tight">Penyaluran Seragam Sekolah Yatim</h3>
                    </div>
                </div>

                <!-- Item 5 -->
                <div class="relative group rounded-xl overflow-hidden shadow-md cursor-pointer h-64 hidden lg:block">
                    <img src="https://images.unsplash.com/photo-1526976663112-004cb7345638?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Pemberdayaan" class="w-full h-full object-cover transform group-hover:scale-110 transition-transform duration-700">
                    <div class="absolute inset-0 bg-gradient-to-t from-dark/90 via-dark/20 to-transparent opacity-80 group-hover:opacity-100 transition-opacity duration-300"></div>
                    <div class="absolute bottom-0 left-0 right-0 p-5 translate-y-4 group-hover:translate-y-0 transition-transform duration-300">
                        <span class="text-secondary text-xs font-bold uppercase tracking-wider mb-1 block">Pemberdayaan</span>
                        <h3 class="text-white text-lg font-bold leading-tight">Penyerahan Modal Usaha Dhuafa</h3>
                    </div>
                </div>

                <!-- Item 6 -->
                <div class="relative group rounded-xl overflow-hidden shadow-md cursor-pointer h-64 hidden lg:block">
                    <img src="https://images.unsplash.com/photo-1497604401993-f2e922e5cb0a?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Pembinaan" class="w-full h-full object-cover transform group-hover:scale-110 transition-transform duration-700">
                    <div class="absolute inset-0 bg-gradient-to-t from-dark/90 via-dark/20 to-transparent opacity-80 group-hover:opacity-100 transition-opacity duration-300"></div>
                    <div class="absolute bottom-0 left-0 right-0 p-5 translate-y-4 group-hover:translate-y-0 transition-transform duration-300">
                        <span class="text-secondary text-xs font-bold uppercase tracking-wider mb-1 block">Pembinaan</span>
                        <h3 class="text-white text-lg font-bold leading-tight">Kegiatan Tahfidz Quran Mingguan</h3>
                    </div>
                </div>
            </div>
            
            <div class="mt-10 text-center md:hidden">
                <a href="#" class="text-primary font-medium hover:underline inline-block border-2 border-primary/20 px-6 py-2 rounded-full">Lihat Semua Galeri</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer id="kontak" class="bg-dark text-gray-300 pt-16 pb-8 border-t-[6px] border-primary">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12 mb-12">
                <!-- Info Yayasan -->
                <div class="lg:col-span-2 md:pr-10">
                    <a href="#" class="flex items-center gap-2 mb-6">
                        <img src="https://cdn.phototourl.com/member/2026-10-03-d82bd2ed-cb64-4aa8-8488-a2c3ed74d69a.png" alt="Logo Yamu'ti Cicalengka" class="h-16 w-auto rounded-full object-cover shadow-sm bg-white p-1">
                        <span class="font-bold text-xl text-white">Yamu'ti Cicalengka</span>
                    </a>
                    <p class="text-gray-400 mb-6 text-sm">Lembaga amil zakat dan lembaga sosial yang berkhidmat dalam menyantuni, membina, dan memberdayakan anak yatim serta kaum dhuafa.</p>
                    <div class="flex space-x-4">
                        <a href="https://www.instagram.com/yamuti_cicalengka?cplk=MTUwbnhpNjNvaDgyMg==" target="_blank" rel="noopener noreferrer" class="bg-gray-800 hover:bg-primary text-white w-10 h-10 rounded-full flex items-center justify-center transition-colors">
                            <i class="fa-brands fa-instagram"></i>
                        </a>
                        <a href="https://www.tiktok.com/@yamuti.cicalengka" target="_blank" rel="noopener noreferrer" class="bg-gray-800 hover:bg-primary text-white w-10 h-10 rounded-full flex items-center justify-center transition-colors">
                            <i class="fa-brands fa-tiktok"></i>
                        </a>
                        <a href="https://www.youtube.com/@yamuti_cicalengka" target="_blank" rel="noopener noreferrer" class="bg-gray-800 hover:bg-primary text-white w-10 h-10 rounded-full flex items-center justify-center transition-colors">
                            <i class="fa-brands fa-youtube"></i>
                        </a>
                    </div>
                </div>

                <!-- Tautan Cepat -->
                <div>
                    <h4 class="text-white font-bold text-lg mb-6 relative pb-2 after:content-[''] after:absolute after:left-0 after:bottom-0 after:h-1 after:w-12 after:bg-primary">Tautan Cepat</h4>
                    <ul class="space-y-3">
                        <li><a href="#tentang" class="hover:text-primary transition-colors flex items-center gap-2"><i class="fa-solid fa-angle-right text-xs"></i> Tentang Kami</a></li>
                        <li><a href="#program" class="hover:text-primary transition-colors flex items-center gap-2"><i class="fa-solid fa-angle-right text-xs"></i> Program Donasi</a></li>
                        <li><a href="#dokumentasi" class="hover:text-primary transition-colors flex items-center gap-2"><i class="fa-solid fa-angle-right text-xs"></i> Dokumentasi Kegiatan</a></li>
                    </ul>
                </div>

                <!-- Kontak -->
                <div>
                    <h4 class="text-white font-bold text-lg mb-6 relative pb-2 after:content-[''] after:absolute after:left-0 after:bottom-0 after:h-1 after:w-12 after:bg-primary">Hubungi Kami</h4>
                    <ul class="space-y-4">
                        <li class="flex items-start gap-3">
                            <i class="fa-solid fa-location-dot mt-1 text-primary"></i>
                            <a href="https://maps.app.goo.gl/qnqGHTyvdV2S7MXV8" target="_blank" rel="noopener noreferrer" class="text-sm hover:text-primary transition-colors">Kp. Babakan Peuteuy RT 03 RW 08 Blok Loa</a>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fa-solid fa-phone text-primary"></i>
                            <span class="text-sm">+62 821 3053 2526</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fa-brands fa-whatsapp text-primary"></i>
                            <span class="text-sm">+62 821 3053 2526</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fa-solid fa-envelope text-primary"></i>
                            <span class="text-sm">yamuticicalengka@gmail.com</span>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="border-t border-gray-800 pt-8 mt-8 text-center text-sm text-gray-500">
                <p>&copy; 2026 Yamu'ti Cicalengka. Hak cipta dilindungi undang-undang.</p>
            </div>
        </div>
    </footer>

    <!-- AI Chat Widget -->
    <div id="ai-chat-container" class="fixed bottom-6 right-6 z-50 flex flex-col items-end">
        
        <!-- Chat Window (Hidden by default) -->
        <div id="chat-window" class="hidden w-80 sm:w-96 bg-white rounded-2xl shadow-2xl border border-gray-200 overflow-hidden mb-4 flex-col h-[500px] max-h-[80vh] transition-all-ease origin-bottom-right scale-95 opacity-0">
            <!-- Header -->
            <div class="bg-primary text-white p-4 flex justify-between items-center">
                <div class="flex items-center gap-3">
                    <img src="https://cdn.phototourl.com/member/2026-10-03-d82bd2ed-cb64-4aa8-8488-a2c3ed74d69a.png" alt="AI Avatar" class="h-10 w-10 rounded-full bg-white p-0.5 object-cover">
                    <div>
                        <h3 class="font-bold text-sm">Asisten AI Yamu'ti</h3>
                        <div class="flex items-center gap-1 text-xs text-red-200">
                            <div class="w-2 h-2 bg-green-400 rounded-full"></div> Online
                        </div>
                    </div>
                </div>
                <button id="close-chat" class="text-white/80 hover:text-white focus:outline-none transition-colors">
                    <i class="fa-solid fa-xmark text-xl"></i>
                </button>
            </div>
            
            <!-- Chat Body -->
            <div id="chat-messages" class="flex-1 p-4 overflow-y-auto bg-gray-50 flex flex-col gap-3">
                <!-- Initial Bot Message -->
                <div class="flex gap-2 max-w-[85%] self-start">
                    <img src="https://cdn.phototourl.com/member/2026-10-03-d82bd2ed-cb64-4aa8-8488-a2c3ed74d69a.png" class="h-6 w-6 rounded-full mt-1 object-cover bg-primary p-0.5" alt="Bot">
                    <div class="bg-white border border-gray-200 text-gray-700 p-3 rounded-2xl rounded-tl-sm text-sm shadow-sm">
                        Halo! Saya adalah Asisten AI dari Yamu'ti Cicalengka. Ada yang bisa saya bantu terkait program, donasi, atau info lembaga kami?
                    </div>
                </div>
            </div>

            <!-- Chat Footer (Input) -->
            <div class="p-3 bg-white border-t border-gray-200">
                <form id="chat-form" class="flex items-center gap-2">
                    <input type="text" id="chat-input" placeholder="Tulis pesan Anda..." class="flex-1 bg-gray-100 border-transparent focus:bg-white focus:border-primary focus:ring-1 focus:ring-primary rounded-full px-4 py-2 text-sm outline-none transition-all" autocomplete="off" required>
                    <button type="submit" class="bg-primary hover:bg-dark text-white h-10 w-10 rounded-full flex items-center justify-center transition-colors flex-shrink-0 shadow-md">
                        <i class="fa-solid fa-paper-plane text-sm -ml-0.5"></i>
                    </button>
                </form>
            </div>
        </div>

        <!-- Floating Action Button -->
        <button id="chat-fab" class="bg-primary text-white h-14 w-14 rounded-full shadow-xl hover:shadow-2xl hover:bg-dark transform hover:-translate-y-1 transition-all flex items-center justify-center animate-bounce-slow focus:outline-none">
            <i class="fa-solid fa-comment-dots text-2xl"></i>
        </button>
    </div>

    <!-- Custom Modal (Pengganti Alert) -->
    <div id="custom-modal" class="hidden fixed inset-0 z-[100] flex items-center justify-center p-4 bg-gray-900/40 backdrop-blur-sm transition-opacity opacity-0">
        <div class="bg-white rounded-2xl shadow-2xl max-w-sm w-full p-6 transform scale-95 transition-transform">
            <div class="text-center">
                <div class="mx-auto flex items-center justify-center h-12 w-12 rounded-full bg-green-100 mb-4">
                    <i id="modal-icon" class="fa-solid fa-check text-green-600 text-xl"></i>
                </div>
                <h3 id="modal-title" class="text-lg leading-6 font-bold text-gray-900 mb-2">Sukses</h3>
                <div class="mt-2">
                    <p id="modal-message" class="text-sm text-gray-500">Pesan berhasil dikirim.</p>
                </div>
            </div>
            <div class="mt-6 text-center">
                <button type="button" onclick="closeCustomModal()" class="inline-flex justify-center w-full rounded-full border border-transparent shadow-sm px-4 py-2 bg-primary text-base font-medium text-white hover:bg-dark focus:outline-none sm:text-sm transition-colors">
                    Tutup
                </button>
            </div>
        </div>
    </div>

    <!-- Donasi Modal -->
    <div id="donasi-modal" class="hidden fixed inset-0 z-[100] flex items-center justify-center p-4 bg-gray-900/60 backdrop-blur-sm transition-opacity opacity-0">
        <div class="bg-white rounded-2xl shadow-2xl max-w-md w-full overflow-hidden transform scale-95 transition-transform duration-300">
            <!-- Header -->
            <div class="bg-primary text-white px-6 py-4 flex justify-between items-center">
                <h3 class="font-bold text-lg"><i class="fa-solid fa-wallet mr-2"></i> Rekening Donasi</h3>
                <button onclick="closeDonasiModal()" class="text-white/80 hover:text-white transition-colors focus:outline-none">
                    <i class="fa-solid fa-xmark text-xl"></i>
                </button>
            </div>
            
            <!-- Body -->
            <div class="p-6">
                <div class="text-center mb-6 border-b pb-4">
                    <p class="text-sm text-gray-500 font-semibold uppercase tracking-wider mb-1">Atas Nama (A/N)</p>
                    <p class="font-bold text-xl text-dark">Yayasan Mutiara Titipan Illahi</p>
                </div>
                
                <div class="space-y-3">
                    <!-- Bank BRI -->
                    <div class="flex justify-between items-center bg-gray-50 p-3 rounded-xl border border-gray-200 hover:border-primary/30 transition-colors">
                        <div>
                            <div class="flex items-center gap-3">
                                <img src="https://lh3.googleusercontent.com/d/1DW1gcwdZtJ2l7L6NAQntmnNObgYIJ43x" alt="Logo BRI" class="h-6 w-12 object-contain mix-blend-multiply">
                                <span class="font-bold text-dark text-sm">Bank BRI</span>
                            </div>
                            <p class="text-gray-700 font-mono font-medium text-lg tracking-wide mt-0.5">1140-01-010665-50-0</p>
                        </div>
                        <button onclick="copyToClipboard('114001010665500', this)" class="text-primary hover:bg-red-50 px-3 py-2 rounded-lg text-sm font-semibold transition-colors flex items-center gap-1.5 focus:outline-none">
                            <i class="fa-regular fa-copy"></i> Salin
                        </button>
                    </div>

                    <!-- Bank BCA -->
                    <div class="flex justify-between items-center bg-gray-50 p-3 rounded-xl border border-gray-200 hover:border-primary/30 transition-colors">
                        <div>
                            <div class="flex items-center gap-3">
                                <img src="https://lh3.googleusercontent.com/d/1dEI9QXaQrZshXGv-yEtxjCZaee9kQHv7" alt="Logo BCA" class="h-6 w-12 object-contain mix-blend-multiply">
                                <span class="font-bold text-dark text-sm">Bank BCA</span>
                            </div>
                            <p class="text-gray-700 font-mono font-medium text-lg tracking-wide mt-0.5">3799-887-887</p>
                        </div>
                        <button onclick="copyToClipboard('3799887887', this)" class="text-primary hover:bg-red-50 px-3 py-2 rounded-lg text-sm font-semibold transition-colors flex items-center gap-1.5 focus:outline-none">
                            <i class="fa-regular fa-copy"></i> Salin
                        </button>
                    </div>

                    <!-- Bank BJB -->
                    <div class="flex justify-between items-center bg-gray-50 p-3 rounded-xl border border-gray-200 hover:border-primary/30 transition-colors">
                        <div>
                            <div class="flex items-center gap-3">
                                <img src="https://lh3.googleusercontent.com/d/1V8sYZdLP5VJXnQmgAuabrD44LNaPEHOk" alt="Logo BJB" class="h-6 w-12 object-contain mix-blend-multiply">
                                <span class="font-bold text-dark text-sm">Bank BJB</span>
                            </div>
                            <p class="text-gray-700 font-mono font-medium text-lg tracking-wide mt-0.5">0102553748100</p>
                        </div>
                        <button onclick="copyToClipboard('0102553748100', this)" class="text-primary hover:bg-red-50 px-3 py-2 rounded-lg text-sm font-semibold transition-colors flex items-center gap-1.5 focus:outline-none">
                            <i class="fa-regular fa-copy"></i> Salin
                        </button>
                    </div>

                    <!-- Bank BNI -->
                    <div class="flex justify-between items-center bg-gray-50 p-3 rounded-xl border border-gray-200 hover:border-primary/30 transition-colors">
                        <div>
                            <div class="flex items-center gap-3">
                                <img src="https://lh3.googleusercontent.com/d/15_g_J0Dk0vbIm1SzQgupffDCU77pe1cV" alt="Logo BNI" class="h-6 w-12 object-contain mix-blend-multiply">
                                <span class="font-bold text-dark text-sm">Bank BNI</span>
                            </div>
                            <p class="text-gray-700 font-mono font-medium text-lg tracking-wide mt-0.5">0953645923</p>
                        </div>
                        <button onclick="copyToClipboard('0953645923', this)" class="text-primary hover:bg-red-50 px-3 py-2 rounded-lg text-sm font-semibold transition-colors flex items-center gap-1.5 focus:outline-none">
                            <i class="fa-regular fa-copy"></i> Salin
                        </button>
                    </div>

                    <!-- Bank Mandiri -->
                    <div class="flex justify-between items-center bg-gray-50 p-3 rounded-xl border border-gray-200 hover:border-primary/30 transition-colors">
                        <div>
                            <div class="flex items-center gap-3">
                                <img src="https://lh3.googleusercontent.com/d/1IuxS-yGJC3kK7N1dhOlDUr0VxxK0JbJy" alt="Logo Mandiri" class="h-6 w-12 object-contain mix-blend-multiply">
                                <span class="font-bold text-dark text-sm">Bank Mandiri</span>
                            </div>
                            <p class="text-gray-700 font-mono font-medium text-lg tracking-wide mt-0.5">130-00-1639734-4</p>
                        </div>
                        <button onclick="copyToClipboard('1300016397344', this)" class="text-primary hover:bg-red-50 px-3 py-2 rounded-lg text-sm font-semibold transition-colors flex items-center gap-1.5 focus:outline-none">
                            <i class="fa-regular fa-copy"></i> Salin
                        </button>
                    </div>
                </div>

                <!-- Footer Note -->
                <div class="mt-5 text-center px-4">
                    <p class="text-xs text-gray-500 font-medium">
                        <span class="text-red-500">*</span> Konfirmasi donasi / pembayaran diperlukan untuk Tertib Administrasi.
                    </p>
                </div>
                
                <!-- WA Button -->
                <div class="mt-6">
                    <a href="https://wa.me/6282130532526?text=Halo%20Admin%20Yamu'ti,%20saya%20ingin%20mengkonfirmasi%20donasi%20saya..." target="_blank" class="w-full flex items-center justify-center gap-2 bg-[#25D366] hover:bg-[#128C7E] text-white py-3.5 rounded-xl font-bold transition-all shadow-md hover:shadow-lg transform hover:-translate-y-0.5">
                        <i class="fa-brands fa-whatsapp text-xl"></i> Konfirmasi via WhatsApp
                    </a>
                </div>
            </div>
        </div>
    </div>

    <!-- Scripts -->
    <script>
        let chatHistory = [];
        const apiKey = ""; // Disuntikkan oleh sistem canvas
        const modelName = "gemini-3-flash-preview";
        const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/${modelName}:generateContent?key=${apiKey}`;
        
        const systemPrompt = `Anda adalah asisten virtual resmi (AI Amil) untuk Yamu'ti Cicalengka. 
Lembaga ini adalah lembaga sosial yang secara khusus berfokus pada penyantunan, pembinaan anak yatim, dan pemberdayaan kaum dhuafa di wilayah Cicalengka, Kabupaten Bandung dan sekitarnya.
Jawab pertanyaan pengguna dengan ramah, sopan, Islami (bila sesuai konteks), dan informatif. 
Gunakan bahasa Indonesia yang baik dan menyejukkan.
Daftar program lembaga kami: Jum'at Berkah, Magrib Mengaji, YAMUGREEN, Puncak MPLS (Mengetuk Pintu Langit dengan Shodaqoh), SILABUS (Silahturahmi Berbagi Untuk Sesama), Tabungan Kurban, dan Sedekah Subuh. Anda menerima donasi berupa Zakat, Infaq, Sedekah, maupun Wakaf.
Arahkan pengguna yang ingin berdonasi, mengikuti program, atau konfirmasi transfer untuk menghubungi kontak WhatsApp lembaga yang tersedia di website.
Jaga respons agar padat dan jelas (maksimal 2-3 paragraf).`;

        /* DOM Elements */
        // Navbar Mobile
        const btn = document.getElementById('mobile-menu-btn');
        const menu = document.getElementById('mobile-menu');
        const icon = btn.querySelector('i');
        const navbar = document.getElementById('navbar');
        
        // Chat UI
        const chatFab = document.getElementById('chat-fab');
        const chatWindow = document.getElementById('chat-window');
        const closeChatBtn = document.getElementById('close-chat');
        const chatForm = document.getElementById('chat-form');
        const chatInput = document.getElementById('chat-input');
        const chatMessages = document.getElementById('chat-messages');

        // Modal UI
        const customModal = document.getElementById('custom-modal');
        const modalContent = customModal.querySelector('div.bg-white');
        const modalTitle = document.getElementById('modal-title');
        const modalMessage = document.getElementById('modal-message');
        const modalIcon = document.getElementById('modal-icon');

        // Navbar Mobile Toggle
        btn.addEventListener('click', () => {
            menu.classList.toggle('hidden');
            if (menu.classList.contains('hidden')) {
                icon.classList.replace('fa-xmark', 'fa-bars');
            } else {
                icon.classList.replace('fa-bars', 'fa-xmark');
            }
        });

        // Close mobile menu on click
        const mobileLinks = menu.querySelectorAll('a');
        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                menu.classList.add('hidden');
                icon.classList.replace('fa-xmark', 'fa-bars');
            });
        });

        // Navbar scroll effect
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                navbar.classList.replace('py-2', 'py-0');
            } else {
                navbar.classList.replace('py-0', 'py-2');
            }
        });

        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                // Intercept Donasi links
                if(targetId === '#donasi') {
                    e.preventDefault();
                    openDonasiModal();
                    return;
                }
                
                e.preventDefault();
                const targetElement = document.querySelector(targetId);
                
                if(targetElement) {
                    const y = targetElement.getBoundingClientRect().top + window.pageYOffset - 80;
                    window.scrollTo({top: y, behavior: 'smooth'});
                }
            });
        });

        // Hero Background Slideshow
        const heroSlides = document.querySelectorAll('.hero-slide');
        const slideDots = document.querySelectorAll('.slide-dot');
        let currentSlide = 0;
        let slideInterval;

        function showSlide(index) {
            if (heroSlides.length === 0) return;
            
            // Sembunyikan slide saat ini
            heroSlides[currentSlide].classList.remove('opacity-50');
            heroSlides[currentSlide].classList.add('opacity-0');
            if(slideDots.length > 0) {
                slideDots[currentSlide].classList.remove('opacity-100');
                slideDots[currentSlide].classList.add('opacity-50');
            }
            
            // Set slide baru
            currentSlide = index;
            
            // Tampilkan slide berikutnya
            heroSlides[currentSlide].classList.remove('opacity-0');
            heroSlides[currentSlide].classList.add('opacity-50');
            if(slideDots.length > 0) {
                slideDots[currentSlide].classList.remove('opacity-50');
                slideDots[currentSlide].classList.add('opacity-100');
            }
        }

        function nextHeroSlide() {
            let next = (currentSlide + 1) % heroSlides.length;
            showSlide(next);
        }

        function goToSlide(index) {
            showSlide(index);
            // Reset interval agar tidak langsung berganti setelah diklik manual
            clearInterval(slideInterval);
            slideInterval = setInterval(nextHeroSlide, 5000);
        }

        // Ganti gambar setiap 5 detik
        if (heroSlides.length > 1) {
            slideInterval = setInterval(nextHeroSlide, 5000);
        }

        // Modal Functions
        function showCustomModal(title, message, isError = false) {
            modalTitle.textContent = title;
            modalMessage.textContent = message;
            
            if (isError) {
                modalIcon.className = "fa-solid fa-triangle-exclamation text-red-600 text-xl";
                modalIcon.parentElement.className = "mx-auto flex items-center justify-center h-12 w-12 rounded-full bg-red-100 mb-4";
            } else {
                modalIcon.className = "fa-solid fa-check text-green-600 text-xl";
                modalIcon.parentElement.className = "mx-auto flex items-center justify-center h-12 w-12 rounded-full bg-green-100 mb-4";
            }

            customModal.classList.remove('hidden');
            // Allow display block to render before animating opacity/scale
            setTimeout(() => {
                customModal.classList.replace('opacity-0', 'opacity-100');
                modalContent.classList.replace('scale-95', 'scale-100');
            }, 10);
        }

        function closeCustomModal() {
            customModal.classList.replace('opacity-100', 'opacity-0');
            modalContent.classList.replace('scale-100', 'scale-95');
            setTimeout(() => {
                customModal.classList.add('hidden');
            }, 300); // match transition duration
        }

        // Donasi Modal Functions
        const donasiModal = document.getElementById('donasi-modal');
        const donasiModalContent = donasiModal.querySelector('div.bg-white');

        function openDonasiModal() {
            donasiModal.classList.remove('hidden');
            // Menutup mobile menu jika terbuka
            if (!menu.classList.contains('hidden')) {
                menu.classList.add('hidden');
                icon.classList.replace('fa-xmark', 'fa-bars');
            }
            setTimeout(() => {
                donasiModal.classList.replace('opacity-0', 'opacity-100');
                donasiModalContent.classList.replace('scale-95', 'scale-100');
            }, 10);
        }

        function closeDonasiModal() {
            donasiModal.classList.replace('opacity-100', 'opacity-0');
            donasiModalContent.classList.replace('scale-100', 'scale-95');
            setTimeout(() => {
                donasiModal.classList.add('hidden');
            }, 300);
        }

        // Copy to clipboard function
        function copyToClipboard(text, btnElement) {
            // Create a temporary input element
            const tempInput = document.createElement("input");
            tempInput.value = text;
            document.body.appendChild(tempInput);
            
            // Select and copy
            tempInput.select();
            tempInput.setSelectionRange(0, 99999); // For mobile devices
            document.execCommand("copy");
            
            // Remove the temporary element
            document.body.removeChild(tempInput);
            
            // Visual feedback on button
            const originalHtml = btnElement.innerHTML;
            btnElement.innerHTML = '<i class="fa-solid fa-check"></i> Tersalin';
            btnElement.classList.remove('text-primary', 'hover:bg-red-50');
            btnElement.classList.add('text-green-600', 'bg-green-50');
            
            // Reset button after 2 seconds
            setTimeout(() => {
                btnElement.innerHTML = originalHtml;
                btnElement.classList.add('text-primary', 'hover:bg-red-50');
                btnElement.classList.remove('text-green-600', 'bg-green-50');
            }, 2000);
        }

        // Chat Toggle Logic
        function toggleChat() {
            if (chatWindow.classList.contains('hidden')) {
                chatWindow.classList.remove('hidden');
                chatFab.classList.remove('animate-bounce-slow');
                // Animate in
                setTimeout(() => {
                    chatWindow.classList.replace('scale-95', 'scale-100');
                    chatWindow.classList.replace('opacity-0', 'opacity-100');
                    chatInput.focus();
                }, 10);
            } else {
                // Animate out
                chatWindow.classList.replace('scale-100', 'scale-95');
                chatWindow.classList.replace('opacity-100', 'opacity-0');
                setTimeout(() => {
                    chatWindow.classList.add('hidden');
                }, 300);
            }
        }

        chatFab.addEventListener('click', toggleChat);
        closeChatBtn.addEventListener('click', toggleChat);

        // Helper to append message to chat
        function appendMessage(text, isUser = false) {
            const msgDiv = document.createElement('div');
            msgDiv.className = `flex gap-2 max-w-[85%] ${isUser ? 'self-end flex-row-reverse' : 'self-start'}`;
            
            const avatar = isUser ? '' : `<img src="https://cdn.phototourl.com/member/2026-10-03-d82bd2ed-cb64-4aa8-8488-a2c3ed74d69a.png" class="h-6 w-6 rounded-full mt-1 object-cover bg-primary p-0.5" alt="Bot">`;
            
            const bubbleStyle = isUser 
                ? 'bg-primary text-white rounded-tl-2xl rounded-bl-2xl rounded-br-sm rounded-tr-2xl' 
                : 'bg-white border border-gray-200 text-gray-700 rounded-tr-2xl rounded-br-2xl rounded-bl-sm rounded-tl-2xl shadow-sm';
            
            // Format line breaks
            const formattedText = text.replace(/\n/g, '<br>');

            msgDiv.innerHTML = `
                ${avatar}
                <div class="${bubbleStyle} p-3 text-sm">
                    ${formattedText}
                </div>
            `;
            
            chatMessages.appendChild(msgDiv);
            scrollToBottom();
        }

        // Helper to add/remove typing indicator
        let typingIndicatorDiv = null;
        function showTyping() {
            if (typingIndicatorDiv) return;
            typingIndicatorDiv = document.createElement('div');
            typingIndicatorDiv.className = 'flex gap-2 max-w-[85%] self-start';
            typingIndicatorDiv.innerHTML = `
                <img src="https://cdn.phototourl.com/member/2026-10-03-d82bd2ed-cb64-4aa8-8488-a2c3ed74d69a.png" class="h-6 w-6 rounded-full mt-1 object-cover bg-primary p-0.5" alt="Bot">
                <div class="bg-white border border-gray-200 p-3 rounded-2xl rounded-tl-sm shadow-sm flex gap-1 items-center h-10">
                    <div class="w-1.5 h-1.5 bg-gray-400 rounded-full typing-dot"></div>
                    <div class="w-1.5 h-1.5 bg-gray-400 rounded-full typing-dot"></div>
                    <div class="w-1.5 h-1.5 bg-gray-400 rounded-full typing-dot"></div>
                </div>
            `;
            chatMessages.appendChild(typingIndicatorDiv);
            scrollToBottom();
        }

        function removeTyping() {
            if (typingIndicatorDiv) {
                typingIndicatorDiv.remove();
                typingIndicatorDiv = null;
            }
        }

        function scrollToBottom() {
            chatMessages.scrollTop = chatMessages.scrollHeight;
        }

        // API Fetch with Exponential Backoff
        async function fetchGeminiAPI(payload, maxRetries = 3) {
            let delay = 1000;
            for (let i = 0; i < maxRetries; i++) {
                try {
                    const response = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });
                    
                    if (!response.ok) {
                        if (response.status === 429 && i < maxRetries - 1) {
                            // Rate limit, backoff and retry
                            await new Promise(res => setTimeout(res, delay));
                            delay *= 2;
                            continue;
                        }
                        throw new Error(`Gagal menghubungi server (Status: ${response.status})`);
                    }
                    
                    return await response.json();
                } catch (error) {
                    if (i === maxRetries - 1) throw error;
                }
            }
        }

        // Handle Form Submit
        chatForm.addEventListener('submit', async (e) => {
            e.preventDefault();
            const text = chatInput.value.trim();
            if (!text) return;

            // 1. Append user message to UI
            appendMessage(text, true);
            chatInput.value = '';
            chatInput.disabled = true; // prevent multiple submissions

            // 2. Append to chat history format for API
            chatHistory.push({ role: "user", parts: [{ text: text }] });

            // 3. Show typing indicator
            showTyping();

            try {
                // 4. Prepare payload
                const payload = {
                    contents: chatHistory,
                    systemInstruction: {
                        parts: [{ text: systemPrompt }]
                    }
                };

                // 5. Call API
                const result = await fetchGeminiAPI(payload);
                
                // 6. Parse response
                const candidate = result?.candidates?.[0];
                if (candidate && candidate.content?.parts?.[0]?.text) {
                    const aiText = candidate.content.parts[0].text;
                    
                    // Add AI response to history
                    chatHistory.push({ role: "model", parts: [{ text: aiText }] });
                    
                    // Render to UI
                    removeTyping();
                    appendMessage(aiText, false);
                } else {
                    throw new Error("Format respons dari server tidak dikenali.");
                }

            } catch (error) {
                removeTyping();
                console.error("Chat Error:", error);
                
                // Remove the last user message from history so they can try again
                chatHistory.pop(); 
                
                // Show error message in chat
                appendMessage("Maaf, saya sedang mengalami gangguan koneksi. Silakan coba beberapa saat lagi.", false);
                
            } finally {
                chatInput.disabled = false;
                chatInput.focus();
            }
        });

    </script>
</body>
</html>
