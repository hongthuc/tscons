<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>TSCONS - CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS | tscons.com</title>
    <meta name="description" content="CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS chuyên Thiết kế Kiến trúc - Thi công Xây dựng - Nội thất trọn gói Nhà phố, Biệt thự, Khách sạn, Căn hộ, Văn phòng tại Đà Nẵng. Hotline: 0933.333.254.">
    
    <!-- Thumbnail là ảnh Logo trang web khi gửi link chia sẻ (Open Graph & Twitter Card) -->
    <meta property="og:type" content="website">
    <meta property="og:site_name" content="tscons.com - CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS">
    <meta property="og:title" content="CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS - Thiết Kế & Thi Công Trọn Gói Đà Nẵng">
    <meta property="og:description" content="Chuyên Thiết kế - Thi công phần thô - Xây nhà trọn gói - Hoàn thiện nội thất tại Đà Nẵng. Địa chỉ: 702 Tôn Đản, Phường An Khê, TP Đà Nẵng. SĐT: 0933.333.254">
    <meta property="og:url" content="https://tscons.com">
    <meta property="og:image" content="https://drive.google.com/thumbnail?id=1sFnkNtXw29XYmXWC973WTwwsRuqAOCO6&sz=w1200">
    <meta property="og:image:width" content="1200">
    <meta property="og:image:height" content="630">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:image" content="https://drive.google.com/thumbnail?id=1sFnkNtXw29XYmXWC973WTwwsRuqAOCO6&sz=w1200">
    <link rel="icon" href="https://drive.google.com/thumbnail?id=1sFnkNtXw29XYmXWC973WTwwsRuqAOCO6&sz=w200">

    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <!-- Google Fonts: Inter & Montserrat -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        tsnavy: {
                            DEFAULT: '#0f2b52',
                            dark: '#091c38',
                            light: '#1c447d'
                        },
                        tsgold: {
                            DEFAULT: '#d97706',
                            light: '#f59e0b',
                            dark: '#b45309'
                        }
                    }
                }
            }
        }
    </script>

    <style>
        /* Chống tràn viền và lệch phải tuyệt đối trên mọi thiết bị */
        *, *::before, *::after {
            box-sizing: border-box;
        }
        html, body {
            width: 100%;
            max-width: 100%;
            overflow-x: hidden;
            margin: 0;
            padding: 0;
            font-family: 'Inter', sans-serif;
            color: #1e293b;
            background-color: #ffffff;
            scroll-behavior: smooth;
        }

        /* Khung chuẩn Flatsome: Chiều ngang trên máy tính bằng 95% màn hình */
        .flatsome-container {
            width: 95%;
            max-width: 95%;
            margin-left: auto;
            margin-right: auto;
        }
        @media (max-width: 767px) {
            .flatsome-container {
                width: 94%;
                max-width: 94%;
            }
        }

        /* Menu danh mục trên máy tính: chữ nhỏ gọn, viết liền trên 1 hàng, không xuống dòng từng từ */
        .desktop-nav-list {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: flex-end;
            gap: 2px 6px;
        }
        .desktop-nav-item {
            white-space: nowrap;
            font-size: 12.5px;
            font-weight: 600;
            letter-spacing: -0.01em;
            padding: 6px 9px;
            border-radius: 6px;
            color: #0f2b52;
            transition: all 0.2s ease;
            display: inline-flex;
            align-items: center;
            gap: 4px;
            line-height: 1.2;
        }
        @media (min-width: 1280px) {
            .desktop-nav-item {
                font-size: 13px;
                padding: 7px 11px;
            }
        }
        .desktop-nav-item:hover, .desktop-nav-item.active {
            background-color: #0f2b52;
            color: #ffffff;
        }

        /* Dropdown menu kiểu Flatsome */
        .has-dropdown {
            position: relative;
        }
        .nav-dropdown {
            position: absolute;
            top: 100%;
            left: 0;
            min-width: 230px;
            background: #ffffff;
            box-shadow: 0 10px 25px rgba(15, 43, 82, 0.15);
            border-top: 3px solid #d97706;
            border-radius: 0 0 8px 8px;
            padding: 6px 0;
            opacity: 0;
            visibility: hidden;
            transform: translateY(8px);
            transition: all 0.2s ease;
            z-index: 100;
        }
        .has-dropdown:hover .nav-dropdown {
            opacity: 1;
            visibility: visible;
            transform: translateY(0);
        }
        .nav-dropdown a {
            display: block;
            padding: 8px 16px;
            font-size: 12.5px;
            font-weight: 500;
            color: #1e293b;
            white-space: nowrap;
            transition: all 0.15s ease;
        }
        .nav-dropdown a:hover {
            background-color: #f1f5f9;
            color: #d97706;
            padding-left: 20px;
        }

        /* Danh mục lọc ở trang chủ: chữ nhỏ gọn, viết liền không xuống dòng tên danh mục */
        .cat-pill-bar {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            gap: 6px;
        }
        .cat-pill {
            white-space: nowrap;
            font-size: 12px;
            font-weight: 600;
            padding: 6px 12px;
            border-radius: 6px;
            border: 1px solid #cbd5e1;
            background-color: #ffffff;
            color: #0f2b52;
            transition: all 0.2s ease;
            cursor: pointer;
            line-height: 1.2;
        }
        .cat-pill:hover, .cat-pill.active {
            background-color: #0f2b52;
            border-color: #0f2b52;
            color: #ffffff;
        }
        @media (max-width: 640px) {
            .cat-pill {
                font-size: 11.5px;
                padding: 5px 10px;
            }
        }

        /* Tiêu đề Section chuẩn Flatsome (Section Title Center) */
        .section-title-container {
            margin-bottom: 1.5rem;
            text-align: center;
        }
        .section-title-main {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            max-width: 800px;
            margin: 0 auto;
        }
        .section-title-main::before,
        .section-title-main::after {
            content: "";
            flex: 1;
            height: 2px;
            background-color: #e2e8f0;
        }
        .section-title-text {
            font-weight: 800;
            color: #0f2b52;
            text-transform: uppercase;
            letter-spacing: 0.02em;
            padding: 0 8px;
            text-align: center;
        }

        /* Box sản phẩm / công trình chuẩn Flatsome: Tên sản phẩm đầy đủ, không bị cắt chữ hoặc tràn ra ngoài */
        .ux-box {
            display: flex;
            flex-direction: column;
            height: 100%;
            background: #ffffff;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }
        .ux-box:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px -5px rgba(15, 43, 82, 0.12);
            border-color: #cbd5e1;
        }
        .ux-box-image {
            position: relative;
            width: 100%;
            aspect-ratio: 4 / 3;
            overflow: hidden;
            background-color: #f1f5f9;
        }
        .ux-box-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.4s ease;
        }
        .ux-box:hover .ux-box-image img {
            transform: scale(1.05);
        }
        .ux-box-text {
            padding: 10px 10px 12px 10px;
            display: flex;
            flex-direction: column;
            flex: 1;
            justify-content: space-between;
            text-align: center;
        }
        .ux-box-title {
            font-size: 13px;
            line-height: 1.4;
            font-weight: 700;
            color: #0f2b52;
            white-space: normal;
            word-wrap: break-word;
            overflow-wrap: break-word;
            margin-bottom: 4px;
        }
        @media (min-width: 768px) {
            .ux-box-text {
                padding: 12px 14px 14px 14px;
            }
            .ux-box-title {
                font-size: 14.5px;
            }
        }

        /* Banner Slider có kích thước bằng nhau tuyệt đối trên cả PC & Mobile */
        .banner-slider-wrapper {
            position: relative;
            width: 100%;
            height: 320px;
            overflow: hidden;
            background-color: #091c38;
        }
        @media (min-width: 640px) {
            .banner-slider-wrapper {
                height: 380px;
            }
        }
        @media (min-width: 1024px) {
            .banner-slider-wrapper {
                height: 470px;
            }
        }
        .banner-slide {
            position: absolute;
            inset: 0;
            width: 100%;
            height: 100%;
            opacity: 0;
            visibility: hidden;
            transition: opacity 0.7s ease-in-out, visibility 0.7s ease-in-out;
        }
        .banner-slide.active {
            opacity: 1;
            visibility: visible;
            z-index: 10;
        }

        /* Hiệu ứng nút liên hệ nổi */
        @keyframes pulse-ring {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(217, 119, 6, 0.7); }
            70% { transform: scale(1); box-shadow: 0 0 0 10px rgba(217, 119, 6, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(217, 119, 6, 0); }
        }
        .pulse-btn {
            animation: pulse-ring 2s infinite;
        }
    </style>
</head>
<body>

<!-- #wrapper chuẩn cấu trúc Flatsome UX Builder -->
<div id="wrapper" class="w-full overflow-x-hidden">

    <!-- ================= TOP BAR ================= -->
    <div id="top-bar" class="bg-tsnavy text-white text-xs py-2 border-b border-white/10">
        <div class="flatsome-container flex flex-wrap items-center justify-between gap-2">
            <div class="flex items-center gap-3 sm:gap-5 flex-wrap">
                <span class="inline-flex items-center gap-1.5 font-medium">
                    <i class="fa-solid fa-building text-tsgold-light"></i>
                    <span>CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS</span>
                </span>
                <span class="hidden md:inline-flex items-center gap-1.5 text-slate-200">
                    <i class="fa-solid fa-location-dot text-tsgold-light"></i>
                    <span>702 Tôn Đản, Phường An Khê, TP Đà Nẵng</span>
                </span>
            </div>
            <div class="flex items-center gap-4 ml-auto">
                <a href="tel:0933333254" class="inline-flex items-center gap-1.5 text-tsgold-light font-bold hover:underline">
                    <i class="fa-solid fa-phone-volume"></i>
                    <span>0933.333.254</span>
                </a>
                <span class="text-white/30">|</span>
                <a href="https://www.facebook.com/tsconsvn" target="_blank" rel="noopener" class="inline-flex items-center gap-1 hover:text-tsgold-light transition">
                    <i class="fa-brands fa-facebook"></i>
                    <span class="hidden sm:inline">fb.com/tsconsvn</span>
                </a>
                <span class="text-white/30 hidden sm:inline">|</span>
                <a href="https://tscons.com" class="hidden sm:inline-flex items-center gap-1 hover:text-tsgold-light transition font-semibold">
                    <i class="fa-solid fa-globe"></i>
                    <span>tscons.com</span>
                </a>
            </div>
        </div>
    </div>

    <!-- ================= HEADER (Không để nút gọi ngay trên header tránh tràn viền, logo nhỏ gọn) ================= -->
    <header id="header" class="sticky top-0 z-40 bg-white shadow-sm border-b border-slate-200">
        <div class="flatsome-container py-2">
            <div class="flex items-center justify-between gap-3">
                <!-- Logo chỉnh gọn nhỏ lại -->
                <a href="#trang-chu" class="flex items-center gap-2.5 shrink-0 group">
                    <img 
                        src="https://drive.google.com/thumbnail?id=1sFnkNtXw29XYmXWC973WTwwsRuqAOCO6&sz=w400" 
                        onerror="handleDriveError(this, '1sFnkNtXw29XYmXWC973WTwwsRuqAOCO6', 'TSCONS')"
                        alt="Logo TSCONS" 
                        class="h-9 sm:h-10 w-auto object-contain rounded border border-slate-100 p-0.5 bg-white"
                    >
                    <div class="leading-tight">
                        <span class="block text-sm sm:text-base font-extrabold text-tsnavy tracking-tight">TSCONS</span>
                        <span class="block text-[10px] font-semibold text-tsgold uppercase tracking-wider">Kiến Trúc & Xây Dựng</span>
                    </div>
                </a>

                <!-- Menu Danh Mục Máy Tính: Chữ nhỏ gọn, viết liền không xuống dòng tên danh mục -->
                <nav class="hidden lg:block flex-1">
                    <ul class="desktop-nav-list">
                        <li><a href="#trang-chu" class="desktop-nav-item active">Trang chủ</a></li>
                        <li><a href="#gioi-thieu" class="desktop-nav-item">Giới thiệu</a></li>
                        <li class="has-dropdown">
                            <a href="#cong-trinh-thuc-te" class="desktop-nav-item">
                                <span>Công trình thực tế</span>
                                <i class="fa-solid fa-chevron-down text-[9px] opacity-70"></i>
                            </a>
                            <div class="nav-dropdown">
                                <a href="#cong-trinh-thuc-te" onclick="filterProjects('actual', 'all')">Tất cả công trình thực tế</a>
                                <a href="#cong-trinh-thuc-te" onclick="filterProjects('actual', 'khach-san')">Khách sạn – Căn hộ – Phòng trọ</a>
                                <a href="#cong-trinh-thuc-te" onclick="filterProjects('actual', 'biet-thu')">Biệt thự</a>
                                <a href="#cong-trinh-thuc-te" onclick="filterProjects('actual', 'nha-pho')">Nhà phố</a>
                                <a href="#cong-trinh-thuc-te" onclick="filterProjects('actual', 'van-phong')">Văn phòng</a>
                            </div>
                        </li>
                        <li class="has-dropdown">
                            <a href="#du-an-da-nang" class="desktop-nav-item">
                                <span>Dự án Đà Nẵng</span>
                                <i class="fa-solid fa-chevron-down text-[9px] opacity-70"></i>
                            </a>
                            <div class="nav-dropdown">
                                <a href="#du-an-da-nang" onclick="filterProjects('danang', 'all')">Tất cả dự án tại Đà Nẵng</a>
                                <a href="#du-an-da-nang" onclick="filterProjects('danang', 'nha-pho-dn')">Nhà phố hiện đại Đà Nẵng</a>
                                <a href="#du-an-da-nang" onclick="filterProjects('danang', 'biet-thu-dn')">Biệt thự & Nghỉ dưỡng</a>
                                <a href="#du-an-da-nang" onclick="filterProjects('danang', 'can-ho-dn')">Căn hộ & Khách sạn</a>
                            </div>
                        </li>
                        <li class="has-dropdown">
                            <a href="#linh-vuc-hoat-dong" class="desktop-nav-item">
                                <span>Lĩnh vực hoạt động</span>
                                <i class="fa-solid fa-chevron-down text-[9px] opacity-70"></i>
                            </a>
                            <div class="nav-dropdown">
                                <a href="#linh-vuc-hoat-dong">Thiết kế Kiến trúc – Nội thất</a>
                                <a href="#linh-vuc-hoat-dong">Thi công phần thô</a>
                                <a href="#linh-vuc-hoat-dong">Thi công hoàn thiện</a>
                                <a href="#linh-vuc-hoat-dong">Thi công nội thất</a>
                            </div>
                        </li>
                        <li class="has-dropdown">
                            <a href="#linh-vuc-hoat-dong" class="desktop-nav-item">
                                <span>Mẫu thiết kế</span>
                                <i class="fa-solid fa-chevron-down text-[9px] opacity-70"></i>
                            </a>
                            <div class="nav-dropdown">
                                <a href="#linh-vuc-hoat-dong">Mẫu thiết kế nhà phố</a>
                                <a href="#linh-vuc-hoat-dong">Mẫu thiết kế biệt thự</a>
                                <a href="#linh-vuc-hoat-dong">Mẫu thiết kế nội thất</a>
                            </div>
                        </li>
                        <li class="has-dropdown">
                            <a href="#bao-gia-tu-van" class="desktop-nav-item">
                                <span>Báo giá</span>
                                <i class="fa-solid fa-chevron-down text-[9px] opacity-70"></i>
                            </a>
                            <div class="nav-dropdown">
                                <a href="#bao-gia-tu-van">Báo giá thiết kế kiến trúc</a>
                                <a href="#bao-gia-tu-van">Báo giá thi công phần thô</a>
                                <a href="#bao-gia-tu-van">Báo giá thi công hoàn thiện</a>
                                <a href="#bao-gia-tu-van">Báo giá thi công trọn gói</a>
                            </div>
                        </li>
                        <li><a href="#doi-tac" class="desktop-nav-item">Đối tác</a></li>
                        <li><a href="#tin-tuc" class="desktop-nav-item">Tin tức</a></li>
                        <li><a href="#lien-he-map" class="desktop-nav-item">Liên hệ</a></li>
                    </ul>
                </nav>

                <!-- Nút mở Menu trên Điện Thoại -->
                <button id="mobile-menu-btn" onclick="toggleMobileMenu()" aria-label="Mở danh mục" class="lg:hidden inline-flex items-center gap-1.5 px-3 py-1.5 rounded-md bg-tsnavy text-white text-xs font-semibold">
                    <i class="fa-solid fa-bars text-sm"></i>
                    <span>DANH MỤC</span>
                </button>
            </div>
        </div>

        <!-- Thanh Danh Mục Nhanh Trên Điện Thoại (Hiển thị gọn đẹp, không tràn viền) -->
        <div class="lg:hidden bg-slate-50 border-t border-slate-200 py-1.5">
            <div class="flatsome-container flex items-center justify-start gap-1.5 overflow-x-auto no-scrollbar">
                <a href="#cong-trinh-thuc-te" class="shrink-0 whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white border border-slate-200 text-tsnavy">Công trình thực tế</a>
                <a href="#du-an-da-nang" class="shrink-0 whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white border border-slate-200 text-tsnavy">Dự án Đà Nẵng</a>
                <a href="#linh-vuc-hoat-dong" class="shrink-0 whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white border border-slate-200 text-tsnavy">Lĩnh vực hoạt động</a>
                <a href="#bao-gia-tu-van" class="shrink-0 whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white border border-slate-200 text-tsnavy">Báo giá</a>
                <a href="#tin-tuc" class="shrink-0 whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white border border-slate-200 text-tsnavy">Tin tức</a>
                <a href="#lien-he-map" class="shrink-0 whitespace-nowrap text-[11px] font-semibold px-2.5 py-1 rounded bg-white border border-slate-200 text-tsnavy">Bản đồ & Liên hệ</a>
            </div>
        </div>

        <!-- Menu Drawer Điện Thoại -->
        <div id="mobile-menu-drawer" class="hidden lg:hidden bg-white border-t border-slate-200 shadow-xl">
            <div class="flatsome-container py-3 grid grid-cols-2 gap-2">
                <a href="#trang-chu" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-house mr-1.5 text-tsgold"></i>Trang chủ</a>
                <a href="#gioi-thieu" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-circle-info mr-1.5 text-tsgold"></i>Giới thiệu</a>
                <a href="#cong-trinh-thuc-te" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-helmet-safety mr-1.5 text-tsgold"></i>Công trình thực tế</a>
                <a href="#du-an-da-nang" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-city mr-1.5 text-tsgold"></i>Dự án Đà Nẵng</a>
                <a href="#linh-vuc-hoat-dong" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-compass-drafting mr-1.5 text-tsgold"></i>Lĩnh vực hoạt động</a>
                <a href="#linh-vuc-hoat-dong" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-layer-group mr-1.5 text-tsgold"></i>Mẫu thiết kế</a>
                <a href="#bao-gia-tu-van" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-file-invoice-dollar mr-1.5 text-tsgold"></i>Báo giá xây dựng</a>
                <a href="#doi-tac" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-handshake mr-1.5 text-tsgold"></i>Đối tác</a>
                <a href="#tin-tuc" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-newspaper mr-1.5 text-tsgold"></i>Tin tức</a>
                <a href="#lien-he-map" onclick="toggleMobileMenu()" class="px-3 py-2 rounded bg-slate-50 text-tsnavy font-semibold text-xs whitespace-nowrap"><i class="fa-solid fa-map-location-dot mr-1.5 text-tsgold"></i>Liên hệ & Bản đồ</a>
            </div>
        </div>
    </header>

    <!-- ================= MAIN CONTENT (#main chuẩn Flatsome) ================= -->
    <main id="main">

        <!-- 1. SLIDER 2 ẢNH BANNER TỰ TRƯỢT KÍCH THƯỚC BẰNG NHAU, CHỮ NẰM GỌN TRONG BANNER & CÁCH XA VIỀN -->
        <section id="trang-chu" class="w-full bg-slate-900">
            <div class="flatsome-container py-2 sm:py-3">
                <div class="banner-slider-wrapper rounded-xl shadow-lg">
                    
                    <!-- BANNER SLIDE 1 -->
                    <div class="banner-slide active" id="slide-0">
                        <img 
                            src="https://drive.google.com/thumbnail?id=157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT&sz=w1600" 
                            onerror="handleDriveError(this, '157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT', 'TSCONS+BANNER+1')"
                            alt="Banner TSCONS Thiết kế và Thi công trọn gói" 
                            class="w-full h-full object-cover"
                        >
                        <div class="absolute inset-0 bg-gradient-to-r from-tsnavy-dark/90 via-tsnavy/80 to-tsnavy-dark/65"></div>
                        <!-- Nội dung chữ cách xa viền ảnh banner, đảm bảo điện thoại & máy tính không bị thiếu chữ -->
                        <div class="absolute inset-0 flex items-center justify-center px-10 sm:px-16 md:px-24 lg:px-32 py-8">
                            <div class="w-full max-w-4xl text-center text-white">
                                <p class="text-[11px] sm:text-xs md:text-sm font-bold uppercase tracking-widest text-tsgold-light mb-1.5 sm:mb-2">
                                    CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS
                                </p>
                                <h1 class="text-base sm:text-2xl md:text-3xl lg:text-4xl font-extrabold leading-snug mb-2 sm:mb-3">
                                    THIẾT KẾ KIẾN TRÚC – THI CÔNG XÂY DỰNG – NỘI THẤT TRỌN GÓI
                                </h1>
                                <p class="text-xs sm:text-sm md:text-base text-slate-200 max-w-2xl mx-auto mb-3 sm:mb-5 leading-relaxed">
                                    Chuyên Biệt thự, Nhà phố, Khách sạn, Căn hộ, Văn phòng tại Đà Nẵng & Miền Trung. Cam kết An toàn – Chất lượng – Đúng tiến độ – Chi phí tối ưu.
                                </p>
                                <div class="flex flex-wrap items-center justify-center gap-2 sm:gap-3">
                                    <a href="#bao-gia-tu-van" class="px-4 py-2 sm:px-5 sm:py-2.5 rounded-lg bg-tsgold hover:bg-tsgold-dark text-white font-bold text-xs sm:text-sm transition shadow">
                                        NHẬN BÁO GIÁ MIỄN PHÍ
                                    </a>
                                    <a href="#cong-trinh-thuc-te" class="px-4 py-2 sm:px-5 sm:py-2.5 rounded-lg bg-white/15 hover:bg-white/25 border border-white/40 text-white font-semibold text-xs sm:text-sm transition">
                                        XEM CÔNG TRÌNH THỰC TẾ
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- BANNER SLIDE 2 (Kích thước bằng nhau 100%) -->
                    <div class="banner-slide" id="slide-1">
                        <img 
                            src="https://drive.google.com/thumbnail?id=1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff&sz=w1600" 
                            onerror="handleDriveError(this, '1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff', 'TSCONS+BANNER+2')"
                            alt="Banner TSCONS Xây nhà trọn gói Đà Nẵng" 
                            class="w-full h-full object-cover"
                        >
                        <div class="absolute inset-0 bg-gradient-to-r from-tsnavy-dark/90 via-tsnavy/80 to-tsnavy-dark/65"></div>
                        <!-- Nội dung chữ cách xa viền ảnh banner, đảm bảo điện thoại & máy tính không bị thiếu chữ -->
                        <div class="absolute inset-0 flex items-center justify-center px-10 sm:px-16 md:px-24 lg:px-32 py-8">
                            <div class="w-full max-w-4xl text-center text-white">
                                <p class="text-[11px] sm:text-xs md:text-sm font-bold uppercase tracking-widest text-tsgold-light mb-1.5 sm:mb-2">
                                    NHÀ Ở GIA ĐÌNH – TIÊU CHUẨN CÔNG TRÌNH
                                </p>
                                <h2 class="text-base sm:text-2xl md:text-3xl lg:text-4xl font-extrabold leading-snug mb-2 sm:mb-3">
                                    GIẢI PHÁP XÂY NHÀ TRỌN GÓI CHÌA KHÓA TRAO TAY TẠI ĐÀ NẴNG
                                </h2>
                                <p class="text-xs sm:text-sm md:text-base text-slate-200 max-w-2xl mx-auto mb-3 sm:mb-5 leading-relaxed">
                                    Trụ sở: 702 Tôn Đản, Phường An Khê, TP Đà Nẵng | Hotline tư vấn 24/7: 0933.333.254. Đồng hành tận tâm kiến tạo tổ ấm bền vững theo thời gian.
                                </p>
                                <div class="flex flex-wrap items-center justify-center gap-2 sm:gap-3">
                                    <a href="#du-an-da-nang" class="px-4 py-2 sm:px-5 sm:py-2.5 rounded-lg bg-tsgold hover:bg-tsgold-dark text-white font-bold text-xs sm:text-sm transition shadow">
                                        DỰ ÁN TẠI ĐÀ NẴNG
                                    </a>
                                    <a href="#lien-he-map" class="px-4 py-2 sm:px-5 sm:py-2.5 rounded-lg bg-white/15 hover:bg-white/25 border border-white/40 text-white font-semibold text-xs sm:text-sm transition">
                                        LIÊN HỆ TSCONS: 0933.333.254
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Nút điều hướng trái/phải nằm gọn sát mép ngoài phần chữ -->
                    <button onclick="prevSlide()" aria-label="Slide trước" class="absolute left-2 sm:left-3 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-9 sm:h-9 rounded-full bg-black/40 hover:bg-tsgold text-white flex items-center justify-center transition">
                        <i class="fa-solid fa-chevron-left text-xs sm:text-sm"></i>
                    </button>
                    <button onclick="nextSlide()" aria-label="Slide tiếp" class="absolute right-2 sm:right-3 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-9 sm:h-9 rounded-full bg-black/40 hover:bg-tsgold text-white flex items-center justify-center transition">
                        <i class="fa-solid fa-chevron-right text-xs sm:text-sm"></i>
                    </button>

                    <!-- Chấm chỉ báo Slide -->
                    <div class="absolute bottom-2.5 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
                        <button onclick="goToSlide(0)" id="dot-0" class="w-6 h-2 rounded-full bg-tsgold transition-all" aria-label="Banner 1"></button>
                        <button onclick="goToSlide(1)" id="dot-1" class="w-2.5 h-2 rounded-full bg-white/60 transition-all" aria-label="Banner 2"></button>
                    </div>

                </div>
            </div>
        </section>

        <!-- 2. DỊCH VỤ TIÊU BIỂU & GIỚI THIỆU CÔNG TY TSCONS (Giống mẫu tintruongthinh.com) -->
        <section id="gioi-thieu" class="py-8 sm:py-12 bg-white">
            <div class="flatsome-container">
                
                <!-- 3 Khối Dịch Vụ Tiêu Biểu: THIẾT KẾ - THI CÔNG - NỘI THẤT -->
                <div class="section-title-container">
                    <div class="section-title-main">
                        <h2 class="section-title-text text-base sm:text-xl">DỊCH VỤ TIÊU BIỂU</h2>
                    </div>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-10">
                    <a href="#linh-vuc-hoat-dong" class="ux-box p-5 text-center hover:border-tsgold group">
                        <div class="w-14 h-14 rounded-full bg-tsnavy/10 text-tsnavy group-hover:bg-tsnavy group-hover:text-white flex items-center justify-center mx-auto mb-3 transition">
                            <i class="fa-solid fa-compass-drafting text-2xl"></i>
                        </div>
                        <h3 class="text-base font-extrabold text-tsnavy mb-1.5">THIẾT KẾ KIẾN TRÚC</h3>
                        <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                            Tư vấn thiết kế kiến trúc Nhà phố, Biệt thự, Khách sạn, Căn hộ cho thuê, Văn phòng hiện đại tối ưu công năng và thẩm mỹ.
                        </p>
                    </a>
                    <a href="#cong-trinh-thuc-te" class="ux-box p-5 text-center hover:border-tsgold group">
                        <div class="w-14 h-14 rounded-full bg-tsgold/15 text-tsgold-dark group-hover:bg-tsgold group-hover:text-white flex items-center justify-center mx-auto mb-3 transition">
                            <i class="fa-solid fa-trowel-bricks text-2xl"></i>
                        </div>
                        <h3 class="text-base font-extrabold text-tsnavy mb-1.5">THI CÔNG XÂY DỰNG</h3>
                        <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                            Thi công phần thô, thi công hoàn thiện và xây nhà trọn gói chìa khóa trao tay đúng tiến độ, vật tư chính hãng, kết cấu bền vững.
                        </p>
                    </a>
                    <a href="#du-an-da-nang" class="ux-box p-5 text-center hover:border-tsgold group">
                        <div class="w-14 h-14 rounded-full bg-tsnavy/10 text-tsnavy group-hover:bg-tsnavy group-hover:text-white flex items-center justify-center mx-auto mb-3 transition">
                            <i class="fa-solid fa-couch text-2xl"></i>
                        </div>
                        <h3 class="text-base font-extrabold text-tsnavy mb-1.5">THIẾT KẾ & THI CÔNG NỘI THẤT</h3>
                        <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
                            Sản xuất và thi công lắp đặt nội thất gỗ công nghiệp, gỗ tự nhiên cao cấp đồng bộ với bản vẽ phối cảnh 3D.
                        </p>
                    </a>
                </div>

                <!-- Giới thiệu tổng quan CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS -->
                <div class="bg-slate-50 border border-slate-200 rounded-xl p-5 sm:p-8 mb-10">
                    <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-center">
                        <div class="lg:col-span-7">
                            <p class="text-xs font-bold uppercase tracking-wider text-tsgold mb-1">VỀ CHÚNG TÔI — TSCONS.COM</p>
                            <h2 class="text-lg sm:text-2xl font-extrabold text-tsnavy mb-3">
                                CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS
                            </h2>
                            <p class="text-xs sm:text-sm text-slate-700 leading-relaxed mb-3">
                                <strong>TSCONS</strong> chuyên <strong>Thiết kế – Xây dựng – Nội thất</strong> các công trình Khách sạn, Biệt thự, Căn hộ, Văn phòng, Nhà phố tại TP Đà Nẵng và khu vực Miền Trung. Với tiêu chí <em>“Nhà ở Gia đình – Tiêu chuẩn Công trình”</em>, chúng tôi luôn mang đến trải nghiệm dịch vụ chuyên nghiệp, minh bạch và tận tâm dành cho Quý Khách hàng.
                            </p>
                            <p class="text-xs sm:text-sm text-slate-700 leading-relaxed mb-4">
                                Đặt cái <strong>“TÂM”</strong> trong nghề lên hàng đầu để mỗi công trình luôn đạt kết quả <strong>“AN TOÀN – CHẤT LƯỢNG – TIẾN ĐỘ – SỰ HÀI LÒNG CỦA KHÁCH HÀNG”</strong>. Đội ngũ kiến trúc sư và kỹ sư xây dựng của TSCONS đồng hành cùng Chủ đầu tư từ khâu xin phép xây dựng, thiết kế bản vẽ đến thi công hoàn thiện và bảo hành dài hạn.
                            </p>
                            <div class="grid grid-cols-2 sm:grid-cols-3 gap-3 text-xs">
                                <div class="bg-white p-3 rounded-lg border border-slate-200">
                                    <span class="block font-extrabold text-tsnavy text-sm">MST: 0402234752</span>
                                    <span class="text-slate-500">Pháp lý minh bạch</span>
                                </div>
                                <div class="bg-white p-3 rounded-lg border border-slate-200">
                                    <span class="block font-extrabold text-tsgold-dark text-sm">0933.333.254</span>
                                    <span class="text-slate-500">Tư vấn kỹ thuật 24/7</span>
                                </div>
                                <div class="col-span-2 sm:col-span-1 bg-white p-3 rounded-lg border border-slate-200">
                                    <span class="block font-extrabold text-tsnavy text-sm">702 Tôn Đản</span>
                                    <span class="text-slate-500">P. An Khê, TP Đà Nẵng</span>
                                </div>
                            </div>
                        </div>
                        <div class="lg:col-span-5">
                            <div class="rounded-xl overflow-hidden border border-slate-200 shadow-sm bg-white p-3">
                                <img 
                                    src="https://drive.google.com/thumbnail?id=13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz&sz=w1000" 
                                    onerror="handleDriveError(this, '13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz', 'TSCONS+Thi+Cong')"
                                    alt="Hoạt động thi công thực tế TSCONS" 
                                    class="w-full h-56 sm:h-64 object-cover rounded-lg"
                                >
                                <div class="pt-2.5 text-center">
                                    <p class="text-xs font-bold text-tsnavy">Đội ngũ Kỹ sư & Giám sát TSCONS trực tiếp tại công trình</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- 6 THẾ MẠNH CỦA CHÚNG TÔI (Chuẩn bố cục web mẫu tintruongthinh.com) -->
                <div class="section-title-container">
                    <div class="section-title-main">
                        <h2 class="section-title-text text-base sm:text-xl">THẾ MẠNH CỦA CHÚNG TÔI</h2>
                    </div>
                </div>

                <div class="grid grid-cols-2 lg:grid-cols-3 gap-3 sm:gap-5">
                    <div class="ux-box p-4 text-left">
                        <div class="flex items-center gap-2.5 mb-2">
                            <span class="w-9 h-9 shrink-0 rounded-lg bg-tsnavy text-white flex items-center justify-center text-sm"><i class="fa-solid fa-user-tie"></i></span>
                            <h3 class="ux-box-title text-left !mb-0">Đội ngũ KTS, kỹ sư chuyên nghiệp</h3>
                        </div>
                        <p class="text-xs text-slate-600 leading-relaxed">Kiến trúc sư sáng tạo cùng đội ngũ kỹ sư chỉ huy công trình giàu kinh nghiệm và thợ lành nghề.</p>
                    </div>
                    <div class="ux-box p-4 text-left">
                        <div class="flex items-center gap-2.5 mb-2">
                            <span class="w-9 h-9 shrink-0 rounded-lg bg-tsgold text-white flex items-center justify-center text-sm"><i class="fa-solid fa-lightbulb"></i></span>
                            <h3 class="ux-box-title text-left !mb-0">Cập nhật xu hướng mới nhất</h3>
                        </div>
                        <p class="text-xs text-slate-600 leading-relaxed">Ứng dụng giải pháp không gian xanh, thông thoáng, vật liệu chống thấm và cách nhiệt hiện đại.</p>
                    </div>
                    <div class="ux-box p-4 text-left">
                        <div class="flex items-center gap-2.5 mb-2">
                            <span class="w-9 h-9 shrink-0 rounded-lg bg-tsnavy text-white flex items-center justify-center text-sm"><i class="fa-solid fa-clipboard-check"></i></span>
                            <h3 class="ux-box-title text-left !mb-0">Giám sát tiến độ chuẩn xác</h3>
                        </div>
                        <p class="text-xs text-slate-600 leading-relaxed">Cam kết hoàn thành đúng tiến độ hợp đồng, báo cáo nhật ký công trình thường xuyên cho Chủ đầu tư.</p>
                    </div>
                    <div class="ux-box p-4 text-left">
                        <div class="flex items-center gap-2.5 mb-2">
                            <span class="w-9 h-9 shrink-0 rounded-lg bg-tsgold text-white flex items-center justify-center text-sm"><i class="fa-solid fa-shield-halved"></i></span>
                            <h3 class="ux-box-title text-left !mb-0">Bảo hành công trình lâu dài</h3>
                        </div>
                        <p class="text-xs text-slate-600 leading-relaxed">Chế độ hậu mãi tận tâm, bảo hành kết cấu dài hạn và hỗ trợ kỹ thuật nhanh chóng khi khách hàng cần.</p>
                    </div>
                    <div class="ux-box p-4 text-left">
                        <div class="flex items-center gap-2.5 mb-2">
                            <span class="w-9 h-9 shrink-0 rounded-lg bg-tsnavy text-white flex items-center justify-center text-sm"><i class="fa-solid fa-scale-balanced"></i></span>
                            <h3 class="ux-box-title text-left !mb-0">Giá cả hợp lý phải chăng</h3>
                        </div>
                        <p class="text-xs text-slate-600 leading-relaxed">Bóc tách dự toán chi tiết từng hạng mục, cam kết không phát sinh chi phí ngoài hợp đồng.</p>
                    </div>
                    <div class="ux-box p-4 text-left">
                        <div class="flex items-center gap-2.5 mb-2">
                            <span class="w-9 h-9 shrink-0 rounded-lg bg-tsgold text-white flex items-center justify-center text-sm"><i class="fa-solid fa-headset"></i></span>
                            <h3 class="ux-box-title text-left !mb-0">Hỗ trợ tư vấn miễn phí 24/7</h3>
                        </div>
                        <p class="text-xs text-slate-600 leading-relaxed">Khảo sát thực tế mặt bằng tại Đà Nẵng và tư vấn phương án thiết kế, dự trù kinh phí hoàn toàn miễn phí.</p>
                    </div>
                </div>

            </div>
        </section>

        <!-- 3. LĨNH VỰC HOẠT ĐỘNG & DANH MỤC SẢN PHẨM DỊCH VỤ (Lấy từ web mẫu, 2 cột trên điện thoại, không nhãn dán) -->
        <section id="linh-vuc-hoat-dong" class="py-8 sm:py-12 bg-slate-50 border-t border-slate-200">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <div class="section-title-main">
                        <h2 class="section-title-text text-base sm:text-xl">LĨNH VỰC HOẠT ĐỘNG & SẢN PHẨM DỊCH VỤ</h2>
                    </div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-1">Giải pháp toàn diện từ Thiết kế Kiến trúc, Thi công Phần thô đến Xây nhà Trọn gói & Nội thất</p>
                </div>

                <!-- Sản phẩm chia thành 2 cột trên giao diện điện thoại (grid-cols-2), 4 cột trên máy tính -->
                <div class="grid grid-cols-2 md:grid-cols-4 gap-2.5 sm:gap-4">
                    
                    <div class="ux-box cursor-pointer" onclick="openDetailModal('Thiết kế Kiến trúc – Nội thất', 'Lĩnh vực hoạt động', 'https://drive.google.com/thumbnail?id=157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT&sz=w1000', 'Hồ sơ thiết kế đầy đủ gồm: Bản vẽ kiến trúc 2D, Phối cảnh 3D mặt tiền & nội thất, Hồ sơ kết cấu, Hồ sơ điện nước M&E và Dự toán thi công chi tiết.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT&sz=w800" onerror="handleDriveError(this, '157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT', 'Thiet+Ke+Kien+Truc')" alt="Thiết kế Kiến trúc – Nội thất">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thiết kế Kiến trúc – Nội thất</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Nhà phố, Biệt thự, Căn hộ, Văn phòng</p>
                        </div>
                    </div>

                    <div class="ux-box cursor-pointer" onclick="openDetailModal('Thi công phần thô & nhân công hoàn thiện', 'Lĩnh vực hoạt động', 'https://drive.google.com/thumbnail?id=13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz&sz=w1000', 'Thi công móng, khung bê tông cốt thép, xây tô tường, chống thấm và lắp đặt hệ thống điện nước âm tường theo tiêu chuẩn kỹ thuật xây dựng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz&sz=w800" onerror="handleDriveError(this, '13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz', 'Thi+Cong+Phan+Tho')" alt="Thi công phần thô">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công phần thô</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Vật tư chuẩn, kết cấu vững chắc</p>
                        </div>
                    </div>

                    <div class="ux-box cursor-pointer" onclick="openDetailModal('Thi công hoàn thiện công trình', 'Lĩnh vực hoạt động', 'https://drive.google.com/thumbnail?id=1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t&sz=w1000', 'Ốp lát gạch, sơn bả hoàn thiện, đóng trần thạch cao, lắp đặt cửa nhôm kính, lan can, thiết bị vệ sinh và hệ thống chiếu sáng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t&sz=w800" onerror="handleDriveError(this, '1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t', 'Thi+Cong+Hoan+Thien')" alt="Thi công hoàn thiện">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công hoàn thiện</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Thẩm mỹ sắc nét, chuẩn bản vẽ</p>
                        </div>
                    </div>

                    <div class="ux-box cursor-pointer" onclick="openDetailModal('Thi công nội thất trọn gói', 'Lĩnh vực hoạt động', 'https://drive.google.com/thumbnail?id=1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N&sz=w1000', 'Thi công nội thất phòng khách, phòng bếp, phòng ngủ, văn phòng làm việc với vật liệu gỗ An Cường, gỗ tự nhiên, đá tự nhiên cao cấp.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N&sz=w800" onerror="handleDriveError(this, '1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N', 'Thi+Cong+Noi+That')" alt="Thi công nội thất">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công nội thất</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Đồng bộ không gian sống tiện nghi</p>
                        </div>
                    </div>

                    <div class="ux-box cursor-pointer" onclick="openDetailModal('Báo giá xây nhà trọn gói – Chìa khóa trao tay', 'Báo giá dịch vụ', 'https://drive.google.com/thumbnail?id=1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff&sz=w1000', 'Gói dịch vụ trọn gói từ xin phép xây dựng, thiết kế kiến trúc, thi công phần thô đến hoàn thiện và bàn giao nhà đưa vào sử dụng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff&sz=w800" onerror="handleDriveError(this, '1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff', 'Xay+Nha+Tron+Goi')" alt="Báo giá thi công trọn gói">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Báo giá thi công trọn gói</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Chìa khóa trao tay – Tối ưu chi phí</p>
                        </div>
                    </div>

                    <div class="ux-box cursor-pointer" onclick="openDetailModal('Mẫu thiết kế nhà phố hiện đại Đà Nẵng', 'Mẫu thiết kế', 'https://drive.google.com/thumbnail?id=1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz&sz=w1000', 'Tuyển tập mẫu thiết kế nhà phố 2 tầng, 3 tầng, 4 tầng hiện đại, thông thoáng, lấy sáng tự nhiên phù hợp khí hậu Đà Nẵng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz&sz=w800" onerror="handleDriveError(this, '1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz', 'Mau+Nha+Pho')" alt="Mẫu thiết kế nhà phố">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Mẫu thiết kế nhà phố</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Kiến trúc hiện đại, thông tầng xanh</p>
                        </div>
                    </div>

                    <div class="ux-box cursor-pointer" onclick="openDetailModal('Mẫu thiết kế Biệt thự & Căn hộ cho thuê', 'Mẫu thiết kế', 'https://drive.google.com/thumbnail?id=1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k&sz=w1000', 'Thiết kế biệt thự phố, biệt thự nghỉ dưỡng, tòa nhà căn hộ dịch vụ và khách sạn tối ưu diện tích khai thác kinh doanh.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k&sz=w800" onerror="handleDriveError(this, '1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k', 'Mau+Biet+Thu')" alt="Mẫu thiết kế biệt thự và căn hộ">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Mẫu thiết kế Biệt thự – Căn hộ</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Sang trọng, đẳng cấp & hiệu quả</p>
                        </div>
                    </div>

                    <div class="ux-box cursor-pointer" onclick="openDetailModal('Cải tạo – Sửa chữa nâng cấp công trình', 'Lĩnh vực hoạt động', 'https://drive.google.com/thumbnail?id=1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn&sz=w1000', 'Khảo sát kết cấu, gia cố nâng tầng, chống thấm dột và cải tạo mặt tiền, nội thất nhà phố, văn phòng, khách sạn tại Đà Nẵng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn&sz=w800" onerror="handleDriveError(this, '1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn', 'Cai+Tao+Sua+Chua')" alt="Cải tạo sửa chữa công trình">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Cải tạo – Sửa chữa nhà trọn gói</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Nâng tầng, chống thấm, làm mới</p>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- 4. CÔNG TRÌNH THỰC TẾ THI CÔNG XÂY DỰNG (9 File ảnh Drive thực tế thi công, chia 2 cột trên điện thoại, không nhãn dán) -->
        <section id="cong-trinh-thuc-te" class="py-8 sm:py-12 bg-white border-t border-slate-200">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <div class="section-title-main">
                        <h2 class="section-title-text text-base sm:text-xl">CÔNG TRÌNH THỰC TẾ THI CÔNG XÂY DỰNG</h2>
                    </div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-1 mb-4">Hình ảnh thực tế thi công xây dựng tại công trường do đội ngũ kỹ sư TSCONS trực tiếp thực hiện</p>

                    <!-- Thanh lọc danh mục nhỏ gọn, viết liền không xuống dòng tên danh mục -->
                    <div class="cat-pill-bar" id="actual-filter-bar">
                        <button onclick="filterProjects('actual', 'all', this)" class="cat-pill active">Tất cả</button>
                        <button onclick="filterProjects('actual', 'nha-pho', this)" class="cat-pill">Nhà phố</button>
                        <button onclick="filterProjects('actual', 'biet-thu', this)" class="cat-pill">Biệt thự</button>
                        <button onclick="filterProjects('actual', 'khach-san', this)" class="cat-pill">Khách sạn – Căn hộ – Phòng trọ</button>
                        <button onclick="filterProjects('actual', 'van-phong', this)" class="cat-pill">Văn phòng</button>
                    </div>
                </div>

                <!-- Grid 9 ảnh thực tế thi công: 2 cột trên điện thoại (grid-cols-2), 3 cột trên máy tính -->
                <div id="actual-projects-grid" class="grid grid-cols-2 md:grid-cols-3 gap-2.5 sm:gap-5">
                    
                    <!-- Ảnh thực tế 1: 13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz -->
                    <div class="ux-box actual-item cursor-pointer" data-category="nha-pho" onclick="openDetailModal('Thi công phần thô & kết cấu bê tông cốt thép Nhà phố Đà Nẵng', 'Công trình thực tế - Nhà phố', 'https://drive.google.com/thumbnail?id=13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz&sz=w1200', 'Công tác nghiệm thu cốt thép sàn, cốp pha và đổ bê tông phần thô công trình nhà phố tại Đà Nẵng do đội ngũ kỹ sư TSCONS trực tiếp giám sát.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz&sz=w800" onerror="handleDriveError(this, '13S9xBPbSGKY6Kmr5Mc0x4Dk-1CdozBlz', 'Thi+Cong+1')" alt="Thi công phần thô kết cấu Nhà phố Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công phần thô & kết cấu bê tông cốt thép Nhà phố Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Hạng mục: Thi công phần thô Nhà phố</p>
                        </div>
                    </div>

                    <!-- Ảnh thực tế 2: 1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR -->
                    <div class="ux-box actual-item cursor-pointer" data-category="nha-pho" onclick="openDetailModal('Thi công xây dựng khung kết cấu Nhà phố 3 tầng hiện đại', 'Công trình thực tế - Nhà phố', 'https://drive.google.com/thumbnail?id=1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR&sz=w1200', 'Thi công xây tường bao, đổ cột và dầm sàn bê tông cốt thép chuẩn kỹ thuật, đảm bảo an toàn lao động và vệ sinh công trường.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR&sz=w800" onerror="handleDriveError(this, '1taZEEvo_cWqkQxBcCPhpoDRIIMQ-50eR', 'Thi+Cong+2')" alt="Thi công xây dựng khung kết cấu Nhà phố 3 tầng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công xây dựng khung kết cấu Nhà phố 3 tầng hiện đại</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Hạng mục: Xây dựng Nhà phố</p>
                        </div>
                    </div>

                    <!-- Ảnh thực tế 3: 1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv -->
                    <div class="ux-box actual-item cursor-pointer" data-category="biet-thu" onclick="openDetailModal('Thi công móng & đài cọc bê tông cốt thép Biệt thự gia đình', 'Công trình thực tế - Biệt thự', 'https://drive.google.com/thumbnail?id=1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv&sz=w1200', 'Gia công lắp dựng cốt thép móng, đà kiềng và nghiệm thu kỹ thuật trước khi đổ bê tông thương phẩm.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv&sz=w800" onerror="handleDriveError(this, '1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv', 'Thi+Cong+3')" alt="Thi công móng và đài cọc Biệt thự">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công móng & đài cọc bê tông cốt thép Biệt thự gia đình</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Hạng mục: Kết cấu móng Biệt thự</p>
                        </div>
                    </div>

                    <!-- Ảnh thực tế 4: 1Wlhms5ZB_mL9OptenKvrBS-rGCP2xU1_ -->
                    <div class="ux-box actual-item cursor-pointer" data-category="khach-san" onclick="openDetailModal('Thi công sàn cốp pha & cốt thép công trình Căn hộ – Khách sạn', 'Công trình thực tế - Khách sạn & Căn hộ', 'https://drive.google.com/thumbnail?id=1Wlhms5ZB_mL9OptenKvrBS-rGCP2xU1_&sz=w1200', 'Lắp dựng hệ giáo chống, cốp pha sàn và bố trí thép sàn 2 lớp đúng bản vẽ thiết kế kết cấu.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1Wlhms5ZB_mL9OptenKvrBS-rGCP2xU1_&sz=w800" onerror="handleDriveError(this, '1Wlhms5ZB_mL9OptenKvrBS-rGCP2xU1_', 'Thi+Cong+4')" alt="Thi công sàn cốp pha Căn hộ Khách sạn">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công sàn cốp pha & cốt thép công trình Căn hộ – Khách sạn</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Hạng mục: Khách sạn – Căn hộ</p>
                        </div>
                    </div>

                    <!-- Ảnh thực tế 5: 1bRJmtvTDnszz8dMG3_a3Z8hoL5igG-hO -->
                    <div class="ux-box actual-item cursor-pointer" data-category="nha-pho" onclick="openDetailModal('Thi công xây tường gạch & tô trát phần thô Nhà phố Cẩm Lệ', 'Công trình thực tế - Nhà phố', 'https://drive.google.com/thumbnail?id=1bRJmtvTDnszz8dMG3_a3Z8hoL5igG-hO&sz=w1200', 'Xây tường gạch tuynel thẳng phẳng, đóng lưới mắt cáo chống nứt tại các vị trí tiếp giáp dầm cột và đi ống điện nước âm tường.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1bRJmtvTDnszz8dMG3_a3Z8hoL5igG-hO&sz=w800" onerror="handleDriveError(this, '1bRJmtvTDnszz8dMG3_a3Z8hoL5igG-hO', 'Thi+Cong+5')" alt="Thi công xây tường gạch Nhà phố Cẩm Lệ">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công xây tường gạch & tô trát phần thô Nhà phố Cẩm Lệ</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Hạng mục: Thi công phần thô</p>
                        </div>
                    </div>

                    <!-- Ảnh thực tế 6: 1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t -->
                    <div class="ux-box actual-item cursor-pointer" data-category="biet-thu" onclick="openDetailModal('Thi công hoàn thiện mặt tiền & chống thấm Biệt thự phố Đà Nẵng', 'Công trình thực tế - Biệt thự', 'https://drive.google.com/thumbnail?id=1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t&sz=w1200', 'Xử lý chống thấm sàn mái, ban công, sơn bả ngoại thất cao cấp và lắp đặt hệ cửa nhôm kính, lan can mặt tiền.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t&sz=w800" onerror="handleDriveError(this, '1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t', 'Thi+Cong+6')" alt="Thi công hoàn thiện mặt tiền Biệt thự phố">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công hoàn thiện mặt tiền & chống thấm Biệt thự phố Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Hạng mục: Thi công hoàn thiện</p>
                        </div>
                    </div>

                    <!-- Ảnh thực tế 7: 1UB12E_spzIvo7TNREjBJXUV9o_HVWOv_ -->
                    <div class="ux-box actual-item cursor-pointer" data-category="van-phong" onclick="openDetailModal('Thi công xây dựng & hoàn thiện Tòa nhà Văn phòng kết hợp Nhà ở', 'Công trình thực tế - Văn phòng', 'https://drive.google.com/thumbnail?id=1UB12E_spzIvo7TNREjBJXUV9o_HVWOv_&sz=w1200', 'Thi công trọn gói công trình văn phòng kết hợp nhà ở gia đình tại Đà Nẵng đảm bảo tiến độ và chất lượng kỹ thuật.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1UB12E_spzIvo7TNREjBJXUV9o_HVWOv_&sz=w800" onerror="handleDriveError(this, '1UB12E_spzIvo7TNREjBJXUV9o_HVWOv_', 'Thi+Cong+7')" alt="Thi công Tòa nhà Văn phòng kết hợp Nhà ở">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công xây dựng & hoàn thiện Tòa nhà Văn phòng kết hợp Nhà ở</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Hạng mục: Văn phòng & Nhà ở</p>
                        </div>
                    </div>

                    <!-- Ảnh thực tế 8: 1wHGqk7znpnGmrOjz4_EdpHnHK8xKyxkT -->
                    <div class="ux-box actual-item cursor-pointer" data-category="khach-san" onclick="openDetailModal('Nghiệm thu kết cấu & đổ bê tông sàn công trình Căn hộ cho thuê', 'Công trình thực tế - Khách sạn & Căn hộ', 'https://drive.google.com/thumbnail?id=1wHGqk7znpnGmrOjz4_EdpHnHK8xKyxkT&sz=w1200', 'Kiểm tra độ sụt bê tông, đầm dùi kỹ lưỡng và bảo dưỡng bê tông sàn đúng quy trình kỹ thuật của TSCONS.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1wHGqk7znpnGmrOjz4_EdpHnHK8xKyxkT&sz=w800" onerror="handleDriveError(this, '1wHGqk7znpnGmrOjz4_EdpHnHK8xKyxkT', 'Thi+Cong+8')" alt="Nghiệm thu kết cấu công trình Căn hộ cho thuê">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Nghiệm thu kết cấu & đổ bê tông sàn công trình Căn hộ cho thuê</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Hạng mục: Khách sạn – Căn hộ</p>
                        </div>
                    </div>

                    <!-- Ảnh thực tế 9: 1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn -->
                    <div class="ux-box actual-item cursor-pointer" data-category="nha-pho" onclick="openDetailModal('Thi công hoàn thiện nội ngoại thất Nhà phố trọn gói tại Đà Nẵng', 'Công trình thực tế - Nhà phố', 'https://drive.google.com/thumbnail?id=1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn&sz=w1200', 'Hoàn thiện ốp lát, trần thạch cao, sơn nước và lắp đặt thiết bị nội thất bàn giao trọn gói cho Chủ đầu tư.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn&sz=w800" onerror="handleDriveError(this, '1-eBgG9wF3I6_gyPir2CmCnwJg4sP7Bnn', 'Thi+Cong+9')" alt="Thi công hoàn thiện nội ngoại thất Nhà phố">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Thi công hoàn thiện nội ngoại thất Nhà phố trọn gói tại Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Hạng mục: Xây nhà trọn gói</p>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- 5. DANH MỤC CÁC DỰ ÁN Ở ĐÀ NẴNG (10 File ảnh Drive dự án Đà Nẵng, chia 2 cột trên điện thoại, không nhãn dán) -->
        <section id="du-an-da-nang" class="py-8 sm:py-12 bg-slate-50 border-t border-slate-200">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <div class="section-title-main">
                        <h2 class="section-title-text text-base sm:text-xl">DỰ ÁN TIÊU BIỂU TẠI ĐÀ NẴNG</h2>
                    </div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-1 mb-4">Các dự án Thiết kế Kiến trúc & Thi công Xây dựng trọn gói tiêu biểu của TSCONS tại TP Đà Nẵng</p>

                    <!-- Thanh lọc danh mục dự án Đà Nẵng nhỏ gọn -->
                    <div class="cat-pill-bar" id="danang-filter-bar">
                        <button onclick="filterProjects('danang', 'all', this)" class="cat-pill active">Tất cả dự án Đà Nẵng</button>
                        <button onclick="filterProjects('danang', 'nha-pho-dn', this)" class="cat-pill">Nhà phố Đà Nẵng</button>
                        <button onclick="filterProjects('danang', 'biet-thu-dn', this)" class="cat-pill">Biệt thự Đà Nẵng</button>
                        <button onclick="filterProjects('danang', 'can-ho-dn', this)" class="cat-pill">Căn hộ – Khách sạn – Văn phòng</button>
                    </div>
                </div>

                <!-- Grid 10 dự án ở Đà Nẵng: 2 cột trên điện thoại (grid-cols-2), 5 cột trên màn hình lớn -->
                <div id="danang-projects-grid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-2.5 sm:gap-4">

                    <!-- Dự án Đà Nẵng 1: 157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT -->
                    <div class="ux-box danang-item cursor-pointer" data-category="nha-pho-dn" onclick="openDetailModal('Dự án Nhà phố hiện đại 3 tầng – Quận Cẩm Lệ, TP Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT&sz=w1200', 'Thiết kế kiến trúc và thi công trọn gói nhà phố 3 tầng phong cách hiện đại, mặt tiền thoáng rộng kết hợp mảng xanh tự nhiên tại Cẩm Lệ, Đà Nẵng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT&sz=w800" onerror="handleDriveError(this, '157Suq0BLEh2zFs3X-uaNTN-ARDWhfjfT', 'Du+An+Da+Nang+1')" alt="Dự án Nhà phố hiện đại 3 tầng Cẩm Lệ Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Nhà phố hiện đại 3 tầng – Cẩm Lệ, Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Thiết kế & Thi công trọn gói</p>
                        </div>
                    </div>

                    <!-- Dự án Đà Nẵng 2: 1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff -->
                    <div class="ux-box danang-item cursor-pointer" data-category="biet-thu-dn" onclick="openDetailModal('Dự án Biệt thự phố 2 mặt tiền – Khu đô thị Hòa Xuân, Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff&sz=w1200', 'Công trình biệt thự phố cao cấp tại Khu đô thị sinh thái Hòa Xuân, Đà Nẵng với kiến trúc sang trọng và không gian mở.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff&sz=w800" onerror="handleDriveError(this, '1FVfIU7HJM8cAb-lO7wnjGvji6ZEvl7ff', 'Du+An+Da+Nang+2')" alt="Dự án Biệt thự phố Khu đô thị Hòa Xuân Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Biệt thự phố – Khu đô thị Hòa Xuân, Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Biệt thự hiện đại Đà Nẵng</p>
                        </div>
                    </div>

                    <!-- Dự án Đà Nẵng 3: 1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz -->
                    <div class="ux-box danang-item cursor-pointer" data-category="nha-pho-dn" onclick="openDetailModal('Dự án Nhà phố 3 tầng 1 tum – Phường An Khê, TP Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz&sz=w1200', 'Thiết kế và thi công hoàn thiện nhà phố 3 tầng 1 tum tối ưu thông gió và ánh sáng tự nhiên tại Phường An Khê, Đà Nẵng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz&sz=w800" onerror="handleDriveError(this, '1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz', 'Du+An+Da+Nang+3')" alt="Dự án Nhà phố 3 tầng 1 tum Phường An Khê Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Nhà phố 3 tầng 1 tum – Phường An Khê, Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Nhà phố trọn gói Đà Nẵng</p>
                        </div>
                    </div>

                    <!-- Dự án Đà Nẵng 4: 1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k -->
                    <div class="ux-box danang-item cursor-pointer" data-category="biet-thu-dn" onclick="openDetailModal('Dự án Biệt thự nghỉ dưỡng sân vườn – Quận Ngũ Hành Sơn, Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k&sz=w1200', 'Thiết kế kiến trúc và nội thất biệt thự nghỉ dưỡng không gian xanh tại Quận Ngũ Hành Sơn, TP Đà Nẵng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k&sz=w800" onerror="handleDriveError(this, '1I7lc3ghS0tyqh6Pq3xsZTidKsr0oT-8k', 'Du+An+Da+Nang+4')" alt="Dự án Biệt thự nghỉ dưỡng Ngũ Hành Sơn Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Biệt thự sân vườn – Ngũ Hành Sơn, Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Biệt thự nghỉ dưỡng Đà Nẵng</p>
                        </div>
                    </div>

                    <!-- Dự án Đà Nẵng 5: 1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N -->
                    <div class="ux-box danang-item cursor-pointer" data-category="can-ho-dn" onclick="openDetailModal('Dự án Căn hộ cho thuê & Khách sạn mini – Quận Sơn Trà, Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N&sz=w1200', 'Tư vấn thiết kế và thi công tòa nhà căn hộ dịch vụ cho thuê kết hợp lưu trú du lịch gần biển Sơn Trà, Đà Nẵng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N&sz=w800" onerror="handleDriveError(this, '1Q8VoCbT7s09UNaoI8GNcYdvKpJ2wz78N', 'Du+An+Da+Nang+5')" alt="Dự án Căn hộ cho thuê Quận Sơn Trà Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Căn hộ dịch vụ cho thuê – Quận Sơn Trà, Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Căn hộ – Khách sạn Đà Nẵng</p>
                        </div>
                    </div>

                    <!-- Dự án Đà Nẵng 6: 1tkQlfZJTkaSunwOIMhfnzkEG2YHwxhML -->
                    <div class="ux-box danang-item cursor-pointer" data-category="nha-pho-dn" onclick="openDetailModal('Dự án Nhà phố lệch tầng thông thoáng – Quận Hải Châu, Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=1tkQlfZJTkaSunwOIMhfnzkEG2YHwxhML&sz=w1200', 'Giải pháp kiến trúc nhà phố trung tâm Quận Hải Châu với giếng trời lớn và mặt tiền lam chắn nắng hiện đại.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1tkQlfZJTkaSunwOIMhfnzkEG2YHwxhML&sz=w800" onerror="handleDriveError(this, '1tkQlfZJTkaSunwOIMhfnzkEG2YHwxhML', 'Du+An+Da+Nang+6')" alt="Dự án Nhà phố Quận Hải Châu Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Nhà phố hiện đại – Quận Hải Châu, Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Thiết kế & Thi công trọn gói</p>
                        </div>
                    </div>

                    <!-- Dự án Đà Nẵng 7: 1An7LyMVwj3rhKZlsVnYQ2UrLe48IeTBF -->
                    <div class="ux-box danang-item cursor-pointer" data-category="nha-pho-dn" onclick="openDetailModal('Dự án Nhà phố kết hợp kinh doanh – Quận Thanh Khê, Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=1An7LyMVwj3rhKZlsVnYQ2UrLe48IeTBF&sz=w1200', 'Thiết kế mặt bằng tầng trệt kinh doanh showroom văn phòng và các tầng trên là không gian sinh hoạt tiện nghi cho gia đình.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1An7LyMVwj3rhKZlsVnYQ2UrLe48IeTBF&sz=w800" onerror="handleDriveError(this, '1An7LyMVwj3rhKZlsVnYQ2UrLe48IeTBF', 'Du+An+Da+Nang+7')" alt="Dự án Nhà phố kết hợp kinh doanh Thanh Khê Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Nhà phố kết hợp kinh doanh – Thanh Khê, Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Nhà phố thương mại Đà Nẵng</p>
                        </div>
                    </div>

                    <!-- Dự án Đà Nẵng 8: 1R1Da04pAYI9-NJz1IsAfa7pVKkuK7J-A -->
                    <div class="ux-box danang-item cursor-pointer" data-category="biet-thu-dn" onclick="openDetailModal('Dự án Biệt thự hiện đại 3 tầng – Khu Nam Việt Á, Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=1R1Da04pAYI9-NJz1IsAfa7pVKkuK7J-A&sz=w1200', 'Công trình biệt thự 3 tầng thiết kế hình khối kiến trúc mạnh mẽ, vật liệu ốp đá và gỗ nhựa ngoài trời bền bỉ.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1R1Da04pAYI9-NJz1IsAfa7pVKkuK7J-A&sz=w800" onerror="handleDriveError(this, '1R1Da04pAYI9-NJz1IsAfa7pVKkuK7J-A', 'Du+An+Da+Nang+8')" alt="Dự án Biệt thự Khu Nam Việt Á Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Biệt thự hiện đại 3 tầng – Khu Nam Việt Á, Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Biệt thự cao cấp Đà Nẵng</p>
                        </div>
                    </div>

                    <!-- Dự án Đà Nẵng 9: 1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80 -->
                    <div class="ux-box danang-item cursor-pointer" data-category="nha-pho-dn" onclick="openDetailModal('Dự án Nhà phố 2 tầng mái Nhật – Quận Liên Chiểu, Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80&sz=w1200', 'Mẫu nhà phố 2 tầng công năng 3 phòng ngủ, phòng thờ, sân để ô tô rộng rãi, chi phí đầu tư hợp lý tại Liên Chiểu, Đà Nẵng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80&sz=w800" onerror="handleDriveError(this, '1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80', 'Du+An+Da+Nang+9')" alt="Dự án Nhà phố 2 tầng Quận Liên Chiểu Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Nhà phố 2 tầng hiện đại – Quận Liên Chiểu, Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Xây nhà trọn gói Đà Nẵng</p>
                        </div>
                    </div>

                    <!-- Dự án Đà Nẵng 10: 1So_3V4rw1y7lHegiIkYmh2Z9UIdozAL4 -->
                    <div class="ux-box danang-item cursor-pointer" data-category="can-ho-dn" onclick="openDetailModal('Dự án Tòa nhà Văn phòng & Căn hộ – TP Đà Nẵng', 'Dự án tại Đà Nẵng', 'https://drive.google.com/thumbnail?id=1So_3V4rw1y7lHegiIkYmh2Z9UIdozAL4&sz=w1200', 'Thiết kế kiến trúc mặt tiền kính hiện đại kết hợp không gian văn phòng làm việc và căn hộ lưu trú cao cấp tại Đà Nẵng.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1So_3V4rw1y7lHegiIkYmh2Z9UIdozAL4&sz=w800" onerror="handleDriveError(this, '1So_3V4rw1y7lHegiIkYmh2Z9UIdozAL4', 'Du+An+Da+Nang+10')" alt="Dự án Tòa nhà Văn phòng và Căn hộ Đà Nẵng">
                        </div>
                        <div class="ux-box-text">
                            <h3 class="ux-box-title">Dự án Tòa nhà Văn phòng & Căn hộ cao cấp – TP Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500">Văn phòng – Căn hộ Đà Nẵng</p>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- 6. FORM YÊU CẦU VÀ BÁO GIÁ TRANG CHỦ (Giống mẫu MIỄN PHÍ TƯ VẤN trên tintruongthinh.com) -->
        <section id="bao-gia-tu-van" class="py-10 sm:py-14 bg-tsnavy text-white">
            <div class="flatsome-container">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                    
                    <!-- Cột thông tin bảng giá tham khảo -->
                    <div class="lg:col-span-5">
                        <span class="inline-block text-xs font-bold uppercase tracking-widest text-tsgold-light mb-2">BÁO GIÁ & DỰ TOÁN XÂY DỰNG</span>
                        <h2 class="text-xl sm:text-2xl md:text-3xl font-extrabold mb-3 leading-snug">
                            ĐĂNG KÝ NHẬN TƯ VẤN & BÁO GIÁ MIỄN PHÍ TỪ TSCONS
                        </h2>
                        <p class="text-xs sm:text-sm text-slate-200 leading-relaxed mb-5">
                            Quý khách hàng đang có kế hoạch xây dựng Nhà phố, Biệt thự, Căn hộ cho thuê hay Văn phòng tại Đà Nẵng? Hãy để lại thông tin để Kỹ sư TSCONS liên hệ tư vấn phương án thiết kế và lập bảng dự toán chi tiết sát thực tế nhất.
                        </p>
                        <div class="space-y-3 text-xs sm:text-sm">
                            <div class="flex items-center gap-3 bg-white/10 p-3 rounded-lg border border-white/15">
                                <i class="fa-solid fa-circle-check text-tsgold-light text-base"></i>
                                <span>Miễn phí 100% chi phí khảo sát hiện trạng & tư vấn mặt bằng công năng</span>
                            </div>
                            <div class="flex items-center gap-3 bg-white/10 p-3 rounded-lg border border-white/15">
                                <i class="fa-solid fa-circle-check text-tsgold-light text-base"></i>
                                <span>Miễn phí hồ sơ xin phép xây dựng & giảm đến 100% phí thiết kế khi thi công trọn gói</span>
                            </div>
                            <div class="flex items-center gap-3 bg-white/10 p-3 rounded-lg border border-white/15">
                                <i class="fa-solid fa-phone-volume text-tsgold-light text-base"></i>
                                <span>Hotline trực tiếp Kỹ sư trưởng: <strong class="text-tsgold-light">0933.333.254</strong></span>
                            </div>
                        </div>
                    </div>

                    <!-- Cột Form Yêu Cầu & Báo Giá (Chuẩn các trường của web mẫu tintruongthinh.com) -->
                    <div class="lg:col-span-7">
                        <div class="bg-white text-slate-800 rounded-xl p-5 sm:p-7 shadow-xl border-t-4 border-tsgold">
                            <h3 class="text-base sm:text-lg font-extrabold text-tsnavy uppercase text-center mb-1">
                                MIỄN PHÍ TƯ VẤN & BÁO GIÁ THI CÔNG
                            </h3>
                            <p class="text-xs text-slate-500 text-center mb-5">Điền thông tin công trình, TSCONS sẽ phản hồi ngay trong vòng 15 phút</p>

                            <form id="quote-form" onsubmit="submitQuoteForm(event)" class="space-y-3.5">
                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Họ tên Quý khách *</label>
                                        <input type="text" id="q-name" required placeholder="Nhập họ và tên..." class="w-full px-3.5 py-2.5 text-xs sm:text-sm rounded-lg border border-slate-300 focus:border-tsnavy focus:outline-none">
                                    </div>
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Số điện thoại / Zalo *</label>
                                        <input type="tel" id="q-phone" required placeholder="Nhập số điện thoại..." class="w-full px-3.5 py-2.5 text-xs sm:text-sm rounded-lg border border-slate-300 focus:border-tsnavy focus:outline-none">
                                    </div>
                                </div>

                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Loại công trình</label>
                                        <select id="q-type" class="w-full px-3.5 py-2.5 text-xs sm:text-sm rounded-lg border border-slate-300 bg-white focus:border-tsnavy focus:outline-none">
                                            <option value="Nhà phố">Nhà phố</option>
                                            <option value="Biệt thự">Biệt thự</option>
                                            <option value="Khách sạn – Căn hộ cho thuê – Phòng trọ">Khách sạn – Căn hộ cho thuê – Phòng trọ</option>
                                            <option value="Văn phòng">Văn phòng</option>
                                            <option value="Cải tạo sửa chữa">Cải tạo sửa chữa</option>
                                        </select>
                                    </div>
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Mức đầu tư dự kiến</label>
                                        <select id="q-budget" class="w-full px-3.5 py-2.5 text-xs sm:text-sm rounded-lg border border-slate-300 bg-white focus:border-tsnavy focus:outline-none">
                                            <option value="Chưa xác định">Chưa xác định</option>
                                            <option value="Dưới 500 triệu">Dưới 500 triệu</option>
                                            <option value="500 triệu - 1 tỷ">500 triệu - 1 tỷ</option>
                                            <option value="1 - 2 tỷ">1 - 2 tỷ</option>
                                            <option value="2 - 3 tỷ">2 - 3 tỷ</option>
                                            <option value="Trên 3 tỷ">Trên 3 tỷ</option>
                                        </select>
                                    </div>
                                </div>

                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3.5">
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Hạng mục quan tâm</label>
                                        <select id="q-service" class="w-full px-3.5 py-2.5 text-xs sm:text-sm rounded-lg border border-slate-300 bg-white focus:border-tsnavy focus:outline-none">
                                            <option value="Xây nhà trọn gói (Chìa khóa trao tay)">Xây nhà trọn gói (Chìa khóa trao tay)</option>
                                            <option value="Thi công phần thô & nhân công hoàn thiện">Thi công phần thô & nhân công hoàn thiện</option>
                                            <option value="Thiết kế Kiến trúc – Nội thất">Thiết kế Kiến trúc – Nội thất</option>
                                            <option value="Thi công hoàn thiện & Nội thất">Thi công hoàn thiện & Nội thất</option>
                                        </select>
                                    </div>
                                    <div>
                                        <label class="block text-xs font-bold text-slate-700 mb-1">Email / Địa điểm xây dựng</label>
                                        <input type="text" id="q-location" placeholder="VD: Cẩm Lệ, Đà Nẵng (Diện tích 5x20m)" class="w-full px-3.5 py-2.5 text-xs sm:text-sm rounded-lg border border-slate-300 focus:border-tsnavy focus:outline-none">
                                    </div>
                                </div>

                                <button type="submit" class="w-full py-3 rounded-lg bg-tsgold hover:bg-tsgold-dark text-white font-extrabold text-xs sm:text-sm uppercase tracking-wider transition shadow-md">
                                    <i class="fa-solid fa-paper-plane mr-1.5"></i> GỬI YÊU CẦU TƯ VẤN & BÁO GIÁ NGAY
                                </button>
                            </form>

                            <!-- Hộp thông báo gửi form thành công -->
                            <div id="quote-success-box" class="hidden mt-4 p-4 rounded-lg bg-emerald-50 border border-emerald-300 text-emerald-900 text-xs sm:text-sm">
                                <p class="font-bold mb-1"><i class="fa-solid fa-circle-check text-emerald-600 mr-1"></i> Đã tiếp nhận yêu cầu báo giá thành công!</p>
                                <p id="quote-success-detail" class="text-xs text-emerald-800"></p>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- 7. DANH MỤC CÁC BÀI VIẾT TRANG CHỦ (TIN TỨC & KINH NGHIỆM XÂY DỰNG - 2 cột trên điện thoại, không nhãn dán) -->
        <section id="tin-tuc" class="py-8 sm:py-12 bg-white border-t border-slate-200">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <div class="section-title-main">
                        <h2 class="section-title-text text-base sm:text-xl">TIN TỨC & KINH NGHIỆM XÂY DỰNG</h2>
                    </div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-1">Cập nhật kiến thức thi công, giải pháp chống thấm, cách nhiệt và báo giá xây dựng mới nhất</p>
                </div>

                <!-- Bài viết chia 2 cột trên giao diện điện thoại (grid-cols-2), 4 cột trên máy tính -->
                <div class="grid grid-cols-2 lg:grid-cols-4 gap-2.5 sm:gap-5">
                    
                    <article class="ux-box cursor-pointer" onclick="openDetailModal('Hướng dẫn bảo dưỡng bê tông móng và sàn đúng kỹ thuật xây dựng', 'Tin tức & Kỹ thuật thi công', 'https://drive.google.com/thumbnail?id=1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv&sz=w1000', 'Trong quá trình xây dựng công trình, bê tông móng và sàn đóng vai trò quyết định đến tuổi thọ ngôi nhà. TSCONS chia sẻ quy trình giữ ẩm, tưới nước bảo dưỡng bê tông tiêu chuẩn giúp đạt cường độ tối đa và hạn chế nứt bề mặt.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv&sz=w800" onerror="handleDriveError(this, '1Y1HUmEwHLU9YbOhwPzHpFwKQecXvLhUv', 'Bao+Duong+Be+Tong')" alt="Hướng dẫn bảo dưỡng bê tông móng đúng cách">
                        </div>
                        <div class="ux-box-text text-left">
                            <h3 class="ux-box-title text-left">Hướng dẫn bảo dưỡng bê tông móng và sàn đúng kỹ thuật xây dựng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500 line-clamp-2">Quy trình tưới nước giữ ẩm bê tông sau khi đổ giúp kết cấu đạt cường độ chuẩn và chống nứt sàn.</p>
                        </div>
                    </article>

                    <article class="ux-box cursor-pointer" onclick="openDetailModal('Giải pháp chống thấm và cách nhiệt hiệu quả khi thi công nhà ở Đà Nẵng', 'Tin tức & Kinh nghiệm xây nhà', 'https://drive.google.com/thumbnail?id=1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t&sz=w1000', 'Với đặc thù khí hậu nắng nóng và mùa mưa kéo dài tại miền Trung, việc xử lý chống thấm sàn mái, tường ngoài, nhà vệ sinh cùng giải pháp tường 2 lớp, gạch mát cách nhiệt ngay từ đầu giúp ngôi nhà luôn bền đẹp.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t&sz=w800" onerror="handleDriveError(this, '1_0OVVXoqQgYvoVEaZSC5iZh_SKGBbr-t', 'Giai+Phap+Chong+Tham')" alt="Giải pháp chống thấm và cách nhiệt hiệu quả">
                        </div>
                        <div class="ux-box-text text-left">
                            <h3 class="ux-box-title text-left">Giải pháp chống thấm và cách nhiệt hiệu quả khi thi công nhà ở Đà Nẵng</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500 line-clamp-2">Kinh nghiệm chống thấm sàn mái, sê nô, tường đứng và chống nóng hướng Tây cho nhà phố.</p>
                        </div>
                    </article>

                    <article class="ux-box cursor-pointer" onclick="openDetailModal('03 Nỗi lo lớn nhất khi xây nhà mà Chủ đầu tư nào cũng cần biết', 'Tư vấn xây nhà trọn gói', 'https://drive.google.com/thumbnail?id=1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz&sz=w1000', 'Kiểm soát ngân sách không phát sinh, lựa chọn vật tư chính hãng đúng hợp đồng và giám sát tiến độ thi công là 3 yếu tố cốt lõi được TSCONS cam kết minh bạch bằng văn bản.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz&sz=w800" onerror="handleDriveError(this, '1wkzckXZhRrWh3V2GIOfdqBmOwQTBVFhz', 'Kinh+Nghiem+Xay+Nha')" alt="03 Nỗi lo lớn nhất khi xây nhà">
                        </div>
                        <div class="ux-box-text text-left">
                            <h3 class="ux-box-title text-left">03 Nỗi lo lớn nhất khi xây nhà mà Chủ đầu tư nào cũng cần biết</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500 line-clamp-2">Giải pháp kiểm soát chi phí, chất lượng vật tư và tiến độ khi ký hợp đồng xây nhà trọn gói.</p>
                        </div>
                    </article>

                    <article class="ux-box cursor-pointer" onclick="openDetailModal('Thiết kế nội thất là gì? Tầm quan trọng của hồ sơ thiết kế đồng bộ', 'Kiến trúc & Nội thất', 'https://drive.google.com/thumbnail?id=1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80&sz=w1000', 'Thiết kế nội thất đồng bộ ngay từ giai đoạn kiến trúc giúp tối ưu không gian sử dụng, bố trí ổ cắm điện nước chính xác và tiết kiệm thời gian thi công hoàn thiện.')">
                        <div class="ux-box-image">
                            <img src="https://drive.google.com/thumbnail?id=1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80&sz=w800" onerror="handleDriveError(this, '1FdQEsiEBrIW5TiN22dvzV5g6amDPp-80', 'Thiet+Ke+Noi+That')" alt="Thiết kế nội thất là gì và tầm quan trọng">
                        </div>
                        <div class="ux-box-text text-left">
                            <h3 class="ux-box-title text-left">Thiết kế nội thất là gì? Tầm quan trọng của hồ sơ thiết kế đồng bộ</h3>
                            <p class="text-[11px] sm:text-xs text-slate-500 line-clamp-2">Lợi ích của việc thiết kế đồng bộ kiến trúc và nội thất trước khi khởi công xây dựng.</p>
                        </div>
                    </article>

                </div>
            </div>
        </section>

        <!-- 8. DANH MỤC CÁC ĐỐI TÁC (ĐỐI TÁC & THƯƠNG HIỆU VẬT TƯ ĐỒNG HÀNH CÙNG TSCONS) -->
        <section id="doi-tac" class="py-8 sm:py-12 bg-slate-50 border-t border-slate-200">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <div class="section-title-main">
                        <h2 class="section-title-text text-base sm:text-xl">ĐỐI TÁC & NHÀ CUNG CẤP VẬT TƯ UY TÍN</h2>
                    </div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-1">TSCONS cam kết sử dụng 100% vật tư xây dựng và hoàn thiện chính hãng từ các thương hiệu hàng đầu</p>
                </div>

                <!-- Chia 2 cột trên điện thoại, 6 cột trên máy tính -->
                <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-6 gap-2.5 sm:gap-4">
                    <div class="ux-box p-3.5 text-center justify-center items-center">
                        <div class="w-10 h-10 rounded-full bg-tsnavy/10 text-tsnavy flex items-center justify-center mb-1.5 font-extrabold text-xs">HP</div>
                        <h3 class="ux-box-title !mb-0.5">Thép Hòa Phát</h3>
                        <p class="text-[11px] text-slate-500">Thép xây dựng chính hãng</p>
                    </div>
                    <div class="ux-box p-3.5 text-center justify-center items-center">
                        <div class="w-10 h-10 rounded-full bg-tsgold/15 text-tsgold-dark flex items-center justify-center mb-1.5 font-extrabold text-xs">SIKA</div>
                        <h3 class="ux-box-title !mb-0.5">Chống thấm Sika</h3>
                        <p class="text-[11px] text-slate-500">Hóa chất xây dựng Thụy Sĩ</p>
                    </div>
                    <div class="ux-box p-3.5 text-center justify-center items-center">
                        <div class="w-10 h-10 rounded-full bg-tsnavy/10 text-tsnavy flex items-center justify-center mb-1.5 font-extrabold text-xs">JOTUN</div>
                        <h3 class="ux-box-title !mb-0.5">Sơn Jotun & Dulux</h3>
                        <p class="text-[11px] text-slate-500">Sơn nội ngoại thất cao cấp</p>
                    </div>
                    <div class="ux-box p-3.5 text-center justify-center items-center">
                        <div class="w-10 h-10 rounded-full bg-tsgold/15 text-tsgold-dark flex items-center justify-center mb-1.5 font-extrabold text-xs">AC</div>
                        <h3 class="ux-box-title !mb-0.5">Gỗ An Cường</h3>
                        <p class="text-[11px] text-slate-500">Vật liệu nội thất tiêu chuẩn</p>
                    </div>
                    <div class="ux-box p-3.5 text-center justify-center items-center">
                        <div class="w-10 h-10 rounded-full bg-tsnavy/10 text-tsnavy flex items-center justify-center mb-1.5 font-extrabold text-xs">XF</div>
                        <h3 class="ux-box-title !mb-0.5">Nhôm Xingfa</h3>
                        <p class="text-[11px] text-slate-500">Hệ cửa nhôm kính cao cấp</p>
                    </div>
                    <div class="ux-box p-3.5 text-center justify-center items-center">
                        <div class="w-10 h-10 rounded-full bg-tsgold/15 text-tsgold-dark flex items-center justify-center mb-1.5 font-extrabold text-xs">PANA</div>
                        <h3 class="ux-box-title !mb-0.5">Panasonic & Toto</h3>
                        <p class="text-[11px] text-slate-500">Thiết bị điện & vệ sinh</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- 9. ĐƯA FANPAGE FACEBOOK VÀ ẢNH/BẢN ĐỒ GOOGLE MAP RA NGOÀI TRANG CHỦ -->
        <section id="lien-he-map" class="py-8 sm:py-12 bg-white border-t border-slate-200">
            <div class="flatsome-container">
                <div class="section-title-container">
                    <div class="section-title-main">
                        <h2 class="section-title-text text-base sm:text-xl">KẾT NỐI FANPAGE & BẢN ĐỒ VỊ TRÍ TSCONS</h2>
                    </div>
                    <p class="text-xs sm:text-sm text-slate-600 mt-1">Địa chỉ: 702 Tôn Đản, Phường An Khê, TP Đà Nẵng — Hotline: 0933.333.254</p>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-stretch">
                    
                    <!-- CỘT 1: FANPAGE FACEBOOK TRANG CHỦ (https://www.facebook.com/tsconsvn) -->
                    <div class="lg:col-span-5 flex flex-col justify-between bg-slate-50 border border-slate-200 rounded-xl p-4 sm:p-5">
                        <div>
                            <div class="flex items-center justify-between gap-2 pb-3 mb-3 border-b border-slate-200">
                                <div class="flex items-center gap-2.5">
                                    <img 
                                        src="https://drive.google.com/thumbnail?id=1sFnkNtXw29XYmXWC973WTwwsRuqAOCO6&sz=w200" 
                                        onerror="handleDriveError(this, '1sFnkNtXw29XYmXWC973WTwwsRuqAOCO6', 'TSCONS')"
                                        alt="Logo TSCONS Fanpage" 
                                        class="w-11 h-11 rounded-lg object-contain bg-white border border-slate-200 p-0.5"
                                    >
                                    <div>
                                        <h3 class="text-sm font-extrabold text-tsnavy leading-tight">CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS</h3>
                                        <p class="text-xs text-blue-600 font-semibold">@tsconsvn • Fanpage Chính Thức</p>
                                    </div>
                                </div>
                            </div>

                            <!-- Khung nhúng Facebook Page Plugin kết hợp thẻ trực quan -->
                            <div class="w-full overflow-hidden rounded-lg border border-slate-200 bg-white mb-3">
                                <iframe 
                                    title="Fanpage TSCONS"
                                    src="https://www.facebook.com/plugins/page.php?href=https%3A%2F%2Fwww.facebook.com%2Ftsconsvn&tabs=timeline&width=500&height=260&small_header=true&adapt_container_width=true&hide_cover=false&show_facepile=true" 
                                    class="w-full h-[250px] border-0 overflow-hidden" 
                                    scrolling="no" 
                                    frameborder="0" 
                                    allowfullscreen="true" 
                                    allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share">
                                </iframe>
                            </div>
                        </div>

                        <div class="flex flex-wrap items-center justify-between gap-2 pt-2 border-t border-slate-200">
                            <span class="text-xs text-slate-600"><i class="fa-brands fa-facebook text-blue-600 mr-1"></i>Theo dõi nhật ký công trình mỗi ngày</span>
                            <a href="https://www.facebook.com/tsconsvn" target="_blank" rel="noopener" class="px-3.5 py-2 rounded-lg bg-blue-600 hover:bg-blue-700 text-white text-xs font-bold transition inline-flex items-center gap-1.5">
                                <i class="fa-brands fa-facebook-f"></i> Truy cập Fanpage TSCONS
                            </a>
                        </div>
                    </div>

                    <!-- CỘT 2: BẢN ĐỒ GOOGLE MAPS & ĐỊA CHỈ TRỤ SỞ TRANG CHỦ (702 Tôn Đản, Phường An Khê, TP Đà Nẵng) -->
                    <div class="lg:col-span-7 flex flex-col justify-between bg-slate-50 border border-slate-200 rounded-xl p-4 sm:p-5">
                        <div>
                            <div class="flex flex-wrap items-center justify-between gap-2 pb-3 mb-3 border-b border-slate-200">
                                <div>
                                    <h3 class="text-sm sm:text-base font-extrabold text-tsnavy">
                                        <i class="fa-solid fa-location-dot text-tsgold mr-1.5"></i>TRỤ SỞ: 702 TÔN ĐẢN, PHƯỜNG AN KHÊ, TP ĐÀ NẴNG
                                    </h3>
                                    <p class="text-xs text-slate-600">Bản đồ chỉ đường Google Maps đến văn phòng CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS</p>
                                </div>
                                <a href="https://share.google/h2WDAhIsZ9GoY5KxN" target="_blank" rel="noopener" class="px-3 py-1.5 rounded-lg bg-tsnavy hover:bg-tsnavy-light text-white text-xs font-bold transition inline-flex items-center gap-1.5 shrink-0">
                                    <i class="fa-solid fa-diamond-turn-right text-tsgold-light"></i> Mở Google Maps
                                </a>
                            </div>

                            <!-- Bản đồ Google Maps trực tiếp ngoài trang chủ -->
                            <div class="w-full h-[260px] sm:h-[290px] rounded-lg overflow-hidden border border-slate-300 bg-slate-200 relative">
                                <iframe 
                                    title="Bản đồ 702 Tôn Đản, Phường An Khê, TP Đà Nẵng"
                                    src="https://maps.google.com/maps?q=702%20T%C3%B4n%20%C4%90%E1%BA%A3n,%20An%20Kh%C3%AA,%20%C4%90%C3%A0%20N%E1%BA%B5ng&t=&z=16&ie=UTF8&iwloc=&output=embed" 
                                    class="w-full h-full border-0" 
                                    allowfullscreen="" 
                                    loading="lazy" 
                                    referrerpolicy="no-referrer-when-downgrade">
                                </iframe>
                            </div>
                        </div>

                        <div class="flex flex-wrap items-center justify-between gap-2 pt-3 mt-3 border-t border-slate-200 text-xs">
                            <div class="text-slate-700">
                                <strong>Địa chỉ:</strong> 702 Tôn Đản, Phường An Khê, TP Đà Nẵng | <strong>SĐT:</strong> <a href="tel:0933333254" class="text-tsgold-dark font-extrabold">0933.333.254</a>
                            </div>
                            <a href="https://share.google/h2WDAhIsZ9GoY5KxN" target="_blank" rel="noopener" class="text-tsnavy font-bold hover:underline inline-flex items-center gap-1">
                                <i class="fa-solid fa-up-right-from-square text-[11px]"></i> Xem vị trí trên Google Map
                            </a>
                        </div>
                    </div>

                </div>
            </div>
        </section>

    </main>

    <!-- ================= FOOTER (#footer chuẩn cấu trúc Flatsome) ================= -->
    <footer id="footer" class="bg-tsnavy-dark text-slate-200 pt-10 pb-6 border-t-4 border-tsgold">
        <div class="flatsome-container">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-12 gap-8 pb-8 border-b border-white/10">
                
                <!-- Thông tin công ty -->
                <div class="lg:col-span-5">
                    <div class="flex items-center gap-3 mb-3">
                        <img 
                            src="https://drive.google.com/thumbnail?id=1sFnkNtXw29XYmXWC973WTwwsRuqAOCO6&sz=w300" 
                            onerror="handleDriveError(this, '1sFnkNtXw29XYmXWC973WTwwsRuqAOCO6', 'TSCONS')"
                            alt="Logo TSCONS Footer" 
                            class="h-11 w-auto object-contain bg-white rounded p-1"
                        >
                        <div>
                            <h3 class="text-sm sm:text-base font-extrabold text-white">CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS</h3>
                            <p class="text-xs text-tsgold-light font-semibold">Website: tscons.com — MST: 0402234752</p>
                        </div>
                    </div>
                    <ul class="space-y-2 text-xs sm:text-sm text-slate-300">
                        <li class="flex items-start gap-2.5">
                            <i class="fa-solid fa-location-dot text-tsgold-light mt-1 shrink-0"></i>
                            <span><strong>Trụ sở:</strong> 702 Tôn Đản, Phường An Khê, TP Đà Nẵng</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-phone-volume text-tsgold-light shrink-0"></i>
                            <span><strong>Hotline / Zalo:</strong> <a href="tel:0933333254" class="text-white font-bold hover:text-tsgold-light">0933.333.254</a></span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-globe text-tsgold-light shrink-0"></i>
                            <span><strong>Website:</strong> <a href="https://tscons.com" class="hover:text-tsgold-light">https://tscons.com</a></span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-brands fa-facebook text-tsgold-light shrink-0"></i>
                            <span><strong>Fanpage:</strong> <a href="https://www.facebook.com/tsconsvn" target="_blank" rel="noopener" class="hover:text-tsgold-light">facebook.com/tsconsvn</a></span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-map-location-dot text-tsgold-light shrink-0"></i>
                            <span><strong>Google Maps:</strong> <a href="https://share.google/h2WDAhIsZ9GoY5KxN" target="_blank" rel="noopener" class="hover:text-tsgold-light underline">Xem bản đồ chỉ đường</a></span>
                        </li>
                    </ul>
                </div>

                <!-- Lĩnh vực hoạt động -->
                <div class="lg:col-span-3">
                    <h4 class="text-sm font-extrabold text-white uppercase tracking-wider mb-3 pb-1.5 border-b border-white/15">
                        LĨNH VỰC HOẠT ĐỘNG
                    </h4>
                    <ul class="space-y-2 text-xs sm:text-sm text-slate-300">
                        <li><a href="#linh-vuc-hoat-dong" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1.5"></i>Thiết kế Kiến trúc – Nội thất</a></li>
                        <li><a href="#linh-vuc-hoat-dong" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1.5"></i>Thi công phần thô</a></li>
                        <li><a href="#linh-vuc-hoat-dong" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1.5"></i>Thi công hoàn thiện</a></li>
                        <li><a href="#linh-vuc-hoat-dong" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1.5"></i>Xây nhà trọn gói Đà Nẵng</a></li>
                        <li><a href="#linh-vuc-hoat-dong" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1.5"></i>Thi công nội thất trọn gói</a></li>
                        <li><a href="#cong-trinh-thuc-te" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1.5"></i>Cải tạo – Sửa chữa công trình</a></li>
                    </ul>
                </div>

                <!-- Danh mục công trình & báo giá -->
                <div class="lg:col-span-4">
                    <h4 class="text-sm font-extrabold text-white uppercase tracking-wider mb-3 pb-1.5 border-b border-white/15">
                        DANH MỤC CÔNG TRÌNH & BÁO GIÁ
                    </h4>
                    <div class="grid grid-cols-2 gap-2 text-xs sm:text-sm text-slate-300">
                        <a href="#cong-trinh-thuc-te" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1"></i>Nhà phố hiện đại</a>
                        <a href="#cong-trinh-thuc-te" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1"></i>Biệt thự gia đình</a>
                        <a href="#cong-trinh-thuc-te" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1"></i>Khách sạn – Căn hộ</a>
                        <a href="#cong-trinh-thuc-te" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1"></i>Tòa nhà Văn phòng</a>
                        <a href="#du-an-da-nang" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1"></i>Dự án tại Đà Nẵng</a>
                        <a href="#bao-gia-tu-van" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1"></i>Báo giá thiết kế</a>
                        <a href="#bao-gia-tu-van" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1"></i>Báo giá phần thô</a>
                        <a href="#bao-gia-tu-van" class="hover:text-tsgold-light transition"><i class="fa-solid fa-angle-right text-tsgold-light mr-1"></i>Báo giá trọn gói</a>
                    </div>
                </div>

            </div>

            <div class="pt-5 flex flex-col sm:flex-row items-center justify-between gap-2 text-xs text-slate-400">
                <p>Copyright 2026 © <strong>CÔNG TY TNHH KIẾN TRÚC VÀ XÂY DỰNG TSCONS (tscons.com)</strong>. All rights reserved.</p>
                <p>Địa chỉ: 702 Tôn Đản, Phường An Khê, TP Đà Nẵng | Hotline: 0933.333.254</p>
            </div>
        </div>
    </footer>

    <!-- ================= CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE) TƯƠNG THÍCH MÁY TÍNH & ĐIỆN THOẠI ================= -->
    <div class="fixed bottom-4 right-3 sm:right-5 z-50 flex flex-col items-end gap-2.5">
        
        <!-- Nút Facebook Fanpage -->
        <a href="https://www.facebook.com/tsconsvn" target="_blank" rel="noopener" title="Fanpage Facebook TSCONS" class="flex items-center gap-2 bg-[#1877F2] hover:bg-blue-700 text-white px-3 py-2 rounded-full shadow-lg transition transform hover:scale-105">
            <span class="w-7 h-7 rounded-full bg-white text-[#1877F2] flex items-center justify-center font-bold text-sm shrink-0">
                <i class="fa-brands fa-facebook-f"></i>
            </span>
            <span class="text-xs font-bold pr-1">Facebook</span>
        </a>

        <!-- Nút Chat Zalo -->
        <a href="https://zalo.me/0933333254" target="_blank" rel="noopener" title="Chat Zalo 0933.333.254" class="flex items-center gap-2 bg-[#0068FF] hover:bg-blue-600 text-white px-3 py-2 rounded-full shadow-lg transition transform hover:scale-105">
            <span class="w-7 h-7 rounded-full bg-white text-[#0068FF] flex items-center justify-center font-extrabold text-[10px] shrink-0">
                Zalo
            </span>
            <span class="text-xs font-bold pr-1">Chat Zalo</span>
        </a>

        <!-- Nút Hotline Nổi Bật -->
        <a href="tel:0933333254" title="Gọi ngay Hotline 0933.333.254" class="pulse-btn flex items-center gap-2 bg-tsgold hover:bg-tsgold-dark text-white px-3.5 py-2.5 rounded-full shadow-xl transition transform hover:scale-105">
            <span class="w-7 h-7 rounded-full bg-white text-tsgold-dark flex items-center justify-center text-xs shrink-0">
                <i class="fa-solid fa-phone-volume"></i>
            </span>
            <span class="text-xs sm:text-sm font-extrabold pr-1">0933.333.254</span>
        </a>

    </div>

    <!-- ================= MODAL XEM CHI TIẾT CÔNG TRÌNH / SẢN PHẨM ================= -->
    <div id="detail-modal" class="fixed inset-0 z-50 hidden bg-black/75 flex items-center justify-center p-3 sm:p-6">
        <div class="bg-white rounded-xl max-w-2xl w-full overflow-hidden shadow-2xl border border-slate-200">
            <div class="flex items-center justify-between px-4 py-3 bg-tsnavy text-white">
                <span id="modal-category" class="text-xs font-bold uppercase tracking-wider text-tsgold-light">Công trình TSCONS</span>
                <button onclick="closeDetailModal()" class="w-7 h-7 rounded-full bg-white/15 hover:bg-white/25 flex items-center justify-center text-white">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div class="p-4 sm:p-6">
                <div class="w-full h-56 sm:h-80 bg-slate-100 rounded-lg overflow-hidden mb-4">
                    <img id="modal-image" src="" alt="Chi tiết công trình TSCONS" class="w-full h-full object-cover">
                </div>
                <h3 id="modal-title" class="text-base sm:text-lg font-extrabold text-tsnavy mb-2"></h3>
                <p id="modal-desc" class="text-xs sm:text-sm text-slate-600 leading-relaxed mb-5"></p>
                <div class="flex flex-wrap items-center justify-between gap-2 pt-3 border-t border-slate-200">
                    <a href="tel:0933333254" class="px-4 py-2 rounded-lg bg-tsgold hover:bg-tsgold-dark text-white font-bold text-xs sm:text-sm inline-flex items-center gap-1.5">
                        <i class="fa-solid fa-phone"></i> Tư vấn trực tiếp: 0933.333.254
                    </a>
                    <a href="#bao-gia-tu-van" onclick="closeDetailModal()" class="px-4 py-2 rounded-lg bg-tsnavy hover:bg-tsnavy-light text-white font-bold text-xs sm:text-sm">
                        Yêu cầu báo giá hạng mục này
                    </a>
                </div>
            </div>
        </div>
    </div>

</div>

<!-- ================= JAVASCRIPT XỬ LÝ SLIDER, BỘ LỌC DANH MỤC & FORM ================= -->
<script>
    // Xử lý dự phòng ảnh Google Drive tự động để luôn hiển thị tốt
    function handleDriveError(imgElement, fileId, fallbackLabel) {
        const currentSrc = imgElement.getAttribute('src') || '';
        if (!currentSrc.includes('lh3.googleusercontent.com')) {
            imgElement.src = 'https://lh3.googleusercontent.com/d/' + fileId + '=w1000';
        } else {
            imgElement.onerror = null;
            imgElement.src = 'https://placehold.co/800x600/0f2b52/ffffff?text=' + fallbackLabel;
        }
    }

    // Điều khiển Menu Điện thoại
    function toggleMobileMenu() {
        const drawer = document.getElementById('mobile-menu-drawer');
        drawer.classList.toggle('hidden');
    }

    // Điều khiển 2 Banner Tự Trượt Chuyên Nghiệp
    let currentSlideIndex = 0;
    const totalSlides = 2;
    let slideInterval = null;

    function showSlide(index) {
        currentSlideIndex = (index + totalSlides) % totalSlides;
        for (let i = 0; i < totalSlides; i++) {
            const slideEl = document.getElementById('slide-' + i);
            const dotEl = document.getElementById('dot-' + i);
            if (i === currentSlideIndex) {
                slideEl.classList.add('active');
                dotEl.className = 'w-6 h-2 rounded-full bg-tsgold transition-all';
            } else {
                slideEl.classList.remove('active');
                dotEl.className = 'w-2.5 h-2 rounded-full bg-white/60 transition-all';
            }
        }
    }

    function nextSlide() {
        showSlide(currentSlideIndex + 1);
        resetSlideTimer();
    }

    function prevSlide() {
        showSlide(currentSlideIndex - 1);
        resetSlideTimer();
    }

    function goToSlide(index) {
        showSlide(index);
        resetSlideTimer();
    }

    function resetSlideTimer() {
        if (slideInterval) clearInterval(slideInterval);
        slideInterval = setInterval(() => {
            showSlide(currentSlideIndex + 1);
        }, 5000);
    }

    // Lọc công trình thực tế và dự án Đà Nẵng
    function filterProjects(group, category, btnElement) {
        const itemClass = group === 'actual' ? '.actual-item' : '.danang-item';
        const barId = group === 'actual' ? 'actual-filter-bar' : 'danang-filter-bar';
        const items = document.querySelectorAll(itemClass);

        items.forEach(item => {
            const itemCat = item.getAttribute('data-category');
            if (category === 'all' || itemCat === category) {
                item.classList.remove('hidden');
            } else {
                item.classList.add('hidden');
            }
        });

        if (btnElement) {
            const buttons = document.getElementById(barId).querySelectorAll('.cat-pill');
            buttons.forEach(btn => btn.classList.remove('active'));
            btnElement.classList.add('active');
        }
    }

    // Mở & Đóng Modal Xem Chi Tiết
    function openDetailModal(title, category, imageSrc, desc) {
        document.getElementById('modal-title').textContent = title;
        document.getElementById('modal-category').textContent = category;
        document.getElementById('modal-image').src = imageSrc;
        document.getElementById('modal-desc').textContent = desc;
        document.getElementById('detail-modal').classList.remove('hidden');
    }

    function closeDetailModal() {
        document.getElementById('detail-modal').classList.add('hidden');
    }

    // Xử lý gửi Form Báo Giá trang chủ
    function submitQuoteForm(event) {
        event.preventDefault();
        const name = document.getElementById('q-name').value.trim();
        const phone = document.getElementById('q-phone').value.trim();
        const type = document.getElementById('q-type').value;
        const budget = document.getElementById('q-budget').value;
        const service = document.getElementById('q-service').value;

        const successBox = document.getElementById('quote-success-box');
        const detailText = document.getElementById('quote-success-detail');
        detailText.textContent = 'Cảm ơn ' + name + ' (' + phone + '). Yêu cầu tư vấn "' + service + ' - ' + type + ' (' + budget + ')" đã được chuyển tới bộ phận Kỹ thuật TSCONS. Chúng tôi sẽ liên hệ lại ngay qua SĐT/Zalo 0933.333.254!';
        successBox.classList.remove('hidden');
        document.getElementById('quote-form').reset();
    }

    window.onload = function () {
        resetSlideTimer();
    };
</script>

</body>
</html>
