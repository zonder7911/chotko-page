
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  
  <style>
    body {
      margin: 0;
      background: #000;
      color: #fff;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      min-height: 100vh;
      padding: 40px 20px; /* Отступы по бокам для мобильных */
      box-sizing: border-box; /* Учитываем padding в ширине */
    }
    .logo-link {
      display: block;
      margin-bottom: 30px;
      transition: transform 0.3s ease;
      text-align: center; /* Центрируем логотип */
    }
    .logo-link:hover {
      transform: scale(1.05);
    }
    .logo-img {
      width: 100%;
      max-width: 260px; /* Максимальная ширина логотипа */
      height: auto;
      border-radius: 12px;
      box-shadow: 0 0 15px rgba(255,255,255,0.3);
    }
    .links {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px; /* Отступы между иконками */
      max-width: 100%;
      padding: 0 10px; /* Небольшие отступы по бокам */
      box-sizing: border-box;
    }
    .link-icon { 
      width: 70px;
      height: 70px; 
      border-radius: 16px;
      overflow: hidden;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      display: flex;
      align-items: center;
      justify-content: center;
      background: transparent; /* Убираем белый фон */
    }
    .link-icon:hover { 
      transform: scale(1.25);
      box-shadow: 0 0 20px rgba(255,255,255,0.4);
    }
    a { text-decoration: none; }
    img, svg { 
      width: 100%; 
      height: 100%; 
      object-fit: contain; 
    }

    /* Адаптация под мобильные устройства */
    @media (max-width: 768px) {
      .logo-img { max-width: 220px; }
      .link-icon { width: 60px; height: 60px; }
      .links { gap: 18px; }
    }

    @media (max-width: 480px) {
      .logo-img { max-width: 200px; }
      .link-icon { width: 50px; height: 50px; }
      .links { gap: 16px; }
      body { padding: 30px 15px; }
    }
  </style>
</head>
<body>

  <!-- Логотип → ведёт на сайт -->
  <a href="https://chotko.pro/" target="_blank" class="logo-link">
    <img src="logo.jpg" class="logo-img" alt="ЧЁТКО РЕМОНТ">
  </a>

  <!-- Иконки соцсетей -->
  <div class="links">
    <!-- Instagram -->
    <a href="https://www.instagram.com/chotko.remont" target="_blank" class="link-icon">
      <svg viewBox="0 0 24 24" fill="#E4405F"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.979 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.979.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/></svg>
    </a>

    <!-- VK — используем предыдущий логотип (на чёрном фоне) -->
    <a href="https://vk.com/chotko_remont" target="_blank" class="link-icon">
      <img src="https://i.pinimg.com/736x/92/91/fa/9291fa922e31b2a1beacec812ed891fa.jpg" alt="VK">
    </a>

    <!-- Telegram — используем изображение из Яндекса -->
    <a href="https://t.me/chotko_remont_krd" target="_blank" class="link-icon">
      <img src="https://avatars.mds.yandex.net/i?id=59ad32b95a3f099f21338cc597ca7f51_sr-5210787-images-thumbs&n=13" alt="Telegram">
    </a>

    <!-- WhatsApp -->
    <a href="https://wa.me/79937711170" target="_blank" class="link-icon">
      <svg viewBox="0 0 24 24" fill="#25D366"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.521.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.521-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
    </a>

    <!-- YouTube — используем изображение из Яндекса -->
    <a href="https://youtube.com/@chotkoremont" target="_blank" class="link-icon">
      <img src="https://avatars.mds.yandex.net/i?id=0bb017a96532bda477444661bfd672a1_l-7675486-images-thumbs&n=13" alt="YouTube">
    </a>
  </div>

</body>
</html>
