<!DOCTYPE html>
<html lang="am">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>መሠረተ አንድነት | በጎ አድራጎት ማህበር</title>

  <meta name="description"
        content="መሠረተ አንድነት በጎ አድራጎት ማህበር። በአንድነት ለማህበረሰባችን የተሻለ ነገ እንገንባ።">

  <style>
    :root {
      --green: #087443;
      --dark-green: #064d30;
      --light-green: #eaf6ee;
      --gold: #e9b949;
      --text: #24342a;
      --muted: #68766d;
      --white: #ffffff;
      --border: #d8e4db;
    }

    * {
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: Arial, "Noto Sans Ethiopic", sans-serif;
      color: var(--text);
      background: #f7faf8;
      line-height: 1.8;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .container {
      width: min(1120px, 92%);
      margin: auto;
    }

    header {
      background: var(--white);
      border-bottom: 1px solid var(--border);
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .navbar {
      min-height: 76px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
      flex-wrap: wrap;
      padding: 12px 0;
    }

    .brand {
      color: var(--green);
      font-size: 19px;
      font-weight: bold;
    }

    nav {
      display: flex;
      flex-wrap: wrap;
      gap: 18px;
      align-items: center;
    }

    nav a {
      font-size: 14px;
      font-weight: bold;
    }

    nav a:hover {
      color: var(--green);
    }

    .button {
      display: inline-block;
      background: var(--green);
      color: var(--white);
      border: none;
      border-radius: 9px;
      padding: 12px 20px;
      font-size: 15px;
      font-weight: bold;
      cursor: pointer;
      text-align: center;
    }

    .button:hover {
      background: var(--dark-green);
    }

    .hero {
      background: linear-gradient(135deg, #e9f7ee, #ffffff);
      padding: 75px 0;
    }

    .hero-content {
      max-width: 800px;
      margin: auto;
      text-align: center;
    }

    .badge {
      display: inline-block;
      background: #d5efdf;
      color: var(--dark-green);
      border-radius: 30px;
      padding: 5px 15px;
      font-size: 14px;
      font-weight: bold;
    }

    h1 {
      font-size: clamp(30px, 5vw, 49px);
      line-height: 1.5;
      color: var(--dark-green);
      margin: 20px 0;
    }

    h2 {
      color: var(--dark-green);
      font-size: 28px;
      line-height: 1.5;
    }

    h3 {
      color: var(--green);
    }

    .hero p {
      font-size: 18px;
      max-width: 720px;
      margin: 0 auto 25px;
    }

    section {
      padding: 65px 0;
      scroll-margin-top: 90px;
    }

    .section-heading {
      text-align: center;
      max-width: 760px;
      margin: 0 auto 35px;
    }

    .section-heading p {
      color: var(--muted);
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 22px;
    }

    .card {
      background: var(--white);
      border: 1px solid var(--border);
      border-radius: 15px;
      padding: 25px;
      box-shadow: 0 5px 20px rgba(0, 0, 0, 0.035);
    }

    .card p {
      color: var(--muted);
    }

    .icon {
      font-size: 30px;
    }

    .about {
      background: var(--light-green);
    }

    .founder-box {
      max-width: 700px;
      margin: auto;
      background: white;
      padding: 30px;
      border-radius: 15px;
      text-align: center;
      border: 1px solid var(--border);
    }

    .founder-name {
      font-size: 23px;
      color: var(--green);
      font-weight: bold;
    }

    .form-section {
      background: #f1f7f3;
    }

    .form-card {
      max-width: 760px;
      margin: auto;
      background: white;
      padding: clamp(20px, 5vw, 40px);
      border: 1px solid var(--border);
      border-radius: 16px;
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.05);
    }

    .form-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 18px;
    }

    .field {
      margin-bottom: 17px;
    }

    .full-width {
      grid-column: 1 / -1;
    }

    label {
      display: block;
      font-weight: bold;
      margin-bottom: 7px;
    }

    input,
    select,
    textarea {
      width: 100%;
      padding: 13px;
      border: 1px solid #cbd9cf;
      border-radius: 8px;
      background: white;
      color: var(--text);
      font-size: 16px;
      font-family: inherit;
    }

    input:focus,
    select:focus,
    textarea:focus {
      outline: 2px solid #9bd5b0;
      border-color: var(--green);
    }

    textarea {
      resize: vertical;
    }

    .required-note,
    .small-note {
      font-size: 13px;
      color: var(--muted);
    }

    .notice {
      background: #fff8df;
      border: 1px solid #f0d88c;
      padding: 14px;
      border-radius: 9px;
      margin: 20px 0;
      font-size: 14px;
    }

    .success-message {
      display: none;
      background: #e2f6e9;
      border: 1px solid #8bc9a0;
      color: #075b30;
      padding: 15px;
      margin-top: 20px;
      border-radius: 8px;
    }

    .rules {
      max-width: 850px;
      margin: auto;
    }

    .rules li {
      margin-bottom: 12px;
    }

    .contact {
      background: var(--light-green);
      text-align: center;
    }

    footer {
      background: #073d27;
      color: white;
      text-align: center;
      padding: 30px 15px;
    }

    footer p {
      margin: 5px 0;
    }

    @media (max-width: 760px) {
      .navbar {
        justify-content: center;
      }

      nav {
        justify-content: center;
        gap: 12px;
      }

      .cards {
        grid-template-columns: 1fr;
      }

      .form-grid {
        grid-template-columns: 1fr;
      }

      .full-width {
        grid-column: auto;
      }

      .hero {
        padding: 50px 0;
      }
    }
  </style>
</head>

<body>

<header>
  <div class="container navbar">
    <a href="#home" class="brand">መሠረተ አንድነት</a>

    <nav aria-label="ዋና ምናሌ">
      <a href="#home">መነሻ</a>
      <a href="#about">ስለ እኛ</a>
      <a href="#activities">ተግባራት</a>
      <a href="#register">ምዝገባ</a>
      <a href="#rules">ደንቦች</a>
      <a href="#contact">እውቂያ</a>
    </nav>
  </div>
</header>

<main>

  <section class="hero" id="home">
    <div class="container hero-content">
      <span class="badge">አንድነት • ርህራሄ • ተስፋ</span>

      <h1>በአንድነት ለተሻለ ነገ እንስራ!</h1>

      <p>
        መሠረተ አንድነት በጎ አድራጎት ማህበር
        በመተባበር፣ በመረዳዳትና በማህበራዊ ኃላፊነት
        ለማህበረሰባችን የተሻለ ሕይወት ለመገንባት የሚያስብ ማህበር ነው።
      </p>

      <a href="#register" class="button">አባል ይሁኑ</a>
      <a href="#about" class="button"
         style="background:white;color:#087443;border:1px solid #087443;margin-left:8px;">
        ስለ ማህበሩ ይወቁ
      </a>
    </div>
  </section>

  <section id="about">
    <div class="container">
      <div class="section-heading">
        <h2>ስለ ማህበራችን</h2>
        <p>
          በጋራ መስራት የለውጥ መሠረት ነው።
          እያንዳንዱ ሰው ለማህበረሰቡ አዎንታዊ ለውጥ ማምጣት ይችላል።
        </p>
      </div>

      <div class="cards">
        <article class="card">
          <div class="icon">🤝</div>
          <h3>ዓላማችን</h3>
          <p>
            የአንድነትና የመረዳዳት መንፈስን ማጠናከር
            እና ለማህበረሰቡ ጠቃሚ ተግባራትን ማከናወን።
          </p>
        </article>

        <article class="card">
          <div class="icon">🌱</div>
          <h3>ራዕያችን</h3>
          <p>
            በትብብር፣ በሰብአዊነትና በኃላፊነት
            የተሻለ ማህበረሰብ ለመገንባት መትጋት።
          </p>
        </article>

        <article class="card">
          <div class="icon">💚</div>
          <h3>እሴቶቻችን</h3>
          <p>
            አንድነት፣ ታማኝነት፣ ግልጽነት፣
            እኩልነትና ለሰው ልጅ ክብር መስጠት።
          </p>
        </article>
      </div>
    </div>
  </section>

  <section class="about" id="activities">
    <div class="container">
      <div class="section-heading">
        <h2>የማህበሩ ተግባራት</h2>
        <p>
          እነዚህ የታቀዱ የተግባር ዘርፎች ምሳሌዎች ናቸው።
          በተግባር የሚከናወኑት በማህበሩ ውሳኔና አቅም መሠረት ይሆናሉ።
        </p>
      </div>

      <div class="cards">
        <article class="card">
          <h3>ማህበራዊ ድጋፍ</h3>
          <p>እርዳታ ለሚያስፈልጋቸው ሰዎች ድጋፍ ለማድረግ መተባበር።</p>
        </article>

        <article class="card">
          <h3>የማህበረሰብ ትብብር</h3>
          <p>የአካባቢ ልማትንና የጋራ ተሳትፎን የሚያበረታቱ ተግባራት።</p>
        </article>

        <article class="card">
          <h3>የግንዛቤ ማሳደግ</h3>
          <p>ስለ መረዳዳት፣ ኃላፊነትና የጋራ ጥቅም ግንዛቤ ማሳደግ።</p>
        </article>
      </div>
    </div>
  </section>

  <section>
    <div class="container">
      <div class="founder-box">
        <h2>የማህበሩ መስራችና ሰብሳቢ</h2>
        <p class="founder-name">ደሳለኝ ጌታቸው</p>
        <p>
          የማህበሩ አመራርና አስተዳደር
          በማህበሩ የጸደቁ ደንቦችና ተፈጻሚ ሕጎች መሠረት ይከናወናል።
        </p>
      </div>
    </div>
  </section>

  <section class="form-section" id="register">
    <div class="container">
      <div class="section-heading">
        <h2>የአባልነት ምዝገባ</h2>
        <p>
          የሚፈለጉትን መረጃዎች በትክክል ያስገቡ።
          በእውነተኛው የድረ-ገጽ ስርዓት ምዝገባዎ ከመጠናቀቁ በፊት
          ኢሜይልዎ መረጋገጥ አለበት።
        </p>
      </div>

      <div class="form-card">
        <form id="registrationForm"
              action="/api/send-otp"
              method="post">

          <div class="form-grid">

            <div class="field full-width">
              <label for="fullname">ሙሉ ስም *</label>
              <input id="fullname" name="fullname" type="text"
                     autocomplete="name" required
                     minlength="3" maxlength="100"
                     placeholder="ሙሉ ስምዎን ያስገቡ">
            </div>

            <div class="field">
              <label for="email">ኢሜይል አድራሻ *</label>
              <input id="email" name="email" type="email"
                     autocomplete="email" required
                     maxlength="254"
                     placeholder="example@email.com">
            </div>

            <div class="field">
              <label for="phone">ስልክ ቁጥር *</label>
              <input id="phone" name="phone" type="tel"
                     autocomplete="tel" required
                     maxlength="20"
                     placeholder="09XXXXXXXX">
            </div>

            <div class="field full-width">
              <label for="membership">የአባልነት ዓይነት *</label>
              <select id="membership" name="membership" required>
                <option value="">ይምረጡ</option>
                <option value="መደበኛ">መደበኛ አባል</option>
                <option value="መስራች">መስራች አባል</option>
                <option value="ቋሚ">ቋሚ አባል</option>
                <option value="ተባባሪ">ተባባሪ አባል</option>
                <option value="ሌላ">ሌላ</option>
              </select>
            </div>

            <div class="field full-width">
              <label for="address">አድራሻ (አማራጭ)</label>
              <input id="address" name="address" type="text"
                     autocomplete="street-address"
                     maxlength="200"
                     placeholder="ከተማ / አካባቢ">
            </div>

            <div class="field full-width">
              <label for="reason">ለምን የማህበሩ አባል መሆን ይፈልጋሉ? (አማራጭ)</label>
              <textarea id="reason" name="reason" rows="4"
                        maxlength="1000"
                        placeholder="አጭር መልዕክትዎን ያስገቡ"></textarea>
            </div>

          </div>

          <div class="notice">
            የግል መረጃዎ ለምዝገባ ዓላማ ብቻ መጠቀም አለበት።
            ከመላክዎ በፊት ያስገቡትን መረጃ ያረጋግጡ።
          </div>

          <button class="button" type="submit" id="submitButton">
            የማረጋገጫ ኮድ ይላክልኝ
          </button>

          <p class="small-note">
            የማረጋገጫ ኮድ መላክ እንዲሰራ የድረ-ገጹ የጀርባ ስርዓት
            እና የኢሜይል አገልግሎት መዋቀር አለባቸው።
          </p>

          <div id="statusMessage"
               class="success-message"
               role="status"
               aria-live="polite"></div>
        </form>

        <div id="verificationSection" hidden>
          <hr>

          <h3>ኢሜይልዎን ያረጋግጡ</h3>

          <p>
            በኢሜይልዎ የተላከልዎትን ባለ 6 አሃዝ የማረጋገጫ ኮድ ያስገቡ።
          </p>

          <form id="verificationForm"
                action="/api/register"
                method="post">

            <input type="hidden" id="verifyEmail" name="email">

            <div class="field">
              <label for="otp">ባለ 6 አሃዝ ኮድ *</label>
              <input id="otp" name="otp"
                     type="text"
                     inputmode="numeric"
                     pattern="[0-9]{6}"
                     minlength="6"
                     maxlength="6"
                     autocomplete="one-time-code"
                     required
                     placeholder="123456">
            </div>

            <button class="button" type="submit">
              ኢሜይልን አረጋግጥና ምዝገባውን ጨርስ
            </button>

            <div id="verificationMessage"
                 class="success-message"
                 role="status"
                 aria-live="polite"></div>
          </form>
        </div>

      </div>
    </div>
  </section>

  <section id="rules">
    <div class="container rules">
      <div class="section-heading">
        <h2>የማህበሩ መተዳደሪያ ደንብ</h2>
        <p>የደንብ ረቂቅ — ለውይይትና ለግምገማ የቀረበ</p>
      </div>

      <div class="notice">
        <strong>ማስጠንቀቂያ፦</strong>
        ከታች ያለው ጽሑፍ አጠቃላይ ረቂቅ ነው፤
        የጸደቀ ሕጋዊ ሰነድ አይደለም።
        ከመጨረሻ አጠቃቀሙ በፊት በማህበሩ አባላት መገምገም፣
        በሕግ ባለሙያ መታየትና ተገቢውን ሕጋዊ ፈቃድ ማሟላት አለበት።
      </div>

      <h3>አንቀጽ 1፡ የማህበሩ ስም</h3>
      <p>የማህበሩ ስም “መሠረተ አንድነት በጎ አድራጎት ማህበር” ነው።</p>

      <h3>አንቀጽ 2፡ ዓላማ</h3>
      <p>
        በሕግ የተፈቀዱ ሰብአዊ፣ ማህበራዊና የበጎ አድራጎት
        ተግባራትን ለማከናወንና የማህበረሰብ ትብብርን ለማጠናከር።
      </p>

      <h3>አንቀጽ 3፡ የአባልነት ዓይነቶች</h3>
      <ul>
        <li>መደበኛ አባል</li>
        <li>መስራች አባል</li>
        <li>ቋሚ አባል</li>
        <li>ተባባሪ አባል</li>
        <li>ሌላ በማህበሩ የሚጸድቅ የአባልነት ዓይነት</li>
      </ul>

      <h3>አንቀጽ 4፡ የአባላት መብቶችና ግዴታዎች</h3>
      <p>
        አባላት በማህበሩ ሕጋዊ ደንብ መሠረት በስብሰባዎችና
        በተግባራት የመሳተፍ፣ መረጃ የማግኘትና የሚጠበቅባቸውን
        ኃላፊነቶች የመወጣት መብትና ግዴታ ይኖራቸዋል።
      </p>

      <h3>አንቀጽ 5፡ አመራርና ስብሰባ</h3>
      <p>
        የማህበሩ የአመራር መዋቅር፣ የምርጫ ሂደት፣
        የስብሰባ ጊዜና የውሳኔ አሰጣጥ ሥርዓት በሚጸድቀው
        የመጨረሻ ደንብና ተፈጻሚ ሕግ መሠረት ይወሰናል።
      </p>

      <h3>አንቀጽ 6፡ የገንዘብ አስተዳደር</h3>
      <p>
        የማህበሩ ገቢና ወጪ በግልጽነት መመዝገብ፣
        የገንዘብ ሰነዶች መጠበቅና ተገቢ የሂሳብ ቁጥጥር
        መደረግ አለበት።
      </p>

      <h3>አንቀጽ 7፡ የደንብ ማሻሻያ</h3>
      <p>
        የደንብ ማሻሻያ በማህበሩ የተወሰነ ሕጋዊ ሂደት
        እና ተገቢው የማጽደቅ ሂደት መሠረት ይከናወናል።
      </p>
    </div>
  </section>

  <section class="contact" id="contact">
    <div class="container">
      <h2>ከእኛ ጋር ይገናኙ</h2>

      <p>
        ለአባልነት ምዝገባና ለማህበሩ ጉዳዮች የኢሜይል አድራሻችን፦
      </p>

      <p>
        <a href="mailto:mesereteandinetdilla@gmail.com">
          mesereteandinetdilla@gmail.com
        </a>
      </p>

      <p>
        ማስታወሻ፦ ይህ የእውቂያ አድራሻ ብቻ ነው።
        የምዝገባ መረጃ በራስ-ሰር እንዲላክ የጀርባ ስርዓት ያስፈልጋል።
      </p>
    </div>
  </section>

</main>

<footer>
  <p><strong>መሠረተ አንድነት በጎ አድራጎት ማህበር</strong></p>
  <p>መስራችና ሰብሳቢ፡ ደሳለኝ ጌታቸው</p>
  <p>© <span id="year"></span> መብቱ በሕግ የተጠበቀ ነው።</p>
</footer>

<script>
  document.getElementById("year").textContent =
    new Date().getFullYear();

  const registrationForm =
    document.getElementById("registrationForm");

  const verificationSection =
    document.getElementById("verificationSection");

  const statusMessage =
    document.getElementById("statusMessage");

  const verificationForm =
    document.getElementById("verificationForm");

  const verificationMessage =
    document.getElementById("verificationMessage");

  registrationForm.addEventListener("submit", async function(event) {
    event.preventDefault();

    statusMessage.style.display = "block";
    statusMessage.textContent = "የማረጋገጫ ኮድ ለመላክ በመሞከር ላይ...";

    const button = document.getElementById("submitButton");
    button.disabled = true;

    try {
      const response = await fetch("/api/send-otp", {
        method: "POST",
        body: new FormData(registrationForm)
      });

      const result = await response.json();

      if (!response.ok) {
        throw new Error(
          result.message || result.error ||
          "የማረጋገጫ ኮድ መላክ አልተሳካም።"
        );
      }

      document.getElementById("verifyEmail").value =
        document.getElementById("email").value.trim();

      verificationSection.hidden = false;

      statusMessage.textContent =
        "ኮዱ ከተላከ ኢሜይልዎን ይመልከቱ።";

      verificationSection.scrollIntoView({
        behavior: "smooth",
        block: "start"
      });

    } catch (error) {
      statusMessage.textContent =
        error.message ||
        "ስህተት ተፈጥሯል። እባክዎ እንደገና ይሞክሩ።";
    } finally {
      button.disabled = false;
    }
  });

  verificationForm.addEventListener("submit", async function(event) {
    event.preventDefault();

    verificationMessage.style.display = "block";
    verificationMessage.textContent =
      "ኮዱን በማረጋገጥ ላይ...";

    const button = verificationForm.querySelector("button");
    button.disabled = true;

    try {
      const response = await fetch("/api/register", {
        method: "POST",
        body: new FormData(verificationForm)
      });

      const result = await response.json();

      if (!response.ok) {
        throw new Error(
          result.message || result.error ||
          "ማረጋገጫው አልተሳካም።"
        );
      }

      verificationMessage.textContent =
        "የአባልነት ምዝገባዎ በተሳካ ሁኔታ ተጠናቋል።";

      registrationForm.reset();
      verificationForm.reset();

    } catch (error) {
      verificationMessage.textContent =
        error.message ||
        "ስህተት ተፈጥሯል። እባክዎ እንደገና ይሞክሩ።";
    } finally {
      button.disabled = false;
    }
  });
</script>

</body>
</html>
