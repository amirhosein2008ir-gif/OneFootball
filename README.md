<!doctype html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>نام سایت شما — خوش آمدید</title>
  <meta name="description" content="قالب زیبا و سبک برای صفحه GitHub Pages شما — قابل ویرایش و واکنش‌گرا">

  <!-- گوگل فونت (بدون نیاز به کتابخانه خارجی پیچیده) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#0f1724; /* رنگ پس‌زمینه تیره */
      --card:#0b1220;
      --muted:#94a3b8;
      --accent:#7c3aed;
      --glass: rgba(255,255,255,0.03);
      --radius:14px;
      --maxw:1100px;
    }
    [data-theme='light']{ --bg:#f8fafc; --card:#ffffff; --muted:#475569; --accent:#6d28d9; --glass: rgba(15,23,42,0.04); }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      background:linear-gradient(180deg,var(--bg), #020617 140%);
      color: #e6eef8;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
      padding:32px 20px;
      display:flex;justify-content:center;
    }

    .wrap{max-width:var(--maxw); width:100%;}
    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:28px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:48px;height:48px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#fb7185);display:grid;place-items:center;font-weight:800;color:white}
    .site-title{font-weight:700;font-size:18px}
    .site-sub{font-size:13px;color:var(--muted)}

    nav a{color:var(--muted);text-decoration:none;margin-left:18px}
    nav a:hover{color:var(--accent)}

    .theme-toggle{background:var(--glass);border:1px solid rgba(255,255,255,0.03);padding:8px 10px;border-radius:10px;cursor:pointer}

    .hero{display:grid;grid-template-columns:1fr 380px;gap:28px;align-items:center;margin-bottom:30px}
    @media (max-width:900px){.hero{grid-template-columns:1fr;}.hero-right{order:-1}}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);border-radius:var(--radius);padding:22px;box-shadow:0 6px 20px rgba(2,6,23,0.6)}

    .intro h1{margin:0 0 10px 0;font-size:32px}
    .intro p{margin:0;color:var(--muted)}
    .cta{margin-top:16px;display:flex;gap:12px}
    .btn{padding:10px 14px;border-radius:12px;border:0;cursor:pointer;font-weight:600}
    .btn-primary{background:linear-gradient(90deg,var(--accent),#fb7185);color:white}
    .btn-ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted)}

    .hero-right{display:flex;flex-direction:column;gap:12px}
    .stats{display:flex;gap:12px}
    .stat{flex:1;background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);padding:12px;border-radius:12px;text-align:center}
    .stat strong{display:block;font-size:18px}
    .projects{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:18px}
    @media (max-width:900px){.projects{grid-template-columns:repeat(2,1fr)}}
    @media (max-width:520px){.projects{grid-template-columns:1fr}}

    .project{padding:12px;border-radius:12px;background:var(--card);border:1px solid rgba(255,255,255,0.02)}
    .project h3{margin:0 0 6px 0}
    .project p{margin:0;color:var(--muted);font-size:13px}

    .grid{display:grid;grid-template-columns:2fr 1fr;gap:20px}
    @media (max-width:900px){.grid{grid-template-columns:1fr}}

    .posts{display:flex;flex-direction:column;gap:12px}
    .post{padding:12px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.01), transparent);border:1px solid rgba(255,255,255,0.02)}
    .post small{color:var(--muted)}

    footer{margin-top:28px;padding:18px;border-radius:12px;background:transparent;display:flex;justify-content:space-between;align-items:center;color:var(--muted)}

    /* small helpers */
    .muted{color:var(--muted)}
    a.social{display:inline-flex;gap:8px;align-items:center;text-decoration:none;color:var(--muted)}

  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">GH</div>
        <div>
          <div class="site-title">نام پروژه شما</div>
          <div class="site-sub">توضیح کوتاه دربارهٔ پروژه</div>
        </div>
      </div>

      <div style="display:flex;align-items:center;gap:12px">
        <nav class="muted">
          <a href="#projects">پروژه‌ها</a>
          <a href="#posts">نوشته‌ها</a>
          <a href="#contact">ارتباط</a>
        </nav>
        <button class="theme-toggle" id="themeToggle" aria-label="تغییر پوسته">تاریک/روشن</button>
      </div>
    </header>

    <main>
      <section class="hero">
        <div class="card intro">
          <h1>سلام! من <span style="color:var(--accent)">نام شما</span> هستم</h1>
          <p>در اینجا پروژه‌ها، آزمایش‌ها و یادداشت‌های من در زمینهٔ توسعه وب و متن‌باز را می‌توانید ببینید. این قالب ساده، سریع و قابل سفارشی‌سازی است.</p>
          <div class="cta">
            <a class="btn btn-primary" href="#projects">مشاهده پروژه‌ها</a>
            <a class="btn btn-ghost" href="https://github.com/USERNAME" target="_blank">رفتن به گیت‌هاب</a>
          </div>

          <div class="projects" id="projects" style="margin-top:20px">
            <!-- هر "project" را با پروژه‌ها یا ریپوهایتان جایگزین کنید -->
            <article class="project">
              <h3>پروژهٔ نمونه ۱</h3>
              <p>توضیح کوتاه — زبان: JavaScript — وضعیت: فعال</p>
            </article>
            <article class="project">
              <h3>پروژهٔ نمونه ۲</h3>
              <p>توضیح کوتاه — زبان: Python — وضعیت: آزمایشی</p>
            </article>
            <article class="project">
              <h3>پروژهٔ نمونه ۳</h3>
              <p>توضیح کوتاه — زبان: HTML/CSS — وضعیت: منتشر شده</p>
            </article>
          </div>
        </div>

        <aside class="hero-right">
          <div class="card">
            <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px">
              <div><strong>خلاصه</strong><div class="muted" style="font-size:13px">خلاصه‌ای از وضعیت شما</div></div>
            </div>
            <div class="stats">
              <div class="stat">
                <small class="muted">ریپوها</small>
                <strong>12</strong>
              </div>
              <div class="stat">
                <small class="muted">ستاره</small>
                <strong>340</strong>
              </div>
              <div class="stat">
                <small class="muted">دنبال‌کننده</small>
                <strong>1.2K</strong>
              </div>
            </div>
          </div>

          <div class="card">
            <strong>مهارت‌ها</strong>
            <div style="margin-top:10px;display:flex;flex-wrap:wrap;gap:8px">
              <span style="padding:8px 10px;border-radius:999px;background:rgba(255,255,255,0.02);font-size:13px">JavaScript</span>
              <span style="padding:8px 10px;border-radius:999px;background:rgba(255,255,255,0.02);font-size:13px">Python</span>
              <span style="padding:8px 10px;border-radius:999px;background:rgba(255,255,255,0.02);font-size:13px">React</span>
              <span style="padding:8px 10px;border-radius:999px;background:rgba(255,255,255,0.02);font-size:13px">CSS</span>
            </div>
          </div>

        </aside>
      </section>

      <section class="grid">
        <div>
          <h2 id="posts">نوشته‌های تازه</h2>
          <div class="posts">
            <article class="post">
              <h3>عنوان نوشتهٔ نمونه</h3>
              <small class="muted">۲۰ آبان ۱۴۰۳ — دسته: توسعه</small>
              <p class="muted" style="margin-top:8px">خلاصه کوتاه از نوشته برای جلب توجه خواننده. لینک کامل به فایل MD یا پست در مخزن گیت‌هاب قرار گیرد.</p>
            </article>
            <article class="post">
              <h3>گزارش پروژهٔ جدید</h3>
              <small class="muted">۵ مهر ۱۴۰۳ — دسته: پروژه</small>
              <p class="muted" style="margin-top:8px">توضیح مختصر دربارهٔ کاری که انجام دادید و نکات مهم آن.</p>
            </article>
          </div>
        </div>

        <aside>
          <div class="card" id="contact">
            <h3>تماس</h3>
            <p class="muted">برای همکاری یا سوال، ایمیل بزنید یا از شبکه‌های اجتماعی دیدن کنید.</p>
            <p style="margin-top:8px"><a class="social" href="mailto:you@example.com">📧 you@example.com</a></p>
            <div style="margin-top:12px;display:flex;gap:10px">
              <a class="social" href="https://github.com/USERNAME" target="_blank">🐙 GitHub</a>
              <a class="social" href="https://twitter.com/USERNAME" target="_blank">🐦 Twitter</a>
            </div>
          </div>

          <div class="card" style="margin-top:12px">
            <h4>دانلود رزومه</h4>
            <p class="muted">لینک به فایل PDF رزومه یا لینک Drive</p>
            <a class="btn btn-ghost" href="#">دانلود</a>
          </div>
        </aside>
      </section>

    </main>

    <footer>
      <div class="muted">© ۲۰۲۵ نام شما — ساخته‌شده با ❤️ و GitHub Pages</div>
      <div class="muted">نسخهٔ قالب: 1.0</div>
    </footer>
  </div>

  <script>
    // تنظیم حالت روشن/تاریک با ذخیره در localStorage
    (function(){
      const root = document.documentElement;
      const t = localStorage.getItem('theme') || (window.matchMedia && window.matchMedia('(prefers-color-scheme: light)').matches ? 'light' : 'dark');
      if(t === 'light') root.setAttribute('data-theme','light');
      const btn = document.getElementById('themeToggle');
      btn.addEventListener('click',()=>{
        const cur = root.getAttribute('data-theme') === 'light' ? 'dark' : 'light';
        root.setAttribute('data-theme', cur === 'light' ? 'light' : '');
        localStorage.setItem('theme', cur);
      });
    })();

    // راهنمای سریع: اگر می‌خواهید پروژه‌ها را از API گیت‌هاب بگیرید، از fetch به https://api.github.com/users/USERNAME/repos استفاده کنید و DOM را با نتایج پر کنید.

  </script>

</body>
</html>


  
