```html name=index.html
<!DOCTYPE html>
<html lang="el">
<head>
    <meta charset="UTF-8">
    <title>Καθαρισμός Επαγγελματικών Σωλήνων Καπνού</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Montserrat:700,400&display=swap" rel="stylesheet">
    <script>
    function showThankYou(event) {
        event.preventDefault();
        document.getElementById('thankyou').style.display = 'block';
        document.getElementById('contactForm').reset();
    }
    function estimatePrice() {
        const shopType = document.getElementById('shopType').value;
        const pipeLength = parseInt(document.getElementById('pipeLength').value) || 0;
        const vents = parseInt(document.getElementById('vents').value) || 1;
        const lastClean = document.getElementById('lastClean').value;
        let base = 60;
        let msg = "";
        if (shopType === "grill") { base += 20; msg += "Απαιτείται ενισχυμένος καθαρισμός για ψητοπωλείο. "; }
        if (shopType === "cafe")  { base -= 10; msg += "Λιγότεροι ρύποι για καφετέρια. "; }
        if (shopType === "bar")   { base -= 5;  msg += "Bar = λιγότερα λίπη. "; }
        if (shopType === "restaurant") { msg += "Τυπικός καθαρισμός εστιατορίου. "; }

        let monthsAgo = 0;
        if (lastClean) {
            const last = new Date(lastClean);
            const now = new Date();
            monthsAgo = (now.getFullYear() - last.getFullYear()) * 12 + (now.getMonth() - last.getMonth());
            if (monthsAgo > 12) {
                base += 20;
                msg += "Έχει περάσει >1 χρόνος. Ενδέχεται να απαιτείται εντατικότερη εργασία.";
            }
        }

        let price = base + (pipeLength * 8) + ((vents-1)*15);
        if (!shopType || pipeLength === 0) price = '—';
        document.getElementById('price').textContent = isNaN(price) ? '—' : price;
        document.getElementById('estimate-msg').textContent = msg;
    }
    </script>
</head>
<body>
    <header>
        <div class="hero">
            <div class="hero-content">
                <h1>Επαγγελματικός Καθαρισμός Σωλήνων Καπνού</h1>
                <p>Εξειδικευμένες υπηρεσίες καθαρισμού σε εξαεριστήρες, καμινάδες &amp; σωληνώσεις για χώρους εστίασης</p>
                <a href="#contact" class="cta-btn">Ζητήστε Προσφορά</a>
            </div>
        </div>
        <nav>
            <ul>
                <li><a href="#services">Υπηρεσίες</a></li>
                <li><a href="#why">Γιατί εμείς</a></li>
                <li><a href="#specs">Εκτίμηση Τιμής</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#faq">Συχνές Ερωτήσεις</a></li>
                <li><a href="#contact">Επικοινωνία</a></li>
            </ul>
        </nav>
    </header>

    <section id="services">
        <h2>Οι Υπηρεσίες μας</h2>
        <div class="services-grid">
            <div class="service-card">
                <img src="icon1.png" alt="Καθαρισμός σωλήνων">
                <h3>Καθαρισμός σωλήνων</h3>
                <p>Αφαίρεση λίπους, επικαθίσεων & ρύπων από σωλήνες απαγωγής καπνού κάθε μεγέθους.</p>
            </div>
            <div class="service-card">
                <img src="icon2.png" alt="Συντήρηση εξαεριστήρων">
                <h3>Συντήρηση εξαεριστήρων</h3>
                <p>Έλεγχος, καθαρισμός &amp; συντήρηση εξαεριστήρων και καμινάδων για άριστη λειτουργία.</p>
            </div>
            <div class="service-card">
                <img src="icon3.png" alt="Πιστοποίηση">
                <h3>Πιστοποίηση καθαρισμού</h3>
                <p>Έγγραφη βεβαίωση καθαρισμού για υγειονομικό έλεγχο και ασφάλεια.</p>
            </div>
        </div>
    </section>

    <section id="why">
        <h2>Γιατί να μας επιλέξετε</h2>
        <div class="why-grid">
            <div>
                <span class="icon">🛠️</span>
                <p>Εξειδικευμένο προσωπικό με πολυετή εμπειρία</p>
            </div>
            <div>
                <span class="icon">⚡</span>
                <p>Γρήγορη & διακριτική εξυπηρέτηση</p>
            </div>
            <div>
                <span class="icon">🌱</span>
                <p>Οικολογικά υλικά & σύγχρονος εξοπλισμός</p>
            </div>
            <div>
                <span class="icon">📜</span>
                <p>Πιστοποίηση & τήρηση όλων των προδιαγραφών</p>
            </div>
        </div>
    </section>

    <!-- MODERN ESTIMATION SECTION -->
    <section id="specs" class="ultra-specs">
      <h2>
        <span class="emoji">🧮</span> Ενδεικτικός Υπολογισμός Τιμής Καθαρισμού
      </h2>
      <form id="specsForm" class="ultra-specs-form" autocomplete="off" oninput="estimatePrice()">
        <div class="spec-row">
          <div class="spec-field">
            <label for="shopType"><span class="icon">🏢</span> Είδος καταστήματος</label>
            <select id="shopType" name="shopType" required>
              <option value="">Επιλέξτε...</option>
              <option value="restaurant">🍽️ Εστιατόριο</option>
              <option value="grill">🥩 Ψητοπωλείο</option>
              <option value="cafe">☕ Καφετέρια</option>
              <option value="bar">🍸 Bar</option>
              <option value="other">Άλλο</option>
            </select>
            <span class="inline-tip">Βοηθά στον ακριβή υπολογισμό.</span>
          </div>
          <div class="spec-field">
            <label for="lastClean"><span class="icon">📆</span> Τελευταίος καθαρισμός</label>
            <input type="date" id="lastClean" name="lastClean" required>
            <span class="inline-tip">Εκτιμήστε αν δεν θυμάστε ακριβώς.</span>
          </div>
        </div>
        <div class="spec-row">
          <div class="spec-field">
            <label for="pipeLength"><span class="icon">📏</span> Μήκος σωλήνα (μ.)</label>
            <input type="number" id="pipeLength" name="pipeLength" min="1" max="100" placeholder="π.χ. 8" required>
            <span class="inline-tip">Συνολικό μήκος σωλήνων.</span>
          </div>
          <div class="spec-field">
            <label for="vents"><span class="icon">🌀</span> Εξαεριστήρες/Καμινάδες</label>
            <input type="number" id="vents" name="vents" min="1" max="10" placeholder="π.χ. 2" required>
            <span class="inline-tip">Σημεία εξαγωγής.</span>
          </div>
        </div>
        <div class="ultra-estimate">
          <span class="emoji">💰</span>
          <strong>Ενδεικτική τιμή:</strong>
          <span id="price" class="ultra-price">—</span> €
          <span id="estimate-msg" class="ultra-remark"></span>
        </div>
        <div class="ultra-cta">
          <span>Η τιμή είναι ενδεικτική. Για ακριβή προσφορά:</span>
          <a href="#contact" class="cta-btn modern-cta">Επικοινωνία</a>
        </div>
      </form>
    </section>
    <!-- END MODERN ESTIMATION SECTION -->

    <section id="gallery">
        <h2>Gallery Εργασιών</h2>
        <div class="photos">
            <img src="photo1.jpg" alt="Πριν τον καθαρισμό">
            <img src="photo2.jpg" alt="Μετά τον καθαρισμό">
            <img src="photo3.jpg" alt="Σωλήνας καθαρισμένος">
        </div>
    </section>

    <section id="faq">
        <h2>Συχνές Ερωτήσεις</h2>
        <div class="faq-list">
            <details>
                <summary>Κάθε πότε πρέπει να γίνεται καθαρισμός σωλήνων καπνού;</summary>
                <p>Συνιστούμε καθαρισμό τουλάχιστον μία φορά το χρόνο, ή συχνότερα ανάλογα με τη χρήση και τους κανονισμούς.</p>
            </details>
            <details>
                <summary>Θα διακοπεί η λειτουργία της κουζίνας μου;</summary>
                <p>Εργαζόμαστε με ταχύτητα και διακριτικότητα, ώστε να μειώσουμε τον χρόνο διακοπής στο ελάχιστο.</p>
            </details>
            <details>
                <summary>Δίνετε πιστοποιητικό καθαρισμού για τους ελέγχους;</summary>
                <p>Ναι, μετά από κάθε εργασία παρέχουμε έγγραφη βεβαίωση καθαρισμού.</p>
            </details>
        </div>
    </section>

    <section id="contact">
        <h2>Επικοινωνία</h2>
        <div class="contact-flex">
            <div class="contact-info">
                <p><strong>Τηλέφωνο:</strong> <a href="tel:+306993129894">+306993129894</a></p>
                <p><strong>Email:</strong> <a href="mailto:to@email.com">to@email.com</a></p>
                <p><strong>WhatsApp:</strong> <a href="https://wa.me/306993129894">Στείλτε μας μήνυμα</a></p>
                <div class="social">
                    <a href="https://www.facebook.com/profile.php?id=61578239975604&sk=about" target="_blank">
                        <img src="facebook.png" alt="Facebook">
                    </a>
                    <a href="#"><img src="instagram.png" alt="Instagram"></a>
                </div>
            </div>
            <form id="contactForm" onsubmit="showThankYou(event)">
                <label for="name">Όνομα *</label>
                <input type="text" id="name" name="name" required>
                <label for="business">Επιχείρηση</label>
                <input type="text" id="business" name="business">
                <label for="phone">Τηλέφωνο *</label>
                <input type="tel" id="phone" name="phone" required>
                <label for="message">Μήνυμα *</label>
                <textarea id="message" name="message" required></textarea>
                <button type="submit">Αποστολή</button>
                <p id="thankyou" style="display:none;color:green;">Ευχαριστούμε! Θα επικοινωνήσουμε σύντομα.</p>
            </form>
        </div>
    </section>

    <footer>
        <p>© 2025 Καθαρισμός Επαγγελματικών Σωλήνων Καπνού</p>
    </footer>
</body>
</html>
```
