<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MA² Beauty Lab</title>

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Georgia', serif;
            color: #333;
            background: #f8f9fa;
        }

        header {
            background: #fff;
            padding: 20px 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 28px;
            font-weight: bold;
            color: #6b7c93;
            cursor: pointer;
        }

        .nav-menu a {
            text-decoration: none;
            color: #6b7c93;
            font-size: 16px;
            cursor: pointer;
        }

        .nav-menu a:hover {
            color: #4a5568;
        }

        .page {
            display: none;
        }

        .page.active {
            display: block;
        }

        /* Products */
        .products-section {
            max-width: 1200px;
            margin: 60px auto;
        }

        .section-title {
            font-size: 42px;
            color: #6b7c93;
            text-align: center;
            margin-bottom: 10px;
        }

        .section-subtitle {
            text-align: center;
            color: #888;
            margin-bottom: 40px;
        }

        .product-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .product-image {
            width: 100%;
            height: 280px;
            object-fit: cover;
        }
     .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
        }
        .product-info {
            padding: 20px;
        }

    footer {
            background: #c770a8;
            color: #fff;
            padding: 80px 0 40px;
            margin-top: 120px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            margin-bottom: 30px;
        }

        .footer-section h3 {
            color: #cbd5e0;
            font-size: 24px;
            margin-bottom: 20px;
        }

        .footer-section p {
            line-height: 1.8;
            color: #cbd5e0;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 10px;
            color:  #cbd5e0; ;
        }

        .footer-links a {
            color: #cbd5e0;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-links a:hover {
            color: #cbd5e0;
        }

        .footer-bottom {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #4a5568;
            color: #cbd5e0;
        }
    </style>
</head>
<body>

<!-- Header -->
<header>
    <div class="container">
        <nav class="d-flex justify-content-between align-items-center">
            <div class="logo" onclick="showPage('home')">MA² Beauty Lab</div>
            <div class="nav-menu d-flex gap-4">
                <a onclick="showPage('home')">Home</a>
                <a onclick="showPage('about')">About</a>
                <a onclick="showPage('products')">Products</a>
                <a onclick="showPage('blog')">Blog</a>
                <a onclick="showPage('contact')">Contact</a>
            </div>
        </nav>
    </div>
</header>

<!-- Home Page (EMPTY – content removed) -->
<div id="home" class="page active"></div>

<!-- About Page -->
<div id="about" class="page container mt-5">
    <h1 class="text-center mb-4">About MA² Beauty Lab</h1>
    <p class="text-center">
        MA² Beauty Lab offers professional makeup services using premium products and modern techniques.
    </p>
</div>

<!-- Products Page -->
<div id="products" class="page">
    <div class="products-section container">
        <h1 class="section-title">Our Makeup Products</h1>
        <p class="section-subtitle">Premium Quality Products</p>

        <div class="row g-4">
            <div class="col-md-4">
                <div class="product-card">
                    <img class="product-image" src="https://images.unsplash.com/photo-1586495777744-4413f21062fa?w=400">
                    <div class="product-info">
                        <h5>Lipstick - Matte Red</h5>
                        <p>PKR 1,200</p>
                        <a href="#" class="btn btn-primary">Go somewhere</a>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="product-card">
                    <img class="product-image" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTkvLFrIW-7vetmKKd3ynSGxaSjGlrWlRzDgQ&s">
                    <div class="product-info">
                        <h5>Eyeshadows palette</h5>
                        <p>PKR 1,800</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="product-card">
                    <img class="product-image" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSUrA_NKS-htu7I84KYhJDJLk1Clbri9zgD0g&s">
                    <div class="product-info">
                        <h5>Blush - Shade Peach</h5>
                        <p>PKR 1,200</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="product-card">
                    <img class="product-image" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTCRSyfxK9diuj1qzKB3OpyjsGL4BLGuH_knA&s">
                    <div class="product-info">
                        <h5>Creamy Tint - Shade Brown </h5>
                        <p>PKR 1,200</p>
                    </div>
                </div>
            </div>
             <div class="col-md-4">
                <div class="product-card">
                    <img class="product-image" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ4DSbcuS3tqjLLBTxJDf9FEIbGNwO7Jjh3dA&s">
                    <div class="product-info">
                        <h5>Face powder - Shade Beige </h5>
                        <p>PKR 1,200</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="product-card">
                    <img class="product-image" src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxIHBgkRBxIVEBUQGBgVFRcQEA8VFRgZFxobGhgXExYYHCggGBslGxUVLTEhJTUrOi4uFx8zODMuNygtLisBCgoKDg0OGhAQGy0lHyM3LS8tLS0tNystLSs1KysrLS0tLS0tMS0tLSstLS41NystKy0tLS0tLSstKy02LTctN//AABEIAOEA4QMBIgACEQEDEQH/xAAbAAEBAQEAAwEAAAAAAAAAAAAABgcFAQMEAv/EAEIQAAIBAgMEBQYLBgcAAAAAAAABAgMRBBIhBQYHMRMiQXGRFDdCUXKhIzJSYXOBsbO0wdEkM2KSssIWJ1OCk+Hw/8QAGAEBAQEBAQAAAAAAAAAAAAAAAAECBAP/xAAjEQEAAQMEAgIDAAAAAAAAAAAAAQIDERIhMUEi8HGxBCMy/9oADAMBAAIRAxEAPwDcQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAzXjHvPjN3Y7Mewq3Q5nLpPgqU82icL507LqzTta+ZamlGZcdMIqm70KjteLVm5JfFkpWStq8ufQCs3N3njvNs6NSMcjcYycbt2UlybaWqd16nbRvW1CYjwZxmWOVXbpynHSNSdtVN/Fd4q036078jbk7rQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABD8YdNysZbTqzWnsS7LPTT5rFwQXGarl3QxMW7ZoVP9TXq2t1fa7dO8DOeEqcsbVWWUl0jekHJa07a5ZKXYuXqRv+H/cU9LaLRpp8u1NswXhFhemxNZuKl8JKydOUnZQitJRaa1nyuk7PXRm+xWWKS7APIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAEpxVq9Dw+21f0oKH/ACTjD+4qyL4x+brantYf8RSA+fgxh4S3A2fJwTlnrttpN36efJ9mkY+CLwheCj/y8wPt1/vpl0AJHbu/tPY22amFeCx2InFJ5sLhoVIPMr6POn2+orjNtqt/4txSln58p9D6uzM1p6teViTOHpbo1zh09l8SKW0dqYah5BtCi6rSUq+FhCmr9s5dJoi2MroabTwObldX6S+Tn6VptM1QROVu29EgAK8gAAAAAAAAAAAAAAAAAAAAAAAAAACK4yebraftYf8AEUi1IrjL5u9pe1h/xFID08EvN7gvpK/3sy7IPgl5vcH9JX+9mXgEvv3tWezsHQVGeTpW02rp6OPJrlz95P7ErU5znPEtylaTvNSk+qm3dtPkovwO3xDpN4HDTS6sG7vTS9mtP9r8DkbuVVkqaN6P0WZ7ddqPDZ82KyPBxnykmmmlZq8rRtb50d7cbas8XUr0q03NQWbrZm1e3a+yzJ7GwhPZ0XUi+1ektNfU/wCJ/wDkjtcPqHw+JqRWlst79rd7WuO1u/zOVsADTjAAAAAAAAAAAAAAAAAAAAAAAAAAAInjL5u9pe1h/wARSLYieMvm72l7WH/EUgPTwS83uD+kr/ezLwg+CPm9wf0lf72ReAR3EifR4LDOTsk236vjQWv1NnK3axWHUKixNWEJXcUm43zKKk132kn9Z0OKUc2yYJ31Ulorv41Pku1mebHnbDVqteThBzjKrKMad/2qoqSySjUT6K0acs2ukItNO1s9ummrFuMe7rOdONbd2nVhZ5rtWSfa+06G4C+Hr/PH80R+G3lp4bcxwdKrlwsYqU+q9ZdE1FrM5JtYiLTfxslT5OthuDpiKq/hf9USdvWuYm3Pva2ABtwgAAAAAAAAAAAAAAAAAAAAAAAAAA8SkorrO3eQvGPEwnw92kozi3moaKUb/v6Z0N/6SnhMM5K9nJa/Ol+hLbKwdKVCtmpQbs+cIfoTO72otaozl0+CmJhDh/g1OcU+kraOUb/vZGgRkprqNPuZkuKwlJYGFqcL+xD9Ck4ZUrU9pSXLNGKt8yf6kzvharOmmZy88UJZdnYZRunJtKzs7uVPk+zlzM13XrxdBRxKzxxCpTqpUY5lTdejO0ZuorQbxtNdHZ2UW7vKlLRuKry4LZzWtql/sI7dvd3NhlKEqvwUYQnFYdTcoQ6CbUJZ0lLNgoa66TaSbs07a0/qifn7cLCU4Yjd3ZspVpzhUjHDpRpRUrZFO1WedpxjUp9VW6rr1Fd5rrTeG0ukjGT7aV/HKQFHdvyfYWHdJ13FKE0lQjGOeLoRzNynd64S+W2nTc3bW/4ZU3ToNT5wgo3atfl2dnL3DsxMUVe9rsAGnMAAAAAAAAAAAAAAAAAAAAAAAAAACf33p59jJr0Zp+Ka/NEZsyVqVbuZf7zUul2Hi16kn/K0/wAjO8BKyrdzMzy67E+L84yX7HT7iu4bUsmwqkn6dST+pJf9kVj5WwkO40bcuh0G7WCT7U5eLf5WJHK358HF4qQb2LRlTSk4ybinycrXSf1pENsLebGYHZlaTwkm8rvGNKu3ouSai/qNG4iUuk3fuvRnF+5klsepalU9l/YXtLcTNG0p6W9GLqYBUVg5KEeTyYiServ6C+0t+E1WticBVntGCpTa1gr9VZpZebfopHIxE/2KmVXD+FsLipetxXgm/wC4dpciYpnMqwAGnKAAAAAAAAAAAAAAAAAAAAAAAAAAD04yl5Rg68PlxlHxVjKKDy1KvczXTKdrUfJdsYuHqlK3dfT3WM1OixPMOdjnmo0167I17ZlHyfZ2Fh8mEV4JXMowNHyzamBp8804p919TYBSv5E8Q4+91Dp93sYl2JPwav7rmcbLqWpS7jWMbR8owdeHy4yj4qxkGGfRzqLvE8rYnxmH0Vp/s1NF9uRS6PYify5N+Fl+TM8lK8aaNT2BR8n2Lg4/wp/zdZ/aSOS/Pi6AANuUAAAAAAAAAAAAAAAAAAAAAAAAAAAzrfyh0G21NcqkU/rXVf2LxNFOPvDsCG3IUelm4Onezik+drpp9yJMPS3VpqzKM3Fw/lG8MJPlSi5e7Kv6vcaWcXd3d2Gw+mdOcqjqWu5JKyV+Vu/3I7QiMFyrVVmAyTblDyTbmMjy60rdz1XuaNbJrb26UdrY51Y1XTk0k1kUk7K1+a7LCYW1XFM7oHB0nicXh4R5zaj4u35mxRjlilHktCW2RuZHZ+Oo1alZ1MmqXRqKv2X6zKokQt2uKp2AAaeIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA//Z">
                    <div class="product-info">
                        <h5>Mascara - Volume Max</h5>
                        <p>PKR 1,500</p>
                    </div>
                </div>
            </div>

            <div class="col-md-4">
                <div class="product-card">
                    <img class="product-image" src= "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSVleUodUrjMy-ie2EwL2M0zPlUDLjymqfSbw&s">
                    <div class="product-info">
                        <h5>Foundation - Beige</h5>
                        <p>PKR 2,500</p>
                    </div>
                </div>
            </div>

            <div class="col-md-4">
                <div class="product-card">
                    <img class="product-image" src="data:image/jpeg;base64,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">
                    <div class="product-info">
                        <h5>Concealer - Beige</h5>
                        <p>PKR 1,700</p>
                    </div>
                </div>
            </div>
            
            
            <div class="col-md-4">
                <div class="product-card">
                    <img class="product-image" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTHOfEr5gm4BbX7t8kipaTcas3PKCqIngAOXQ&s">
                    <div class="product-info">
                        <h5> Liner - Brown</h5>
                        <p>PKR 1000</p>
                    </div>
                    
        </div>
    </div>
</div>

<!-- Blog Page -->
<div id="blog" class="page container mt-5">
    <h1 class="text-center">Our Blog</h1>
    <p class="text-center">Makeup tips & beauty guides</p>
</div>

<!-- Contact Page -->
<div id="contact" class="page container mt-5 text-center">
    <h1>Contact Us</h1>
    <p>Email: MA²beautylab@gmail.com</p>
    <p>Phone: +92 322 784 6291</p>
</div>

<!-- Footer -->
<footer>
     <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h3>About MA² Beauty Lab</h3>
                <p>MA² Beauty Lab is a professional beauty space offering customized makeup services for every occasion. We focus on enhancing natural beauty using quality products and modern techniques, ensuring every client feels confident and satisfied with their look.</p>
            </div>
            
            <div class="footer-section">
                <h3>Quick Links</h3>
                <ul class="footer-links">
                    <li><a onclick="showPage('home')">Home</a></li>
                    <li><a onclick="showPage('about')">About</a></li>
                    <li><a onclick="showPage('products')">Products</a></li>
                    <li><a onclick="showPage('blog')">Blog</a></li>
                    <li><a onclick="showPage('contact')">Contact</a></li>
                </ul>
            </div>
            
            <div class="footer-section">
                <h3>Contact Info</h3>
                <ul class="footer-links">
                    <li>📧 MA²beautylab@gmail.com</li>
                    <li>📞 +92 322 784 6291</li>
                    <li>📍 Gulzar-e-Hijri, Karachi, Pakistan</li>
                    <li>🕒 Open Daily</li>
                </ul>
            </div>
        </div>
        
        <div class="footer-bottom">
            <div class="container">
                <p>&copy; 2025 MA² Beauty Lab. All rights reserved. | Designed by MA²beautylab </p>
            </div>
        </div>
    </footer>

<script>
    function showPage(pageId) {
        document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
        document.getElementById(pageId).classList.add('active');
        window.scrollTo(0, 0);
    }
</script>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
# APTECH-PROJECT-2-
