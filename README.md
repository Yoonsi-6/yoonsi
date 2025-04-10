<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>数字化博物馆</title>
    <style>
        /* 全局样式 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            background-color: #121212;
            color: #ffffff;
            line-height: 1.6;
        }
        
        /* 导航栏 */
        header {
            background-color: #000000;
            padding: 1rem 2rem;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.5);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        nav {
            display: flex;
            justify-content: center;
            align-items: center;
        }
        
        .nav-container {
            display: flex;
            width: 100%;
            max-width: 1200px;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #ffffff;
            text-decoration: none;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 2rem;
        }
        
        .nav-links a {
            color: #ffffff;
            text-decoration: none;
            font-weight: 500;
            padding: 0.5rem 1rem;
            border-radius: 4px;
            transition: all 0.3s ease;
        }
        
        .nav-links a:hover, .nav-links a.active {
            background-color: #333333;
        }
        
        /* 主要内容 */
        .main-content {
            padding: 2rem;
            max-width: 1400px;
            margin: 0 auto;
        }
        
        .hero {
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #ffffff;
        }
        
        .hero p {
            font-size: 1.1rem;
            color: #cccccc;
            max-width: 800px;
            margin: 0 auto 2rem;
        }
        
        /* 3D模型展示区 */
        .model-container {
            width: 100%;
            height: 600px;
            margin: 2rem 0;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }
        
        .sketchfab-embed-wrapper {
            width: 100%;
            height: 100%;
        }
        
        .sketchfab-embed-wrapper iframe {
            width: 100%;
            height: 100%;
            border: none;
        }
        
        /* 页脚 */
        footer {
            background-color: #000000;
            padding: 2rem;
            text-align: center;
            margin-top: 3rem;
        }
        
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .footer-content p {
            color: #aaaaaa;
            margin-bottom: 1rem;
        }
        
        /* 响应式设计 */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
            }
            
            .logo {
                margin-bottom: 1rem;
            }
            
            .nav-links {
                width: 100%;
                justify-content: space-around;
            }
            
            .nav-links li {
                margin-left: 0;
            }
            
            .model-container {
                height: 400px;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
        }
        
        @media (max-width: 480px) {
            .nav-links {
                flex-direction: column;
                align-items: center;
            }
            
            .nav-links li {
                margin: 0.5rem 0;
            }
            
            .model-container {
                height: 300px;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="nav-container">
                <a href="#" class="logo">数字化博物馆</a>
                <ul class="nav-links">
                    <li><a href="#" class="active">首页</a></li>
                    <li><a href="#">展品</a></li>
                    <li><a href="#">展览</a></li>
                    <li><a href="#">联系我们</a></li>
                </ul>
            </div>
        </nav>
    </header>
    
    <div class="main-content">
        <section class="hero">
            <h1>探索数字化的文化遗产</h1>
            <p>通过最先进的3D扫描和虚拟现实技术，体验前所未有的博物馆参观方式。我们的数字化收藏让您足不出户就能欣赏世界各地的珍贵文物。</p>
        </section>
        
        <div class="model-container">
            <div class="sketchfab-embed-wrapper"> 
                <iframe title="Bull shark (Carcharhinus leucas, Zambezi shark)" frameborder="0" allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" allow="autoplay; fullscreen; xr-spatial-tracking" xr-spatial-tracking execution-while-out-of-viewport execution-while-not-rendered web-share width="1980" height="1080" src="https://sketchfab.com/models/550b855f9ea64ab68f3dcf59c3526971/embed?ui_theme=dark"> </iframe> 
            </div>
        </div>
        
        <section class="info-section">
            <h2>特色展品</h2>
            <p>我们的数字化收藏包括来自世界各地的珍贵文物，从古代文明到现代艺术，应有尽有。所有展品都经过高精度3D扫描，让您可以从各个角度欣赏细节。</p>
        </section>
    </div>
    
    <footer>
        <div class="footer-content">
            <p>© 2023 数字化博物馆 版权所有</p>
            <p>联系我们: info@digitalmuseum.com | 电话: 123-456-7890</p>
        </div>
    </footer>
</body>
</html>
