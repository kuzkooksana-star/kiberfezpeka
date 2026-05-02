<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Вступ до Кібербезпеки</title>
  <style>
    * { 
      box-sizing: border-box; 
      margin: 0; 
      padding: 0; 
    }
    body { 
      font-family: Arial, sans-serif; 
      line-height: 1.6; 
      background-color: #f4f4f4; 
      color: #333; 
      scroll-behavior: smooth; 
    }
    header { 
      background-color: #0b3e6f; 
      color: white; 
      padding: 1rem 2rem; 
      position: sticky; 
      top: 0; 
      z-index: 10; 
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    header h1 { 
      margin-bottom: 0.5rem; 
    }
    nav { 
      display: flex; 
      flex-wrap: wrap; 
      gap: 1rem; 
    }
    nav a { 
      color: #fff; 
      text-decoration: none; 
      font-size: 0.95rem; 
      padding: 0.5rem 1rem; 
      border-radius: 4px; 
      transition: all 0.3s; 
      border: 1px solid transparent;
    }
    nav a:hover { 
      background-color: #fff2; 
      border-color: #fff; 
    }
    nav a.active { 
      background-color: #fff; 
      color: #0b3e6f; 
      font-weight: bold;
    }
    main { 
      max-width: 1000px; 
      margin: 2rem auto; 
      padding: 0 1rem; 
    }
    section { 
      margin-bottom: 3rem; 
      padding: 2.5rem; 
      background: linear-gradient(135deg, #e8f4f8 0%, #d1ecf1 100%); 
      border-radius: 12px; 
      box-shadow: 0 4px 15px rgba(0,0,0,0.1);
      scroll-margin-top: 100px; 
    }
    h2 { 
      color: #0b3e6f; 
      margin-bottom: 1.5rem; 
      font-size: 2rem;
      border-bottom: 3px solid #0b3e6f;
      padding-bottom: 0.5rem;
    }
    h3 { 
      color: #0b3e6f; 
      margin: 1.5rem 0 1rem 0;
    }
    p {
      margin-bottom: 1rem;
    }
    ul { 
      margin: 1rem 0 1rem 2rem; 
    }
    li {
      margin-bottom: 0.5rem;
    }
    code {
      background: #f4f4f4;
      padding: 0.2rem 0.4rem;
      border-radius: 3px;
      font-family: monospace;
    }
    footer { 
      text-align: center; 
      padding: 2rem; 
      background-color: #0b3e6f; 
      color: white; 
      margin-top: 4rem;
      font-size: 0.9rem;
    }
    .intro {
      background: linear-gradient(135deg, #b8e6ff 0%, #e8f4f8 100%);
      border: 2px solid #0b3e6f;
    }
    @media (max-width: 768px) {
      nav { justify-content: center; }
      section { padding: 1.5rem; margin-bottom: 2rem; }
      h2 { font-size: 1.5rem; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Вступ до Кібербезпеки</h1>
    <nav>
      <a href="#home" onclick="setActive(this)">Головна</a>
      <a href="#history" onclick="setActive(this)">Кібербезпека. Минуле. Сучасність.</a>
      <a href="#attacks" onclick="setActive(this)">Атаки та загрози</a>
      <a href="#protection" onclick="setActive(this)">Кіберзахист</a>
      <a href="#countermeasures" onclick="setActive(this)">Протидія кіберзагрозам</a>
      <a href="#math" onclick="setActive(this)">Математика в кібербезпеці</a>
      <a href="#programming" onclick="setActive(this)">Програмування і кібербезпека</a>
      <a href="#osint" onclick="setActive(this)">OSINT</a>
      <a href="#theme" onclick="setActive(this)">Тема проекту</a>
    </nav>
  </header>

  <main>
    <section id="home" class="intro">
      <h2>Вступ до Кібербезпеки</h2>
      <p>Навчальний веб-проект з основ кібербезпеки. Сайт містить структурований теоретичний матеріал по ключових аспектах: історія розвитку, типи кібератак, методи захисту, протидія загрозам, математичні основи, програмування та OSINT-розвідка.</p>
      
      <h3>Основні поняття</h3>
      <p>Кібербезпека — це комплекс організаційних та технічних заходів для захисту конфіденційності, цілісності та доступності інформації в кіберпросторі. Ключова модель — CIA-триада: Confidentiality (конфіденційність), Integrity (цілісність), Availability (доступність). [web:7][web:10]</p>
      <p>У 2026 році кіберзагрози досягли критичного рівня: державні атаки, ransomware, AI-генерований фішинг. Захист стає національною безпекою.</p>
    </section>
<section id="history">
      <h2>Кібербезпека. Минуле. Сучасність.</h2>
      <p>Історія кібербезпеки починається з 1960-х років та ARPANET — прототипу інтернету. Перша масова атака — Morris Worm (1988), яка заразила 6000 комп'ютерів та паралізувала 10% тодішнього інтернету.</p>
      <p>2000-і роки: віруси (ILOVEYOU, Code Red), троянські програми. 2010-і: Stuxnet (2010) — перша кіберзброя проти ядерних об'єктів. Сучасність: AI-атаки, deepfake фішинг, квантові загрози для RSA. [web:6]</p>
      <p>В Україні Закон України №2163-VIII від 5 жовтня 2017 року "Про основні засади забезпечення кібербезпеки України" визначає кіберпростір як об'єкт національної безпеки. CERT-UA координує протидію. [web:13]</p>
    </section>

    <section id="attacks">
      <h2>Атаки та загрози</h2>
      
      <h3>Класифікація кібератак</h3>
      <p>Фішинг — соціальна інженерія для отримання облікових даних. DDoS (Distributed Denial of Service) — масовий трафік для відключення сервісів. Ransomware — шифрування даних з вимогою викупу.</p>
      <p>Технічні атаки: XSS (Cross-Site Scripting) — ін'єкція JavaScript, SQL-ін'єкції — маніпуляція базами даних, Zero-Day — експлойти невідомих вразливостей. [web:16][web:19]</p>
      <p>Статистика 2025: Україна зазнала понад 40% зростання кібератак через гібридну війну. Фішинг становить 90% успішних інцидентів.</p>
    </section>

    <section id="protection">
      <h2>Кіберзахист</h2>
      <p>Технічні засоби: антивірусне ПЗ (Kaspersky, ESET), мережеві фаєрволи (pfSense), системи виявлення вторгнень IDS/IPS, VPN (WireGuard, OpenVPN), шифрування AES-256.</p>
      <p>Організаційні заходи: двофакторна аутентифікація (2FA/TOTP), політики складних паролів, регулярні аудити безпеки, резервне копіювання за правилом 3-2-1.</p>
      <p>Стандарти: ISO/IEC 27001 (системи менеджменту інформаційної безпеки), NIST Cybersecurity Framework, CIS Controls. [web:7][web:12]</p>
    </section>

    <section id="countermeasures">
      <h2>Протидія кіберзагрозам</h2>
      <p>Життєвий цикл кібербезпеки за NIST: Identify → Protect → Detect → Respond → Recover. Моніторинг через SIEM-системи (Splunk, ELK Stack).</p>
      <p>Пентестинг (penetration testing) — моделювання атак етичними хакерами. Red Team (атака) vs Blue Team (захист). Bug Bounty програми.</p>
      <p>В Україні CERT-UA обробляє понад 1000 інцидентів щомісяця, координує міжвідомчу взаємодію. [web:21][web:5]</p>
    </section>

    <section id="math">
      <h2>Математика в кібербезпеці</h2>
      <p>RSA-алгоритм: вибір двох великих простих чисел \\( p \\) та \\( q \\), обчислення модуля \\( n = p \times q \\), функція Ейлера \\( \phi(n) = (p-1)(q-1) \\), вибір \\( e \\) та обчислення \\( d \\).</p>
      <p>Хеш-функції: SHA-256 генерує 256-бітний дайджест. Властивості: незворотність, лавинний ефект, стійкість до колізій.</p>
      <p>Еліптична криптографія (ECC): точки на еліптичній кривій \\( y^2 = x^3 + ax + b \\). ECC-512 еквівалентна RSA-15360 за безпекою. [web:5][web:9]</p>
    </section>

    <section id="programming">
      <h2>Програмування і кібербезпека</h2>
      <p>Python для кібербезпеки: nmap для сканування портів, requests/scapy для тестування, hashlib/pycryptodome для криптографії, pwntools для CTF.</p>
      <p>Безпека веб-додатків: валідація input() → .strip().lower(), захист від SQL-ін'єкцій параметризованими запитами, CSRF-токени, Content Security Policy.</p>
      <p>Приклад безпечного хешування паролів: <code>hashlib.pbkdf2_hmac('sha256', password.encode(), salt, 100000)</code>. JWT для API-аутентифікації. [web:8]</p>
    </section>

    <section id="osint">
      <h2>OSINT (Open Source Intelligence)</h2>
      <p>Методологія розвідки з відкритих джерел: пасивна (WHOIS, DNS), активна (Shodan, Censys). Інструменти: theHarvester, recon-ng, Spiderfoot.</p>
      <p>Google Dorks: <code>site:ua filetype:pdf конфіденційно</code>, <code>inurl:(admin|login) intitle:"panel admin"</code>, <code>intext:"password" filetype:xls</code>.</p>
<p>Спеціалізовані: Shodan для IoT-пристроїв, Have I Been Pwned для компрометацій, Maltego для зв'язків сутностей. Етика: тільки публічна інформація. [web:11]</p>
    </section>

    <section id="theme">
      <h2>Тема проекту</h2>
      
      <h3>Мета та завдання</h3>
      <p>Розробити веб-ресурс для систематизації теоретичних знань з кібербезпеки. Охопити 9 ключових тем від історії до сучасних методів OSINT-розвідки.</p>
      
      <h3>Використані джерела</h3>
      <ul>
        <li>Закон України №2163-VIII "Про основні засади забезпечення кібербезпеки України"</li>
        <li>Методичні рекомендації ДССЗЗІ та CERT-UA</li>
        <li>Стандарти ISO/IEC 27001, NIST SP 800-53</li>
        <li>OWASP Top 10 Web Application Security Risks</li>
        <li>Матеріали конференцій Black Hat, DEF CON</li>
      </ul>
      
      <h3>Технологічний стек</h3>
      <p>Розробка: HTML5, CSS3 (Flexbox, Grid, Animations), Vanilla JavaScript (smooth scroll, active nav). Адаптивний дизайн для desktop/mobile.</p>
      
      <h3>Висновки</h3>
      <p>Кібербезпека у 2026 році — комплексна дисципліна на стику IT, математики, права та психології. Базові знання дозволяють протистояти 95% загроз. Постійне навчання та моніторинг — ключ до захисту.</p>
    </section>
  </main>

  <footer>
    <p>&copy; 2026 Вступ до Кібербезпеки<br>
    Оксана Кузько | Саперна Слобідка, Київ<br>
    Навчальний проект з інформаційної безпеки</p>
  </footer>

  <script>
    function setActive(link) {
      document.querySelectorAll('nav a').forEach(a => a.classList.remove('active'));
      link.classList.add('active');
    }

    window.addEventListener('hashchange', function() {
      const hash = window.location.hash || '#home';
      const activeLink = document.querySelector(`nav a[href="${hash}"]`);
      if (activeLink) {
        setActive(activeLink);
      }
    });

    window.addEventListener('load', function() {
      const hash = window.location.hash || '#home';
      const activeLink = document.querySelector(`nav a[href="${hash}"]`);
      if (activeLink) {
        setActive(activeLink);
      }
    });
  </script>
</body>
</html>
