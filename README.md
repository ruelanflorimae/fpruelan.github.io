[index.html](https://github.com/user-attachments/files/33013522/index.html)
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Flori Mae | General Virtual Assistant</title>
<meta name="description" content="Flori Mae is a general virtual assistant from the Philippines with 7+ years of experience in customer service, collections, admin support and team leadership.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=League+Spartan:wght@600;700;800&family=Mrs+Saint+Delafield&family=Arimo:wght@400;700&display=swap" rel="stylesheet">
<style>
:root{
  --green:#2c542f;
  --green-deep:#1f3d22;
  --cream:#f2f4e6;
  --cream-2:#e6ebd2;
  --ink:#233326;
  --muted:#4d6050;
  --white:#fff;
  --radius:14px;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:'Arimo',system-ui,sans-serif;background:var(--cream);color:var(--ink);line-height:1.65;font-size:17px}
img{max-width:100%;display:block}
a{color:inherit}
h1,h2,h3{font-family:'League Spartan',sans-serif;color:var(--green);line-height:1.1;letter-spacing:.01em}
.wrap{width:min(1120px,100% - 40px);margin-inline:auto}
section{padding:88px 0}

/* nav */
header{position:sticky;top:0;z-index:20;background:rgba(242,244,230,.92);backdrop-filter:blur(8px);border-bottom:1px solid rgba(44,84,47,.12)}
nav{display:flex;align-items:center;justify-content:space-between;height:64px}
.brand{font-family:'Mrs Saint Delafield',cursive;font-size:2.1rem;color:var(--green);text-decoration:none;line-height:1}
nav ul{display:flex;gap:26px;list-style:none}
nav a.link{text-decoration:none;font-weight:700;font-size:.92rem;color:var(--green)}
nav a.link:hover{text-decoration:underline;text-underline-offset:5px}
.btn{display:inline-block;background:var(--green);color:var(--white);padding:13px 28px;border-radius:999px;font-weight:700;text-decoration:none;transition:transform .15s,background .15s;border:0;cursor:pointer;font-size:1rem}
.btn:hover{background:var(--green-deep);transform:translateY(-2px)}
.btn.ghost{background:transparent;color:var(--green);border:2px solid var(--green)}
.btn.ghost:hover{background:var(--green);color:var(--white)}

/* hero */
.hero{padding:64px 0 80px}
.hero .wrap{display:grid;grid-template-columns:minmax(260px,380px) 1fr;gap:64px;align-items:center}
.portrait{position:relative}
.portrait img{border-radius:var(--radius);width:100%;aspect-ratio:5/6;object-fit:cover;object-position:top;box-shadow:14px 14px 0 var(--green)}
.hero .script{font-family:'Mrs Saint Delafield',cursive;font-size:clamp(3.4rem,7vw,5.4rem);color:var(--green);line-height:.9;margin-bottom:6px}
.eyebrow{font-weight:700;letter-spacing:.2em;font-size:.85rem;color:var(--muted);text-transform:uppercase}
.hero h1{font-size:clamp(2.2rem,4.6vw,3.6rem);margin:22px 0 8px}
.hero h2{font-size:clamp(1.3rem,2.4vw,1.8rem);color:var(--ink);font-weight:700;margin-bottom:18px}
.hero p.lead{max-width:50ch;color:var(--muted);margin-bottom:30px}
.cta{display:flex;gap:14px;flex-wrap:wrap}
.stats{display:flex;gap:34px;margin-top:44px;padding-top:26px;border-top:2px solid rgba(44,84,47,.18);flex-wrap:wrap}
.stats b{display:block;font-family:'League Spartan',sans-serif;font-size:2rem;color:var(--green)}
.stats span{font-size:.85rem;color:var(--muted)}

/* about */
.about{background:var(--cream-2)}
.about .wrap{display:grid;grid-template-columns:minmax(220px,320px) 1fr;gap:60px;align-items:center}
.about img{border:10px solid var(--green);border-radius:6px;width:100%}
h2.title{font-size:clamp(2rem,4vw,2.9rem);margin-bottom:22px}
.about p{margin-bottom:16px;max-width:62ch}

/* skills */
.skills{background:var(--green);color:var(--cream)}
.skills h2.title{color:var(--cream);text-align:center;letter-spacing:.22em;margin-bottom:48px}
.skill-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:22px}
.skill{background:rgba(255,255,255,.07);border:1px solid rgba(242,244,230,.22);border-radius:var(--radius);padding:26px}
.skill h3{color:var(--cream);font-size:1.15rem;letter-spacing:.04em;margin-bottom:14px;display:flex;gap:10px;align-items:center}
.skill ul{list-style:none;display:flex;flex-direction:column;gap:5px;font-size:.95rem}
.skill li::before{content:"•";color:#b9d3a8;margin-right:9px}

/* services */
.services .wrap{display:grid;grid-template-columns:1.15fr 1fr;gap:56px;align-items:start}
.services p{margin-bottom:16px;color:var(--muted)}
.services p strong{color:var(--ink)}
.cards{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.cards img{border-radius:10px;border:3px solid #111;background:#fff}

/* works */
.works{background:var(--cream-2)}
.works h2.title{text-align:center;letter-spacing:.06em}
.works .sub{text-align:center;color:var(--muted);margin:-8px auto 44px;max-width:52ch}
.work-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:26px;align-items:start}
.work{background:var(--white);border-radius:var(--radius);padding:14px 14px 18px;box-shadow:0 8px 24px rgba(31,61,34,.1);display:flex;flex-direction:column}
.work.wide{grid-column:1/-1}
.work button{border:0;background:#f7f8f1;border-radius:8px;cursor:zoom-in;padding:0;overflow:hidden;flex:1;display:flex;align-items:center;justify-content:center}
.work img{width:100%;height:100%;object-fit:contain;transition:transform .3s}
.work button:hover img{transform:scale(1.03)}
.work figcaption{font-family:'League Spartan',sans-serif;color:var(--green);font-weight:700;letter-spacing:.08em;text-transform:uppercase;text-align:center;margin-top:14px}
.work .pair{display:grid;grid-template-columns:1fr 1fr;gap:12px;flex:1}

/* tools */
.tools{text-align:center}
.tools img{margin:30px auto 0;border-radius:var(--radius);max-width:880px;width:100%}

/* contact */
.contact{background:var(--green);color:var(--cream)}
.contact .wrap{display:grid;grid-template-columns:1.2fr 1fr;gap:56px;align-items:center}
.contact h2{color:var(--cream);font-size:clamp(2rem,4.4vw,3.2rem)}
.contact h3{color:var(--cream);font-size:1.4rem;margin:14px 0 18px;font-weight:700}
.contact p{max-width:48ch;margin-bottom:12px;color:#dfe8d2}
.contact .getin{background:var(--cream);color:var(--green);border-radius:var(--radius);padding:34px}
.contact .getin h2{color:var(--green);margin-bottom:16px;font-size:2rem}
.contact .getin a.row{display:flex;gap:12px;align-items:center;padding:12px 0;border-top:1px solid rgba(44,84,47,.18);text-decoration:none;font-weight:700;color:var(--green)}
.contact .getin a.row:hover{text-decoration:underline}
.contact .getin small{display:block;color:var(--muted);margin-top:14px}
footer{background:var(--green-deep);color:#b8c9b0;text-align:center;padding:20px;font-size:.85rem}

/* lightbox */
dialog{border:0;background:transparent;max-width:min(1200px,94vw);max-height:92vh;margin:auto;overflow:visible}
dialog::backdrop{background:rgba(15,28,17,.85)}
dialog img{max-height:86vh;border-radius:8px;background:#fff}
dialog button{position:absolute;top:-14px;right:-14px;width:38px;height:38px;border-radius:50%;border:0;background:var(--cream);color:var(--green);font-size:1.3rem;font-weight:700;cursor:pointer}

@media (max-width:860px){
  section{padding:64px 0}
  nav ul{display:none}
  .hero .wrap,.about .wrap,.services .wrap,.contact .wrap{grid-template-columns:1fr;gap:38px}
  .portrait{max-width:330px}
  .about img{max-width:260px}
  .work-grid{grid-template-columns:1fr}
}
@media (prefers-reduced-motion:reduce){*{transition:none!important;scroll-behavior:auto!important}}
</style>
</head>
<body>

<header>
  <nav class="wrap" aria-label="Main">
    <a class="brand" href="#top">Flori Mae</a>
    <ul>
      <li><a class="link" href="#about">About</a></li>
      <li><a class="link" href="#skills">Skills</a></li>
      <li><a class="link" href="#services">Services</a></li>
      <li><a class="link" href="#works">Sample Works</a></li>
      <li><a class="link" href="#tools">Tools</a></li>
    </ul>
    <a class="btn" href="#contact">Let’s Connect</a>
  </nav>
</header>

<main id="top">
  <section class="hero">
    <div class="wrap">
      <div class="portrait">
        <img src="images/portrait.jpg" alt="Portrait of Flori Mae, general virtual assistant" width="591" height="699">
      </div>
      <div>
        <p class="script">Flori Mae</p>
        <p class="eyebrow">General Virtual Assistant</p>
        <h1>Your Business Has Enough</h1>
        <h2>On Its Plate. Let Me Help.</h2>
        <p class="lead">I provide reliable virtual assistance that takes care of the details so you can focus on running and growing your business.</p>
        <div class="cta">
          <a class="btn" href="#contact">Let’s Connect!</a>
          <a class="btn ghost" href="#works">See my work</a>
        </div>
        <div class="stats">
          <div><b>7+</b><span>years of experience</span></div>
          <div><b>45–50</b><span>WPM typing speed</span></div>
          <div><b>PH</b><span>based in the Philippines</span></div>
        </div>
      </div>
    </div>
  </section>

  <section class="about" id="about">
    <div class="wrap">
      <img src="images/desk.jpg" alt="A tidy desk with a laptop, coffee, planner and glasses" loading="lazy">
      <div>
        <h2 class="title">About Me</h2>
        <p>Hi, I’m Flori Mae, a dedicated Virtual Assistant from the Philippines with 7+ years of experience in customer service, collections, administrative support, and team leadership.</p>
        <p>Throughout my career, I’ve developed strong skills in data management, documentation, email communication, follow-ups, research, reporting, and organizing information.</p>
        <p>These experiences taught me how to manage multiple tasks, work with attention to detail, meet deadlines, and communicate professionally.</p>
        <p>As a Virtual Assistant, my goal is simple: to make your work easier and give you more time to focus on what matters most, growing your business.</p>
        <p>I can support you with administrative tasks, lead generation, data entry, email and calendar management, social media support, and other day-to-day business needs.</p>
        <p><strong>I’m a fast learner, adaptable, organized, and committed to providing reliable support you can count on. Let’s get things done one task at a time.</strong></p>
      </div>
    </div>
  </section>

  <section class="skills" id="skills">
    <div class="wrap">
      <h2 class="title">S-K-I-L-L-S</h2>
      <div class="skill-grid">
        <article class="skill">
          <h3><span aria-hidden="true">🔎</span> Lead Generation</h3>
          <ul><li>Social Media Outreach</li><li>B2B &amp; B2C Prospecting</li><li>Prospect List Creation</li><li>Data Scraping</li><li>Skip Tracing</li><li>Lead Research</li><li>Email Marketing</li><li>Online Research</li></ul>
        </article>
        <article class="skill">
          <h3><span aria-hidden="true">📱</span> Social Media Management</h3>
          <ul><li>Social Media Marketing</li><li>Social Media Outreach</li><li>Content Creation</li><li>Post Creation</li><li>Content Scheduling</li><li>Canva Graphic Design</li><li>Basic Video Editing</li><li>Social Media Calendar Management</li><li>Meta Business Suite</li><li>Buffer</li><li>Publer</li></ul>
        </article>
        <article class="skill">
          <h3><span aria-hidden="true">📊</span> Data Entry &amp; Admin Support</h3>
          <ul><li>Data Entry &amp; Encoding</li><li>Data Collection &amp; Organization</li><li>Google Sheets</li><li>Google Docs</li><li>Microsoft Excel</li><li>Microsoft Office</li><li>Data Management</li><li>File &amp; Document Organization</li><li>Database Updating</li><li>45–50 WPM Typing Speed</li></ul>
        </article>
        <article class="skill">
          <h3><span aria-hidden="true">👩‍💼</span> Executive / Administrative Support</h3>
          <ul><li>Calendar Management</li><li>Email Management</li><li>Microsoft Outlook</li><li>Administrative Tasks</li><li>Meeting &amp; Schedule Coordination</li><li>Email Correspondence</li><li>Document Preparation</li><li>Data Organization</li><li>Online Research</li><li>Task &amp; File Management</li></ul>
        </article>
      </div>
    </div>
  </section>

  <section class="services" id="services">
    <div class="wrap">
      <div>
        <h2 class="title">What Can I Do?</h2>
        <p>I provide reliable virtual support to help businesses stay organized, productive, and on track. With experience in administrative support, data entry, lead generation, customer service, and online research, I help manage the day-to-day tasks that keep your business running smoothly.</p>
        <p>From document preparation, email and calendar management, data entry, lead research, prospect list building, and outreach to task tracking and customer support, I focus on <strong>accuracy, organization, and getting things done efficiently.</strong></p>
        <p>I also provide basic Canva graphic design and content support. While I’m not an advanced graphic designer, I can create clean, simple, and professional visuals, make layout adjustments, and follow your brand guidelines and requirements.</p>
        <p><strong>My goal is simple: to take care of the details, support your workflow, and give you more time to focus on growing your business.</strong></p>
      </div>
      <div class="cards">
        <img src="images/card-admin.jpg" alt="Admin task services card" loading="lazy">
        <img src="images/card-data.jpg" alt="Data entry services card" loading="lazy">
        <img src="images/card-lead.jpg" alt="Lead generation services card" loading="lazy">
        <img src="images/card-graphic.jpg" alt="Graphic designer services card" loading="lazy">
      </div>
    </div>
  </section>

  <section class="works" id="works">
    <div class="wrap">
      <h2 class="title">Selected Sample Works</h2>
      <p class="sub">A few examples of the kind of work I do. Tap any image to view it larger.</p>
      <div class="work-grid">
        <figure class="work wide"><button type="button" data-zoom><img src="images/leadgen.jpg" alt="Lead generation prospect list in a spreadsheet, with contact emails blurred" loading="lazy"></button><figcaption>Lead Generation</figcaption></figure>
        <figure class="work wide"><button type="button" data-zoom><img src="images/calendar.jpg" alt="Google Calendar events being scheduled" loading="lazy"></button><figcaption>Calendar Management</figcaption></figure>
        <figure class="work"><button type="button" data-zoom><img src="images/email-mgmt.jpg" alt="Organized Gmail inbox with labels" loading="lazy"></button><figcaption>Email Management</figcaption></figure>
        <figure class="work"><button type="button" data-zoom><img src="images/data-entry.jpg" alt="Data entry in Google Sheets" loading="lazy"></button><figcaption>Data Entry</figcaption></figure>
        <figure class="work wide"><button type="button" data-zoom><img src="images/content-creation.jpg" alt="Content calendar with captions and hashtags in Google Sheets" loading="lazy"></button><figcaption>Content Creation</figcaption></figure>
        <figure class="work wide"><button type="button" data-zoom><img src="images/email-marketing.jpg" alt="Scheduled marketing email in Gmail" loading="lazy"></button><figcaption>Email Marketing</figcaption></figure>
        <figure class="work wide"><button type="button" data-zoom><img src="images/task-mgmt.jpg" alt="Task boards in a project management tool" loading="lazy"></button><figcaption>Task Management</figcaption></figure>
        <figure class="work wide"><button type="button" data-zoom><img src="images/graphic-design.jpg" alt="Social media graphics designed in Canva" loading="lazy"></button><figcaption>Graphic Designing</figcaption></figure>
        <figure class="work wide"><button type="button" data-zoom><img src="images/scheduling.jpg" alt="Scheduling a Facebook post in Meta Business Suite" loading="lazy"></button><figcaption>Content Scheduling</figcaption></figure>
      </div>
    </div>
  </section>

  <section class="tools" id="tools">
    <div class="wrap">
      <h2 class="title">I am Familiar With:</h2>
      <img src="images/logos.jpg" alt="Tools I use: LinkedIn Sales Solutions, Apollo.io, Canva, Zoom, Lark, Notion, Microsoft Teams, Clay, Google Workspace, Gemini, Gmail, Microsoft Office, Yelp, Buffer, Dropbox, Outlook, CapCut, ClickUp, LinkedIn, ChatGPT, Slack and monday.com" loading="lazy">
    </div>
  </section>

  <section class="contact" id="contact">
    <div class="wrap">
      <div>
        <h2>Your Business<br>Has Enough</h2>
        <h3>On Its Plate. Let Me Help.</h3>
        <p>If you’re looking for a dependable, creative, and hardworking freelancer, I’m here for you. Please let me know how I can assist you and your company in succeeding.</p>
        <p>A remote and trusted asset for you and/or your business, accomplishing the projects left untouched on your “To Do List.”</p>
        <p><em>The only way to do great work is to love what you do.</em></p>
      </div>
      <div class="getin">
        <h2>Get In Touch</h2>
        <!-- TODO: replace the email below with your real contact details -->
        <a class="row" href="mailto:youremail@example.com">✉️ youremail@example.com</a>
        <small>Message me and let’s talk about how I can help.</small>
      </div>
    </div>
  </section>
</main>

<footer>© <span id="y"></span> Flori Mae · General Virtual Assistant</footer>

<dialog id="lb" aria-label="Enlarged sample"><button type="button" aria-label="Close">×</button><img alt=""></dialog>

<script>
document.getElementById('y').textContent = new Date().getFullYear();
const lb = document.getElementById('lb'), lbImg = lb.querySelector('img');
document.querySelectorAll('[data-zoom]').forEach(b => b.addEventListener('click', () => {
  const i = b.querySelector('img'); lbImg.src = i.src; lbImg.alt = i.alt; lb.showModal();
}));
lb.addEventListener('click', e => { if (e.target === lb || e.target.tagName === 'BUTTON') lb.close(); });
</script>
</body>
</html>
