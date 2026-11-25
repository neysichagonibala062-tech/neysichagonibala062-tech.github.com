  <!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Neysicha Cinta Gonibala — Personal Profile</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Plus Jakarta Sans & Playfair Display -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,500;0,600;0,700;1,400&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['"Plus Jakarta Sans"', 'sans-serif'],
                        serif: ['"Playfair Display"', 'serif'],
                    },
                    colors: {
                        earth: {
                            50: '#FAF8F5',
                            100: '#F3EFEA',
                            200: '#E5DDD3',
                            300: '#D1C3B2',
                            400: '#B8A28B',
                            500: '#9E8368',
                            600: '#826850',
                            700: '#68523F',
                            800: '#554436',
                            900: '#46382E',
                        },
                        sage: {
                            50: '#F4F6F3',
                            100: '#E5EAE3',
                            500: '#6B7F66',
                            700: '#485744',
                            800: '#3B4738',
                        }
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-earth-50 text-earth-900 font-sans antialiased selection:bg-earth-300 selection:text-earth-900">

    <!-- Notifikasi Toast (Pengganti alert) -->
    <div id="toast" class="fixed bottom-5 right-5 z-50 transform translate-y-20 opacity-0 transition-all duration-300 pointer-events-none">
        <div class="bg-earth-800 text-earth-50 px-5 py-3.5 rounded-2xl shadow-xl flex items-center gap-3 border border-earth-700">
            <i data-lucide="sparkles" class="w-5 h-5 text-earth-300"></i>
            <span id="toast-message" class="text-sm font-medium">Pesan berhasil diperbarui!</span>
        </div>
    </div>

    <!-- Navigasi Atas -->
    <nav class="sticky top-0 z-40 bg-earth-50/85 backdrop-blur-md border-b border-earth-200/70">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16 sm:h-20">
                <!-- Logo / Nama -->
                <a href="#beranda" class="font-serif text-xl sm:text-2xl font-bold tracking-tight text-earth-900 flex items-center gap-2">
                    <span class="w-8 h-8 rounded-full bg-earth-800 text-earth-50 flex items-center justify-center text-sm font-sans font-semibold">N</span>
                    <span>Neysicha<span class="text-earth-500">.</span></span>
                </a>

                <!-- Menu Desktop -->
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#beranda" class="text-sm font-medium text-earth-700 hover:text-earth-900 transition-colors">Beranda</a>
                    <a href="#tentang" class="text-sm font-medium text-earth-700 hover:text-earth-900 transition-colors">Tentang Saya</a>
                    <a href="#perjalanan" class="text-sm font-medium text-earth-700 hover:text-earth-900 transition-colors">Biodata & Cerita</a>
                    <a href="#galeri" class="text-sm font-medium text-earth-700 hover:text-earth-900 transition-colors">Minat & Hobi</a>
                    <a href="#kontak" class="px-5 py-2.5 rounded-full bg-earth-800 text-earth-50 text-sm font-medium hover:bg-earth-700 transition-all shadow-sm hover:shadow">
                        Sapa Saya
                    </a>
                </div>

                <!-- Tombol Menu Mobile -->
                <button id="mobile-menu-btn" aria-label="Buka Menu" class="md:hidden p-2.5 rounded-xl text-earth-800 hover:bg-earth-200/60 transition-colors">
                    <i data-lucide="menu" class="w-6 h-6"></i>
                </button>
            </div>
        </div>

        <!-- Dropdown Menu Mobile -->
        <div id="mobile-menu" class="hidden md:hidden bg-earth-50 border-b border-earth-200 px-4 pt-2 pb-5 space-y-2">
            <a href="#beranda" class="block px-4 py-2.5 rounded-xl text-base font-medium text-earth-800 hover:bg-earth-100">Beranda</a>
            <a href="#tentang" class="block px-4 py-2.5 rounded-xl text-base font-medium text-earth-800 hover:bg-earth-100">Tentang Saya</a>
            <a href="#perjalanan" class="block px-4 py-2.5 rounded-xl text-base font-medium text-earth-800 hover:bg-earth-100">Biodata & Cerita</a>
            <a href="#galeri" class="block px-4 py-2.5 rounded-xl text-base font-medium text-earth-800 hover:bg-earth-100">Minat & Hobi</a>
            <a href="#kontak" class="block px-4 py-2.5 rounded-xl text-base font-medium bg-earth-800 text-earth-50 text-center mt-2">Sapa Saya</a>
        </div>
    </nav>

    <!-- HERO SECTION (Halaman Depan dengan Foto Utama) -->
    <section id="beranda" class="relative overflow-hidden pt-10 pb-20 sm:pt-16 sm:pb-28">
        <!-- Dekorasi Latar Belakang Lembut -->
        <div class="absolute top-0 right-0 -z-10 w-96 h-96 bg-earth-200/50 rounded-full blur-3xl opacity-70 translate-x-1/3 -translate-y-1/4"></div>
        <div class="absolute bottom-0 left-0 -z-10 w-80 h-80 bg-sage-100 rounded-full blur-3xl opacity-80 -translate-x-1/4 translate-y-1/4"></div>

        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-10 items-center">
                
                <!-- Kolom Teks Perkenalan -->
                <div class="lg:col-span-7 space-y-6 text-center lg:text-left order-2 lg:order-1">
                    <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-earth-100 border border-earth-200 text-earth-700 text-xs sm:text-sm font-medium">
                        <i data-lucide="map-pin" class="w-4 h-4 text-earth-600"></i>
                        <span>Lahir di Kotamobagu • 25 Januari 2007</span>
                    </div>

                    <h1 class="font-serif text-4xl sm:text-5xl lg:text-6xl font-bold text-earth-900 leading-tight">
                        Halo, Saya <br class="hidden sm:inline">
                        <span class="text-earth-600 italic font-semibold">Neysicha Cinta Gonibala</span>
                    </h1>

                    <p class="text-base sm:text-lg text-earth-700 max-w-2xl mx-auto lg:mx-0 leading-relaxed">
                        Selamat datang di ruang digital pribadi saya. Tempat di mana saya berbagi cerita, langkah perjalanan hidup, hobi, serta hal-hal sederhana yang membawa kebahagiaan setiap harinya.
                    </p>

                    <!-- Info Singkat Usia & Zodiak -->
                    <div class="flex flex-wrap justify-center lg:justify-start gap-3 pt-1">
                        <div class="px-4 py-2.5 rounded-2xl bg-white border border-earth-200/80 shadow-sm flex items-center gap-2.5">
                            <i data-lucide="cake" class="w-4 h-4 text-earth-500"></i>
                            <span class="text-sm font-medium text-earth-800" id="umur-display">19 Tahun</span>
                        </div>
                        <div class="px-4 py-2.5 rounded-2xl bg-white border border-earth-200/80 shadow-sm flex items-center gap-2.5">
                            <i data-lucide="sparkles" class="w-4 h-4 text-earth-500"></i>
                            <span class="text-sm font-medium text-earth-800">Aquarius</span>
                        </div>
                        <div class="px-4 py-2.5 rounded-2xl bg-white border border-earth-200/80 shadow-sm flex items-center gap-2.5">
                            <i data-lucide="compass" class="w-4 h-4 text-earth-500"></i>
                            <span class="text-sm font-medium text-earth-800">Sulawesi Utara</span>
                        </div>
                    </div>

                    <!-- Tombol Aksi -->
                    <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-3">
                        <a href="#tentang" class="w-full sm:w-auto px-7 py-3.5 rounded-full bg-earth-800 text-earth-50 font-medium text-sm hover:bg-earth-700 transition-all shadow-md hover:shadow-lg flex items-center justify-center gap-2">
                            <span>Kenali Lebih Dekat</span>
                            <i data-lucide="arrow-down-right" class="w-4 h-4"></i>
                        </a>
                        <button onclick="document.getElementById('photo-upload').click()" class="w-full sm:w-auto px-6 py-3.5 rounded-full bg-white text-earth-800 border border-earth-300 font-medium text-sm hover:bg-earth-100 transition-all flex items-center justify-center gap-2">
                            <i data-lucide="camera" class="w-4 h-4 text-earth-600"></i>
                            <span>Pilih / Ganti Foto Profil</span>
                        </button>
                    </div>
                </div>

                <!-- Kolom Foto Profil Utama -->
                <div class="lg:col-span-5 order-1 lg:order-2 flex justify-center">
                    <div class="relative w-full max-w-sm sm:max-w-md group">
                        <!-- Bingkai Dekoratif Belakang -->
                        <div class="absolute -inset-3 bg-gradient-to-tr from-earth-300 via-earth-200 to-sage-100 rounded-[2.2rem] rotate-3 transition-transform duration-500 group-hover:rotate-6"></div>
                        
                        <!-- Kartu Foto Utama -->
                        <div class="relative bg-white p-3 rounded-[2rem] shadow-xl border border-earth-200/80">
                            <div class="relative aspect-[4/5] w-full overflow-hidden rounded-[1.5rem] bg-earth-200">
                                <!-- Foto Utama dengan Fallback Elegan -->
                                <img 
                                    id="profile-photo" 
                                    src="1000246877.jpg" 
                                    alt="Foto Profil Neysicha Cinta Gonibala" 
                                    onerror="handleImageFallback(this)"
                                    class="w-full h-full object-cover object-center transition-transform duration-700 group-hover:scale-105"
                                >
                                
                                <!-- Overlay Tombol Ganti Foto Saat Hover / Tap -->
                                <label for="photo-upload" class="cursor-pointer absolute inset-0 bg-earth-900/40 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex flex-col items-center justify-center text-white p-4 text-center backdrop-blur-[2px]">
                                    <div class="w-12 h-12 rounded-full bg-white/20 backdrop-blur-md flex items-center justify-center mb-2 border border-white/40">
                                        <i data-lucide="image-plus" class="w-6 h-6 text-white"></i>
                                    </div>
                                    <span class="text-sm font-semibold">Unggah Foto Anda</span>
                                    <span class="text-xs text-earth-100 mt-1">Klik untuk memilih file 1000246877.jpg dari perangkat</span>
                                </label>
                                <input type="file" id="photo-upload" accept="image/*" class="hidden" onchange="previewProfilePhoto(event)">
                            </div>

                            <!-- Caption Polaroid / Bingkai Bawah -->
                            <div class="pt-4 pb-2 px-3 flex items-center justify-between">
                                <div>
                                    <p class="font-serif font-semibold text-earth-900 text-base">Neysicha C. Gonibala</p>
                                    <p class="text-xs text-earth-500">Kotamobagu, 25 Januari 2007</p>
                                </div>
                                <span class="inline-flex items-center justify-center w-9 h-9 rounded-full bg-earth-100 text-earth-700">
                                    <i data-lucide="heart" class="w-4 h-4 fill-earth-400 text-earth-600"></i>
                                </span>
                            </div>
                        </div>

                        <!-- Petunjuk Kecil Jika Foto Belum Terlihat di Pratinjau Browser -->
                        <div id="photo-helper-badge" class="hidden mt-4 text-center">
                            <button onclick="document.getElementById('photo-upload').click()" class="inline-flex items-center gap-2 px-4 py-2 rounded-xl bg-amber-50 border border-amber-200 text-amber-800 text-xs font-medium hover:bg-amber-100 transition-colors">
                                <i data-lucide="upload" class="w-3.5 h-3.5"></i>
                                <span>Klik di sini untuk memuat foto dari galeri Anda</span>
                            </button>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- SECTION: TENTANG SAYA & BIODATA -->
    <section id="tentang" class="py-16 sm:py-24 bg-white border-y border-earth-200/70">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-14">
                <span class="text-xs font-bold uppercase tracking-widest text-earth-500">Tentang Saya</span>
                <h2 class="font-serif text-3xl sm:text-4xl font-bold text-earth-900 mt-2">Mengenal Neysicha Lebih Dekat</h2>
                <p class="text-earth-600 mt-3 text-sm sm:text-base">
                    Setiap orang memiliki cerita uniknya masing-masing. Berikut adalah sekilas informasi pribadi dan nilai-nilai yang saya pegang.
                </p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
                <!-- Kartu Biodata Lengkap -->
                <div class="lg:col-span-5 bg-earth-50 rounded-3xl p-6 sm:p-8 border border-earth-200/80 shadow-sm">
                    <h3 class="font-serif text-xl font-bold text-earth-900 mb-6 flex items-center gap-2.5">
                        <span class="w-8 h-8 rounded-xl bg-earth-800 text-earth-50 flex items-center justify-center">
                            <i data-lucide="user" class="w-4 h-4"></i>
                        </span>
                        <span>Informasi Pribadi</span>
                    </h3>

                    <dl class="space-y-4">
                        <div class="pb-3 border-b border-earth-200/70">
                            <dt class="text-xs font-medium text-earth-500 uppercase tracking-wider">Nama Lengkap</dt>
                            <dd class="text-base font-semibold text-earth-900 mt-1">Neysicha Cinta Gonibala</dd>
                        </div>
                        <div class="pb-3 border-b border-earth-200/70">
                            <dt class="text-xs font-medium text-earth-500 uppercase tracking-wider">Tempat Lahir</dt>
                            <dd class="text-base font-semibold text-earth-900 mt-1">Kotamobagu, Sulawesi Utara</dd>
                        </div>
                        <div class="pb-3 border-b border-earth-200/70">
                            <dt class="text-xs font-medium text-earth-500 uppercase tracking-wider">Tanggal Lahir</dt>
                            <dd class="text-base font-semibold text-earth-900 mt-1">25 Januari 2007</dd>
                        </div>
                        <div class="pb-3 border-b border-earth-200/70">
                            <dt class="text-xs font-medium text-earth-500 uppercase tracking-wider">Zodiak</dt>
                            <dd class="text-base font-semibold text-earth-900 mt-1">Aquarius ♒</dd>
                        </div>
                        <div>
                            <dt class="text-xs font-medium text-earth-500 uppercase tracking-wider">Kewarganegaraan</dt>
                            <dd class="text-base font-semibold text-earth-900 mt-1">Indonesia</dd>
                        </div>
                    </dl>
                </div>

                <!-- Narasi Kepribadian & Nilai Hidup -->
                <div class="lg:col-span-7 space-y-6">
                    <div class="bg-earth-50/60 rounded-3xl p-6 sm:p-8 border border-earth-200/80">
                        <h3 class="font-serif text-2xl font-bold text-earth-900 mb-4">Halo, Senang Bertemu Denganmu!</h3>
                        <div class="space-y-4 text-earth-700 leading-relaxed text-sm sm:text-base">
                            <p>
                                Saya <strong class="text-earth-900">Neysicha Cinta Gonibala</strong>, lahir di kota yang sejuk dan penuh kehangatan, <strong class="text-earth-900">Kotamobagu</strong>, pada tanggal <strong class="text-earth-900">25 Januari 2007</strong>. Tumbuh di lingkungan yang dikelilingi keindahan alam Sulawesi Utara membuat saya sangat menghargai ketenangan, keindahan alam, dan momen-momen bermakna bersama orang-orang terdekat.
                            </p>
                            <p>
                                Sebagai pribadi yang lahir di bulan Januari, saya senang mengeksplorasi hal-hal baru, belajar dari setiap pengalaman, dan selalu berusaha membawa energi positif ke mana pun saya melangkah. Bagi saya, setiap hari adalah kesempatan baru untuk bertumbuh menjadi versi diri yang lebih baik.
                            </p>
                        </div>
                    </div>

                    <!-- 3 Pilar Karakter -->
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-4">
                        <div class="p-5 rounded-2xl bg-sage-50 border border-sage-100">
                            <div class="w-10 h-10 rounded-xl bg-sage-500 text-white flex items-center justify-center mb-3">
                                <i data-lucide="sun" class="w-5 h-5"></i>
                            </div>
                            <h4 class="font-semibold text-earth-900 text-sm">Hangat & Ramah</h4>
                            <p class="text-xs text-earth-600 mt-1 leading-relaxed">Menghargai setiap pertemuan dan menjalin pertemanan yang tulus.</p>
                        </div>

                        <div class="p-5 rounded-2xl bg-earth-100/70 border border-earth-200">
                            <div class="w-10 h-10 rounded-xl bg-earth-700 text-white flex items-center justify-center mb-3">
                                <i data-lucide="mountain" class="w-5 h-5"></i>
                            </div>
                            <h4 class="font-semibold text-earth-900 text-sm">Pecinta Alam</h4>
                            <p class="text-xs text-earth-600 mt-1 leading-relaxed">Menemukan ketenangan di alam terbuka, perbukitan, dan suasana senja.</p>
                        </div>

                        <div class="p-5 rounded-2xl bg-earth-100/70 border border-earth-200">
                            <div class="w-10 h-10 rounded-xl bg-earth-600 text-white flex items-center justify-center mb-3">
                                <i data-lucide="book-open" class="w-5 h-5"></i>
                            </div>
                            <h4 class="font-semibold text-earth-900 text-sm">Terus Belajar</h4>
                            <p class="text-xs text-earth-600 mt-1 leading-relaxed">Selalu antusias mengasah wawasan, kreativitas, dan potensi diri.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECTION: JEJAK LANGKAH & MILESTONE -->
    <section id="perjalanan" class="py-16 sm:py-24 bg-earth-50">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-14">
                <span class="text-xs font-bold uppercase tracking-widest text-earth-500">Jejak Cerita</span>
                <h2 class="font-serif text-3xl sm:text-4xl font-bold text-earth-900 mt-2">Garis Waktu Kehidupan</h2>
            </div>

            <div class="relative border-l-2 border-earth-300 ml-4 sm:ml-6 space-y-10">
                <!-- Item 1 -->
                <div class="relative pl-8 sm:pl-10">
                    <span class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-earth-800 ring-4 ring-earth-50"></span>
                    <div class="bg-white p-6 rounded-2xl border border-earth-200/80 shadow-sm">
                        <span class="inline-block px-3 py-1 rounded-full bg-earth-100 text-earth-700 text-xs font-semibold mb-2">25 Januari 2007</span>
                        <h3 class="font-serif text-lg font-bold text-earth-900">Awal Perjalanan di Kotamobagu</h3>
                        <p class="text-sm text-earth-600 mt-2 leading-relaxed">
                            Lahir di Kotamobagu dengan nama Neysicha Cinta Gonibala. Sebuah awal dari perjalanan penuh kasih sayang dari keluarga tercinta.
                        </p>
                    </div>
                </div>

                <!-- Item 2 -->
                <div class="relative pl-8 sm:pl-10">
                    <span class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-earth-600 ring-4 ring-earth-50"></span>
                    <div class="bg-white p-6 rounded-2xl border border-earth-200/80 shadow-sm">
                        <span class="inline-block px-3 py-1 rounded-full bg-sage-100 text-sage-800 text-xs font-semibold mb-2">Masa Tumbuh & Belajar</span>
                        <h3 class="font-serif text-lg font-bold text-earth-900">Menemukan Minat & Kreativitas</h3>
                        <p class="text-sm text-earth-600 mt-2 leading-relaxed">
                            Menghabiskan masa sekolah dengan aktif belajar, membangun persahabatan, serta menyukai fotografi bernuansa estetik dan eksplorasi alam.
                        </p>
                    </div>
                </div>

                <!-- Item 3 -->
                <div class="relative pl-8 sm:pl-10">
                    <span class="absolute -left-[9px] top-1.5 w-4 h-4 rounded-full bg-earth-500 ring-4 ring-earth-50"></span>
                    <div class="bg-white p-6 rounded-2xl border border-earth-200/80 shadow-sm">
                        <span class="inline-block px-3 py-1 rounded-full bg-earth-100 text-earth-700 text-xs font-semibold mb-2">Masa Kini & Masa Depan</span>
                        <h3 class="font-serif text-lg font-bold text-earth-900">Melangkah Menuju Impian</h3>
                        <p class="text-sm text-earth-600 mt-2 leading-relaxed">
                            Fokus mengembangkan diri, mengukir karya, dan mempersiapkan masa depan yang cerah dengan penuh rasa syukur dan semangat.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECTION: MINAT & HOBI -->
    <section id="galeri" class="py-16 sm:py-24 bg-white border-t border-earth-200/70">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-14">
                <span class="text-xs font-bold uppercase tracking-widest text-earth-500">Hal yang Saya Sukai</span>
                <h2 class="font-serif text-3xl sm:text-4xl font-bold text-earth-900 mt-2">Minat & Hobi</h2>
                <p class="text-earth-600 mt-3 text-sm sm:text-base">
                    Beberapa aktivitas favorit yang selalu berhasil mengembalikan semangat di waktu luang.
                </p>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Hobi 1 -->
                <div class="group p-6 rounded-3xl bg-earth-50 border border-earth-200/80 hover:bg-earth-800 hover:text-earth-50 transition-all duration-300">
                    <div class="w-12 h-12 rounded-2xl bg-white text-earth-800 flex items-center justify-center mb-5 shadow-sm group-hover:scale-110 transition-transform">
                        <i data-lucide="camera" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-serif text-lg font-bold mb-2">Fotografi Estetik</h3>
                    <p class="text-sm text-earth-600 group-hover:text-earth-200 leading-relaxed">
                        Mengabadikan momen bernuansa hangat, lanskap alam, dan kenangan berharga dalam bingkai foto.
                    </p>
                </div>

                <!-- Hobi 2 -->
                <div class="group p-6 rounded-3xl bg-earth-50 border border-earth-200/80 hover:bg-earth-800 hover:text-earth-50 transition-all duration-300">
                    <div class="w-12 h-12 rounded-2xl bg-white text-earth-800 flex items-center justify-center mb-5 shadow-sm group-hover:scale-110 transition-transform">
                        <i data-lucide="trees" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-serif text-lg font-bold mb-2">Menikmati Alam</h3>
                    <p class="text-sm text-earth-600 group-hover:text-earth-200 leading-relaxed">
                        Mengunjungi tempat-tempat tinggi, menikmati angin sejuk perbukitan dan pemandangan laut dari kejauhan.
                    </p>
                </div>

                <!-- Hobi 3 -->
                <div class="group p-6 rounded-3xl bg-earth-50 border border-earth-200/80 hover:bg-earth-800 hover:text-earth-50 transition-all duration-300">
                    <div class="w-12 h-12 rounded-2xl bg-white text-earth-800 flex items-center justify-center mb-5 shadow-sm group-hover:scale-110 transition-transform">
                        <i data-lucide="music" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-serif text-lg font-bold mb-2">Mendengar Musik</h3>
                    <p class="text-sm text-earth-600 group-hover:text-earth-200 leading-relaxed">
                        Menikmati alunan lagu-lagu lembut yang menenangkan pikiran saat bersantai atau belajar.
                    </p>
                </div>

                <!-- Hobi 4 -->
                <div class="group p-6 rounded-3xl bg-earth-50 border border-earth-200/80 hover:bg-earth-800 hover:text-earth-50 transition-all duration-300">
                    <div class="w-12 h-12 rounded-2xl bg-white text-earth-800 flex items-center justify-center mb-5 shadow-sm group-hover:scale-110 transition-transform">
                        <i data-lucide="coffee" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-serif text-lg font-bold mb-2">Quality Time</h3>
                    <p class="text-sm text-earth-600 group-hover:text-earth-200 leading-relaxed">
                        Berbincang santai bersama keluarga dan sahabat sambil menikmati suasana yang nyaman.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- SECTION: KONTAK & SAPA SAYA -->
    <section id="kontak" class="py-16 sm:py-24 bg-earth-100/60 border-t border-earth-200">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="bg-white rounded-[2.5rem] p-8 sm:p-12 shadow-lg border border-earth-200/80">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-10 items-center">
                    <div>
                        <span class="text-xs font-bold uppercase tracking-widest text-earth-500">Tetap Terhubung</span>
                        <h2 class="font-serif text-3xl font-bold text-earth-900 mt-2">Kirim Pesan Singkat</h2>
                        <p class="text-sm text-earth-600 mt-3 leading-relaxed">
                            Ingin menyapa atau berteman? Jangan ragu untuk meninggalkan pesan hangat di bawah ini.
                        </p>

                        <div class="mt-6 space-y-3">
                            <div class="flex items-center gap-3 text-sm text-earth-700">
                                <div class="w-9 h-9 rounded-full bg-earth-100 flex items-center justify-center text-earth-700">
                                    <i data-lucide="map-pin" class="w-4 h-4"></i>
                                </div>
                                <span>Kotamobagu, Sulawesi Utara, Indonesia</span>
                            </div>
                            <div class="flex items-center gap-3 text-sm text-earth-700">
                                <div class="w-9 h-9 rounded-full bg-earth-100 flex items-center justify-center text-earth-700">
                                    <i data-lucide="calendar" class="w-4 h-4"></i>
                                </div>
                                <span>25 Januari 2007</span>
                            </div>
                        </div>
                    </div>

                    <form id="contact-form" onsubmit="handleContactSubmit(event)" class="space-y-4">
                        <div>
                            <label for="sender-name" class="block text-xs font-semibold text-earth-700 uppercase tracking-wider mb-1.5">Nama Anda</label>
                            <input type="text" id="sender-name" required placeholder="Masukkan nama Anda..." class="w-full px-4 py-3 rounded-xl bg-earth-50 border border-earth-200 text-sm text-earth-900 focus:outline-none focus:ring-2 focus:ring-earth-500">
                        </div>
                        <div>
                            <label for="sender-message" class="block text-xs font-semibold text-earth-700 uppercase tracking-wider mb-1.5">Pesan</label>
                            <textarea id="sender-message" rows="3" required placeholder="Tulis sapaan hangat untuk Neysicha..." class="w-full px-4 py-3 rounded-xl bg-earth-50 border border-earth-200 text-sm text-earth-900 focus:outline-none focus:ring-2 focus:ring-earth-500"></textarea>
                        </div>
                        <button type="submit" class="w-full py-3.5 px-6 rounded-xl bg-earth-800 text-earth-50 font-medium text-sm hover:bg-earth-700 transition-all flex items-center justify-center gap-2 shadow-sm">
                            <span>Kirim Sapaan</span>
                            <i data-lucide="send" class="w-4 h-4"></i>
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-earth-900 text-earth-200 py-10">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row items-center justify-between gap-4 text-center sm:text-left">
            <div>
                <p class="font-serif text-lg font-semibold text-white">Neysicha Cinta Gonibala</p>
                <p class="text-xs text-earth-400 mt-1">Lahir di Kotamobagu, 25 Januari 2007</p>
            </div>
            <p class="text-xs text-earth-400">
                &copy; <span id="current-year">2026</span> Neysicha Cinta Gonibala. Dibuat dengan penuh kehangatan.
            </p>
        </div>
    </footer>

    <!-- JAVASCRIPT -->
    <script>
        // Inisialisasi Lucide Icons
        lucide.createIcons();

        // Set Tahun Saat Ini & Hitung Usia Otomatis berdasarkan 25 Januari 2007
        document.addEventListener('DOMContentLoaded', () => {
            const now = new Date();
            document.getElementById('current-year').textContent = now.getFullYear();

            const birthDate = new Date(2007, 0, 25); // 25 Januari 2007
            let age = now.getFullYear() - birthDate.getFullYear();
            const monthDiff = now.getMonth() - birthDate.getMonth();
            if (monthDiff < 0 || (monthDiff === 0 && now.getDate() < birthDate.getDate())) {
                age--;
            }
            document.getElementById('umur-display').textContent = `${age} Tahun`;

            // Cek apakah ada foto yang tersimpan sebelumnya di localStorage
            try {
                const savedPhoto = localStorage.getItem('neysicha_profile_photo');
                if (savedPhoto) {
                    document.getElementById('profile-photo').src = savedPhoto;
                }
            } catch (e) {
                console.warn('Local storage tidak tersedia:', e);
            }
        });

        // Toggle Menu Mobile
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Tutup menu mobile saat link diklik
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // Fungsi Fallback Jika File Gambar Lokal Belum Terhubung di Lingkungan Preview
        function handleImageFallback(imgElement) {
            imgElement.onerror = null;
            // Placeholder estetik bernuansa earth-tone
            imgElement.src = "https://placehold.co/600x750/D1C3B2/46382E?text=Neysicha+Cinta+Gonibala%0A(Klik+untuk+Memuat+Foto)";
            const helperBadge = document.getElementById('photo-helper-badge');
            if (helperBadge) {
                helperBadge.classList.remove('hidden');
            }
        }

        // Fungsi Pratinjau Foto Saat Pengguna Memilih File Gambar
        function previewProfilePhoto(event) {
            const file = event.target.files[0];
            if (!file) return;

            const reader = new FileReader();
            reader.onload = function(e) {
                const imgElement = document.getElementById('profile-photo');
                imgElement.src = e.target.result;
                
                // Sembunyikan tombol helper jika sudah diganti
                const helperBadge = document.getElementById('photo-helper-badge');
                if (helperBadge) {
                    helperBadge.classList.add('hidden');
                }

                // Simpan sementara agar tidak hilang saat refresh
                try {
                    localStorage.setItem('neysicha_profile_photo', e.target.result);
                } catch (err) {
                    console.warn('Ukuran gambar terlalu besar untuk disimpan di cache browser.');
                }

                showToast('Foto profil berhasil ditampilkan!');
            };
            reader.readAsDataURL(file);
        }

        // Fungsi Kirim Form Kontak
        function handleContactSubmit(event) {
            event.preventDefault();
            const nameInput = document.getElementById('sender-name');
            const messageInput = document.getElementById('sender-message');
            
            showToast(`Terima kasih ${nameInput.value}, pesan Anda telah terkirim!`);
            nameInput.value = '';
            messageInput.value = '';
        }

        // Fungsi Toast Notification (Pengganti alert)
        function showToast(message) {
            const toast = document.getElementById('toast');
            const toastMsg = document.getElementById('toast-message');
            toastMsg.textContent = message;

            toast.classList.remove('translate-y-20', 'opacity-0');
            toast.classList.add('translate-y-0', 'opacity-100');

            setTimeout(() => {
                toast.classList.remove('translate-y-0', 'opacity-100');
                toast.classList.add('translate-y-20', 'opacity-0');
            }, 3500);
        }
    </script>
</body>
</html>                                        
