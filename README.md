# Espoir-plus-<!DOCTYPE html><html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Espoir+</title>
  <style>
    body { font-family: 'Arial', sans-serif; margin: 0; padding: 0; background: #f9f9f9; }
    header { background: #1e90ff; color: white; padding: 2em; text-align: center; }
    header img { max-width: 150px; margin-bottom: 1em; }
    nav { display: flex; justify-content: center; gap: 1.5em; background: #eee; padding: 1em; border-top: 3px solid #1e90ff; }
    nav a { color: #333; text-decoration: none; font-weight: bold; transition: color 0.3s; }
    nav a:hover { color: #1e90ff; }
    main { padding: 2em; }
    section { margin-bottom: 3em; }
    .lang-switch { position: absolute; top: 1em; right: 1em; }
    button { background: #1e90ff; color: white; border: none; padding: 0.7em 1.5em; border-radius: 8px; cursor: pointer; transition: background 0.3s; }
    button:hover { background: #0056b3; }
    input, textarea { width: 100%; padding: 0.7em; margin-top: 0.5em; border-radius: 8px; border: 1px solid #ccc; }
    footer { background: #1e90ff; color: white; text-align: center; padding: 1.5em 0; }
    .icon { width: 30px; height: 30px; margin-right: 10px; vertical-align: middle; }
  </style>
</head>
<body>
  <div class="lang-switch">
    <button onclick="switchLang('fr')">FR</button>
    <button onclick="switchLang('en')">EN</button>
  </div>
  <header>
    <img src="logo-placeholder.png" alt="Espoir+ Logo" />
    <h1 id="title">Espoir+</h1>
    <p id="slogan">S'entraider pour que plus aucun avenir ne soit abandonné</p>
  </header>
  <nav>
    <a href="#mission" id="navMission"><img src="mission-icon.png" class="icon" />Mission</a>
    <a href="#mentorat" id="navMentorat"><img src="mentorship-icon.png" class="icon" />Mentorat</a>
    <a href="#dons" id="navDons"><img src="donation-icon.png" class="icon" />Dons & Entraide</a>
    <a href="#outils" id="navOutils"><img src="toolbox-icon.png" class="icon" />Boîte à outils</a>
    <a href="#admin" id="navAdmin"><img src="admin-icon.png" class="icon" />Espace admin</a>
    <a href="#contact" id="navContact"><img src="contact-icon.png" class="icon" />Contact</a>
  </nav>
  <main>
    <section id="mission">
      <h2>Notre mission</h2>
      <p id="missionText">Aider les jeunes déscolarisés, orphelins ou exclus à retrouver le chemin de l’école ou d’une formation.</p>
    </section>
    <section id="mentorat">
      <h2>Mentorat</h2>
      <p id="mentoratText">Inscris-toi pour devenir mentor ou bénéficier d’un accompagnement.</p>
      <button>Je veux être mentor</button>
      <button>Je cherche un mentor</button>
    </section>
    <section id="dons">
      <h2>Dons & Entraide</h2>
      <p id="donsText">Contribuez en donnant du matériel, du temps ou un soutien financier.</p>
    </section>
    <section id="outils">
      <h2>Boîte à outils</h2>
      <p id="outilsText">Accédez à des cours, vidéos, fiches pratiques pour accompagner les jeunes.</p>
    </section>
    <section id="admin">
      <h2>Espace Admin</h2>
      <input type="text" placeholder="Identifiant admin">
      <input type="password" placeholder="Mot de passe">
      <button>Connexion</button>
    </section>
    <section id="contact">
      <h2>Contact</h2>
      <textarea placeholder="Votre message..."></textarea>
      <button>Envoyer</button>
    </section>
  </main>
  <footer>
    <p>© 2025 Espoir+. Tous droits réservés.</p>
  </footer>  <script>
    const translations = {
      fr: {
        title: "Espoir+",
        slogan: "S'entraider pour que plus aucun avenir ne soit abandonné",
        navMission: "Notre mission",
        navMentorat: "Mentorat",
        navDons: "Dons & Entraide",
        navOutils: "Boîte à outils",
        navAdmin: "Espace admin",
        navContact: "Contact",
        missionText: "Aider les jeunes déscolarisés, orphelins ou exclus à retrouver le chemin de l’école ou d’une formation.",
        mentoratText: "Inscris-toi pour devenir mentor ou bénéficier d’un accompagnement.",
        donsText: "Contribuez en donnant du matériel, du temps ou un soutien financier.",
        outilsText: "Accédez à des cours, vidéos, fiches pratiques pour accompagner les jeunes."
      },
      en: {
        title: "Espoir+",
        slogan: "Helping so that no future is left behind",
        navMission: "Our Mission",
        navMentorat: "Mentorship",
        navDons: "Donations & Help",
        navOutils: "Toolbox",
        navAdmin: "Admin Area",
        navContact: "Contact",
        missionText: "Helping out-of-school, orphaned, or excluded youth return to education or training.",
        mentoratText: "Sign up to become a mentor or get support.",
        donsText: "Contribute by donating supplies, time, or financial support.",
        outilsText: "Access courses, videos, and practical tools to support youth."
      }
    };

    function switchLang(lang) {
      for (let key in translations[lang]) {
        document.getElementById(key).innerText = translations[lang][key];
      }
    }
  </script></body>
</html>
