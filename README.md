<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Portofolio Modern</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        primary: '#3b82f6', // blue-500
                        secondary: '#1e293b', // slate-800
                        dark: '#0f172a', // slate-900
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom Animations */
        .fade-in-up {
            animation: fadeInUp 0.8s ease-out forwards;
            opacity: 0;
            transform: translateY(20px);
        }
        
        .delay-100 { animation-delay: 100ms; }
        .delay-200 { animation-delay: 200ms; }
        .delay-300 { animation-delay: 300ms; }

        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Gradient Text */
        .text-gradient {
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-image: linear-gradient(to right, #3b82f6, #8b5cf6);
        }
    </style>
</head>
<body class="bg-dark text-slate-300 font-sans antialiased selection:bg-primary selection:text-white">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 top-0 transition-all duration-300 backdrop-blur-md bg-dark/80 border-b border-slate-800" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logo -->
                <div class="flex-shrink-0 flex items-center">
                    <a href="#" class="text-2xl font-bold text-white tracking-tighter">
                        Dev<span class="text-primary">Folio.</span>
                    </a>
                </div>
                
                <!-- Desktop Menu -->
                <div class="hidden md:flex space-x-8 items-center">
                    <a href="#beranda" class="text-sm font-medium hover:text-primary transition-colors text-white">Beranda</a>
                    <a href="#tentang" class="text-sm font-medium hover:text-primary transition-colors">Tentang</a>
                    <a href="#portofolio" class="text-sm font-medium hover:text-primary transition-colors">Portofolio</a>
                    <a href="#kontak" class="text-sm font-medium hover:text-primary transition-colors">Kontak</a>
                    <a href="#kontak" class="px-5 py-2.5 bg-primary text-white text-sm font-medium rounded-lg hover:bg-blue-600 transition-all shadow-lg shadow-blue-500/30">Mulai Proyek</a>
                </div>

                <!-- Mobile Menu Button -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-btn" class="text-slate-300 hover:text-white focus:outline-none p-2">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu Panel -->
        <div id="mobile-menu" class="hidden md:hidden bg-secondary border-b border-slate-800">
            <div class="px-4 pt-2 pb-6 space-y-2 shadow-xl">
                <a href="#beranda" class="block px-3 py-2 rounded-md text-base font-medium text-white hover:bg-slate-700 hover:text-primary transition-colors">Beranda</a>
                <a href="#tentang" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-slate-700 hover:text-primary transition-colors">Tentang</a>
                <a href="#portofolio" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-slate-700 hover:text-primary transition-colors">Portofolio</a>
                <a href="#kontak" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-slate-700 hover:text-primary transition-colors">Kontak</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="beranda" class="relative pt-32 pb-20 lg:pt-48 lg:pb-32 overflow-hidden flex items-center min-h-screen">
        <!-- Background decoration -->
        <div class="absolute top-1/4 left-1/4 w-96 h-96 bg-primary/20 rounded-full mix-blend-multiply filter blur-3xl opacity-50 animate-blob"></div>
        <div class="absolute top-1/3 right-1/4 w-96 h-96 bg-purple-500/20 rounded-full mix-blend-multiply filter blur-3xl opacity-50 animate-blob animation-delay-2000"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 w-full">
            <div class="text-center max-w-3xl mx-auto">
                <span class="text-primary font-semibold tracking-wider uppercase text-sm mb-4 block fade-in-up">Selamat Datang</span>
                <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold text-white tracking-tight mb-6 fade-in-up delay-100 leading-tight">
                    Membangun Pengalaman Digital yang <span class="text-gradient">Luar Biasa</span>
                </h1>
                <p class="text-lg sm:text-xl text-slate-400 mb-10 fade-in-up delay-200 leading-relaxed">
                    Saya seorang Web Developer dan Desainer UI/UX yang bersemangat menciptakan website interaktif, responsif, dan mudah digunakan untuk membantu bisnis Anda berkembang.
                </p>
                <div class="flex flex-col sm:flex-row justify-center gap-4 fade-in-up delay-300">
                    <a href="#portofolio" class="px-8 py-4 bg-primary text-white font-medium rounded-xl hover:bg-blue-600 transition-all shadow-lg shadow-blue-500/30 flex items-center justify-center gap-2">
                        Lihat Karya Saya <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    <a href="#kontak" class="px-8 py-4 bg-transparent border border-slate-700 text-white font-medium rounded-xl hover:bg-slate-800 transition-all flex items-center justify-center">
                        Hubungi Saya
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="tentang" class="py-20 bg-secondary/30">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <!-- Image -->
                <div class="relative group rounded-2xl overflow-hidden shadow-2xl">
                    <div class="absolute inset-0 bg-primary/20 group-hover:bg-transparent transition-colors duration-500 z-10"></div>
                    <img src="https://placehold.co/800x800/1e293b/3b82f6?text=Foto+Profil" alt="Foto Profil" class="w-full h-auto object-cover transform group-hover:scale-105 transition-transform duration-700">
                </div>
                
                <!-- Text -->
                <div>
                    <h2 class="text-3xl sm:text-4xl font-bold text-white mb-6">Tentang <span class="text-gradient">Saya</span></h2>
                    <p class="text-slate-400 mb-6 leading-relaxed">
                        Halo! Saya seorang pengembang web berbasis di Indonesia dengan pengalaman lebih dari 3 tahun dalam merancang dan membangun aplikasi web. Saya memiliki ketertarikan mendalam pada teknologi front-end dan arsitektur desain yang bersih.
                    </p>
                    <p class="text-slate-400 mb-8 leading-relaxed">
                        Misi saya adalah mengubah ide-ide kompleks menjadi antarmuka yang sederhana, elegan, dan intuitif. Ketika tidak sedang ngoding, saya biasanya membaca artikel teknologi atau bermain game strategi.
                    </p>
                    
                    <!-- Skills -->
                    <h3 class="text-xl font-semibold text-white mb-4">Keahlian Utama</h3>
                    <div class="flex flex-wrap gap-3">
                        <span class="px-4 py-2 bg-slate-800 text-sm font-medium rounded-lg border border-slate-700 text-blue-400"><i class="fa-brands fa-html5 mr-2"></i>HTML5</span>
                        <span class="px-4 py-2 bg-slate-800 text-sm font-medium rounded-lg border border-slate-700 text-blue-400"><i class="fa-brands fa-css3-alt mr-2"></i>CSS3 / Tailwind</span>
                        <span class="px-4 py-2 bg-slate-800 text-sm font-medium rounded-lg border border-slate-700 text-yellow-400"><i class="fa-brands fa-js mr-2"></i>JavaScript</span>
                        <span class="px-4 py-2 bg-slate-800 text-sm font-medium rounded-lg border border-slate-700 text-cyan-400"><i class="fa-brands fa-react mr-2"></i>React</span>
                        <span class="px-4 py-2 bg-slate-800 text-sm font-medium rounded-lg border border-slate-700 text-green-400"><i class="fa-brands fa-node-js mr-2"></i>Node.js</span>
                        <span class="px-4 py-2 bg-slate-800 text-sm font-medium rounded-lg border border-slate-700 text-white"><i class="fa-brands fa-figma mr-2"></i>Figma</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portofolio" class="py-24">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold text-white mb-4">Karya <span class="text-gradient">Terbaru</span></h2>
                <p class="text-slate-400 max-w-2xl mx-auto">Beberapa proyek pilihan yang telah saya kerjakan. Dari website perusahaan hingga aplikasi web yang kompleks.</p>
            </div>

            <!-- Portfolio Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- Project 1 -->
                <div class="bg-secondary/50 rounded-2xl overflow-hidden border border-slate-800 hover:border-slate-600 transition-colors group">
                    <div class="overflow-hidden">
                        <img src="https://placehold.co/600x400/0f172a/3b82f6?text=Proyek+E-Commerce" alt="Proyek 1" class="w-full h-48 object-cover transform group-hover:scale-110 transition-transform duration-500">
                    </div>
                    <div class="p-6">
                        <div class="flex gap-2 mb-3">
                            <span class="text-xs font-semibold text-primary bg-primary/10 px-2 py-1 rounded">React</span>
                            <span class="text-xs font-semibold text-purple-400 bg-purple-400/10 px-2 py-1 rounded">Tailwind</span>
                        </div>
                        <h3 class="text-xl font-bold text-white mb-2 group-hover:text-primary transition-colors">Platform E-Commerce</h3>
                        <p class="text-slate-400 text-sm mb-4 line-clamp-2">Aplikasi toko online lengkap dengan keranjang belanja, integrasi pembayaran, dan dashboard admin.</p>
                        <a href="#" class="text-sm font-medium text-white hover:text-primary transition-colors inline-flex items-center gap-1">Lihat Detail <i class="fa-solid fa-arrow-right text-xs"></i></a>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="bg-secondary/50 rounded-2xl overflow-hidden border border-slate-800 hover:border-slate-600 transition-colors group">
                    <div class="overflow-hidden">
                        <img src="https://placehold.co/600x400/0f172a/10b981?text=Aplikasi+Manajemen" alt="Proyek 2" class="w-full h-48 object-cover transform group-hover:scale-110 transition-transform duration-500">
                    </div>
                    <div class="p-6">
                        <div class="flex gap-2 mb-3">
                            <span class="text-xs font-semibold text-emerald-400 bg-emerald-400/10 px-2 py-1 rounded">Vue.js</span>
                            <span class="text-xs font-semibold text-blue-400 bg-blue-400/10 px-2 py-1 rounded">Firebase</span>
                        </div>
                        <h3 class="text-xl font-bold text-white mb-2 group-hover:text-primary transition-colors">Sistem Manajemen Tugas</h3>
                        <p class="text-slate-400 text-sm mb-4 line-clamp-2">Aplikasi produktivitas untuk tim melacak proyek, memberikan tugas, dan berkolaborasi secara real-time.</p>
                        <a href="#" class="text-sm font-medium text-white hover:text-primary transition-colors inline-flex items-center gap-1">Lihat Detail <i class="fa-solid fa-arrow-right text-xs"></i></a>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="bg-secondary/50 rounded-2xl overflow-hidden border border-slate-800 hover:border-slate-600 transition-colors group">
                    <div class="overflow-hidden">
                        <img src="https://placehold.co/600x400/0f172a/f59e0b?text=Website+Perusahaan" alt="Proyek 3" class="w-full h-48 object-cover transform group-hover:scale-110 transition-transform duration-500">
                    </div>
                    <div class="p-6">
                        <div class="flex gap-2 mb-3">
                            <span class="text-xs font-semibold text-orange-400 bg-orange-400/10 px-2 py-1 rounded">HTML/CSS</span>
                            <span class="text-xs font-semibold text-yellow-400 bg-yellow-400/10 px-2 py-1 rounded">JavaScript</span>
                        </div>
                        <h3 class="text-xl font-bold text-white mb-2 group-hover:text-primary transition-colors">Company Profile Startup</h3>
                        <p class="text-slate-400 text-sm mb-4 line-clamp-2">Desain ulang website perusahaan rintisan teknologi dengan fokus pada SEO dan performa yang sangat cepat.</p>
                        <a href="#" class="text-sm font-medium text-white hover:text-primary transition-colors inline-flex items-center gap-1">Lihat Detail <i class="fa-solid fa-arrow-right text-xs"></i></a>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="kontak" class="py-24 bg-secondary/30">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="max-w-4xl mx-auto">
                <div class="text-center mb-16">
                    <h2 class="text-3xl sm:text-4xl font-bold text-white mb-4">Mari <span class="text-gradient">Bekerjasama</span></h2>
                    <p class="text-slate-400">Punya proyek menarik atau sekadar ingin menyapa? Jangan ragu untuk menghubungi saya.</p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-5 gap-12">
                    <!-- Contact Info -->
                    <div class="md:col-span-2 space-y-8">
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 bg-primary/10 rounded-xl flex items-center justify-center text-primary text-xl flex-shrink-0">
                                <i class="fa-solid fa-envelope"></i>
                            </div>
                            <div>
                                <h4 class="text-white font-semibold mb-1">Email</h4>
                                <a href="mailto:halo@email.com" class="text-slate-400 hover:text-primary transition-colors">halo@email.com</a>
                            </div>
                        </div>
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 bg-primary/10 rounded-xl flex items-center justify-center text-primary text-xl flex-shrink-0">
                                <i class="fa-solid fa-phone"></i>
                            </div>
                            <div>
                                <h4 class="text-white font-semibold mb-1">Telepon</h4>
                                <a href="tel:+628123456789" class="text-slate-400 hover:text-primary transition-colors">+62 812 3456 7890</a>
                            </div>
                        </div>
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 bg-primary/10 rounded-xl flex items-center justify-center text-primary text-xl flex-shrink-0">
                                <i class="fa-solid fa-location-dot"></i>
                            </div>
                            <div>
                                <h4 class="text-white font-semibold mb-1">Lokasi</h4>
                                <p class="text-slate-400">Jakarta, Indonesia</p>
                            </div>
                        </div>
                    </div>

                    <!-- Contact Form -->
                    <div class="md:col-span-3 bg-dark p-8 rounded-2xl border border-slate-800">
                        <form onsubmit="event.preventDefault(); showMessage();">
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-6 mb-6">
                                <div>
                                    <label for="name" class="block text-sm font-medium text-slate-400 mb-2">Nama Lengkap</label>
                                    <input type="text" id="name" class="w-full bg-secondary border border-slate-700 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-primary focus:ring-1 focus:ring-primary transition-colors" placeholder="John Doe" required>
                                </div>
                                <div>
                                    <label for="email" class="block text-sm font-medium text-slate-400 mb-2">Email</label>
                                    <input type="email" id="email" class="w-full bg-secondary border border-slate-700 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-primary focus:ring-1 focus:ring-primary transition-colors" placeholder="john@example.com" required>
                                </div>
                            </div>
                            <div class="mb-6">
                                <label for="message" class="block text-sm font-medium text-slate-400 mb-2">Pesan</label>
                                <textarea id="message" rows="4" class="w-full bg-secondary border border-slate-700 rounded-lg px-4 py-3 text-white focus:outline-none focus:border-primary focus:ring-1 focus:ring-primary transition-colors resize-none" placeholder="Tuliskan pesan Anda di sini..." required></textarea>
                            </div>
                            <button type="submit" class="w-full bg-primary text-white font-medium py-3 rounded-lg hover:bg-blue-600 transition-all shadow-lg shadow-blue-500/30">Kirim Pesan</button>
                            
                            <!-- Success Message Placeholder -->
                            <div id="form-message" class="hidden mt-4 p-3 bg-green-500/10 border border-green-500/20 text-green-400 rounded-lg text-sm text-center">
                                Pesan Anda telah terkirim! Terima kasih.
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark border-t border-slate-800 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row justify-between items-center gap-6">
            <div class="text-2xl font-bold text-white tracking-tighter">
                Dev<span class="text-primary">Folio.</span>
            </div>
            
            <p class="text-slate-500 text-sm text-center md:text-left">
                &copy; 2026 DevFolio. Dibuat dengan <i class="fa-solid fa-heart text-red-500 mx-1"></i> di Indonesia.
            </p>

            <div class="flex gap-4">
                <a href="#" class="w-10 h-10 bg-secondary rounded-full flex items-center justify-center text-slate-400 hover:text-white hover:bg-primary transition-all">
                    <i class="fa-brands fa-github"></i>
                </a>
                <a href="#" class="w-10 h-10 bg-secondary rounded-full flex items-center justify-center text-slate-400 hover:text-white hover:bg-primary transition-all">
                    <i class="fa-brands fa-linkedin-in"></i>
                </a>
                <a href="#" class="w-10 h-10 bg-secondary rounded-full flex items-center justify-center text-slate-400 hover:text-white hover:bg-primary transition-all">
                    <i class="fa-brands fa-instagram"></i>
                </a>
                <a href="#" class="w-10 h-10 bg-secondary rounded-full flex items-center justify-center text-slate-400 hover:text-white hover:bg-primary transition-all">
                    <i class="fa-brands fa-twitter"></i>
                </a>
            </div>
        </div>
    </footer>

    <!-- JavaScript for Interactivity -->
    <script>
        // Mobile Menu Toggle
        const btn = document.getElementById('mobile-menu-btn');
        const menu = document.getElementById('mobile-menu');
        const icon = btn.querySelector('i');

        btn.addEventListener('click', () => {
            menu.classList.toggle('hidden');
            if(menu.classList.contains('hidden')) {
                icon.classList.remove('fa-xmark');
                icon.classList.add('fa-bars');
            } else {
                icon.classList.remove('fa-bars');
                icon.classList.add('fa-xmark');
            }
        });

        // Close mobile menu when a link is clicked
        const mobileLinks = menu.querySelectorAll('a');
        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                menu.classList.add('hidden');
                icon.classList.remove('fa-xmark');
                icon.classList.add('fa-bars');
            });
        });

        // Add shadow to navbar on scroll
        const navbar = document.getElementById('navbar');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 20) {
                navbar.classList.add('shadow-lg');
            } else {
                navbar.classList.remove('shadow-lg');
            }
        });

        // Fake form submission handler
        function showMessage() {
            const msg = document.getElementById('form-message');
            msg.classList.remove('hidden');
            setTimeout(() => {
                msg.classList.add('hidden');
                document.querySelector('form').reset();
            }, 3000);
        }
    </script>
</body>
</html>
