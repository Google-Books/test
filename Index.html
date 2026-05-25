<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Google Books - Premium Laser Portal</title>
    <style>
        /* =============================================================
           ۱. متغیرهای رنگی پیشرفته لیزری تم تیره وب‌سایت شما
           ============================================================= */
        :root {
            --bg-dark-premium: #0d1326;   /* رنگ دقیق پس‌زمینه تیره و لوکس پوسته تصویر */
            --row-bg: rgba(255, 255, 255, 0.02); /* پس‌زمینه شیشه‌ای فوق‌العاده ملایم ردیف‌ها */
            --laser-glow-color: rgba(139, 92, 246, 0.25); /* هاله نئونی لیزری بنفش-فیروزه‌ای */
            --text-gray-muted: #7f92a5;   /* خاکستری ملایم برای توضیحات ارشیوها */
            --transition-smooth: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }

        * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'Segoe UI', system-ui, sans-serif; }

        body {
            background-color: var(--bg-dark-premium); color: #ffffff; display: flex; flex-direction: column;
            align-items: center; justify-content: flex-start; min-height: 100vh; 
            /* ایجاد فضای خالی لازم در پایین صفحه برای جلوگیری از افتادن بنر شناور روی ردیف‌ها */
            padding: 60px 24px 150px 24px;
            position: relative; overflow-x: hidden; -webkit-font-smoothing: antialiased;
        }

        /* =============================================================
           ۲. ساختار هدر و عنوان اصلی صفحه
           ============================================================= */
        .header-container { width: 100%; max-width: 900px; margin-bottom: 50px; }
        
        .back-btn {
            display: inline-flex; align-items: center; color: #ffffff; text-decoration: none;
            font-size: 16px; font-weight: 600; margin-bottom: 35px; transition: var(--transition-smooth);
        }
        .back-btn:hover { transform: translateX(-4px); color: #00f0ff; }

        .main-title { 
            font-size: 2.4rem; font-weight: 900; text-align: center; line-height: 1.35; letter-spacing: -0.5px;
            background: linear-gradient(180deg, #ffffff 0%, #b0c4de 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent;
            text-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
        }

        /* =============================================================
           ۳. استایل ردیف‌های آرشیو با دیواره خط لیزری بسیار قشنگ
           ============================================================= */
        .archive-list { width: 100%; max-width: 900px; display: flex; flex-direction: column; gap: 18px; }

        .archive-row {
            display: flex; align-items: center; width: 100%; background-color: var(--row-bg);
            border: 1px solid rgba(139, 92, 246, 0.2); border-radius: 20px; padding: 22px 28px;
            text-decoration: none; color: #ffffff; transition: var(--transition-smooth);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2), 0 0 10px var(--laser-glow-color);
        }
        
        .archive-row:hover {
            background-color: rgba(255, 255, 255, 0.04); border-color: #00f0ff;
            transform: translateY(-3px) scale(1.01); 
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.5), 0 0 20px rgba(0, 240, 255, 0.3);
        }

        /* فریم کپسولی/دایره‌ای شیک دور آیکون‌ها */
        .icon-box { 
            display: flex; align-items: center; justify-content: center; width: 52px; height: 52px;
            background: rgba(139, 92, 246, 0.1); border: 1px solid rgba(139, 92, 246, 0.3);
            border-radius: 50%; margin-right: 24px; flex-shrink: 0; transition: var(--transition-smooth);
        }
        .archive-row:hover .icon-box { background: rgba(0, 240, 255, 0.15); border-color: #00f0ff; box-shadow: 0 0 12px rgba(0, 240, 255, 0.4); }

        /* استایل آیکون‌های شاهکار چندرنگ کتاب */
        .book-icon-master { width: 34px; height: 34px; transition: var(--transition-smooth); }
        .archive-row:hover .book-icon-master { transform: scale(1.1) rotate(-3deg); filter: drop-shadow(0 0 8px #00f0ff); }

        .text-box { display: flex; flex-direction: column; gap: 6px; }
        .archive-title { font-size: 18px; font-weight: 700; letter-spacing: -0.1px; transition: var(--transition-smooth); }
        .archive-row:hover .archive-title { color: #00f0ff; text-shadow: 0 0 8px rgba(0, 240, 255, 0.3); }
        .archive-desc { font-size: 14px; color: var(--text-gray-muted); line-height: 1.45; }

        /* =============================================================
           ۴. سیستم استایل هوشمند بنر تبلیغاتی شناور پایین صفحه (رسپانسیو)
           ============================================================= */
        .floating-ad-container {
            position: fixed; bottom: 0; left: 0; width: 100%; z-index: 99999;
            background: rgba(13, 19, 38, 0.95); backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px); border-top: 1px solid rgba(255, 255, 255, 0.05);
            padding: 10px 0; display: flex; justify-content: center; align-items: center;
            box-shadow: 0 -10px 30px rgba(0, 0, 0, 0.5);
        }

        /* کانتینرهای مجزا برای مدیریت اندازه بنر بر اساس سایز مانیتور */
        .ad-desktop, .ad-tablet, .ad-mobile { display: none; }

        /* دسکتاپ و مانیتور: بنر ۷۲۸ در ۹۰ روشن می‌شود */
        @media (min-width: 992px) { .ad-desktop { display: block; } }

        /* تبلت و موبایل بزرگ: بنر متوسط ۴۶۸ در ۶۰ روشن می‌شود */
        @media (min-width: 601px) and (max-width: 991px) { .ad-tablet { display: block; } }

        /* موبایل‌های هوشمند کوچک: بنر کوچک ۳۲۰ در ۵۰ روشن می‌شود */
        @media (max-width: 600px) {
            .ad-mobile { display: block; }
            body { padding: 40px 16px 110px 16px; }
            .main-title { font-size: 1.6rem; }
            .archive-row { padding: 18px; border-radius: 16px; }
            .icon-box { margin-right: 16px; width: 46px; height: 44px; }
            .book-icon-master { width: 28px; height: 28px; }
            .archive-title { font-size: 16px; }
            .archive-desc { font-size: 12px; }
        }
    </style>
</head>
<body>

    <div class="header-container">
        <a href="index.html" class="back-btn">&larr; Back</a>
        <h1 class="main-title">We Try Our Best To Provide You The Best And Largest Sources!</h1>
    </div>

    <div class="archive-list">
        <!-- آرشیو ۱: اقیانوس کتاب‌ها -->
        <a href="https://oceanofpdf.com" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <defs>
                        <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="100%">
                            <stop offset="0%" style="stop-color:#00f0ff;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#ec4899;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <path d="M2 26s5-4 14-4 14 4 14 4V6s-5-4-14-4-14 4-14 4v20z" fill="url(#grad1)" />
                    <path d="M16 2v20" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round"/>
                    <path d="M6 8h6M6 12h6M6 16h4M20 8h6M20 12h6M22 16h4" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The First Archive</div>
                <div class="archive-desc">The fastest and safest library in the world with new books and romances.</div>
            </div>
        </a>

        <!-- آرشیو ۲: وی‌لیب -->
        <a href="https://welib.st" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <defs>
                        <linearGradient id="grad2" x1="0%" y1="0%" x2="100%" y2="100%">
                            <stop offset="0%" style="stop-color:#38bdf8;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#a855f7;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <path d="M4 24s4-3 12-3 12 3 12 3V7s-4-3-12-3-12 3-12 3v17z" fill="url(#grad2)" opacity="0.8"/>
                    <circle cx="16" cy="14" r="6" fill="none" stroke="#00f0ff" stroke-width="2" />
                    <line x1="20.5" y1="18.5" x2="26" y2="24" stroke="#00f0ff" stroke-width="2.5" stroke-linecap="round"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Second Archive</div>
                <div class="archive-desc">PDF search engine with an extensive categorized database.</div>
            </div>
        </a>

        <!-- آرشیو ۳: اینترنت آرشیو -->
        <a href="https://archive.org" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <defs>
                        <linearGradient id="grad3" x1="0%" y1="0%" x2="0%" y2="100%">
                            <stop offset="0%" style="stop-color:#eab308;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#3b82f6;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <path d="M4 24h24v3H4z" fill="#eab308"/>
                    <path d="M6 21h3v3H6zm5 0h3v3h-3zm5 0h3v3h-3zm5 0h3v3h-3zm5 0h3v3h-3z" fill="#ffffff"/>
                    <path d="M5 11l11-7 11 7v3H5z" fill="url(#grad3)"/>
                    <path d="M2 25c0 1.1.9 2 2 2h24c1.1 0 2-.9 2-2s-.9-2-2-2H4c-1.1 0-2 .9-2 2z" fill="#ffffff"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Third Archive</div>
                <div class="archive-desc">Digital library with millions of books, articles, magazines, plus movies, music.</div>
            </div>
        </a>

        <!-- آرشیو ۴: ویکی‌سورس -->
        <a href="https://wikisource.org" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <defs>
                        <linearGradient id="grad4" x1="0%" y1="0%" x2="100%" y2="100%">
                            <stop offset="0%" style="stop-color:#f43f5e;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#f97316;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <path d="M19 2H6c-1.1 0-2 .9-2 2v24c0 1.1.9 2 2 2h20c1.1 0 2-.9 2-2V11l-9-9z" fill="url(#grad4)"/>
                    <path d="M19 2v9h9M8 12h10M8 17h16M8 22h16" stroke="#ffffff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Fourth Archive</div>
                <div class="archive-desc">Free digital library with full-text books, novels, historical documents, and speeches.</div>
            </div>
        </a>

        <!-- آرشیو ۵: اوپن لایبرری -->
        <a href="https://openlibrary.org" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <defs>
                        <linearGradient id="grad5" x1="0%" y1="0%" x2="100%" y2="100%">
                            <stop offset="0%" style="stop-color:#10b981;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#059669;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <rect x="4" y="4" width="24" height="24" rx="4" fill="url(#grad5)"/>
                    <path d="M9 8h2v16H9zm5 0h3v16h-3zm6 0h3v16h-3z" fill="#ffffff" opacity="0.9"/>
                    <line x1="4" y1="14" x2="28" y2="14" stroke="#0d1326" stroke-width="2"/>
                    <line x1="4" y1="20" x2="28" y2="20" stroke="#0d1326" stroke-width="2"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Fifth Archive</div>
                <div class="archive-desc">Old archive with millions of valuable scanned vintage books.</div>
            </div>
        </a>

        <!-- آرشیو mechanism: گوگل اسکالر -->
        <a href="https://google.com" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <defs>
                        <linearGradient id="grad6" x1="0%" y1="0%" x2="100%" y2="100%">
                            <stop offset="0%" style="stop-color:#06b6d4;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#3b82f6;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <path d="M16 4L3 10l13 6 13-6-13-6z" fill="url(#grad6)"/>
                    <path d="M7 13.5V20c0 2 4 4 9 4s9-2 9-4v-6.5" fill="none" stroke="#00f0ff" stroke-width="2"/>
                    <path d="M25 11v8" fill="none" stroke="#ffffff" stroke-width="2"/>
                    <circle cx="25" cy="19" r="2" fill="#ffffff"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Sixth Archive</div>
                <div class="archive-desc">Access millions of articles and books with a fast and reliable download system.</div>
            </div>
        </a>
        <!-- آرشیو ۷: جیوتمبرگ -->
        <a href="https://gutenberg.org" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <rect x="6" y="4" width="20" height="24" rx="3" fill="#f59e0b" />
                    <line x1="10" y1="9" x2="22" y2="9" stroke="#0d1326" stroke-width="2"/>
                    <line x1="10" y1="14" x2="22" y2="14" stroke="#0d1326" stroke-width="2"/>
                    <line x1="10" y1="19" x2="18" y2="19" stroke="#0d1326" stroke-width="2"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Seventh Archive</div>
                <div class="archive-desc">The oldest digital library project focused on classic works.</div>
            </div>
        </a>

        <!-- آرشیو ۸: منی‌بوکس -->
        <a href="https://manybooks.net" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <path d="M2 26s5-4 14-4 14 4 14 4V6s-5-4-14-4-14 4-14 4v20z" fill="#f59e0b" />
                    <path d="M16 2v20" stroke="#0d1326" stroke-width="2"/>
                    <polygon points="16,8 18,12 22,12 19,15 20,19 16,17 12,19 13,15 10,12 14,12" fill="#ffffff"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Eighth Archive</div>
                <div class="archive-desc">Simple and beautiful interface with suggested book topics.</div>
            </div>
        </a>

        <!-- آرشیو ۹: اوپن‌استکس -->
        <a href="https://openstax.org" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <defs>
                        <linearGradient id="grad8" x1="0%" y1="0%" x2="100%" y2="0%">
                            <stop offset="0%" style="stop-color:#6366f1;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#4f46e5;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <rect x="6" y="12" width="20" height="14" rx="3" fill="url(#grad8)"/>
                    <rect x="4" y="6" width="20" height="14" rx="3" fill="#38bdf8"/>
                    <path d="M4 16h20M6 22h20" stroke="#ffffff" stroke-width="2"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Ninth Archive</div>
                <div class="archive-desc">Millions of high-quality, standard-compliant textbooks (specially designed for students).</div>
            </div>
        </a>

        <!-- آرشیو ۱۰: استاندارد ایبوکس -->
        <a href="https://standardebooks.org" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <defs>
                        <linearGradient id="grad9" x1="0%" y1="0%" x2="100%" y2="100%">
                            <stop offset="0%" style="stop-color:#a855f7;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#ec4899;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <polygon points="16,2 28,10 24,26 8,26 4,10" fill="url(#grad9)"/>
                    <polygon points="16,6 24,12 20,22 12,22 8,12" fill="#ffffff" opacity="0.3"/>
                    <path d="M12 14h8M10 18h12" stroke="#ffffff" stroke-width="1.5" stroke-linecap="round"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Tenth Archive</div>
                <div class="archive-desc">Free high-quality classic ebooks in EPUB and Kindle formats.</div>
            </div>
        </a>

        <!-- آرشیو ۱۱: بوک‌بون -->
        <a href="https://bookboon.com" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <path d="M16 4L4 12v12l12 4 12-4V12L16 4z" fill="#1d4ed8"/>
                    <path d="M16 4v24l12-4V12L16 4z" fill="#2563eb"/>
                    <path d="M7 13.5l9 3.5 9-3.5" fill="none" stroke="#00f0ff" stroke-width="2"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Eleventh Archive</div>
                <div class="archive-desc">Free academic and business books, great for students and learning skills.</div>
            </div>
        </a>

        <!-- آرشیو ۱۲: فری ایبوکس -->
        <a href="https://free-ebooks.net" target="_blank" class="archive-row">
            <div class="icon-box">
                <svg class="book-icon-master" viewBox="0 0 32 32">
                    <defs>
                        <linearGradient id="grad11" x1="0%" y1="0%" x2="100%" y2="100%">
                            <stop offset="0%" style="stop-color:#00f0ff;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#3b82f6;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    <path d="M26 15a7 7 0 0 0-13.93-1A5.5 5.5 0 0 0 3 19.5 5.5 5.5 0 0 0 8.5 25h17a4.5 4.5 0 0 0 0-9z" fill="url(#grad11)"/>
                    <path d="M12 14v6h4l-4 4-4-4h4v-6z" fill="#ffffff"/>
                </svg>
            </div>
            <div class="text-box">
                <div class="archive-title">The Twelfth Archive</div>
                <div class="archive-desc">Free e-Books Thousands of novels, educational and scientific ebooks in PDF or EPUB.</div>
            </div>
        </a>

    </div> <!-- انتهای کانتینر .archive-list -->

    <!-- =============================================================
       ۵. بخش کانتینر هوشمند تبلیغاتی شناور پایین صفحه (تست سایز خودکار)
       ============================================================= */ -->
    <div class="floating-ad-container">
        
        <!-- حالت لپ‌تاپ و مانیتور بزرگ (728x90) -->
        <div class="ad-desktop">
            <script>
                atOptions = { 'key' : '30c18b6ace1c2676949453fd6ac33776', 'format' : 'iframe', 'height' : 90, 'width' : 728, 'params' : {} };
            </script>
            <script src="https://speedingdeadlyplays.com"></script>
        </div>

        <!-- حالت تبلت و لپ‌تاپ کوچک (468x60) -->
        <div class="ad-tablet">
            <script>
                atOptions = { 'key' : '27bf67bdd07dd3734a6fdff8c7879c99', 'format' : 'iframe', 'height' : 60, 'width' : 468, 'params' : {} };
            </script>
            <script src="https://speedingdeadlyplays.com"></script>
        </div>

        <!-- حالت موبایل هوشمند با کمترین عرض مانیتور (320x50) -->
        <div class="ad-mobile">
            <script>
                atOptions = { 'key' : '3b8048b78e2b0fb0b882483f96fca8a2', 'format' : 'iframe', 'height' : 50, 'width' : 320, 'params' : {} };
            </script>
            <script src="https://speedingdeadlyplays.com"></script>
        </div>

    </div>

    <!-- اسکریپت فعال و دائمی سیستم تبلیغاتی سوشیال بار شما بدون تغییر -->
    <script src="https://speedingdeadlyplays.com"></script>

</body>
</html>
