<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>高端艺术 | 现代极简官网</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#64748b',
                        muted: '#94a3b8',
                        light: '#f8fafc',
                        dark: '#1e293b'
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .glass {
                background: rgba(255, 255, 255, 0.25);
                backdrop-filter: blur(12px);
                -webkit-backdrop-filter: blur(12px);
                border: 1px solid rgba(255, 255, 255, 0.3);
            }
            .text-balance {
                text-wrap: balance;
            }
            .soft-shadow {
                box-shadow: 0 8px 32px rgba(0, 0, 0, 0.06);
            }
            .slow-fade {
                transition: all 0.3s ease-in-out;
            }
            .img-fit {
                width: 100%;
                height: 100%;
                object-fit: cover;
                border-radius: 0.375rem;
            }
        }
        html {
            scroll-behavior: smooth;
        }
        body {
            background-color: #fafafa;
            background-image: radial-gradient(#e2e8f0 0.8px, transparent 0.8px);
            background-size: 16px 16px;
        }
    </style>
</head>
<body class="font-sans text-dark bg-[#fafafa]">
    <!-- 顶部导航 -->
    <nav class="glass fixed w-full top-0 z-50 soft-shadow">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-xl font-medium tracking-wide text-dark">STUDIO·ART</a>
            <div class="hidden md:flex gap-8 text-sm text-muted">
                <a href="#home" class="slow-fade hover:text-primary">首页</a>
                <a href="#about" class="slow-fade hover:text-primary">关于</a>
                <a href="#works" class="slow-fade hover:text-primary">作品</a>
                <a href="#contact" class="slow-fade hover:text-primary">联系</a>
            </div>
            <button class="md:hidden text-dark">
                <i class="fa fa-bars text-lg"></i>
            </button>
        </div>
    </nav>

    <!-- 英雄区 -->
    <section id="home" class="pt-32 pb-28 px-6 container mx-auto">
        <div class="max-w-3xl mx-auto text-center">
            <h1 class="text-[clamp(2.5rem,5vw,4rem)] font-light leading-tight mb-6 text-balance">
                极简美学 · 高端视觉设计
            </h1>
            <p class="text-muted text-lg mb-10 leading-relaxed max-w-2xl mx-auto">
                商务与艺术双向融合，克制的视觉表达，柔和光影与留白构图，打造沉浸式品牌体验
            </p>
            <div class="flex justify-center gap-4 flex-wrap">
                <a href="#works" class="px-8 py-3 bg-primary text-white rounded-sm slow-fade hover:opacity-90">
                    浏览作品
                </a>
                <a href="#about" class="px-8 py-3 border border-muted rounded-sm slow-fade hover:bg-slate-100">
                    了解更多
                </a>
            </div>
        </div>
    </section>

    <!-- 关于板块（左侧文字 + 右侧大图） -->
    <section id="about" class="py-24 px-6 bg-white/60">
        <div class="container mx-auto max-w-6xl">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div>
                    <span class="text-muted text-sm tracking-widest">设计理念</span>
                    <h2 class="text-3xl font-light mt-3 mb-6">秩序 · 质感 · 极简</h2>
                    <p class="text-muted leading-loose">
                        坚持低饱和高级配色、轻渐变层次、微阴影质感，以大面积留白梳理视觉层级。
                        融合磨砂玻璃拟态与柔和光影，兼顾商务理性与艺术氛围感，打造干净、精致、耐看的现代视觉体系。
                    </p>
                </div>
                <!-- 这里替换【关于页大图】链接 -->
                <div class="rounded-md h-72 soft-shadow overflow-hidden">
                    <img src="此处粘贴图片链接1" class="img-fit" alt="关于视觉">
                </div>
            </div>
        </div>
    </section>

    <!-- 作品卡片板块 -->
    <section id="works" class="py-24 px-6">
        <div class="container mx-auto max-w-6xl">
            <div class="text-center mb-16">
                <span class="text-muted text-sm tracking-widest">精选项目</span>
                <h2 class="text-3xl font-light mt-3">艺术与商业视觉案例</h2>
            </div>
            <div class="grid md:grid-cols-3 gap-8">
                <!-- 卡片1 作品图 -->
                <div class="glass rounded-md soft-shadow slow-fade hover:-translate-y-1 overflow-hidden">
                    <div class="h-48">
                        <img src="此处粘贴图片链接2" class="img-fit" alt="作品一">
                    </div>
                    <div class="p-6">
                        <h3 class="font-medium mb-2">品牌视觉设计</h3>
                        <p class="text-muted text-sm">低饱和极简视觉，品牌高端系统化构建</p>
                    </div>
                </div>
                <!-- 卡片2 作品图 -->
                <div class="glass rounded-md soft-shadow slow-fade hover:-translate-y-1 overflow-hidden">
                    <div class="h-48">
                        <img src="此处粘贴图片链接3" class="img-fit" alt="作品二">
                    </div>
                    <div class="p-6">
                        <h3 class="font-medium mb-2">艺术作品集</h3>
                        <p class="text-muted text-sm">画廊式沉浸式布局，艺术内容展示</p>
                    </div>
                </div>
                <!-- 卡片3 作品图 -->
                <div class="glass rounded-md soft-shadow slow-fade hover:-translate-y-1 overflow-hidden">
                    <div class="h-48">
                        <img src="此处粘贴图片链接4" class="img-fit" alt="作品三">
                    </div>
                    <div class="p-6">
                        <h3 class="font-medium mb-2">高端官网定制</h3>
                        <p class="text-muted text-sm">多模块分区，专业UX/UI体验设计</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 联系板块 -->
    <section id="contact" class="py-24 px-6 bg-white/60">
        <div class="container mx-auto max-w-3xl text-center">
            <span class="text-muted text-sm tracking-widest">合作联系</span>
            <h2 class="text-3xl font-light mt-3 mb-6">开启定制化设计合作</h2>
            <p class="text-muted mb-10">简约沟通，精致呈现，为品牌与艺术创作提供高质量视觉解决方案</p>
            <a href="mailto:hello@example.com" class="px-10 py-3 bg-dark text-white rounded-sm slow-fade hover:bg-primary">
                立即联系
            </a>
        </div>
    </section>

    <!-- 页脚 -->
    <footer class="py-8 text-center text-muted text-sm border-t border-slate-200">
        <div class="container mx-auto">
            <p>© 2025 STUDIO·ART 高端现代视觉设计 | 极简艺术官网</p>
        </div>
    </footer>
</body>
</html>
