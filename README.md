
<html lang="en">
    <meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Executive District | Fractional C-Suite Leadership</title>
  <meta name="description" content="Fractional C-suite leadership for founders struggling with profit, isolation, and unclear next steps.">
  <link href="https://fonts.googleapis.com/css2?family=Instrument+Serif&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --warm-black: #0c0e14;
      --charcoal: #2e2a25;
      --terra: #c07a4a;
      --terra-soft: #d4805e;
      --sand: #f5efe6;
      --sand-dark: #e8dfd2;
      --cream: #faf8f4;
      --warm-gray: #8a8680;
      --text: #3d3833;
      --text-light: #706860;
      --white: #ffffff;
    }

    html { scroll-behavior: smooth; }

    body {
      font-family: 'Inter', -apple-system, sans-serif;
      color: var(--text);
      background: var(--cream);
      line-height: 1.7;
      font-weight: 300;
    }

    h1, h2, h3, .serif { font-family: 'Instrument Serif', Georgia, serif; font-weight: 400; }

    /* -- Sticky Nav -- */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 100;
      padding: 1.25rem 3rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      transition: background 0.4s, box-shadow 0.4s;
    }

    nav.scrolled {
      background: rgba(250, 248, 244, 0.95);
      backdrop-filter: blur(16px);
      box-shadow: 0 1px 0 rgba(0,0,0,0.05);
    }

    .logo {
      display: flex;
      flex-direction: column;
      text-decoration: none;
      line-height: 1.1;
    }

    .logo-primary {
      font-family: Georgia, 'Times New Roman', serif;
      font-size: 1.4rem;
      letter-spacing: 2px;
      color: var(--warm-black);
    }

    .logo-accent {
      font-family: Georgia, 'Times New Roman', serif;
      font-size: 1.4rem;
      letter-spacing: 2px;
      color: var(--terra);
    }

    .nav-cta {
      font-size: 0.72rem;
      font-weight: 500;
      letter-spacing: 2px;
      text-transform: uppercase;
      text-decoration: none;
      color: var(--terra);
      border: 1px solid var(--terra);
      padding: 0.6rem 1.5rem;
      border-radius: 100px;
      transition: all 0.3s;
    }

    .nav-cta:hover {
      background: var(--terra);
      color: var(--white);
    }

    /* -- Hero -- */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 8rem 3rem 6rem;
      max-width: 1200px;
      margin: 0 auto;
    }

    .hero h1 {
      font-size: clamp(3rem, 7vw, 6rem);
      line-height: 1.05;
      color: var(--warm-black);
      max-width: 900px;
      margin-bottom: 2.5rem;
    }

    .hero h1 span {
      color: var(--terra);
      font-style: italic;
    }

    .hero-body {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 4rem;
      align-items: start;
      max-width: 900px;
    }

    .hero-body p {
      font-size: 1.15rem;
      color: var(--text-light);
      line-height: 1.8;
    }

    .hero-body .lead {
      font-family: 'Instrument Serif', Georgia, serif;
      font-size: 1.5rem;
      line-height: 1.5;
      color: var(--text);
    }

    .hero-image {
      margin-top: 3rem;
      max-width: 100%;
      border-radius: 4px;
      overflow: hidden;
    }

    .hero-image img {
      width: 100%;
      height: 400px;
      object-fit: cover;
      display: block;
      filter: grayscale(20%) contrast(1.05);
    }

    .scroll-hint {
      margin-top: 4rem;
      font-size: 0.7rem;
      font-weight: 500;
      letter-spacing: 3px;
      text-transform: uppercase;
      color: var(--warm-gray);
      display: flex;
      align-items: center;
      gap: 1rem;
    }

    .scroll-hint::before {
      content: '';
      width: 40px;
      height: 1px;
      background: var(--warm-gray);
    }

    /* -- Divider -- */
    .divider {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 3rem;
    }

    .divider hr {
      border: none;
      height: 1px;
      background: var(--sand-dark);
    }

    /* -- Pain Point Sections -- */
    .pain {
      max-width: 1200px;
      margin: 0 auto;
      padding: 7rem 3rem;
    }

    .pain-layout {
      display: grid;
      grid-template-columns: 280px 1fr;
      gap: 5rem;
      align-items: start;
    }

    .pain-marker {
      position: sticky;
      top: 8rem;
    }

    .pain-number {
      font-family: 'Instrument Serif', Georgia, serif;
      font-size: 8rem;
      line-height: 0.85;
      color: var(--sand-dark);
    }

    .pain-label {
      font-size: 0.7rem;
      font-weight: 600;
      letter-spacing: 4px;
      text-transform: uppercase;
      color: var(--terra);
      margin-top: 1rem;
    }

    .pain-content h2 {
      font-size: clamp(2rem, 4vw, 3rem);
      line-height: 1.15;
      color: var(--warm-black);
      margin-bottom: 2rem;
    }

    .pain-content h2 em { color: var(--terra); font-style: italic; }

    .pain-body {
      font-size: 1.08rem;
      color: var(--text-light);
      max-width: 580px;
      line-height: 1.85;
    }

    .pain-body p + p { margin-top: 1.5rem; }

    .pain-body strong {
      color: var(--text);
      font-weight: 500;
    }

    .pain-quote {
      margin: 2.5rem 0;
      padding: 2rem 2.5rem;
      background: var(--sand);
      border-radius: 2px;
      font-family: 'Instrument Serif', Georgia, serif;
      font-size: 1.3rem;
      line-height: 1.55;
      color: var(--charcoal);
      max-width: 580px;
      position: relative;
    }

    .pain-quote::before {
      content: '';
      position: absolute;
      left: 0;
      top: 0;
      bottom: 0;
      width: 3px;
      background: var(--terra);
      border-radius: 3px;
    }

    .pain-what-changes {
      margin-top: 2.5rem;
      max-width: 580px;
    }

    .pain-what-changes h3 {
      font-family: 'Inter', sans-serif;
      font-size: 0.7rem;
      font-weight: 600;
      letter-spacing: 3px;
      text-transform: uppercase;
      color: var(--terra);
      margin-bottom: 1.25rem;
    }

    .pain-what-changes ul {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 0.75rem;
    }

    .pain-what-changes li {
      font-size: 0.95rem;
      color: var(--text);
      padding-left: 1.75rem;
      position: relative;
      line-height: 1.6;
    }

    .pain-what-changes li::before {
      content: '';
      position: absolute;
      left: 0;
      top: 0.55rem;
      width: 8px;
      height: 8px;
      border-radius: 50%;
      border: 1.5px solid var(--terra);
    }

    /* -- Alternating BG -- */
    .pain.shaded { background: var(--sand); margin: 0 auto; max-width: 100%; padding-left: calc((100% - 1200px) / 2 + 3rem); padding-right: calc((100% - 1200px) / 2 + 3rem); }

    /* -- Bridge -- */
    .bridge {
      padding: 7rem 3rem;
      text-align: center;
      background: var(--warm-black);
      color: var(--white);
    }

    .bridge-inner {
      max-width: 700px;
      margin: 0 auto;
    }

    .bridge h2 {
      font-size: clamp(2rem, 4vw, 3.2rem);
      line-height: 1.2;
      color: var(--white);
      margin-bottom: 1.5rem;
    }

    .bridge p {
      font-size: 1.15rem;
      color: var(--warm-gray);
      line-height: 1.8;
    }

    .bridge p + p { margin-top: 1.25rem; }

    .bridge .accent { color: var(--terra-soft); }

    /* -- How -- */
    .how {
      max-width: 1200px;
      margin: 0 auto;
      padding: 7rem 3rem;
    }

    .how-header {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 4rem;
      margin-bottom: 4rem;
      align-items: end;
    }

    .how-header h2 {
      font-size: clamp(2rem, 3.5vw, 2.8rem);
      line-height: 1.2;
    }

    .how-header p {
      font-size: 1.05rem;
      color: var(--text-light);
    }

    .how-steps {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 0;
    }

    .how-step {
      padding: 2.5rem 2rem;
      border-top: 2px solid var(--sand-dark);
      position: relative;
      transition: border-color 0.3s;
    }

    .how-step:hover { border-color: var(--terra); }

    .how-step-num {
      font-family: 'Instrument Serif', Georgia, serif;
      font-size: 2.5rem;
      color: var(--sand-dark);
      margin-bottom: 1rem;
      transition: color 0.3s;
    }

    .how-step:hover .how-step-num { color: var(--terra); }

    .how-step h3 {
      font-family: 'Inter', sans-serif;
      font-size: 0.95rem;
      font-weight: 500;
      margin-bottom: 0.75rem;
      color: var(--warm-black);
    }

    .how-step p {
      font-size: 0.88rem;
      color: var(--text-light);
      line-height: 1.7;
    }

    /* -- CTA -- */
    .cta {
      padding: 8rem 3rem;
      background: var(--sand);
    }

    .cta-inner {
      max-width: 1200px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: 1.2fr 1fr;
      gap: 5rem;
      align-items: center;
    }

    .cta h2 {
      font-size: clamp(2.2rem, 4vw, 3.2rem);
      line-height: 1.15;
      color: var(--warm-black);
      margin-bottom: 1.5rem;
    }

    .cta h2 em { color: var(--terra); font-style: italic; }

    .cta p {
      font-size: 1.08rem;
      color: var(--text-light);
      line-height: 1.8;
      margin-bottom: 1rem;
    }

    .cta-buttons { margin-top: 2rem; display: flex; gap: 1rem; flex-wrap: wrap; }

    .btn-warm {
      display: inline-block;
      font-family: 'Inter', sans-serif;
      font-size: 0.82rem;
      font-weight: 500;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      text-decoration: none;
      padding: 1.1rem 2.5rem;
      border-radius: 100px;
      transition: all 0.3s;
    }

    .btn-warm.filled {
      background: var(--terra);
      color: var(--white);
      border: 1.5px solid var(--terra);
    }

    .btn-warm.filled:hover {
      background: var(--charcoal);
      border-color: var(--charcoal);
    }

    .btn-warm.ghost {
      border: 1.5px solid var(--charcoal);
      color: var(--charcoal);
    }

    .btn-warm.ghost:hover {
      border-color: var(--terra);
      color: var(--terra);
    }

    .cta-right {
      background: var(--white);
      padding: 3rem;
      border-radius: 3px;
    }

    .cta-right h3 {
      font-size: 1.3rem;
      margin-bottom: 0.75rem;
    }

    .cta-right p {
      font-size: 0.92rem;
      margin-bottom: 0;
    }

    .cta-promises {
      list-style: none;
      margin-top: 1.5rem;
      display: flex;
      flex-direction: column;
      gap: 0.75rem;
    }

    .cta-promises li {
      font-size: 0.88rem;
      color: var(--text);
      padding-left: 1.75rem;
      position: relative;
    }

    .cta-promises li::before {
      content: '\2713';
      position: absolute;
      left: 0;
      color: var(--terra);
      font-weight: 600;
    }

    /* -- Footer -- */
    footer {
      padding: 3rem;
      text-align: center;
      background: var(--cream);
      border-top: 1px solid var(--sand-dark);
    }

    .footer-logo {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-bottom: 1.5rem;
      line-height: 1.2;
    }

    .footer-logo .logo-primary {
      font-size: 1.2rem;
    }

    .footer-logo .logo-accent {
      font-size: 1.2rem;
    }

    .footer-divider {
      width: 80px;
      height: 1px;
      background: var(--terra);
      margin: 0.5rem auto 0.75rem;
    }

    .footer-tagline {
      font-size: 0.6rem;
      font-weight: 500;
      letter-spacing: 4px;
      text-transform: uppercase;
      color: var(--warm-gray);
    }

    footer p {
      font-size: 0.75rem;
      color: var(--warm-gray);
      letter-spacing: 1px;
      margin-top: 1rem;
    }

    footer a { color: var(--terra); text-decoration: none; }

    /* -- Responsive -- */
    @media (max-width: 1000px) {
      .pain-layout { grid-template-columns: 1fr; gap: 2rem; }
      .pain-marker { position: static; display: flex; align-items: center; gap: 1.5rem; }
      .pain-number { font-size: 4rem; }
      .how-steps { grid-template-columns: 1fr 1fr; }
      .how-header { grid-template-columns: 1fr; gap: 1rem; }
      .cta-inner { grid-template-columns: 1fr; }
      .hero-body { grid-template-columns: 1fr; gap: 1.5rem; }
    }

    @media (max-width: 640px) {
      nav { padding: 1rem 1.5rem; }
      .hero, .pain, .how { padding-left: 1.5rem; padding-right: 1.5rem; }
      .pain.shaded { padding-left: 1.5rem; padding-right: 1.5rem; }
      .hero h1 { font-size: 2.5rem; }
      .how-steps { grid-template-columns: 1fr; }
      .cta { padding: 5rem 1.5rem; }
      .cta-buttons { flex-direction: column; }
      .btn-warm { text-align: center; }
      .logo-primary, .logo-accent { font-size: 1.1rem; }
    }
  </style>
</head>
<body>

  <!-- Nav -->
  <nav id="nav">
    <a href="#" class="logo">
      <span class="logo-primary">Executive</span>
      <span class="logo-accent">District</span>
    </a>
    <a href="#contact" class="nav-cta">Let's Talk</a>
  </nav>

  <!-- Hero -->
  <section class="hero">
    <h1>Building a company is hard. Building it <span>alone</span> is harder.</h1>
    <div class="hero-body">
      <p class="lead serif">We're fractional C-suite operators who step into the trenches with founders and owners who are carrying too much, seeing too little profit, and wondering what comes next.</p>
      <p>You built something real. But somewhere between the early momentum and now, things got heavier. The margins aren't where they should be. The decisions all land on you. And the future &mdash; whether that's growth, an exit, or just breathing room &mdash; feels unclear. That's exactly where we come in.</p>
    </div>
    <div class="hero-image">
      <img src="Gemini_Generated_Image_mq9fxqmq9fxqmq9f.png" alt="Executive District ~ Fractional C-Suite Leadership">    </div>
    <div class="scroll-hint">Three things we hear every week</div>
  </section>

  <div class="divider"><hr></div>

  <!-- Pain 1: Profit -->
  <section class="pain" id="profit">
    <div class="pain-layout">
      <div class="pain-marker">
        <div class="pain-number">01</div>
        <div class="pain-label">The Profit Problem</div>
      </div>
      <div class="pain-content">
        <h2>"Revenue is up. So why isn't there any <em>money?</em>"</h2>
        <div class="pain-body">
          <p>You're doing more business than ever. The top line looks healthy. But cash is tight, margins are thin, and every month feels like a math problem that doesn't quite solve. You've cut costs, pushed harder, and still &mdash; the money doesn't stick.</p>
          <p><strong>This is the most common pattern we see.</strong> Growth without profitability isn't a revenue problem. It's a structural one. Pricing that hasn't been revisited in three years. Overhead that scaled faster than income. Profitable work subsidizing unprofitable work without anyone noticing. The answers are in the business &mdash; they just need someone who knows where to look.</p>
        </div>
        <div class="pain-quote">
          We don't cut your way to health. We re-engineer how money moves through your business so that growth and profit are the same story.
        </div>
        <div class="pain-what-changes">
          <h3>What changes when we engage</h3>
          <ul>
            <li>True profitability by service line, client, and team &mdash; not just one blended number</li>
            <li>Pricing rebuilt around your actual cost structure and the value you deliver</li>
            <li>Cash flow forecasting that lets you make decisions with confidence, not anxiety</li>
            <li>The financial clarity to know exactly where your next dollar of profit comes from</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Pain 2: Loneliness -->
  <section class="pain shaded" id="loneliness">
    <div class="pain-layout">
      <div class="pain-marker">
        <div class="pain-number">02</div>
        <div class="pain-label">The Loneliness Problem</div>
      </div>
      <div class="pain-content">
        <h2>"I have a team. But I don't have <em>a partner.</em>"</h2>
        <div class="pain-body">
          <p>There's a particular kind of isolation that comes with running a company. You have employees who depend on you, clients who demand from you, and a board or investors who expect from you. But when it comes to the hardest decisions &mdash; the ones that keep you up at 2am &mdash; there's nobody across the table who truly gets it.</p>
          <p>Your spouse is supportive but can't advise on whether to fire your VP of Sales. Your accountant gives you numbers but not judgment. Your peers are dealing with their own weight. <strong>What you're missing isn't more people. It's someone who has been where you are and can think with you at your level.</strong></p>
        </div>
        <div class="pain-quote">
          We don't report to you from a distance. We sit beside you and carry the weight of the hard calls. That's the difference between a consultant and an operator.
        </div>
        <div class="pain-what-changes">
          <h3>What changes when we engage</h3>
          <ul>
            <li>A seasoned executive partner who shares the cognitive load of running the business</li>
            <li>Honest, experienced counsel on the decisions you can't talk about with anyone else</li>
            <li>Someone who will challenge your thinking when you need it &mdash; not just validate it</li>
            <li>The space to be a founder again instead of a one-person executive team</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Pain 3: Confusion -->
  <section class="pain" id="clarity">
    <div class="pain-layout">
      <div class="pain-marker">
        <div class="pain-number">03</div>
        <div class="pain-label">The Clarity Problem</div>
      </div>
      <div class="pain-content">
        <h2>"I don't know if I should scale, sell, or <em>just survive.</em>"</h2>
        <div class="pain-body">
          <p>You've been in the business long enough to know something needs to change. But what? Double down on growth? Start preparing for an exit? Restructure? Bring in investors? Every option has a case, and every advisor has an opinion shaped by what they're selling.</p>
          <p><strong>The confusion isn't a sign of weakness. It's a sign that you've outgrown the frame you've been using to evaluate the business.</strong> You need someone who can step back, see the whole picture, and help you build a plan that matches your actual goals &mdash; not someone else's playbook.</p>
        </div>
        <div class="pain-quote">
          We help you answer the only question that matters: What do you actually want? Then we build the plan and the team to go get it.
        </div>
        <div class="pain-what-changes">
          <h3>What changes when we engage</h3>
          <ul>
            <li>A clear, honest assessment of what the business is worth today and what it could be worth</li>
            <li>A defined path forward &mdash; whether that's growth, exit, restructuring, or a combination</li>
            <li>The operational roadmap to get from here to there, with milestones that matter</li>
            <li>Decisions made from clarity and conviction instead of fatigue and guesswork</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Bridge -->
  <section class="bridge">
    <div class="bridge-inner">
      <h2>These three problems are connected. So is the solution.</h2>
      <p>When profit is unclear, every decision feels risky. When every decision is yours alone, the weight becomes paralyzing. When you're paralyzed, the future stays foggy. <span class="accent">It's one cycle, and it breaks in one place: the executive layer.</span></p>
      <p>We bring the operators who break that cycle. A fractional CFO who makes the money make sense. A fractional COO who takes operations off your shoulders. A fractional CEO or CRO who helps you see around corners. Not all at once &mdash; just what you need, when you need it.</p>
    </div>
  </section>

  <!-- How We Work -->
  <section class="how">
    <div class="how-header">
      <h2>The engagement is simple. The impact isn't.</h2>
      <p>We don't do twelve-week discovery phases or hundred-page reports. We get inside the business, understand what's real, and start working. Here's how it goes.</p>
    </div>
    <div class="how-steps">
      <div class="how-step">
        <div class="how-step-num">01</div>
        <h3>Confidential Conversation</h3>
        <p>A candid call where we listen. What's working, what's not, what you want. No pitch, no pressure. Just two operators talking.</p>
      </div>
      <div class="how-step">
        <div class="how-step-num">02</div>
        <h3>Diagnostic Deep Dive</h3>
        <p>We spend time inside the business &mdash; financials, operations, team, customers &mdash; and come back with what we actually see. No sugarcoating.</p>
      </div>
      <div class="how-step">
        <div class="how-step-num">03</div>
        <h3>Embedded Execution</h3>
        <p>We step into the seat. Attend the meetings, make the calls, manage the numbers, and drive the outcomes &mdash; alongside you, not above you.</p>
      </div>
      <div class="how-step">
        <div class="how-step-num">04</div>
        <h3>Outcome Delivered</h3>
        <p>Whether the goal is profit, an exit, or a business that runs without you in every chair &mdash; we stay until the outcome is real, then we step back.</p>
      </div>
    </div>
  </section>

  <!-- CTA -->
  <section class="cta" id="contact">
    <div class="cta-inner">
      <div>
        <h2>You've carried this long enough. <em>Let's carry it together.</em></h2>
        <p>This starts with a conversation &mdash; private, unhurried, and completely confidential. Tell us where you are. We'll tell you honestly what we see and whether we can help.</p>
        <p>No contracts, no obligations, no twelve-page proposals. Just a real conversation between people who understand what it takes to build and run a company.</p>
        <div class="cta-buttons">
          <a href="mailto:hello@executivedistrict.com" class="btn-warm filled">Start the Conversation</a>
          <a href="tel:+1 (616) 828-8711" class="btn-warm ghost">Call Directly</a>
        </div>
      </div>
      <div class="cta-right">
        <h3 class="serif">What to expect</h3>
        <p>Your first call with us will be different from any consulting pitch you've sat through.</p>
        <ul class="cta-promises">
          <li>30&ndash;45 minutes, founder to executive</li>
          <li>We listen first, talk second</li>
          <li>Completely confidential &mdash; always</li>
          <li>Honest assessment, even if the answer is "you don't need us"</li>
          <li>Zero follow-up pressure</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="footer-logo">
      <span class="logo-primary">Executive</span>
      <span class="logo-accent">District</span>
      <div class="footer-divider"></div>
      <span class="footer-tagline">Fractional C-Suite Leadership</span>
    </div>
    <p>&copy; 2026 Executive District &nbsp;&middot;&nbsp; <a href="mailto:hello@executivedistrict.com">hello@executivedistrict.com</a></p>
  </footer>

  <script>
    // Nav background on scroll
    const nav = document.getElementById('nav');
    window.addEventListener('scroll', () => {
      nav.classList.toggle('scrolled', window.scrollY > 60);
    });
  </script>

</body>
