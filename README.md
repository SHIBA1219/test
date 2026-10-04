<!DOCTYPE html>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>個人作品集 / 一頁式網站</title>
    <style>
        /* 平滑滾動效果 */
        html {
            scroll-behavior: smooth;
        }

        body {
            margin: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            color: #333;
            line-height: 1.6;
        }

        /* 導覽列 */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            z-index: 1000;
        }

        nav {
            max-width: 1000px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        .logo {
            font-weight: bold;
            font-size: 1.2rem;
            color: #2563eb;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 1.5rem;
            margin: 0;
            padding: 0;
        }

        nav a {
            text-decoration: none;
            color: #4b5563;
            font-weight: 500;
            transition: color 0.2s;
        }

        nav a:hover {
            color: #2563eb;
        }

        /* 區塊共同樣式 */
        section {
            padding: 100px 20px 80px;
            min-height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        .container {
            max-width: 800px;
            width: 100%;
        }

        /* 首頁 Banner 區塊 */
        #home {
            background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
        }

        #home h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #1e3a8a;
        }

        .btn {
            display: inline-block;
            background: #2563eb;
            color: white;
            padding: 0.8rem 1.8rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 500;
            margin-top: 1rem;
        }

        .btn:hover {
            background: #1d4ed8;
        }

        /* 關於我們區塊 */
        #about {
            background: #ffffff;
        }

        /* 服務項目區塊 */
        #services {
            background: #f8fafc;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .card {
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }

        /* 聯絡我們區塊 */
        #contact {
            background: #ffffff;
        }

        footer {
            background: #1e293b;
            color: white;
            text-align: center;
            padding: 1.5rem;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <!-- 固定導覽列 -->
    <header>
        <nav>
            <div class="logo">MyBrand</div>
            <ul>
                <li><a href="#home">首頁</a></li>
                <li><a href="#about">關於我們</a></li>
                <li><a href="#services">服務項目</a></li>
                <li><a href="#contact">聯絡我們</a></li>
            </ul>
        </nav>
    </header>

    <!-- 1. 首頁區塊 -->
    <section id="home">
        <div class="container">
            <h1>打造你的專屬品牌形象</h1>
            <p>這是一個簡單、快速且具備響應式設計的一頁式網站範本。</p>
            <a href="#contact" class="btn">立即聯絡</a>
        </div>
    </section>

    <!-- 2. 關於我們區塊 -->
    <section id="about">
        <div class="container">
            <h2>關於我們</h2>
            <p>這裡可以介紹個人背景、品牌理念或是產品的核心價值。單頁式設計能夠讓訪客專注於最關鍵的資訊。</p>
        </div>
    </section>

    <!-- 3. 服務項目區塊 -->
    <section id="services">
        <div class="container">
            <h2>服務項目</h2>
            <div class="grid">
                <div class="card">
                    <h3>網頁設計</h3>
                    <p>提供客製化且符合行動裝置瀏覽的網頁排版設計。</p>
                </div>
                <div class="card">
                    <h3>前端開發</h3>
                    <p>使用最新技術建構高效能、載入速度極快的網站。</p>
                </div>
                <div class="card">
                    <h3>SEO 優化</h3>
                    <p>優化網站結構與內容，提升搜尋引擎排名與曝光度。</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 4. 聯絡我們區塊 -->
    <section id="contact">
        <div class="container">
            <h2>聯絡我們</h2>
            <p>如果有任何合作想法或需求，歡迎透過以下方式聯繫：</p>
            <p>Email: contact@example.com</p>
            <a href="mailto:contact@example.com" class="btn">寄送 Email</a>
        </div>
    </section>

    <footer>
        <p>© 2026 MyBrand. All rights reserved.</p>
    </footer>

</body>
</html>
