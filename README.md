<!DOCTYPE html>
<html lang="el">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Επαγγελματικός Καθαρισμός Καπναγωγών | Καθαρισμός Σωληνώσεων Καπνού</title>
    <meta name="description" content="Εξειδικευμένες υπηρεσίες καθαρισμού καπναγωγών και σωληνώσεων καπνού. Ασφάλεια, υγιεινή και γρήγορη εξυπηρέτηση πανελλαδικά.">
    <meta name="keywords" content="καθαρισμός καπναγωγών, σωληνώσεις καπνού, επαγγελματικός καθαρισμός, συντήρηση, πιστοποιητικό καθαρισμού">
    <meta name="author" content="Καθαρισμός Καπναγωγών">
    <link rel="icon" type="image/png" href="https://img.icons8.com/ios-filled/50/ff7043/fire-extinguisher.png">
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Roboto&display=swap" rel="stylesheet">
    <style>
        :root {
            --main: #123456;
            --accent: #ff7043;
            --accent-light: #ffab91;
            --bg: #f6f7fb;
            --white: #fff;
            --gray: #707070;
            --success: #2a9d8f;
            --shadow: 0 2px 18px #d6d6d6;
        }
        html { scroll-behavior: smooth; }
        body {
            margin: 0; font-family: 'Montserrat', Arial, sans-serif; background: var(--bg); color: var(--main);
        }
        header {
            background: linear-gradient(100deg, rgba(18,52,86,0.8), rgba(255,112,67,0.5)), url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1350&q=80') center/cover no-repeat;
            color: var(--white);
            text-align: center;
            padding: 110px 20px 80px;
            position: relative;
        }
        header h1 { margin: 0; font-size: 2.7em; font-weight: bold; letter-spacing: 1px;}
        header p { font-size: 1.2em; margin: 30px auto 0; max-width: 600px;}
        .hero-btn {
            background: var(--accent); color: var(--white); border: none;
            border-radius: 30px; padding: 18px 44px; font-size: 1.1em; margin-top: 38px; letter-spacing:0.5px;
            cursor: pointer; font-weight: 700; box-shadow: 0 2px 10px #0002;
            transition: background 0.2s, transform 0.2s;
            display: inline-block;
        }
        .hero-btn:hover { background: #ff5722; transform: translateY(-2px) scale(1.03);}
        nav {
            background: var(--main); text-align: center; box-shadow: 0 1px 7px #0001;
            position: sticky; top: 0; z-index: 10;
        }
        nav a {
            color: var(--white); text-decoration: none; display: inline-block;
            padding: 20px 33px; font-size: 1.08em; font-weight: 500; letter-spacing: 0.3px;
            transition: background 0.20s, color 0.15s;
        }
        nav a:hover, nav a.active { background: var(--accent); color: var(--main);}
        .cta-bar {
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            background: var(--accent);
            padding: 18px 0;
            margin-bottom: 0;
            box-shadow: 0 2px 8px #0001;
        }
        .cta-bar .hero-btn {
            background: var(--white);
            color: var(--accent);
            margin-top: 0;
            font-size: 1.13em;
            font-weight: 700;
            box-shadow: none;
            border-radius: 26px;
            padding: 15px 40px;
            border: 2px solid var(--accent);
            transition: background 0.2s, color 0.2s, border 0.2s;
        }
        .cta-bar .hero-btn:hover {
            background: var(--accent-light);
            color: var(--main);
            border-color: var(--main);
        }
        .section-indicator {
            position: fixed;
            right: 35px;
            top: 50%;
            transform: translateY(-50%);
            background: var(--accent);
            color: #fff;
            padding: 18px 24px;
            border-radius: 30px;
            font-size: 1.15em;
            font-weight: 700;
            box-shadow: 0 2px 12px #ff704366;
            z-index: 2000;
            transition: background 0.2s, color 0.2s;
            pointer-events: none;
            user-select: none;
            min-width: 120px;
            text-align: center;
            letter-spacing: 0.4px;
            opacity: 0.93;
            white-space: nowrap;
        }
        @media (max-width: 800px) {
            .section-indicator { right: 10px; font-size: 1em; padding: 12px 14px; min-width: 68px;}
        }
        @media (max-width: 600px) {
            .section-indicator { display: none; }
        }
        .container {
            max-width: 1120px; margin: 48px auto 0 auto; background: var(--white);
            padding: 46px 40px; border-radius: 13px; box-shadow: var(--shadow);
        }
        h2 { color: var(--accent); margin-top: 0; font-weight: 700;}
        .section-subtitle {color: var(--gray); font-size: 1.08em;}
        .services { display: flex; flex-wrap: wrap; gap: 24px; margin-top: 24px;}
        .service-item {
            flex: 1 1 250px; background: #f5f6fa; padding: 24px 20px 18px 20px; border-radius: 8px; min-width: 252px;
            box-shadow: 0 1px 7px #eaeaea;
            border-left: 5px solid var(--accent);
            transition: box-shadow .17s;
        }
        .service-item strong { font-size: 1.1em; color: var(--main);}
        .service-item:hover { box-shadow: 0 4px 20px #e76f5111;}
        .service-icon {font-size: 2em; margin-bottom: 10px; color: var(--accent);}
        .steps { display: flex; gap: 18px; margin: 36px 0 0 0; flex-wrap: wrap;}
        .step {
            background: #e3f2fd; flex: 1 1 150px; padding: 22px 16px; border-radius: 7px;
            text-align: center; min-width: 170px; color: #1565c0; box-shadow: 0 1px 6px #bbdefb66;
        }
        .step-icon {font-size: 2.1em; margin-bottom: 8px;}
        .step strong {display: block; margin-bottom: 6px;}
        ul.checklist { list-style: none; padding: 0; margin: 0;}
        ul.checklist li { margin-bottom: 13px; font-size: 1.08em;}
        ul.checklist li::before { content: "✔️"; margin-right: 10px; color: var(--success); font-size: 1.1em;}
        .cost-calc-section {
            margin: 52px 0 32px 0;
            background: #fff3e0;
            border-radius: 12px;
            box-shadow: 0 2px 10px #ff70431a;
            padding: 38px 20px 28px 20px;
            text-align: center;
        }
        .cost-calc-section .section-subtitle {
            margin-bottom: 8px;
        }
        .cost-calc-form {
            display: flex;
            flex-wrap: wrap;
            gap: 18px 34px;
            align-items: flex-end;
            justify-content: center;
            margin-top: 22px;
        }
        .cost-calc-form label {
            display: block;
            margin-bottom: 5px;
            font-size: 1em;
            color: #d35400;
            font-weight: 600;
        }
        .cost-calc-form select,
        .cost-calc-form input {
            padding: 9px 11px;
            border: 1px solid #bbb;
            border-radius: 5px;
            font-size: 1em;
            min-width: 135px;
        }
        .cost-result {
            font-size: 1.15em;
            color: var(--main);
            margin-top: 24px;
            font-weight: 700;
            background: #fffde7;
            border-radius: 6px;
            padding: 13px 0 10px 0;
            display: inline-block;
            min-width: 250px;
            box-shadow: 0 1px 6px #ff704322;
        }
        .cost-breakdown {
            font-size: 0.98em;
            color: #333;
            margin-top: 8px;
            background: #fff9f0;
            border-radius: 6px;
            padding: 10px 14px 7px 14px;
            display: inline-block;
            min-width: 220px;
        }
        .cost-breakdown span {
            display: block;
            margin-bottom: 2px;
        }
        .cost-tooltip {
            display: inline-block;
            position: relative;
            cursor: pointer;
            color: var(--accent);
            font-weight: bold;
            font-size: 1.1em;
            margin-left: 4px;
        }
        .cost-tooltip:hover .tooltip-text,
        .cost-tooltip:focus .tooltip-text {
            display: block;
        }
        .tooltip-text {
            display: none;
            position: absolute;
            bottom: 110%;
            left: 50%;
            transform: translateX(-50%);
            background: #333;
            color: #fff;
            padding: 7px 16px;
            border-radius: 7px;
            font-size: 0.95em;
            white-space: pre-line;
            z-index: 10;
            width: 260px;
        }
        .faq { margin-top: 44px;}
        .faq-item { margin-bottom: 22px; border-bottom: 1px solid #eee;}
        .faq-q { font-weight: bold; cursor: pointer; position: relative; padding: 12px 0 12px 0;}
        .faq-q::after {
            content: '▼'; position: absolute; right: 0; color: var(--accent); font-size: 1.1em;
            transition: transform 0.2s;
        }
        .faq-item.open .faq-q::after {transform: rotate(-180deg);}
        .faq-a { display: none; color: var(--gray); margin: 0 0 14px 0; font-size: 1em;}
        .faq-item.open .faq-a { display: block; animation: fadeIn 0.3s;}
        @keyframes fadeIn {from{opacity:0;} to{opacity:1;}}
        .contact-section { display: flex; flex-wrap: wrap; gap: 40px; margin-top: 38px;}
        .contact-details { flex: 1 1 290px;}
        .contact-form { flex: 1 1 350px;}
        .contact-form form { display: flex; flex-direction: column; gap: 14px;}
        input, textarea {
            padding: 13px; border: 1px solid #bbb; border-radius: 6px; font-size: 1em;
            font-family: 'Roboto', Arial, sans-serif;
        }
        textarea { resize: vertical;}
        button[type="submit"] {
            background: var(--accent); color: var(--white); border: none; padding: 15px; border-radius: 6px;
            font-size: 1.13em; font-weight: 700; cursor: pointer; transition: background 0.2s;
        }
        button[type="submit"]:hover { background: var(--main);}
        .socials {
            margin: 27px 0 0 0; display: flex; gap: 18px;
        }
        .socials a {
            color: var(--main); font-size: 1.9em; border-radius: 50%; background: #f4f4f4;
            display: inline-flex; align-items: center; justify-content: center; width: 38px; height: 38px;
            box-shadow: 0 1px 4px #0001; transition: background 0.18s, color 0.18s;
            position: relative;
        }
        .socials a:hover { background: var(--accent); color: var(--white);}
        .socials a span {
            display: none; position: absolute; bottom: -32px; left: 50%; transform: translateX(-50%);
            background: #222; color: #fff; padding: 4px 10px; border-radius: 4px; font-size: 0.88em;
            white-space: nowrap;
        }
        .socials a:hover span {display: block;}
        .map {
            width: 100%; height: 210px; border-radius: 11px; border: none; margin-top: 28px; box-shadow: 0 2px 6px #0001;
        }
        footer {
            background: var(--main); color: var(--white); text-align: center;
            padding: 23px 0 7px 0; font-size: 1em; margin-top: 52px; letter-spacing: 0.3px;
        }
        footer .footer-row {margin-bottom: 6px;}
        footer a {color:#ffab91; text-decoration:none; margin:0 4px;}
        @media (max-width: 1100px) {
            .container { padding: 28px 5vw;}
            .services, .steps {flex-direction: column;}
        }
        @media (max-width: 820px) {
            .contact-section { flex-direction: column; gap:18px;}
        }
        @media (max-width: 600px) {
            header {padding: 62px 8px 40px;}
            .container {padding: 14px 2vw;}
            nav a {padding: 15px 12px;}
            .cost-result, .cost-breakdown {min-width: unset;}
        }
    </style>
</head>
<body>
    <div class="section-indicator" id="sectionIndicator">Αρχική</div>
    <header>
        <h1>Επαγγελματικός Καθαρισμός Καπναγωγών</h1>
        <p>Ασφαλής, αποτελεσματικός καθαρισμός σωληνώσεων καπνού και απαγωγής, για κάθε επαγγελματικό χώρο. Εγγυόμαστε τη συμμόρφωση με τα πρότυπα υγιεινής και πυρασφάλειας.</p>
    </header>
    <nav>
        <a href="#services" class="active">Υπηρεσίες</a>
        <a href="#process">Διαδικασία</a>
        <a href="#about">Γιατί εμάς</a>
        <a href="#cost-calc">Υπολογισμός Κόστους</a>
        <a href="#faq">FAQ</a>
        <a href="#contact">Επικοινωνία</a>
    </nav>
    <div class="cta-bar">
        <a href="#contact" class="hero-btn">Ζητήστε Προσφορά</a>
    </div>
    <div class="container">
        <section id="services">
            <h2>Υπηρεσίες</h2>
            <div class="section-subtitle">Εξειδικευμένες λύσεις καθαρισμού για κάθε επαγγελματικό χώρο</div>
            <div class="services">
                <div class="service-item">
                    <div class="service-icon" aria-label="Σκούπα" title="Καθαρισμός">🧹</div>
                    <strong>Καθαρισμός Καπναγωγών & Σωληνώσεων</strong>
                    <p>Απομάκρυνση αιθάλης, λιπών, σκόνης και επικίνδυνων καταλοίπων από κάθε τύπο σωλήνα καπνού ή απαγωγής. Σύγχρονες τεχνικές για απόλυτη ασφάλεια.</p>
                </div>
                <div class="service-item">
                    <div class="service-icon" aria-label="Μεγεθυντικός φακός" title="Έλεγχος">🔍</div>
                    <strong>Έλεγχος & Συντήρηση</strong>
                    <p>Τακτικός έλεγχος, συντήρηση και απολύμανση για μέγιστη διάρκεια ζωής και υγιεινή του συστήματος εξαερισμού.</p>
                </div>
                <div class="service-item">
                    <div class="service-icon" aria-label="Πιστοποιητικό" title="Πιστοποιητικό">📄</div>
                    <strong>Έκδοση Πιστοποιητικού</strong>
                    <p>Παρέχουμε πιστοποιητικό καθαρισμού, απαραίτητο για ελέγχους πυρασφάλειας και υγειονομικού ενδιαφέροντος.</p>
                </div>
                <div class="service-item">
                    <div class="service-icon" aria-label="Αστραπή" title="Άμεση εξυπηρέτηση">⚡</div>
                    <strong>Άμεση Εξυπηρέτηση</strong>
                    <p>Εξυπηρετούμε εστιατόρια, φούρνους, βιομηχανίες, ξενοδοχεία, μονάδες μαζικής εστίασης σε όλη την Ελλάδα.</p>
                </div>
            </div>
        </section>
        <section id="process" style="margin-top: 45px;">
            <h2>Η Διαδικασία μας</h2>
            <div class="section-subtitle">Απλή, γρήγορη και αποτελεσματική!</div>
            <div class="steps">
                <div class="step">
                    <div class="step-icon" aria-label="Τηλέφωνο" title="Επικοινωνία">📞</div>
                    <strong>1. Επικοινωνία</strong>
                    <span>Λαμβάνουμε το αίτημά σας και κανονίζουμε ραντεβού.</span>
                </div>
                <div class="step">
                    <div class="step-icon" aria-label="Μικροσκόπιο" title="Έλεγχος">🔬</div>
                    <strong>2. Έλεγχος & Εκτίμηση</strong>
                    <span>Ελέγχουμε επιτόπου τις εγκαταστάσεις σας και προτείνουμε λύση.</span>
                </div>
                <div class="step">
                    <div class="step-icon" aria-label="Τεχνικός" title="Καθαρισμός">🧑‍🔧</div>
                    <strong>3. Καθαρισμός</strong>
                    <span>Εξειδικευμένη ομάδα καθαρίζει με επαγγελματικό εξοπλισμό.</span>
                </div>
                <div class="step">
                    <div class="step-icon" aria-label="Τσεκ" title="Παράδοση">✅</div>
                    <strong>4. Πιστοποιητικό & Παράδοση</strong>
                    <span>Σας παραδίδουμε καθαρό σύστημα & επίσημο πιστοποιητικό.</span>
                </div>
            </div>
        </section>
        <section id="about" style="margin-top: 48px;">
            <h2>Γιατί να μας επιλέξετε</h2>
            <ul class="checklist">
                <li>Εξειδικευμένο προσωπικό & πολυετής εμπειρία</li>
                <li>Σύγχρονος, επαγγελματικός εξοπλισμός</li>
                <li>Πιστοποιημένες διαδικασίες καθαρισμού</li>
                <li>Συμμόρφωση με τα πρότυπα πυρασφάλειας & υγιεινής</li>
                <li>Γραπτή εγγύηση & πιστοποιητικό καθαρισμού</li>
                <li>24ωρη εξυπηρέτηση & άμεση ανταπόκριση</li>
            </ul>
        </section>
        <section id="cost-calc" class="cost-calc-section">
            <h2>Υπολογισμός Κόστους 
                <span class="cost-tooltip" tabindex="0">?
                    <span class="tooltip-text">
                        Το τελικό κόστος καθορίζεται μετά από αυτοψία & συνεννόηση.
                        Ο παρακάτω υπολογισμός είναι ενδεικτικός και αφορά καθαρισμό μεσαίας δυσκολίας. 
                        Οι τιμές περιλαμβάνουν παροχή εξειδικευμένου προσωπικού, πιστοποιητικό & υλικά καθαρισμού.
                        Δίνονται εκπτώσεις για τακτική συντήρηση ή μεγάλους χώρους.
                        Προσφέρεται και μηνιαία συνδρομή για καθαρισμό κάθε 2 εβδομάδες.
                    </span>
                </span>
            </h2>
            <div class="section-subtitle">
                Δείτε άμεσα το πιθανό κόστος καθαρισμού, με βάση τις ανάγκες σας.
            </div>
            <form class="cost-calc-form" id="costForm" autocomplete="off">
                <div>
                    <label for="spaceType">Τύπος Χώρου</label>
                    <select id="spaceType" name="spaceType" required autofocus>
                        <option value="restaurant">Εστιατόριο</option>
                        <option value="bakery">Φούρνος</option>
                        <option value="industry">Βιομηχανία</option>
                        <option value="cafe">Καφετέρια</option>
                        <option value="hotel">Ξενοδοχείο</option>
                        <option value="other">Άλλο</option>
                    </select>
                </div>
                <div>
                    <label for="length">Μήκος Σωληνώσεων (μέτρα)</label>
                    <input type="number" id="length" name="length" min="1" max="200" step="1" value="10" required>
                </div>
                <div>
                    <label for="freq">Συχνότητα Καθαρισμού</label>
                    <select id="freq" name="freq" required>
                        <option value="once">1 φορά/έτος</option>
                        <option value="twice">2 φορές/έτος</option>
                        <option value="quarter">Κάθε τρίμηνο</option>
                        <option value="month">Κάθε μήνα</option>
                        <option value="sub_biweek">Συνδρομή: κάθε 2 εβδομάδες (σταθερό κόστος)</option>
                    </select>
                </div>
            </form>
            <div class="cost-result" id="costResult"></div>
            <div class="cost-breakdown" id="costBreakdown" style="display:none"></div>
        </section>
        <section id="faq" class="faq">
            <h2>Συχνές Ερωτήσεις (FAQ)</h2>
            <div class="faq-item">
                <div class="faq-q">Πόσο συχνά χρειάζεται καθαρισμός καπναγωγών σε επαγγελματικούς χώρους;</div>
                <div class="faq-a">Η συχνότητα εξαρτάται από τη χρήση και τη φύση του χώρου. Για εστιατόρια, φούρνους και μονάδες με έντονη παραγωγή καπνού ή λίπους, συνιστούμε καθαρισμό κάθε 3-6 μήνες. Για άλλους επαγγελματικούς χώρους, τουλάχιστον 1 φορά το χρόνο.</div>
            </div>
            <div class="faq-item">
                <div class="faq-q">Παρέχετε πιστοποιητικό καθαρισμού για τους ελέγχους;</div>
                <div class="faq-a">Ναι, μετά από κάθε εργασία παραδίδουμε επίσημο πιστοποιητικό καθαρισμού, απαραίτητο για επιθεωρήσεις πυρασφάλειας, υγιεινής ή ασφαλιστικούς λόγους.</div>
            </div>
            <div class="faq-item">
                <div class="faq-q">Πόσο διαρκεί ο καθαρισμός;</div>
                <div class="faq-a">Η διάρκεια εξαρτάται από το μήκος και την κατάσταση των σωληνώσεων. Συνήθως απαιτούνται 1-3 ώρες για έναν τυπικό επαγγελματικό χώρο. Σε πολύ μεγάλες εγκαταστάσεις ή σε δύσκολες περιπτώσεις μπορεί να διαρκέσει περισσότερο.</div>
            </div>
            <div class="faq-item">
                <div class="faq-q">Επηρεάζεται η λειτουργία της επιχείρησής μου;</div>
                <div class="faq-a">Οχι, ο καθαρισμός γίνεται με τρόπο που να μην διακόπτει τη λειτουργία της επιχείρησης σας. Μπορούμε να εξυπηρετήσουμε και εκτός ωραρίου λειτουργίας.</div>
            </div>
            <div class="faq-item">
                <div class="faq-q">Είναι ασφαλή τα υλικά και οι μέθοδοι που χρησιμοποιείτε;</div>
                <div class="faq-a">Ναι, χρησιμοποιούμε υλικά και τεχνολογίες φιλικές προς το περιβάλλον και τον άνθρωπο, με έμφαση στην ασφάλεια προσωπικού και πελατών.</div>
            </div>
        </section>
        <section id="contact" class="contact-section">
            <div class="contact-details">
                <h2>Επικοινωνία</h2>
                <p>
                    <strong>Τηλέφωνο:</strong> <a href="tel:2101234567">210 1234567</a><br>
                    <strong>Email:</strong> <a href="mailto:info@kapnagwgoi.gr">info@kapnagwgoi.gr</a>
                </p>
                <div class="socials">
                    <a href="#" aria-label="Facebook"><i class="fa fa-facebook"></i><span>Facebook</span></a>
                    <a href="#" aria-label="Instagram"><i class="fa fa-instagram"></i><span>Instagram</span></a>
                    <a href="#" aria-label="LinkedIn"><i class="fa fa-linkedin"></i><span>LinkedIn</span></a>
                </div>
                <iframe class="map"
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3143.129069167134!2d23.7275!3d37.9838!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x14a1bd2d5e7b0657%3A0x9a8f8c2e6e8b!2zQXRoZW5zLCBHcmVlY2U!5e0!3m2!1sel!2sgr!4v1688859999999!5m2!1sel!2sgr"
                    allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
            <div class="contact-form">
                <h2>Φόρμα Επικοινωνίας</h2>
                <form onsubmit="event.preventDefault(); alert('Το μήνυμά σας εστάλη!'); this.reset();">
                    <input type="text" placeholder="Ονοματεπώνυμο" required>
                    <input type="email" placeholder="Email" required>
                    <input type="tel" placeholder="Τηλέφωνο" required>
                    <textarea rows="4" placeholder="Το μήνυμά σας..." required></textarea>
                    <button type="submit">Αποστολή</button>
                </form>
            </div>
        </section>
    </div>
    <footer>
        <div class="footer-row">
            &copy; 2025 Καθαρισμός Επαγγελματικών Καπναγωγών | Designed by marten291
        </div>
        <div>
            <a href="#services">Υπηρεσίες</a> | 
            <a href="#about">Γιατί εμάς</a> | 
            <a href="#contact">Επικοινωνία</a>
        </div>
    </footer>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
    <script>
        // FAQ toggle
        document.querySelectorAll('.faq-q').forEach(q => {
            q.addEventListener('click', function(){
                const parent = this.parentElement;
                parent.classList.toggle('open');
            });
        });

        // Υπολογιστής κόστους με επιλογή συνδρομής
        function calcCost() {
            const spaceType = document.getElementById('spaceType').value;
            const length = parseInt(document.getElementById('length').value, 10) || 0;
            const freq = document.getElementById('freq').value;

            const resultEl = document.getElementById('costResult');
            const breakdownEl = document.getElementById('costBreakdown');

            // Νέα επιλογή για σταθερή συνδρομή
            if (freq === 'sub_biweek') {
                resultEl.textContent =
                    "Συνδρομή: 350€ / μήνα (πλέον ΦΠΑ)";
                breakdownEl.innerHTML =
                    "<span>Περιλαμβάνει 2 καθαρισμούς κάθε μήνα (ανά 2 εβδομάδες)</span>" +
                    "<span style='color:#e76f51;'>Ιδανικό για εντατική χρήση και μεγάλους χώρους</span>" +
                    "<span style='color: #777;'>Όλες οι υπηρεσίες, υλικά, προσωπικό και πιστοποιητικό περιλαμβάνονται.</span>";
                breakdownEl.style.display = "block";
                return;
            }

            // Υπόλοιπη λογική όπως πριν
            let base, perMeter;
            switch (spaceType) {
                case 'industry': base = 130; perMeter = 12; break;
                case 'hotel':    base = 95;  perMeter = 9;  break;
                case 'bakery':   base = 85;  perMeter = 8;  break;
                case 'cafe':     base = 75;  perMeter = 7;  break;
                case 'restaurant': base = 70; perMeter = 7; break;
                case 'other':    base = 70;  perMeter = 7;  break;
                default:         base = 70;  perMeter = 7;  break;
            }

            let lengthCost;
            if (length <= 10) {
                lengthCost = perMeter * length;
            } else if (length <= 20) {
                lengthCost = perMeter * 10 + (perMeter * 0.9) * (length - 10);
            } else {
                lengthCost = perMeter * 10 + (perMeter * 0.9) * 10 + (perMeter * 0.75) * (length - 20);
            }

            let freqDiscount = 1;
            let discountInfo = "";
            if (freq === 'twice') { freqDiscount = 0.93; discountInfo = "Έκπτωση 7% για τακτική συντήρηση"; }
            else if (freq === 'quarter') { freqDiscount = 0.85; discountInfo = "Έκπτωση 15% για πακέτο 4 επισκέψεων"; }
            else if (freq === 'month') { freqDiscount = 0.70; discountInfo = "Έκπτωση 30% για πακέτο 12 επισκέψεων"; }

            let visitCost = (base + lengthCost) * freqDiscount;
            let visitsPerYear = 1;
            if (freq === 'twice') visitsPerYear = 2;
            else if (freq === 'quarter') visitsPerYear = 4;
            else if (freq === 'month') visitsPerYear = 12;
            let totalCost = visitCost * visitsPerYear;

            let minCost = Math.round(totalCost * 0.9);
            let maxCost = Math.round(totalCost * 1.1);

            let minVisit = Math.round(visitCost * 0.9);
            let maxVisit = Math.round(visitCost * 1.1);

            if (length < 1 || length > 200) {
                resultEl.textContent = "Συμπληρώστε σωστά τα στοιχεία για να δείτε το κόστος.";
                breakdownEl.style.display = "none";
                return;
            }

            let period = "ετήσιου πακέτου";
            let freqLabel = "";
            if (freq === 'once') freqLabel = "(1 επίσκεψη)";
            else if (freq === 'twice') { period = "πακέτου 2 επισκέψεων"; freqLabel = "(ανά επίσκεψη)"; }
            else if (freq === 'quarter') { period = "πακέτου 4 επισκέψεων"; freqLabel = "(ανά επίσκεψη)"; }
            else if (freq === 'month') { period = "πακέτου 12 επισκέψεων"; freqLabel = "(ανά επίσκεψη)"; }

            resultEl.textContent =
                "Περίπου κόστος " + period + ": " + minCost + "€ έως " + maxCost + "€ (πλέον ΦΠΑ)";

            breakdownEl.innerHTML =
                "<span>Ενδεικτική τιμή " + freqLabel + ": <b>" + minVisit + "€ έως " + maxVisit + "€</b></span>"
                + (discountInfo ? "<span style='color: #e76f51;'>" + discountInfo + "</span>" : "")
                + "<span style='color: #777;'>Περιλαμβάνει προσωπικό, υλικά και πιστοποιητικό καθαρισμού.</span>";

            breakdownEl.style.display = "block";
        }

        document.getElementById('spaceType').addEventListener('input', calcCost);
        document.getElementById('length').addEventListener('input', calcCost);
        document.getElementById('freq').addEventListener('input', calcCost);
        window.addEventListener('DOMContentLoaded', calcCost);

        // Δείκτης ενότητας
        const indicator = document.getElementById('sectionIndicator');
        const sections = [
            {id: "services", label: "Υπηρεσίες"},
            {id: "process", label: "Διαδικασία"},
            {id: "about", label: "Γιατί εμάς"},
            {id: "cost-calc", label: "Κόστος"},
            {id: "faq", label: "FAQ"},
            {id: "contact", label: "Επικοινωνία"}
        ];
        function updateSectionIndicator() {
            const scrollY = window.scrollY + window.innerHeight/3;
            let found = false;
            for (let i = sections.length-1; i >= 0; i--) {
                const s = document.getElementById(sections[i].id);
                if (s && s.offsetTop < scrollY) {
                    indicator.textContent = sections[i].label;
                    found = true;
                    break;
                }
            }
            if (!found) indicator.textContent = "Αρχική";
        }
        window.addEventListener('scroll', updateSectionIndicator);
        window.addEventListener('resize', updateSectionIndicator);
        window.addEventListener('DOMContentLoaded', updateSectionIndicator);
    </script>
</body>
</html>
