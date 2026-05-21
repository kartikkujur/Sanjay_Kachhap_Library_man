# Sanjay_Kachhap_Library_man <!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Library Man of Jharkhand - Sanjay Kachhap</title>
    <style>
        /* CSS Reset & Variables */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --primary-color: #2c3e50;
            --secondary-color: #e67e22;
            --bg-light: #f8f9fa;
            --text-dark: #333;
            --text-light: #fff;
        }

        body {
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        /* Header & Navigation */
        header {
            background-color: var(--primary-color);
            color: var(--text-light);
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .nav-container {
            width: 85%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: var(--secondary-color);
        }

        nav a {
            color: var(--text-light);
            text-decoration: none;
            margin-left: 20px;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--secondary-color);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(44, 62, 80, 0.8), rgba(44, 62, 80, 0.9)), url('https://images.unsplash.com/photo-1524995997946-a1c2e315a42f?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80') no-repeat center center/cover;
            height: 60vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--text-light);
            padding: 0 20px;
        }

        .hero-content h1 {
            font-size: 45px;
            margin-bottom: 15px;
            letter-spacing: 1px;
        }

        .hero-content p {
            font-size: 20px;
            color: #bdc3c7;
            max-width: 700px;
            margin: 0 auto;
        }

        /* Main Wrapper */
        .container {
            width: 85%;
            margin: 50px auto;
        }

        /* Section Title */
        .section-title {
            text-align: center;
            font-size: 32px;
            margin-bottom: 40px;
            position: relative;
            color: var(--primary-color);
        }

        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background-color: var(--secondary-color);
            margin: 10px auto 0 auto;
            border-radius: 2px;
        }

        /* Highlight Box */
        .main-story-highlight {
            background: linear-gradient(135deg, #fff 0%, #fffbf2 100%);
            border-top: 6px solid var(--secondary-color);
            border-bottom: 2px solid rgba(230, 126, 34, 0.2);
            padding: 35px;
            border-radius: 8px;
            margin-bottom: 50px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.06);
            text-align: center;
        }

        .main-story-highlight h2 {
            font-size: 28px;
            color: var(--primary-color);
            margin-bottom: 20px;
            font-weight: 700;
        }

        .main-story-highlight p {
            font-size: 18px;
            color: #444;
            max-width: 950px;
            margin: 0 auto;
            line-height: 1.8;
            font-style: italic;
        }

        /* About / Biography Section */
        .bio-section {
            display: flex;
            gap: 40px;
            align-items: center;
            margin-bottom: 60px;
            background: #fff;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }

        .bio-img {
            flex: 1;
            min-width: 300px;
        }

        .bio-img img {
            width: 100%;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.15);
        }

        .bio-text {
            flex: 2;
        }

        .bio-text h3 {
            font-size: 24px;
            color: var(--secondary-color);
            margin-bottom: 15px;
        }

        .bio-text p {
            margin-bottom: 15px;
            font-size: 16px;
            text-align: justify;
        }

        /* History Highlight Box */
        .history-box {
            background-color: #fff;
            border-left: 5px solid var(--secondary-color);
            padding: 30px;
            border-radius: 0 10px 10px 0;
            margin-bottom: 60px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .history-box h3 {
            font-size: 24px;
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        .history-box p {
            font-size: 16px;
            color: #555;
            margin-bottom: 10px;
        }

        /* Features Grid */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }

        .card {
            background: #fff;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            border-top: 4px solid var(--primary-color);
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
            border-top-color: var(--secondary-color);
        }

        .card h3 {
            font-size: 20px;
            margin-bottom: 12px;
            color: var(--primary-color);
        }

        /* Photo Gallery Section */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .gallery-item {
            background: #fff;
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.08);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            overflow: hidden;
        }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 6px;
        }

        .gallery-item p {
            font-size: 14px;
            color: #555;
            text-align: center;
            margin-top: 8px;
            font-weight: 500;
        }

        .gallery-item:hover {
            transform: scale(1.03);
            box-shadow: 0 8px 20px rgba(0,0,0,0.15);
        }

        /* Image Upload Form Box Layout */
        .upload-section {
            background: #fff;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            margin-bottom: 60px;
            border: 2px dashed var(--secondary-color);
            text-align: center;
        }

        .upload-section h3 {
            color: var(--primary-color);
            margin-bottom: 15px;
            font-size: 20px;
        }

        .upload-controls {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
            align-items: center;
        }

        .upload-controls input[type="file"] {
            padding: 10px;
            background: var(--bg-light);
            border-radius: 5px;
            border: 1px solid #ddd;
            cursor: pointer;
        }

        .upload-controls input[type="text"] {
            padding: 11px;
            border: 1px solid #ddd;
            border-radius: 5px;
            width: 250px;
            outline: none;
        }

        .upload-controls input[type="text"]:focus {
            border-color: var(--secondary-color);
        }

        .upload-btn {
            background-color: var(--secondary-color);
            color: white;
            border: none;
            padding: 11px 25px;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: background-color 0.3s;
        }

        .upload-btn:hover {
            background-color: var(--primary-color);
        }

        /* Quote Section */
        .quote-box {
            background-color: var(--primary-color);
            color: var(--text-light);
            padding: 40px;
            border-left: 8px solid var(--secondary-color);
            border-radius: 4px;
            font-style: italic;
            font-size: 22px;
            text-align: center;
            margin-bottom: 60px;
        }

        /* Contact & Form Grid Container */
        .contact-section-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 40px;
            margin-bottom: 60px;
        }

        .contact-info-box, .contact-form-box {
            background: #fff;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }

        .contact-info-box h3, .contact-form-box h3 {
            font-size: 22px;
            color: var(--primary-color);
            margin-bottom: 20px;
            border-bottom: 2px solid var(--secondary-color);
            padding-bottom: 8px;
            display: inline-block;
        }

        .contact-details p {
            margin-bottom: 15px;
            font-size: 16px;
        }

        .contact-details strong {
            color: var(--secondary-color);
        }

        /* Form Styling */
        .form-group {
            margin-bottom: 15px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 500;
            color: #555;
        }

        .form-group input, .form-group textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 15px;
            outline: none;
            transition: border-color 0.3s;
        }

        .form-group input:focus, .form-group textarea:focus {
            border-color: var(--secondary-color);
        }

        .submit-btn {
            background-color: var(--primary-color);
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            font-weight: bold;
            transition: background-color 0.3s;
            width: 100%;
        }

        .submit-btn:hover {
            background-color: var(--secondary-color);
        }

        /* Footer Modern Layout */
        footer {
            background-color: var(--primary-color);
            color: var(--text-light);
            padding: 40px 0 20px 0;
            border-top: 4px solid var(--secondary-color);
        }

        .footer-grid {
            width: 85%;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            padding-bottom: 20px;
            border-bottom: 1px solid #34495e;
        }

        .footer-about h3, .footer-links h3 {
            color: var(--secondary-color);
            margin-bottom: 15px;
            font-size: 18px;
        }

        .footer-about p {
            font-size: 14px;
            color: #bdc3c7;
            text-align: justify;
        }

        .footer-links ul {
            list-style: none;
        }

        .footer-links ul li {
            margin-bottom: 8px;
        }

        .footer-links ul li a {
            color: #bdc3c7;
            text-decoration: none;
            font-size: 14px;
            transition: color 0.3s;
        }

        .footer-links ul li a:hover {
            color: var(--secondary-color);
        }

        .footer-bottom {
            text-align: center;
            padding-top: 20px;
            font-size: 14px;
            color: #bdc3c7;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
                gap: 15px;
            }
            nav a {
                margin: 0 10px;
            }
            .bio-section {
                flex-direction: column;
            }
            .hero-content h1 {
                font-size: 32px;
            }
            .hero-content p {
                font-size: 16px;
            }
            .main-story-highlight p {
                font-size: 16px;
            }
            .upload-controls {
                flex-direction: column;
                width: 100%;
            }
            .upload-controls input[type="text"], .upload-btn {
                width: 100%;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <div class="logo">झारखंड के लाइब्रेरी मैन</div>
            <nav>
                <a href="#about">परिचय</a>
                <a href="#movement">आंदोलन</a>
                <a href="#achievements">उपलब्धियां</a>
                <a href="#gallery">फोटो गैलरी</a>
                <a href="#contact">संपर्क करें</a>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>संजय कच्छप (Sanjay Kachhap)</h1>
            <p>हंडिया बेचने के संघर्ष से लेकर 40+ डिजिटल लाइब्रेरी खड़ी करने और प्रधानमंत्री से सम्मान पाने वाले "लाइब्रेरी मैन ऑफ झारखंड" की महागाथा।</p>
        </div>
    </section>

    <div class="container">

        <section class="main-story-highlight">
            <h2>झारखंड के "लाइब्रेरी मैन": संजय कच्छप की प्रेरणादायक कहानी</h2>
            <p>"कहते हैं कि अगर आप समाज में बदलाव देखना चाहते हैं, तो उसकी शुरुआत खुद से करनी होगी। इस बात को सच कर दिखाया है झारखंड के संजय कच्छप ने। पेशे से कृषि बाजार समिति में मार्केटिंग सेक्रेटरी (सरकारी अधिकारी) संजय कच्छप आज किसी परिचय के मोहताज नहीं हैं। उन्होंने झारखंड के सुदूर, ग्रामीण और नक्सल प्रभावित इलाकों में शिक्षा का अलख जगाने के लिए 40 से ज्यादा डिजिटल और फिजिकल लाइब्रेरी खड़ी कर दी हैं। देश के प्रधानमंत्री नरेंद्र मोदी ने भी अपने 'मन की बात' कार्यक्रम में उनके इस जज्बे की सराहना की है।"</p>
        </section>

        <section id="about">
            <h2 class="section-title">शुरुआती जीवन और संघर्ष</h2>
            <div class="bio-section">
                <div class="bio-img">
                    <img src="https://i.ibb.co/TqPbHTTW/Gemini-Generated-Image-tucb6utucb6utucb-2.png" alt="Sanjay Kachhap Portrait">
                </div>
                <div class="bio-text">
                    <h3>गरीबी को हराकर पाया मुकाम</h3>
                    <p>संजय कच्छप का जन्म झारखंड के पश्चिमी सिंहभूम ( चाईबासा ) जिले के एक बेहद गरीब आदिवासी परिवार में हुआ था। वह बचपन से ही पढ़ाई में मेधावी थे और उनका सपना एक IAS अधिकारी बनने का था। लेकिन आर्थिक तंगी उनके आड़े आ गई।</p>
                    <p>अपनी पढ़ाई का खर्च उठाने के लिए संजय को दोपहर में स्थानीय स्तर पर बनने वाली चावल की शराब (हंडिया) बेचनी पड़ती थी, और वह रात के समय पढ़ाई किया करते थे। संसाधनों की कमी के कारण वह IAS तो नहीं बन पाए, लेकिन उन्होंने हार नहीं मानी और कड़ी मेहनत के दम पर झारखंड सरकार के कृषि विभाग में <strong>मार्केटिंग सेक्रेटरी</strong> के पद पर चयनित हुए।</p>
                    <p>नौकरी मिलने के बाद संजय ने संकल्प लिया कि जो दर्द और कमी उन्होंने झेली है, वह झारखंड के किसी और गरीब या आदिवासी बच्चे को नहीं झेलनी पड़ेगी।</p>
                </div>
            </div>
        </section>

        <section class="history-box">
            <h3>📚 पुस्तकालय आंदोलन की शुरुआत: "मोहल्ला लाइब्रेरी"</h3>
            <p>साल 2008 में संजय कच्छप ने अपने इस मिशन की शुरुआत की। उन्होंने पश्चिमी सिंहभूम के एक खाली पड़े सरकारी भवन से पहली 'मोहल्ला लाइब्रेरी' शुरू की। शुरुआत में उन्होंने अपनी सैलरी से पैसे बचाकर और दोस्तों से पुरानी किताबें मांगकर इस लाइब्रेरी को खड़ा किया।</p>
            <p>धीरे-धीरे यह एक बड़ा जन-आंदोलन बन गया। आज उनके द्वारा स्थापित की गई लाइब्रेरीज़ की कुछ खास बातें इस प्रकार हैं:</p>
        </section>
        
        <section id="movement">
            <h2 class="section-title">पुस्तकालय आंदोलन की विशेषताएं</h2>
            <div class="grid">
                <div class="card">
                    <h3>40+ लाइब्रेरी का नेटवर्क</h3>
                    <p>संजय ने चाईबासा, सरायकेला, खूंटी, duमका और साहेबगंज जैसे सुदूर और नक्सल प्रभावित जिलों के गांवों में 40 से अधिक लाइब्रेरी खोली हैं, ताकि गरीब बच्चों को शहर न जाना पड़े।</p>
                </div>
                <div class="card">
                    <h3>20+ हाई-टेक डिजिटल केंद्र</h3>
                    <p>इनकी कई लाइब्रेरीज़ पूरी तरह से डिजिटल हैं, जहाँ कंप्यूटर, हाई-स्पीड वाई-फाई और ई-बुक्स मौजूद हैं। छात्र यहाँ UPSC, JPSC, बैंकिंग और रेलवे की ऑनलाइन तैयारी करते हैं</p>
                </div>
                <div class="card">
                    <h3>चलती-फिरती 'कार लाइब्रेरी'</h3>
                    <p>छुट्टी के दिनों में संजय अपनी निजी कार में किताबें भरकर सुदूर जंगलों और गांवों में पहुंच जाते हैं और बच्चों के बीच मुफ्त में किताबें बांटकर शिक्षा की अलख जगाते हैं</p>
                </div>
                <div class="card">
                    <h3>अनोखा 'चैन सिस्टम'</h3>
                    <p>लाइब्रेरी से पढ़कर सफल होने वाले सीनियर छात्रों के लिए नियम है कि वे नौकरी मिलने के बाद जूनियर बच्चों को मुफ्त में कोचिंग देंगे और लाइब्रेरी के लिए किताबें दान करेंगे।</p>
                </div>
            </div>
        </section>

        <div class="quote-box">
            "किताबें गरीबी से लड़ने और समाज में सकारात्मक बदलाव लाने का सबसे बड़ा हथियार हैं।" <br> — संजय कच्छप
        </div>

        <section id="achievements">
            <h2 class="section-title">राष्ट्रीय सम्मान और पहचान</h2>
            <div class="bio-section" style="flex-direction: row-reverse;">
                <div class="bio-img">
                    <img src="https://wpmedia.prabhatkhabar.com/uploads/2024/01/Sanjay-kachap.jpg" alt="PM Mann ki Baat Achievement">
                </div>
                <div class="bio-text">
                    <h3>'मन की बात' में गूंजा नाम</h3>
                    <p>संजय कच्छप के इस बेमिसाल प्रयास की गूंज देश की राजधानी तक पहुंची। भारत के <strong>प्रधानमंत्री नरेंद्र मोदी</strong> ने अपने प्रसिद्ध रेडियो कार्यक्रम <strong>'मन की बात'</strong> में संजय के इस अनूठे लाइब्रेरी आंदोलन की जमकर तारीफ की।</p>
                    <p>इसी संबोधन के बाद से उन्हें देश भर में आधिकारिक तौर पर <strong>"लाइब्रेरी मैन ऑफ झारखंड"</strong> का गौरवशाली नाम मिला। आज उनकी लाइब्रेरी में पढ़कर सैकड़ों ग्रामीण युवा झारखंड पुलिस, सेना, रेलवे और राज्य प्रशासनिक पदों पर देश की सेवा कर रहे हैं। बॉलीवुड अभिनेता सोनू सूद ने भी उनके इस नेक कार्य में हाथ बंटाते हुए पुस्तकें और कंप्यूटर भेंट किए हैं।</p>
                </div>
            </div>
        </section>

        <section id="gallery">
            <h2 class="section-title">फोटो गैलरी (Photo Gallery)</h2>
            
            <div class="gallery-grid" id="galleryGrid">
                <div class="gallery-item">
                    <img src="https://i.ibb.co/r27DwqWs/Whats-App-Image-2026-04-14-at-5-45-16-PM.jpg" alt="संजय कच्छप लाइब्रेरी में">
                    <p>संजय कच्छप अपनी लाइब्रेरी में</p>
                </div>

                <div class="gallery-item">
                    <img src="https://i.ibb.co/zKMxzM2/Whats-App-Image-2026-05-21-at-1-12-37-PM.jpg" alt="डिजिटल लाइब्रेरी">
                    <p>डिजिटल लाइब्रेरी और कंप्यूटर का उदघाटन</p>
                </div>

                <div class="gallery-item">
                    <img src="https://i.ibb.co/xt5T6gK1/Whats-App-Image-2026-05-21-at-1-12-36-PM.jpg" alt="ग्रामीण छात्र">
                    <p>लाइब्रेरी में पढ़ते ग्रामीण छात्र</p>
                </div>
                     
                <div class="gallery-item">
                    <img src="https://scontent.fixr3-3.fna.fbcdn.net/v/t39.30808-6/571283347_24950289084629407_1708663552109111320_n.jpg?stp=cp6_dst-jpg_tt6&_nc_cat=109&ccb=1-7&_nc_sid=833d8c&_nc_ohc=KDt5JlAZkFMQ7kNvwGvw-8w&_nc_oc=AdpFWZyHoCLn5eyDkFD15JyJzlpGBAvQINkq4kVnNwcz08J6CvO1nY1XLSkDGxLc3bZ6D-ZueEamx7Gj7eRo2kuK&_nc_zt=23&_nc_ht=scontent.fixr3-3.fna&_nc_gid=lBRR6QPUHTk3euSliaoDKw&_nc_ss=7b2a8&oh=00_Af5XZ9dBmrxA0IGE9wmMoSDTiYW0mNCE-wExhZAhkk05gw&oe=6A14818B" alt="विवरण">
                    <p>बच्चों के साथ थोड़ी मस्ती</p>
                </div>

                <div class="gallery-item">
                    <img src="https://scontent.fixr3-4.fna.fbcdn.net/v/t39.30808-6/571583824_24950288161296166_3333090433103577097_n.jpg?stp=cp6_dst-jpg_tt6&_nc_cat=106&ccb=1-7&_nc_sid=833d8c&_nc_ohc=e7UT-9PTDhgQ7kNvwGGqklq&_nc_oc=AdorWoW3lpo7fZaW7VigvuQsqYVhX82cXmtSHxp6M_DEATWt-22cwPsQmj3IZxOvGVeFOIztw5wIbvQsl8GUdyNf&_nc_zt=23&_nc_ht=scontent.fixr3-4.fna&_nc_gid=kEtdLcwKdLXm7GJxE3WZrA&_nc_ss=7b2a8&oh=00_Af6dEv3eC8DYsiXEfxITKtwEkK5yBTfuHaoQbOg4MHlHSw&oe=6A14AE59" alt="मोबाइल लाइब्रेरी">
                    <p>नया डिजिटल पुस्तकालय का उदघाटन</p>
                </div>

                <div class="gallery-item">
                    <img src="https://i.ibb.co/60XnYMwW/Whats-App-Image-2026-05-11-at-11-31-22-PM.jpg" alt="Whats-App-Image-2026-05-11-at-11-31-22-PM">
                    <p>संजय कच्छप बच्चों के साथ लाइब्रेरी में अपना जन्मदिन मनाते हुए</p>
                </div>
            </div>

            <div class="upload-section">
                <h3>📸 गैलरी में अपनी फोटो जोड़ें</h3>
                <div class="upload-controls">
                    <input type="file" id="imageInput" accept="image/*">
                    <input type="text" id="captionInput" placeholder="फोटो के नीचे का नाम/विवरण लिखें">
                    <button class="upload-btn" onclick="uploadUserPhoto()">फोटो अपलोड करें</button>
                </div>
            </div>
        </section>

        <section id="contact">
            <h2 class="section-title">हमसे संपर्क करें</h2>
            <div class="contact-section-grid">
                
                <div class="contact-info-box">
                    <h3>हमारे बारे में (About Us)</h3>
                    <p style="margin-bottom: 20px; font-size: 15px; color:#555; text-align: justify;">
                       मैं कार्तिक कुजूर झारखंड के साहिबगंज जिले से हूँ, यह वेबसाइट झारखंड के सुदूर ग्रामीण और आदिवासी क्षेत्रों में शिक्षा का उजियारा फैलाने वाले "लाइब्रेरी मैन" संजय कच्छप जी के लाइब्रेरी आंदोलन को समर्पित है। हमारा उद्देश्य उनकी इस मुहिम को जन-जन तक पहुंचाना और अधिक से अधिक छात्रों को जोड़ना है।
                    </p>
                    
                    <h3>संपर्क विवरण (Contact Details)</h3>
                    <div class="contact-details">
                        <p><strong>📍 मुख्य केंद्र:</strong>  साहिबगंज , झारखंड, भारत</p>
                        <p><strong>✉️ ईमेल:</strong> kartikkujur98256@gmail.com</p>
                        <p><strong>🌐 वेबसाइट:</strong> www.jharkhandlibraryman.org</p>
                        <p><strong>🕒 समय:</strong> सुबह 09:00 बजे से शाम 06:00 बजे तक (रविवार भी चालू)</p>
                    </div>
                </div>

                <div class="contact-form-box">
                    <h3>संदेश या सुझाव भेजें</h3>
                    <form action="#" method="POST" onsubmit="alert('आपका संदेश सुरक्षित रूप से प्राप्त हो गया है! धन्यवाद।'); return false;">
                        <div class="form-group">
                            <label for="name">आपका नाम</label>
                            <input type="text" id="name" placeholder="अपना नाम लिखें" required>
                        </div>
                        <div class="form-group">
                            <label for="email">ईमेल आईडी</label>
                            <input type="email" id="email" placeholder="अपनी ईमेल आईडी लिखें" required>
                        </div>
                        <div class="form-group">
                            <label for="message">आपका संदेश / किताबें दान करने का विवरण</label>
                            <textarea id="message" rows="4" placeholder="यहाँ अपना संदेश या सुझाव लिखें..." required></textarea>
                        </div>
                        <button type="submit" class="submit-btn">संदेश भेजें</button>
                    </form>
                </div>

            </div>
        </section>

    </div>

    <footer>
        <div class="footer-grid">
            <div class="footer-about">
                <h3>लाइब्रेरी आंदोलन</h3>
                <p>संजय कच्छप जी की यह पहल आज झारखंड के 40 से अधिक सुदूर और नक्सल प्रभावित गांवों में बच्चों के भविष्य को संवारने का कार्य कर रही है। 'चैन सिस्टम' के जरिए आज सैकड़ों युवा आत्मनिर्भर बन रहे हैं।</p>
            </div>
            <div class="footer-links">
                <h3>त्वरित लिंक्स (Quick Links)</h3>
                <ul>
                    <li><a href="#about">» संजय जी का जीवन परिचय</a></li>
                    <li><a href="#movement">» आंदोलन की विशेषताएं</a></li>
                    <li><a href="#achievements">» राष्ट्रीय उपलब्धियां</a></li>
                    <li><a href="#gallery">» फोटो गैलरी देखें</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-bottom">
            <p>© 2026 | संजय कच्छप - लाइब्रेरी मैन ऑफ झारखंड के जीवन पर आधारित एक आदरपूर्ण प्रस्तुति।</p>
        </div>
    </footer>

    <script>
        window.onload = function() {
            loadSavedPhotos();
        };

        function uploadUserPhoto() {
            const imageInput = document.getElementById('imageInput');
            const captionInput = document.getElementById('captionInput');

            if (imageInput.files && imageInput.files[0]) {
                const file = imageInput.files[0];
                const reader = new FileReader();

                reader.onload = function(e) {
                    const imageSrc = e.target.result;
                    const captionText = captionInput.value.trim() || "यूज़र द्वारा अपलोड की गई तस्वीर";

                    createGalleryItem(imageSrc, captionText);
                    savePhotoToLocalStorage(imageSrc, captionText);

                    imageInput.value = '';
                    captionInput.value = '';
                    alert('फोटो सफलतापूर्वक गैलरी में जोड़ दी गई है!');
                };

                reader.readAsDataURL(file);
            } else {
                alert('कृपया पहले अपने कंप्यूटर या मोबाइल से एक फोटो चुनें!');
            }
        }

        function createGalleryItem(src, caption) {
            const galleryGrid = document.getElementById('galleryGrid');
            
            const itemDiv = document.createElement('div');
            itemDiv.className = 'gallery-item';

            const img = document.createElement('img');
            img.src = src;
            img.alt = caption;

            const p = document.createElement('p');
            p.textContent = caption;

            itemDiv.appendChild(img);
            itemDiv.appendChild(p);
            galleryGrid.appendChild(itemDiv);
        }

        function savePhotoToLocalStorage(src, caption) {
            let photos = JSON.parse(localStorage.getItem('userUploadedPhotos')) || [];
            photos.push({ src: src, caption: caption });
            localStorage.setItem('userUploadedPhotos', JSON.stringify(photos));
        }

        function loadSavedPhotos() {
            let photos = JSON.parse(localStorage.getItem('userUploadedPhotos')) || [];
            photos.forEach(photo => {
                createGalleryItem(photo.src, photo.caption);
            });
        }
    </script>

</body>
</html>
