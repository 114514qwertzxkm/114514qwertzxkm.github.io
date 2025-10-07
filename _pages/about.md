---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Z脚本 - 科技平台</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Exo+2:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            background-image: url('https://picsum.photos/id/119/1920/1080');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            font-family: 'Exo 2', sans-serif;
        }
        .glow-text {
            text-shadow: 0 0 8px rgba(0, 255, 255, 0.7), 0 0 20px rgba(0, 255, 255, 0.5);
        }
        .glass {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        /* 默认样式 - 所有设备通用 */
        .test-beta-banner {
            background: linear-gradient(90deg, rgba(0, 255, 255, 0.3), rgba(0, 100, 255, 0.3));
            backdrop-filter: blur(5px);
            -webkit-backdrop-filter: blur(5px);
            color: #ffffff;
            padding: 10px 0;
            text-align: center;
            font-size: 16px;
            font-weight: bold;
            margin-bottom: 20px;
        }
        /* 电脑端样式 */
        @media (min-width: 1024px) {
            .test-beta-banner {
                box-shadow: 0 0 20px rgba(0, 255, 255, 0.4);
            }
            .glow-on-desktop {
                box-shadow: 0 0 15px rgba(0, 255, 255, 0.3);
                transition: all 0.3s ease;
            }
            .glow-on-desktop:hover {
                box-shadow: 0 0 25px rgba(0, 255, 255, 0.6);
                transform: translateY(-2px);
            }
        }
        /* 平板和手机端样式 */
        @media (max-width: 1023px) {
            .test-beta-banner {
                box-shadow: 0 0 20px rgba(0, 255, 255, 0.6);
            }
        }
    </style>
</head>
<body class="bg-slate-900 text-white min-h-screen flex flex-col">
    <!-- 导航栏 -->
    <nav class="glass sticky top-0 z-50 px-6 py-4 flex justify-between items-center">
        <div class="flex items-center space-x-2">
            <div class="text-3xl md:text-5xl font-black text-cyan-400 glow-text">Z</div>
            <span class="text-xl md:text-3xl font-bold">脚本</span>
        </div>
        <div class="hidden md:flex space-x-8">
            <a href="#" class="text-cyan-400 border-b-2 border-cyan-400 pb-1">主页</a>
            <a href="#" id="navMore" class="hover:text-cyan-400 transition-colors">了解更多</a>
            <a href="#" class="hover:text-cyan-400 transition-colors">关于</a>
        </div>
        <button id="loginBtn" class="glass hover:bg-cyan-500/20 transition-all px-4 py-2 rounded-lg glow-on-desktop">
            Roblox登录
        </button>
    </nav>

    <!-- 测试版标签 -->
    <div class="test-beta-banner">
        🚀 Z脚本 V0.8 测试版抢先体验中 - 欢迎反馈！
    </div>

    <!-- 首页内容 -->
    <main id="homeContent" class="flex-grow flex flex-col items-center justify-center px-6 py-12 text-center">
        <div class="max-w-4xl mx-auto">
            <!-- 公告卡片 - 静态展示 -->
            <div class="glass rounded-xl p-8 mb-10">
                <h2 class="text-3xl font-bold mb-4 text-cyan-400">最新公告</h2>
                <p class="text-2xl font-bold">Z脚本V0.8正在测试</p>
                <p class="text-base text-gray-300 mt-2">感谢您的支持，我们正在全力开发中！</p>
            </div>
            
            <h1 class="text-5xl md:text-7xl font-black mb-8">
                <span class="text-cyan-400 glow-text">Z脚本</span>
                <br>
                <span class="text-white">重新定义你的体验</span>
            </h1>
            <p class="text-xl md:text-2xl text-gray-300 mb-12 max-w-2xl mx-auto">强大的脚本工具，为你的Roblox世界带来无限可能。</p>
            <div class="flex flex-col sm:flex-row justify-center gap-6">
                <a href="#" id="moreBtn" class="glass hover:bg-cyan-500/20 transition-all px-8 py-4 rounded-lg text-xl font-bold glow-on-desktop">
                    了解更多
                </a>
                <a href="#" id="demoBtn" class="glass border-2 border-cyan-400 hover:bg-cyan-500/20 transition-all px-8 py-4 rounded-lg text-xl font-bold glow-on-desktop">
                    查看演示
                </a>
            </div>
        </div>
    </main>

    <!-- 了解更多内容 -->
    <main id="moreContent" class="flex-grow px-6 py-12 hidden">
        <div class="max-w-5xl mx-auto">
            <div class="mb-10">
                <button id="backBtn" class="glass hover:bg-cyan-500/20 transition-all px-6 py-3 rounded-lg text-lg glow-on-desktop">
                    ← 返回首页
                </button>
            </div>
            
            <div class="glass rounded-xl p-10 mb-10">
                <h2 class="text-4xl font-bold mb-8 text-cyan-400">关于 Z脚本</h2>
                <p class="text-lg mb-6">Z脚本源于Roblox社区熟知的"皮脚本"，我们在其基础上进行了全面的优化和创新，致力于打造一个更强大、更稳定的脚本平台。</p>
                
                <p class="text-lg mb-6">很遗憾地告诉大家，目前Z脚本仍在紧张的开发测试阶段，尚未正式发布。但请放心，我们的开发团队正在全力以赴，争取早日将这个工具呈现给大家。</p>
                
                <p class="text-lg mb-6">Z脚本的核心功能非常强大，我们相信它将为Roblox玩家带来全新的体验。虽然现在还不能展示全部功能，但我们可以先分享一些未来的发展方向。</p>
                
                <p class="text-2xl font-bold text-center my-10">预计 2026 年正式发布，我们 2026 年再见面！</p>
            </div>

            <div class="glass rounded-xl p-10">
                <h3 class="text-3xl font-bold mb-8 text-center">未来目标</h3>
                <div class="grid md:grid-cols-2 gap-8">
                    <div class="glass p-8 rounded-lg hover:bg-cyan-500/10 transition-all glow-on-desktop">
                        <h4 class="text-2xl font-bold mb-4">性能优化</h4>
                        <p class="text-lg">极致的运行效率，更低的资源占用，让脚本运行更加流畅。</p>
                    </div>
                    
                    <div class="glass p-8 rounded-lg hover:bg-cyan-500/10 transition-all glow-on-desktop">
                        <h4 class="text-2xl font-bold mb-4">安全保障</h4>
                        <p class="text-lg">多重安全机制，保护用户账号安全，远离封号风险。</p>
                    </div>
                    
                    <div class="glass p-8 rounded-lg hover:bg-cyan-500/10 transition-all glow-on-desktop">
                        <h4 class="text-2xl font-bold mb-4">脚本库</h4>
                        <p class="text-lg">丰富的官方脚本库，覆盖各种游戏场景，一键启用。</p>
                    </div>
                    
                    <div class="glass p-8 rounded-lg hover:bg-cyan-500/10 transition-all glow-on-desktop">
                        <h4 class="text-2xl font-bold mb-4">社区支持</h4>
                        <p class="text-lg">活跃的社区交流平台，用户可以分享脚本、交流经验。</p>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <!-- 登录模态框 -->
    <div id="loginModal" class="fixed inset-0 z-50 flex items-center justify-center hidden">
        <div class="absolute inset-0 bg-black/50 backdrop-blur-sm" id="modalOverlay"></div>
        <div class="glass relative z-10 w-full max-w-md mx-4 p-8 rounded-xl">
            <div class="flex justify-between items-center mb-8">
                <h2 class="text-3xl font-bold">账号登录</h2>
                <button id="closeModal" class="text-3xl hover:text-cyan-400 transition-colors">&times;</button>
            </div>
            <div class="space-y-6">
                <p class="text-lg text-gray-300">本软件尚未发布，登录功能暂不可用。</p>
                <p class="text-lg text-gray-300">请关注我们的官方渠道获取上线通知。</p>
                <div class="mt-10 flex justify-center">
                    <button id="closeBtn" class="glass hover:bg-cyan-500/20 transition-all px-8 py-3 rounded-lg w-full text-lg glow-on-desktop">
                        我知道了
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- 页脚 -->
    <footer class="glass mt-auto py-8 px-6 text-center text-base text-gray-400">
        <p>&copy; 2025 Z脚本 - 保留所有权利</p>
    </footer>

    <!-- 脚本放在页面底部，确保所有元素都已加载 -->
    <script>
        // 页面切换功能
        const homeContent = document.getElementById('homeContent');
        const moreContent = document.getElementById('moreContent');
        const navMore = document.getElementById('navMore');
        const moreBtn = document.getElementById('moreBtn');
        const backBtn = document.getElementById('backBtn');

        function showHome() {
            homeContent.classList.remove('hidden');
            moreContent.classList.add('hidden');
        }

        function showMore() {
            homeContent.classList.add('hidden');
            moreContent.classList.remove('hidden');
        }

        navMore.addEventListener('click', showMore);
        moreBtn.addEventListener('click', showMore);
        backBtn.addEventListener('click', showHome);

        // 登录模态框控制
        const loginBtn = document.getElementById('loginBtn');
        const loginModal = document.getElementById('loginModal');
        const closeModal = document.getElementById('closeModal');
        const closeBtn = document.getElementById('closeBtn');
        const modalOverlay = document.getElementById('modalOverlay');

        function openModal() {
            loginModal.classList.remove('hidden');
            document.body.style.overflow = 'hidden';
        }

        function closeModalFunc() {
            loginModal.classList.add('hidden');
            document.body.style.overflow = '';
        }

        loginBtn.addEventListener('click', openModal);
        closeModal.addEventListener('click', closeModalFunc);
        closeBtn.addEventListener('click', closeModalFunc);
        modalOverlay.addEventListener('click', closeModalFunc);

        // 演示按钮 - 阻止默认跳转并显示提示
        const demoBtn = document.getElementById('demoBtn');
        
        demoBtn.addEventListener('click', function(event) {
            event.preventDefault(); // 阻止链接默认的跳转行为
            alert('查看演示功能正在调试中，暂时无法使用。我们团队对此深表歉意！');
        });
    </script>
</body>
</html>
