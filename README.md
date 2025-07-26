<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>دیجی‌شاپ</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        *{margin:0;padding:0;box-sizing:border-box;font-family:'Segoe UI',Tahoma,Geneva,Verdana,sans-serif}
        body{background:#f5f5f5;color:#333;direction:rtl}
        .container{width:90%;max-width:1200px;margin:0 auto}
        .header{background:#a62626}
        .top-bar{background:#424750;color:#fff;padding:10px 0;font-size:14px}
        .top-bar .container{display:flex;justify-content:space-between}
        .main-header{padding:15px 0}
        .main-header .container{display:flex;align-items:center;justify-content:space-between}
        .logo img{height:40px}
        .search-box{display:flex;width:50%}
        .search-box input{width:100%;padding:10px 15px;border:none;border-radius:5px 0 0 5px}
        .search-box button{background:#424750;color:#fff;border:none;padding:0 20px;border-radius:0 5px 5px 0;cursor:pointer}
        .header-actions a{color:#fff;margin-right:15px;font-size:18px}
        .main-menu{background:#3d3d3d}
        .main-menu ul{display:flex;list-style:none}
        .main-menu li:hover{background:#a62626}
        .main-menu a{color:#fff;text-decoration:none;display:block;padding:15px 20px;font-size:14px}
        .main-slider{margin:20px 0}
        .slider{position:relative;height:400px;overflow:hidden;border-radius:5px;box-shadow:0 2px 5px rgba(0,0,0,.1)}
        .slide{position:absolute;top:0;left:0;width:100%;height:100%;opacity:0;transition:opacity .5s}
        .slide.active{opacity:1}
        .slide img{width:100%;height:100%;object-fit:cover}
        .categories{display:flex;justify-content:space-between;margin-top:15px}
        .category{background:#fff;width:18%;text-align:center;padding:15px 0;border-radius:5px;box-shadow:0 1px 3px rgba(0,0,0,.1);cursor:pointer;transition:transform .3s}
        .category:hover{transform:translateY(-5px)}
        .section-header{display:flex;justify-content:space-between;align-items:center;margin-bottom:20px}
        .products-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:20px}
        .product{background:#fff;border-radius:5px;overflow:hidden;box-shadow:0 1px 3px rgba(0,0,0,.1);transition:transform .3s,box-shadow .3s}
        .product:hover{transform:translateY(-5px);
                    box-shadow:0 5px 15px rgba(0,0,0,.1)}

        .product 
        img{width:100%;height:200px;object-fit:contain;padding:15px}
        .add-to-cart{display:block;width:100%;padding:10px;background:#a62626;color:#fff;border:none;cursor:pointer}
        .footer{background:#3d3d3d;color:#fff;padding:40px 0 20px}
        @media (max-width:768px){.products-grid{grid-template-columns:repeat(2,1fr)}}
    </style>
</head>
<body>
    <header class="header">
        <div class="top-bar">
            <div class="container">
                <div class="contact-info">
                    <span><i class="fas fa-phone"></i> 021-12345678</span>
                </div>
                <div class="user-menu">
                    <a href="#"><i class="fas fa-user"></i> ورود / ثبت‌نام</a>
                </div>
            </div>
        </div>
        <div class="main-header">
            <div class="container">
                <div class="logo">
                    <h1>دیجی‌شاپ</h1>
                </div>
                <div class="search-box">
                    <input type="text" placeholder="جستجوی محصولات...">
                    <button><i class="fas fa-search"></i></button>
                </div>
                <div class="header-actions">
                    <a href="#" class="cart"><i class="fas fa-shopping-cart"></i></a>
                </div>
            </div>
        </div>
        <nav class="main-menu">
            <div class="container">
                <ul>
                    <li><a href="#"><i class="fas fa-home"></i> خانه</a></li>
                    <li><a href="#"><i class="fas fa-box-open"></i> محصولات</a></li>
                    <li><a href="#"><i class="fas fa-percentage"></i> تخفیف‌ها</a></li>
                </ul>
            </div>
        </nav>
    </header>

    <section class="main-slider">
        <div class="container">
            <div class="slider">
                <div class="slide active">
                    <img src="https://via.placeholder.com/1200x400?text=Slider+1" alt="تخفیف ویژه">
                </div>
                <div class="slide">
                    <img src="https://via.placeholder.com/1200x400?text=Slider+2" alt="محصولات جدید">
                </div>
            </div>
        </div>
    </section>

    <section class="featured-products">
        <div class="container">
            <div class="section-header">
                <h2>محصولات ویژه</h2>
                <a href="#" class="view-all">مشاهده همه</a>
            </div>
            <div class="products-grid">
                <div class="product">
                    <img src="https://via.placeholder.com/300x300?text=محصول+1" alt="گوشی موبایل">
                    <h3>گوشی موبایل سامسونگ</h3>
                    <div class="price">۱۲,۹۹۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
                <div class="product">
                    <img src="https://via.placeholder.com/300x300?text=محصول+2" alt="لپ‌تاپ">
                    <h3>لپ‌تاپ 15 اینچی ایسوس</h3>
                    <div class="price">۲۴,۷۹۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
                <div class="product">
                    <img src="https://via.placeholder.com/300x300?text=محصول+3" alt="هدفون">
                    <h3>هدفون بی‌سیم</h3>
                    <div class="price">۱,۲۹۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
                <div class="product">
                    <img src="https://via.placeholder.com/300x300?text=محصول+4" alt="ماوس">
                    <h3>ماوس گیمینگ</h3>
                    <div class="price">۵۹۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
            </div>
        </div>
    </section>

    <footer class="footer">
        <div class="container">
            <p>© ۱۴۰۲ دیجی‌شاپ - تمام حقوق محفوظ است</p>
        </div>
    </footer>

    <script>
        // اسلایدر ساده
        const slides = document.querySelectorAll('.slide');
        let currentSlide = 0;
        
        function showSlide() {
            slides.forEach(slide => slide.classList.remove('active'));
            slides[currentSlide].classList.add('active');
            currentSlide = (currentSlide + 1) % slides.length;
        }
        
        setInterval(showSlide, 3000);
        
        // افزودن به سبد خرید
        document.querySelectorAll('.add-to-cart').forEach(btn => {
            btn.addEventListener('click', () => {
                alert('محصول به سبد خرید اضافه شد!');
            });
        });
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>رفع خطای GitHub Pages</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a2a3a, #2c3e50);
            color: #ecf0f1;
            min-height: 100vh;
            padding: 20px;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            background: rgba(26, 37, 48, 0.8);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            backdrop-filter: blur(10px);
        }
        
        header {
            text-align: center;
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 2px solid #3498db;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: #3498db;
        }
        
        .problem {
            background: rgba(231, 76, 60, 0.2);
            border-left: 4px solid #e74c3c;
            padding: 20px;
            border-radius: 0 8px 8px 0;
            margin-bottom: 30px;
        }
        
        .solution {
            background: rgba(46, 204, 113, 0.2);
            border-left: 4px solid #2ecc71;
            padding: 20px;
            border-radius: 0 8px 8px 0;
            margin-bottom: 30px;
        }
        
        h2 {
            margin-bottom: 15px;
            color: #3498db;
        }
        
        .steps {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin: 30px 0;
        }
        
        .step {
            flex: 1;
            min-width: 300px;
            background: rgba(52, 152, 219, 0.1);
            padding: 20px;
            border-radius: 10px;
        }
        
        .step-number {
            display: inline-block;
            background: #3498db;
            color: white;
            width: 30px;
            height: 30px;
            text-align: center;
            line-height: 30px;
            border-radius: 50%;
            margin-bottom: 15px;
        }
        
        .code {
            background: #1a2530;
            padding: 15px;
            border-radius: 8px;
            margin: 15px 0;
            font-family: monospace;
            overflow-x: auto;
        }
        
        .tip {
            background: rgba(241, 196, 15, 0.2);
            border-left: 4px solid #f1c40f;
            padding: 15px;
            border-radius: 0 8px 8px 0;
            margin: 20px 0;
        }
        
        .success {
            text-align: center;
            margin-top: 30px;
            padding: 20px;
            background: rgba(46, 204, 113, 0.2);
            border-radius: 10px;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 15px;
            }
            
            h1 {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>رفع خطای 404 در GitHub Pages</h1>
            <p>راهنمای گام به گام برای رفع مشکل "There isn't a GitHub Pages site here"</p>
        </header>
        
        <div class="problem">
            <h2>مشکل شما:</h2>
            <p>هنگام مراجعه به آدرس سایت خود با پیام زیر مواجه می‌شوید:</p>
            <div class="code">
                404
                There isn't a GitHub Pages site here.
                
                If you're trying to publish one, read the full documentation to learn how to set up GitHub Pages for your repository, organization, or user account.
            </div>
        </div>
        
        <div class="solution">
            <h2>راه حل:</h2>
            <p>برای رفع این مشکل، لطفاً مراحل زیر را به ترتیب انجام دهید:</p>
            
            <div class="steps">
                <div class="step">
                    <div class="step-number">1</div>
                    <h3>نام ریپازیتوری را بررسی کنید</h3>
                    <p>برای سایت‌های شخصی، نام ریپازیتوری باید دقیقاً به این شکل باشد:</p>
                    <div class="code">username.github.io</div>
                    <p>مثال برای شما:</p>
                    <div class="code">mahdibayatlajax.github.io</div>
                </div>
                
                <div class="step">
                    <div class="step-number">2</div>
                    <h3>تنظیمات GitHub Pages</h3>
                    <p>به بخش تنظیمات ریپازیتوری بروید:</p>
                    <div class="code">
                        Settings > Pages
                    </div>
                    <p>در بخش "Source":</p>
                    <ul>
                        <li>Branch: main (یا شاخه‌ای که فایل‌های شما در آن است)</li>
                        <li>Folder: / (root)</li>
                    </ul>
                </div>
                
                <div class="step">
                    <div class="step-number">3</div>
                    <h3>فایل index.html</h3>
                    <p>مطمئن شوید که فایل اصلی شما:</p>
                    <ul>
                        <li>نام آن دقیقاً index.html باشد</li>
                        <li>در ریشه ریپازیتوری قرار داشته باشد</li>
                        <li>حاوی کد معتبر HTML باشد</li>
                    </ul>
                </div>
            </div>
            
            <div class="tip">
                <h3>نکته مهم:</h3>
                <p>پس از ایجاد تغییرات، ممکن است 1-5 دقیقه طول بکشد تا GitHub Pages به‌روزرسانی شود. صبور باشید!</p>
            </div>
            
            <div class="steps">
                <div class="step">
                    <div class="step-number">4</div>
                    <h3>بررسی ساختار فایل‌ها</h3>
                    <p>ساختار ریپازیتوری شما باید مشابه این باشد:</p>
                    <div class="code">
                        mahdibayatlajax.github.io/
                        ├── index.html
                        ├── css/
                        │   └── style.css
                        ├── js/
                        │   └── script.js
                        └── images/
                    </div>
                </div>
                
                <div class="step">
                    <div class="step-number">5</div>
                    <h3>رفع مشکلات رایج</h3>
                    <p>اگر هنوز مشکل دارید:</p>
                    <ul>
                        <li>از عدم وجود Custom Domain اطمینان حاصل کنید</li>
                        <li>یک فایل خالی به نام .nojekyll در ریشه ایجاد کنید</li>
                        <li>از صحت نام کاربری و نام ریپازیتوری اطمینان حاصل کنید</li>
                    </ul>
                </div>
                
                <div class="step">
                    <div class="step-number">6</div>
                    <h3>بررسی نهایی</h3>
                    <p>پس از انجام مراحل:</p>
                    <ol>
                        <li>تغییرات را commit و push کنید</li>
                        <li>5 دقیقه منتظر بمانید</li>
                        <li>به آدرس زیر مراجعه کنید:</li>
                    </ol>
                    <div class="code">https://mahdibayatlajax.github.io</div>
                </div>
            </div>
        </div>
        
        <div class="success">
            <h2>✅ مشکل حل شد!</h2>
            <p>پس از انجام این مراحل، سایت شما باید به درستی نمایش داده شود.</p>
            <p>اگر هنوز مشکل دارید، می‌توانید از بخش Issues در ریپازیتوری خود کمک بگیرید.</p>
        </div>
    </div>
</body>
</html>
