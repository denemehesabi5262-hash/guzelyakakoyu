<!DOCTYPE html>
<html lang="tr" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Güzelyaka Köyü Muhtarlığı | Çaycuma, Zonguldak</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome İkonlar -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts (Inter) -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        emerald: {
                            50: '#ecfdf5',
                            100: '#d1fae5',
                            600: '#059669',
                            700: '#047857',
                            800: '#065f46',
                            900: '#064e3b',
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    
    <style>
        .glass {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }
        .dark .glass {
            background: rgba(6, 78, 59, 0.9);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f5f9;
        }
        ::-webkit-scrollbar-thumb {
            background: #059669;
            border-radius: 4px;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 dark:bg-slate-900 dark:text-slate-100 font-sans antialiased selection:bg-emerald-600 selection:text-white">

    <!-- Üst Duyuru Çubuğu (Top Header) -->
    <div class="bg-emerald-900 text-emerald-100 text-xs sm:text-sm py-2 px-4">
        <div class="max-w-7xl mx-auto flex flex-col sm:flex-row justify-between items-center gap-2">
            <div class="flex items-center gap-4">
                <span><i class="fa-solid fa-location-dot text-emerald-400 mr-1"></i> Güzelyaka Köyü, Çaycuma / Zonguldak</span>
                <span class="hidden md:inline">|</span>
                <span class="hidden md:inline"><i class="fa-solid fa-user-tie text-emerald-400 mr-1"></i> Muhtar: Mürteza Oruç</span>
            </div>
            <div class="flex items-center gap-4">
                <a href="tel:+905326606372" class="hover:text-white transition-colors flex items-center gap-1 font-semibold">
                    <i class="fa-solid fa-phone text-emerald-400"></i> +90 532 660 63 72
                </a>
            </div>
        </div>
    </div>

    <!-- Üst Navigasyon Çubuğu (Header) -->
    <header class="sticky top-0 z-50 glass border-b border-emerald-100 dark:border-emerald-900/50 shadow-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <!-- Logo & Başlık -->
            <a href="#hero" class="flex items-center gap-3">
                <div class="w-11 h-11 rounded-xl bg-emerald-700 text-white flex items-center justify-center text-xl shadow-md shadow-emerald-700/20">
                    <i class="fa-solid fa-building-columns"></i>
                </div>
                <div>
                    <span class="text-lg sm:text-xl font-extrabold tracking-tight block text-emerald-950 dark:text-emerald-100 leading-tight">Güzelyaka Köyü</span>
                    <span class="text-xs font-semibold uppercase tracking-wider text-emerald-600 dark:text-emerald-400">T.C. Muhtarlığı</span>
                </div>
            </a>

            <!-- Masaüstü Menü -->
            <nav class="hidden md:flex items-center space-x-8 font-medium text-sm">
                <a href="#hero" class="hover:text-emerald-600 dark:hover:text-emerald-400 transition-colors">Ana Sayfa</a>
                <a href="#muhtar" class="hover:text-emerald-600 dark:hover:text-emerald-400 transition-colors">Muhtarımızın Mesajı</a>
                <a href="#services" class="hover:text-emerald-600 dark:hover:text-emerald-400 transition-colors">Hizmetler</a>
                <a href="#about-village" class="hover:text-emerald-600 dark:hover:text-emerald-400 transition-colors">Köyümüz</a>
                <a href="#contact" class="hover:text-emerald-600 dark:hover:text-emerald-400 transition-colors">İletişim</a>
            </nav>

            <!-- Hızlı Arama Butonu -->
            <div class="hidden sm:flex items-center space-x-3">
                <a href="tel:+905326606372" class="px-4 py-2.5 bg-emerald-600 hover:bg-emerald-700 text-white rounded-xl font-semibold text-sm shadow-md shadow-emerald-600/20 transition-all flex items-center gap-2">
                    <i class="fa-solid fa-phone"></i> Muhtarı Ara
                </a>
            </div>

            <!-- Mobil Menü Butonu -->
            <button id="mobile-menu-btn" aria-label="Menüyü Aç" class="md:hidden p-2 rounded-lg bg-emerald-50 text-emerald-800 dark:bg-emerald-900 dark:text-emerald-100 focus:outline-none">
                <i class="fa-solid fa-bars text-xl"></i>
            </button>
        </div>

        <!-- Mobil Menü -->
        <div id="mobile-menu" class="hidden md:hidden border-t border-emerald-100 dark:border-emerald-900 bg-white dark:bg-slate-900 px-4 pt-3 pb-6 space-y-3 shadow-xl">
            <a href="#hero" class="block px-4 py-2.5 rounded-xl font-medium hover:bg-emerald-50 dark:hover:bg-emerald-950">Ana Sayfa</a>
            <a href="#muhtar" class="block px-4 py-2.5 rounded-xl font-medium hover:bg-emerald-50 dark:hover:bg-emerald-950">Muhtarımızın Mesajı</a>
            <a href="#services" class="block px-4 py-2.5 rounded-xl font-medium hover:bg-emerald-50 dark:hover:bg-emerald-950">Hizmetlerimiz</a>
            <a href="#about-village" class="block px-4 py-2.5 rounded-xl font-medium hover:bg-emerald-50 dark:hover:bg-emerald-950">Köyümüz</a>
            <a href="#contact" class="block px-4 py-2.5 rounded-xl font-medium hover:bg-emerald-50 dark:hover:bg-emerald-950">İletişim</a>
            <a href="tel:+905326606372" class="block w-full text-center px-4 py-3 bg-emerald-600 text-white font-semibold rounded-xl mt-2">
                <i class="fa-solid fa-phone mr-1"></i> +90 532 660 63 72
            </a>
        </div>
    </header>

    <!-- Hero / Karşılama Bölümü -->
    <section id="hero" class="relative bg-gradient-to-b from-emerald-900 via-emerald-800 to-slate-900 text-white py-24 lg:py-32 overflow-hidden">
        <div class="absolute inset-0 opacity-20 bg-[url('https://images.unsplash.com/photo-1500382017468-9049fed747ef?auto=format&fit=crop&w=1600&q=80')] bg-cover bg-center"></div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 text-center">
            <span class="inline-block px-4 py-1.5 rounded-full bg-emerald-500/20 border border-emerald-400/30 text-emerald-200 text-sm font-semibold mb-6">
                T.C. Zonguldak / Çaycuma
            </span>
            <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight mb-6 leading-tight">
                Güzelyaka Köyü Muhtarlığı <br/> Resmî Web Sitesi
            </h1>
            <p class="text-lg sm:text-xl text-emerald-100 max-w-2xl mx-auto mb-10 font-light">
                Köyümüzle ilgili muhtarlık hizmetlerinden faydalanabilir ve muhtarımız ile iletişime geçebilirsiniz.
            </p>
            
            <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
                <a href="tel:+905326606372" class="w-full sm:w-auto px-8 py-4 bg-emerald-500 hover:bg-emerald-400 text-emerald-950 font-bold rounded-xl shadow-lg shadow-emerald-500/30 transition-all flex items-center justify-center gap-2">
                    <i class="fa-solid fa-phone text-lg"></i> Muhtarı Ara (+90 532 660 63 72)
                </a>
                <a href="https://wa.me/905326606372" target="_blank" class="w-full sm:w-auto px-8 py-4 bg-emerald-950/80 hover:bg-emerald-900 border border-emerald-600/50 text-white font-semibold rounded-xl transition-all flex items-center justify-center gap-2">
                    <i class="fa-brands fa-whatsapp text-emerald-400 text-xl"></i> WhatsApp Hattı
                </a>
            </div>

            <!-- Muhtar Kartı Rozeti -->
            <div class="mt-12 inline-flex items-center gap-4 p-3 pr-6 rounded-2xl bg-white/10 backdrop-blur-md border border-white/10 text-left">
                <div class="w-12 h-12 rounded-xl bg-emerald-600 flex items-center justify-center text-xl font-bold text-white shadow-inner">
                    <i class="fa-solid fa-user-tie"></i>
                </div>
                <div>
                    <h3 class="font-bold text-white text-sm sm:text-base">Mürteza Oruç</h3>
                    <p class="text-xs text-emerald-200">Güzelyaka Köyü Muhtarı</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Muhtarımızın Mesajı -->
    <section id="muhtar" class="py-20 bg-white dark:bg-slate-900">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid lg:grid-cols-12 gap-12 items-center">
                <div class="lg:col-span-5">
                    <div class="relative">
                        <div class="absolute -inset-4 bg-emerald-600/10 rounded-3xl transform -rotate-2"></div>
                        <div class="relative bg-emerald-800 rounded-2xl overflow-hidden shadow-xl text-white p-8 text-center">
                            <div class="w-28 h-28 mx-auto rounded-full bg-emerald-700 border-4 border-emerald-500 flex items-center justify-center text-5xl mb-4 text-emerald-200 shadow-md">
                                <i class="fa-solid fa-user-tie"></i>
                            </div>
                            <h3 class="text-2xl font-bold">Mürteza Oruç</h3>
                            <p class="text-emerald-300 font-medium text-sm mt-1">Güzelyaka Köyü Muhtarı</p>
                            <div class="mt-6 pt-6 border-t border-emerald-700/60 flex flex-col gap-3 text-sm">
                                <a href="tel:+905326606372" class="text-emerald-200 hover:text-white flex items-center justify-center gap-2">
                                    <i class="fa-solid fa-phone text-emerald-400"></i> +90 532 660 63 72
                                </a>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="lg:col-span-7 space-y-6">
                    <div class="inline-flex items-center gap-2 text-emerald-700 dark:text-emerald-400 font-bold text-sm uppercase tracking-wider">
                        <i class="fa-solid fa-quote-left"></i> Muhtarımızın Mesajı
                    </div>
                    <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 dark:text-white leading-tight">
                        Köyümüze Hizmet Etmekten Onur Duyuyoruz
                    </h2>
                    <p class="text-slate-600 dark:text-slate-300 leading-relaxed">
                        Değerli Güzelyaka Köyü sakinleri ve kıymetli hemşehrilerim, <br/><br/>
                        Güzelyaka Köyümüzün huzuru, gelişimi ve refahı için muhtarlık ekibimizle birlikte gece gündüz demeden çalışıyoruz. Altyapı çalışmalarından çevre düzenlemelerine, resmi evrak işlemlerinden komşularımızın ihtiyaçlarına kadar her konuda sizlerin hizmetindeyiz.
                    </p>
                    <p class="text-slate-600 dark:text-slate-300 leading-relaxed">
                        Köyümüzle ilgili her türlü talep, öneri ve ihtiyacınızda bana doğrudan telefon numaramdan ulaşabilirsiniz. Birlik ve beraberlik içinde köyümüzü daha güzel yarınlara taşıyacağız.
                    </p>
                    <div class="pt-4 border-t border-slate-100 dark:border-slate-800 flex items-center justify-between">
                        <div>
                            <p class="font-bold text-slate-900 dark:text-white">Mürteza Oruç</p>
                            <p class="text-xs text-slate-500">Güzelyaka Köyü Muhtarı</p>
                        </div>
                        <a href="tel:+905326606372" class="px-5 py-2.5 bg-emerald-50 dark:bg-emerald-950 text-emerald-700 dark:text-emerald-300 rounded-xl font-semibold text-sm hover:bg-emerald-100 transition-colors">
                            Bana Ulaşın
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Muhtarlık Hizmetleri -->
    <section id="services" class="py-20 bg-slate-100/80 dark:bg-slate-800/50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-emerald-700 dark:text-emerald-400 font-bold text-sm uppercase tracking-wider">Kurumsal</span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 dark:text-white mt-1 mb-4">Muhtarlık Hizmetleri</h2>
                <div class="w-16 h-1 bg-emerald-600 mx-auto rounded-full mb-4"></div>
                <p class="text-slate-600 dark:text-slate-400">
                    Köy muhtarlığımız tarafından vatandaşlarımıza sunulan resmi belge ve danışmanlık hizmetleri.
                </p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Hizmet 1 -->
                <div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200 dark:border-slate-800 shadow-sm hover:shadow-md transition-shadow">
                    <div class="w-14 h-14 bg-emerald-100 dark:bg-emerald-900/50 text-emerald-700 dark:text-emerald-400 rounded-xl flex items-center justify-center text-2xl mb-6">
                        <i class="fa-solid fa-file-signature"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">İkametgah & Evrak İşlemleri</h3>
                    <p class="text-slate-600 dark:text-slate-400 text-sm leading-relaxed">
                        Yerleşim yeri belgesi, nakil bildirimleri ve muhtarlık onaylı resmi evrak düzenleme hizmetleri.
                    </p>
                </div>

                <!-- Hizmet 2 -->
                <div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200 dark:border-slate-800 shadow-sm hover:shadow-md transition-shadow">
                    <div class="w-14 h-14 bg-emerald-100 dark:bg-emerald-900/50 text-emerald-700 dark:text-emerald-400 rounded-xl flex items-center justify-center text-2xl mb-6">
                        <i class="fa-solid fa-tractor"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Arazi & Tarım Destekleri</h3>
                    <p class="text-slate-600 dark:text-slate-400 text-sm leading-relaxed">
                        ÇKS (Çiftçi Kayıt Sistemi) onayları, tarımsal destek bildirimleri ve arazi beyan rehberliği.
                    </p>
                </div>

                <!-- Hizmet 3 -->
                <div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200 dark:border-slate-800 shadow-sm hover:shadow-md transition-shadow">
                    <div class="w-14 h-14 bg-emerald-100 dark:bg-emerald-900/50 text-emerald-700 dark:text-emerald-400 rounded-xl flex items-center justify-center text-2xl mb-6">
                        <i class="fa-solid fa-hand-holding-heart"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Sosyal Yardım Başvuruları</h3>
                    <p class="text-slate-600 dark:text-slate-400 text-sm leading-relaxed">
                        İhtiyaç sahibi köylülerimizin kaymakamlık ve valilik sosyal yardımlarına yönlendirilmesi ve takibi.
                    </p>
                </div>

                <!-- Hizmet 4 -->
                <div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200 dark:border-slate-800 shadow-sm hover:shadow-md transition-shadow">
                    <div class="w-14 h-14 bg-emerald-100 dark:bg-emerald-900/50 text-emerald-700 dark:text-emerald-400 rounded-xl flex items-center justify-center text-2xl mb-6">
                        <i class="fa-solid fa-road"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Köy Altyapı & Çevre İşleri</h3>
                    <p class="text-slate-600 dark:text-slate-400 text-sm leading-relaxed">
                        Yol bakımı, su hatları, elektrik arızaları ve çevre temizliği taleplerinin resmi kurumlara iletilmesi.
                    </p>
                </div>

                <!-- Hizmet 5 -->
                <div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200 dark:border-slate-800 shadow-sm hover:shadow-md transition-shadow">
                    <div class="w-14 h-14 bg-emerald-100 dark:bg-emerald-900/50 text-emerald-700 dark:text-emerald-400 rounded-xl flex items-center justify-center text-2xl mb-6">
                        <i class="fa-solid fa-comments"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Dilekçe & Talep İletimi</h3>
                    <p class="text-slate-600 dark:text-slate-400 text-sm leading-relaxed">
                        Çaycuma Belediyesi ve Kaymakamlığına iletilmek istenen resmi talep ve dilekçelerin hazırlanması.
                    </p>
                </div>

                <!-- Hizmet 6 -->
                <div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200 dark:border-slate-800 shadow-sm hover:shadow-md transition-shadow">
                    <div class="w-14 h-14 bg-emerald-100 dark:bg-emerald-900/50 text-emerald-700 dark:text-emerald-400 rounded-xl flex items-center justify-center text-2xl mb-6">
                        <i class="fa-solid fa-bullhorn"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Resmi İlan & Bilgilendirme</h3>
                    <p class="text-slate-600 dark:text-slate-400 text-sm leading-relaxed">
                        Aşı takvimleri, elektrik/su kesintileri, kamu bilgilendirmeleri ve köy içi süreçlerin takibi.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Köyümüz Hakkında / Galeri -->
    <section id="about-village" class="py-20 bg-white dark:bg-slate-900">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid lg:grid-cols-2 gap-12 items-center">
                <div class="space-y-6">
                    <span class="text-emerald-700 dark:text-emerald-400 font-bold text-sm uppercase tracking-wider">Yeşil ve Huzurlu</span>
                    <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 dark:text-white">Güzelyaka Köyü'nü Tanıyın</h2>
                    <p class="text-slate-600 dark:text-slate-300 leading-relaxed">
                        Zonguldak ilinin Çaycuma ilçesine bağlı olan Güzelyaka Köyü, eşsiz doğası, temiz havası ve sıcakkanlı insanlarıyla Batı Karadeniz'in şirin yerleşim yerlerinden biridir. 
                    </p>
                    <p class="text-slate-600 dark:text-slate-300 leading-relaxed">
                        Tarım ve hayvancılığın yanı sıra geleneksel Karadeniz kültürünün yaşatıldığı köyümüz, yeşil ormanları ve huzurlu atmosferi ile hem yerlilerine hem de ziyaretçilerine eşsiz bir yaşam alanı sunmaktadır.
                    </p>

                    <div class="grid grid-cols-2 gap-4 pt-2">
                        <div class="p-4 bg-slate-50 dark:bg-slate-800 rounded-xl border border-slate-200 dark:border-slate-700">
                            <h4 class="text-2xl font-bold text-emerald-700 dark:text-emerald-400">Çaycuma</h4>
                            <p class="text-xs text-slate-500 mt-1">Bağlı Olduğu İlçe</p>
                        </div>
                        <div class="p-4 bg-slate-50 dark:bg-slate-800 rounded-xl border border-slate-200 dark:border-slate-700">
                            <h4 class="text-2xl font-bold text-emerald-700 dark:text-emerald-400">Zonguldak</h4>
                            <p class="text-xs text-slate-500 mt-1">Bağlı Olduğu İl</p>
                        </div>
                    </div>
                </div>

                <!-- Görsel Galerisi -->
                <div class="grid grid-cols-2 gap-4">
                    <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?auto=format&fit=crop&w=600&q=80" alt="Güzelyaka Doğa Manzarası" class="w-full h-48 object-cover rounded-2xl shadow-md">
                    <img src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?auto=format&fit=crop&w=600&q=80" alt="Köy Yeşilliği" class="w-full h-48 object-cover rounded-2xl shadow-md mt-6">
                </div>
            </div>
        </div>
    </section>

    <!-- İletişim & Konum -->
    <section id="contact" class="py-20 bg-slate-100/80 dark:bg-slate-800/50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-emerald-700 dark:text-emerald-400 font-bold text-sm uppercase tracking-wider">Bizimle İletişime Geçin</span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 dark:text-white mt-1 mb-4">Muhtarlık İletişim & Konum</h2>
                <div class="w-16 h-1 bg-emerald-600 mx-auto rounded-full mb-4"></div>
                <p class="text-slate-600 dark:text-slate-400">
                    Soru, talep ve evrak bildirimleriniz için muhtarlığımız ile iletişime geçebilirsiniz.
                </p>
            </div>

            <!-- İletişim Bilgileri Kartları -->
            <div class="grid md:grid-cols-2 gap-6 mb-12">
                <!-- Muhtar Telefon Kartı -->
                <a href="tel:+905326606372" class="flex items-start gap-4 p-6 bg-white dark:bg-slate-900 rounded-2xl border border-slate-200 dark:border-slate-800 hover:border-emerald-600 transition-all group">
                    <div class="w-12 h-12 bg-emerald-600 text-white rounded-xl flex items-center justify-center text-xl shrink-0 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-phone"></i>
                    </div>
                    <div>
                        <h4 class="font-bold text-slate-900 dark:text-white mb-1">Muhtar Telefon / WhatsApp</h4>
                        <p class="text-base font-bold text-emerald-700 dark:text-emerald-400">+90 532 660 63 72</p>
                        <p class="text-xs text-slate-500 mt-1">Mürteza Oruç (Aramak için tıklayın)</p>
                    </div>
                </a>

                <!-- Adres Kartı -->
                <div class="flex items-start gap-4 p-6 bg-white dark:bg-slate-900 rounded-2xl border border-slate-200 dark:border-slate-800">
                    <div class="w-12 h-12 bg-emerald-600 text-white rounded-xl flex items-center justify-center text-xl shrink-0">
                        <i class="fa-solid fa-location-dot"></i>
                    </div>
                    <div>
                        <h4 class="font-bold text-slate-900 dark:text-white mb-1">Muhtarlık Adresi</h4>
                        <p class="text-sm text-slate-700 dark:text-slate-300 font-medium">Güzelyaka Köyü Muhtarlığı</p>
                        <p class="text-xs text-slate-500 mt-1">Çaycuma / Zonguldak, Türkiye</p>
                    </div>
                </div>
            </div>

            <!-- Harita Görünümü -->
            <div class="rounded-2xl overflow-hidden border border-slate-200 dark:border-slate-800 h-96 shadow-md">
                <iframe 
                    class="w-full h-full border-0"
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d95514.80164825964!2d32.0000!3d41.4250!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x409b83b38ef0fa69%3A0x6a0a038c1103f53!2xC3%87aycuma%2C%20Zonguldak!5e0!3m2!1str!2str!4v1680000000000!5m2!1str!2str" 
                    allowfullscreen="" 
                    loading="lazy" 
                    referrerpolicy="no-referrer-when-downgrade">
                </iframe>
            </div>
        </div>
    </section>

    <!-- Alt Bilgi (Footer) -->
    <footer class="bg-emerald-950 text-emerald-200 py-12 border-t border-emerald-900">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row justify-between items-center gap-6">
                <div class="text-center md:text-left">
                    <h3 class="text-xl font-bold text-white flex items-center justify-center md:justify-start gap-2">
                        <i class="fa-solid fa-building-columns text-emerald-400"></i> Güzelyaka Köyü Muhtarlığı
                    </h3>
                    <p class="text-xs text-emerald-400 mt-1">Muhtar: Mürteza Oruç | Çaycuma / Zonguldak</p>
                </div>

                <div class="flex flex-wrap justify-center gap-6 text-sm">
                    <a href="#hero" class="hover:text-white transition-colors">Ana Sayfa</a>
                    <a href="#muhtar" class="hover:text-white transition-colors">Muhtarımızın Mesajı</a>
                    <a href="#services" class="hover:text-white transition-colors">Hizmetler</a>
                    <a href="#about-village" class="hover:text-white transition-colors">Köyümüz</a>
                    <a href="#contact" class="hover:text-white transition-colors">İletişim</a>
                </div>

                <div>
                    <a href="tel:+905326606372" class="px-4 py-2 bg-emerald-800 hover:bg-emerald-700 text-white text-xs font-bold rounded-xl transition-colors inline-flex items-center gap-2">
                        <i class="fa-solid fa-phone"></i> +90 532 660 63 72
                    </a>
                </div>
            </div>

            <div class="mt-8 pt-8 border-t border-emerald-900/80 text-center text-xs text-emerald-500">
                &copy; 2026 T.C. Güzelyaka Köyü Muhtarlığı. Tüm Hakları Saklıdır.
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // Mobil Menü Mantığı
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });
    </script>
</body>
</html>
