# Weblajax
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>دیجی‌کالا - نسخه مشابه</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- هدر سایت -->
    <header class="header">
        <div class="logo">
            <img src="images/logo.png" alt="دیجی‌کالا">
        </div>
        <div class="search-box">
            <input type="text" placeholder="جستجو در دیجی‌کالا...">
            <button><i class="fas fa-search"></i></button>
        </div>
        <div class="user-actions">
            <a href="#"><i class="fas fa-user"></i> ورود | ثبت‌نام</a>
            <a href="#"><i class="fas fa-shopping-cart"></i> سبد خرید</a>
        </div>
    </header>

    <!-- منوی اصلی -->
    <nav class="main-menu">
        <ul>
            <li><a href="#">خانه</a></li>
            <li><a href="#">کالاهای سوپرمارکتی</a></li>
            <li><a href="#">پرفروش‌ترین‌ها</a></li>
            <li><a href="#">تخفیف‌ها و پیشنهادها</a></li>
            <li><a href="#">دسته‌بندی‌ها</a></li>
        </ul>
    </nav>

    <!-- اسلایدر محصولات -->
    <section class="product-slider">
        <div class="slider-container">
            <!-- محتوای اسلایدر -->
     </div>
    </section>

    <!-- بخش محصولات -->
    <section class="products">
        <h2>پرفروش‌ترین محصولات</h2>
        <div class="product-grid">
            <!-- محصولات اینجا نمایش داده می‌شوند -->
        </div>
    </section>

    <!-- فوتر -->
    <footer class="footer">
        <div class="footer-sections">            <!-- بخش‌های فوتر -->
        </div>
    </footer>

    <script src="js/script.js"></script>
</body>
</html>
Online trading 
</body>
</html>
/* تنظیمات پایه */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    background-color: #f5f5f5;
    color: #333;
    direction: rtl;
}

/* استایل هدر */
.header {
    background-color: #a62626;
    padding: 15px 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.logo img {
    height: 40px;
}

.search-box {
    display: flex;
    width: 50%;
}

.search-box input {
    width: 100%;
    padding: 10px;
    border: none;
    border-radius: 5px 0 0 5px;
}

.search-box button {
    background-color: #424750;
    color: white;
    border: none;
    padding: 0 15px;
    border-radius: 0 5px 5px 0;
    cursor: pointer;
}

.user-actions a {
    color: white;
    margin-right: 15px;
    text-decoration: none;
}

/* استایل منوی اصلی */
.main-menu {
    background-color: #424750;
    padding: 10px 0;
}

.main-menu ul {
    display: flex;
    list-style: none;
}

.main-menu li {
    margin-left: 20px;
}

.main-menu a {
    color: white;
    text-decoration: none;
    font-size: 14px;
}

/* استایل اسلایدر */
.product-slider {
    margin: 20px 0;
    background-color: white;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 1px 3px rgba(0,0,0,0.1);
}

/* استایل محصولات */
.products {
    margin: 20px 0;
}

.products h2 {
    margin-bottom: 15px;
    font-size: 18px;
}

.product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 15px;
}

/* استایل فوتر */
.footer {
    background-color: #424750;
    color: white;
    padding: 30px 0;
    margin-top: 30px;
}

.footer-sections {
    display: flex;
    justify-content: space-around;
}
