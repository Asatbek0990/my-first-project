# my-first-project

<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Asatbek's Portfolio</title>
<style>
  body {
    margin: 0;
    font-family: 'Georgia', serif;
    background: linear-gradient(to bottom right, #6a11cb, #2575fc);
    color: white;
    text-align: center;
  }
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background-color: rgba(0, 0, 0, 0.2);
  }
  .title {
    font-size: 28px;
    font-weight: bold;
    margin: 0 auto;
  }
  .lang-select {
    margin-left: auto;
  }
  .lang-select select {
    padding: 8px 12px;
    font-weight: bold;
    background-color: #ffdd57;
    border: none;
    border-radius: 6px;
  }
  nav {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 20px;
  }
  nav button {
    padding: 12px 24px;
    font-size: 16px;
    font-weight: bold;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    transition: background 0.3s;
  }
  nav button:hover {
    background-color: #ff9800;
    color: white;
  }
  section {
    display: none;
    margin-top: 40px;
    padding: 20px;
  }
  section.active {
    display: block;
  }
  /* Ijtimoiy tarmoqlar linklari uchun */
  .social-links {
    margin-top: 20px;
    display: flex;
    justify-content: center;
    gap: 30px;
  }
  .social-links a {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    text-decoration: none;
    font-weight: bold;
    font-size: 18px;
    padding: 10px 20px;
    border-radius: 12px;
    color: white;
    box-shadow: 0 0 10px rgba(0,0,0,0.3);
    transition: transform 0.3s, box-shadow 0.3s;
  }
  .social-links a:hover {
    transform: scale(1.1);
    box-shadow: 0 0 20px #ff9800;
  }
  .telegram {
    background: #0088cc;
  }
  .instagram {
    background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fd5949 45%, #d6249f 60%, #285aeb 90%);
  }
  .github {
    background: #333;
  }
  /* Ikonalar uchun */
  .social-links svg {
    width: 24px;
    height: 24px;
    fill: white;
  }
</style>
</head>
<body>
<header>
  <div class="title">Asatbek's Portfolio</div>
  <div class="lang-select">
    <select id="language" onchange="changeLanguage()">
      <option value="uz">O'zbekcha</option>
      <option value="en">English</option>
      <option value="ru">Русский</option>
      <option value="ko">한국어</option>
      <option value="tr">Türkçe</option>
    </select>
  </div>
</header>
<nav>
  <button id="btn-about" onclick="showSection('about')">Men haqimda</button>
  <button id="btn-projects" onclick="showSection('projects')">Mening loyihalarim</button>
  <button id="btn-contact" onclick="showSection('contact')">Men bilan bogʻlanish</button>
</nav>

<section id="about" class="active">
  <p id="about-text">
    Men Sadikboyev Asatbek O'zbekiston Respublikasi Namangan tumanida yashayman, yoshim 18 da. Dasturlash, o'yin va dastur yaratishga qiziqaman va shu sohada kelajakda yaxshi dasturchi bo'lishni maqsad qilganman. Bu mening birinchi portfolio saytim. Agar men bilan yaqindan tanishmoqchi bo‘lsangiz, albatta bogʻlaning.
  </p>
</section>

<section id="projects">
  <p id="projects-text">(Loyihalar hozircha mavjud emas)</p>
</section>

<section id="contact">
  <p id="contact-text">(Bogʻlanish maʼlumotlari tez orada qoʻshiladi)</p>
  <div class="social-links">
    <a href="https://t.me/sadikjanovf" class="telegram" target="_blank" rel="noopener noreferrer">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M9.04 16.29l-.38 5.4c.55 0 .8-.23 1.1-.5l2.63-2.54 5.45 4c1 .55 1.74.26 2-.91l3.64-17.03c.35-1.62-.6-2.27-1.64-1.88L1.96 9.75c-1.5.58-1.47 1.4-.26 1.78l5.15 1.6 11.94-7.56c.55-.35 1.05-.16.64.22"/></svg>
      Telegram
    </a>
    <a href="https://instagram.com/asatbeksadikboyev" class="instagram" target="_blank" rel="noopener noreferrer">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M7 2C4.79 2 3 3.79 3 6v12c0 2.21 1.79 4 4 4h10c2.21 0 4-1.79 4-4V6c0-2.21-1.79-4-4-4H7zm10 3a1 1 0 1 1 0 2 1 1 0 0 1 0-2zM12 7a5 5 0 1 1 0 10 5 5 0 0 1 0-10zm0 2a3 3 0 1 0 0 6 3 3 0 0 0 0-6z"/></svg>
      Instagram
    </a>
    <a href="https://github.com/Asatbek0990/my-first-project" class="github" target="_blank" rel="noopener noreferrer">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 .5C5.65.5.5 5.64.5 12a11.5 11.5 0 0 0 7.85 10.94c.58.1.8-.25.8-.56v-2.1c-3.19.7-3.86-1.54-3.86-1.54-.53-1.35-1.3-1.7-1.3-1.7-1.07-.74.08-.73.08-.73 1.18.08 1.8 1.21 1.8 1.21 1.05 1.8 2.75 1.28 3.42.98.1-.77.41-1.28.74-1.57-2.55-.3-5.23-1.28-5.23-5.7 0-1.26.45-2.3 1.2-3.11-.12-.3-.52-1.53.11-3.18 0 0 .98-.31 3.21 1.2a11.25 11.25 0 0 1 5.84 0c2.23-1.51 3.21-1.2 3.21-1.2.63 1.65.23 2.88.11 3.18.75.81 1.2 1.85 1.2 3.11 0 4.43-2.68 5.4-5.24 5.7.42.37.79 1.11.79 2.25v3.34c0 .31.22.67.81.56A11.5 11.5 0 0 0 23.5 12C23.5 5.64 18.35.5 12 .5z"/></svg>
      GitHub
    </a>
  </div>
</section>

<script>
  function showSection(id) {
    document.querySelectorAll('section').forEach(s => s.classList.remove('active'));
    document.getElementById(id).classList.add('active');
  }
  const translations = {
    uz: {
      'btn-about': 'Men haqimda',
      'btn-projects': 'Mening loyihalarim',
      'btn-contact': 'Men bilan bogʻlanish',
      'about-text': "Men Sadikboyev Asatbek O'zbekiston Respublikasi Namangan tumanida yashayman, yoshim 18 da. Dasturlash, o'yin va dastur yaratishga qiziqaman va shu sohada kelajakda yaxshi dasturchi bo'lishni maqsad qilganman. Bu mening birinchi portfolio saytim. Agar men bilan yaqindan tanishmoqchi bo‘lsangiz, albatta bogʻlaning.",
      'projects-text': '(Loyihalar hozircha mavjud emas)',
      'contact-text': '(Bogʻlanish maʼlumotlari tez orada qoʻshiladi)'
    },
    en: {
      'btn-about': 'About Me',
      'btn-projects': 'My Projects',
      'btn-contact': 'Contact Me',
      'about-text': "I am Sadikboyev Asatbek from Namangan, Uzbekistan. I am 18 years old. I am interested in programming, game and app development, and I aim to become a great developer in the future. This is my first portfolio site. If you'd like to know more, feel free to contact me.",
      'projects-text': '(Projects coming soon)',
      'contact-text': '(Contact info will be added soon)'
    },
    ru: {
      'btn-about': 'Обо мне',
      'btn-projects': 'Мои проекты',
      'btn-contact': 'Связаться со мной',
      'about-text': "Я Садикбоев Асатбек из Намангана, Узбекистан. Мне 18 лет. Я интересуюсь программированием, созданием игр и приложений, и стремлюсь стать отличным разработчиком. Это мой первый портфолио-сайт. Если хотите узнать больше — свяжитесь со мной.",
      'projects-text': '(Проекты скоро появятся)',
      'contact-text': '(Контактная информация будет добавлена скоро)'
    },
    ko: {
      'btn-about': '소개',
      'btn-projects': '내 프로젝트',
      'btn-contact': '연락하기',
      'about-text': "저는 우즈베키스탄 남안간 출신의 사디크보예프 아사트벡입니다. 저는 18세이며, 프로그래밍과 게임 및 앱 개발에 관심이 많습니다. 미래에 훌륭한 개발자가 되는 것이 목표입니다. 이것은 제 첫 번째 포트폴리오 사이트입니다. 더 알고 싶으시면 언제든지 연락 주세요.",
      'projects-text': '(곧 프로젝트가 추가됩니다)',
      'contact-text': '(연락처 정보는 곧 추가됩니다)'
    },
    tr: {
      'btn-about': 'Hakkımda',
      'btn-projects': 'Projelerim',
      'btn-contact': 'İletişim',
      'about-text': "Ben Sadıkboyev Asatbek, Özbekistan'ın Namangan bölgesindenim. 18 yaşındayım. Programlama, oyun ve uygulama geliştirmeye ilgi duyuyorum ve gelecekte iyi bir yazılımcı olmayı hedefliyorum. Bu benim ilk portfolyo sitem. Daha fazla bilgi almak isterseniz benimle iletişime geçin.",
      'projects-text': '(Projeler yakında eklenecek)',
      'contact-text': '(İletişim bilgileri yakında eklenecek)'
    }
  };
  function changeLanguage() {
    const lang = document.getElementById('language').value;
    const t = translations[lang];
    for (const id in t) {
      document.getElementById(id).innerText = t[id];
    }
  }
</script>
</body>
</html>



