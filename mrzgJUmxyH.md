<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="/css/markdown.css">
<script>(function(){try{var t=localStorage.getItem('brewpage-theme');if(t!=='light'&&t!=='dark'){t=(window.matchMedia&&window.matchMedia('(prefers-color-scheme: light)').matches)?'light':'dark';}document.documentElement.setAttribute('data-theme',t);}catch(e){document.documentElement.setAttribute('data-theme','dark');}})();</script>
</head>
<body class="markdown-body">
<pre><code class="language-html">&lt;!DOCTYPE html&gt;
&lt;html lang=&quot;id&quot;&gt;
&lt;head&gt;
    &lt;meta charset=&quot;UTF-8&quot;&gt;
    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;
    &lt;title&gt;Rumah Subsidi Pesona Sambi Residence&lt;/title&gt;
    &lt;link rel=&quot;preconnect&quot; href=&quot;https://fonts.googleapis.com&quot;&gt;
    &lt;link rel=&quot;preconnect&quot; href=&quot;https://fonts.gstatic.com&quot; crossorigin&gt;
    &lt;link href=&quot;https://fonts.googleapis.com/css2?family=Merriweather:wght@700&amp;family=Roboto:wght@400;500;700&amp;display=swap&quot; rel=&quot;stylesheet&quot;&gt;
    &lt;style&gt;
        /* Base Reset &amp; Variables */
        :root {
            --primary-green: #108020; /* Extracted background color */
            --text-light: #ffffff;
            --text-dark: #333333;
            --font-serif: 'Merriweather', serif;
            --font-sans: 'Roboto', sans-serif;
            --wa-green: #25D366;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background-color: #f0f0f0; /* Outer background to show flyer shape */
            font-family: var(--font-sans);
            display: flex;
            justify-content: center;
            padding: 20px;
        }

        /* Main Container - Simulating Flyer aspect ratio */
        .flyer-container {
            background-color: var(--primary-green);
            color: var(--text-light);
            max-width: 600px; /* Mobile/Flyer width */
            width: 100%;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            padding-bottom: 30px;
        }

        /* --- Header Section --- */
        .header {
            text-align: center;
            padding: 30px 20px 20px;
        }

        .logo-container {
            background-color: white;
            display: inline-block;
            padding: 5px;
            margin-bottom: 15px;
            width: 80px;
            height: 80px;
        }

        .logo-placeholder {
            width: 100%;
            height: 100%;
            object-fit: contain;
            /* Simple placeholder styling for the logo */
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--primary-green);
            font-size: 10px;
            font-weight: bold;
            text-align: center;
            border: 2px solid #d4af37; /* Gold-ish border mimicking logo */
        }

        .header h1 {
            font-family: var(--font-serif);
            font-size: 32px;
            font-weight: 700;
            letter-spacing: 1px;
            margin-bottom: 5px;
            line-height: 1.2;
        }

        .header h2 {
            font-family: var(--font-serif);
            font-size: 26px;
            font-weight: 700;
            letter-spacing: 0.5px;
            line-height: 1.2;
        }

        /* --- Features Section --- */
        .features-section {
            padding: 0 25px;
            margin-bottom: 25px;
        }

        .features-box {
            border: 2px solid white;
            border-radius: 20px;
            padding: 20px;
        }

        .features-box h3 {
            text-align: center;
            font-size: 20px;
            font-weight: 500;
            margin-bottom: 15px;
        }

        .features-grid {
            display: flex;
            justify-content: space-between;
            gap: 15px;
        }

        .features-list {
            list-style: none;
            width: 50%;
        }

        .features-list li {
            position: relative;
            padding-left: 15px;
            margin-bottom: 10px;
            font-size: 16px;
            line-height: 1.4;
        }

        /* Custom Bullet Point */
        .features-list li::before {
            content: '';
            position: absolute;
            left: 0;
            top: 7px;
            width: 6px;
            height: 6px;
            background-color: white;
            border-radius: 50%;
        }

        /* --- Gallery Section --- */
        .gallery-section {
            display: flex;
            flex-direction: column;
            margin-bottom: 20px;
        }

        .gallery-main-img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            display: block;
        }

        .gallery-bottom-row {
            display: flex;
            width: 100%;
        }

        .gallery-half-img-container {
            width: 50%;
            position: relative;
        }

        .gallery-half-img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            display: block;
        }

        /* Promo Overlay */
        .location-tag {
            position: absolute;
            top: 5px;
            right: 10px;
            font-size: 10px;
            color: white;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.8);
            display: flex;
            align-items: center;
            gap: 3px;
        }

        .promo-overlay {
            position: absolute;
            bottom: 15px;
            left: 10px;
            right: 10px;
            background-color: rgba(255, 255, 255, 0.9);
            color: var(--text-dark);
            padding: 10px;
            border-radius: 8px;
            font-size: 12px;
        }

        .promo-overlay h4 {
            font-size: 13px;
            font-weight: 700;
            margin-bottom: 8px;
            line-height: 1.2;
        }

        .promo-list {
            list-style: none;
        }

        .promo-list li {
            margin-bottom: 5px;
            display: flex;
            align-items: flex-start;
            gap: 5px;
            font-size: 11px;
        }
        
        .check-icon {
            color: #4CAF50;
            font-size: 12px;
        }

        /* --- Footer Section --- */
        .footer-section {
            display: flex;
            justify-content: space-between;
            align-items: flex-end; /* Align to bottom */
            padding: 0 25px;
            margin-top: 10px;
        }

        /* Profile Block */
        .profile-block {
            display: flex;
            flex-direction: column;
            align-items: center;
            width: 25%;
        }

        .profile-img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 10px;
            border: 2px solid transparent; /* To match spacing visually */
        }

        .profile-name {
            font-weight: 700;
            font-size: 16px;
            text-decoration: underline;
            margin-bottom: 2px;
            text-align: center;
        }

        .profile-title {
            font-size: 14px;
            text-align: center;
        }

        /* Contact Center Block */
        .contact-block {
            display: flex;
            flex-direction: column;
            align-items: center;
            width: 50%;
            text-align: center;
        }

        .btn-hubungi {
            background-color: white;
            color: var(--primary-green);
            padding: 8px 30px;
            border-radius: 20px;
            font-weight: 700;
            font-size: 20px;
            text-decoration: none;
            margin-bottom: 10px;
            display: inline-block;
        }

        .phone-number {
            font-size: 22px;
            font-weight: 700;
            text-decoration: underline;
            margin-bottom: 10px;
        }

        .website-link {
            font-size: 14px;
            color: white;
            text-decoration: underline;
            margin-bottom: 3px;
        }

        .address-text {
            font-size: 14px;
            text-decoration: underline;
        }

        /* WhatsApp Block */
        .wa-block {
            display: flex;
            flex-direction: column;
            align-items: center;
            width: 25%;
        }

        .wa-icon {
            width: 60px;
            height: 60px;
            background-color: var(--wa-green);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 5px;
            border: 3px solid white;
        }
        
        .wa-icon svg {
            width: 35px;
            height: 35px;
            fill: white;
        }

        .wa-text {
            font-size: 14px;
            text-align: center;
            line-height: 1.2;
        }
        
        .wa-text span {
            display: block;
            text-decoration: underline;
        }

        /* Responsive Adjustments for very small screens */
        @media (max-width: 480px) {
            .header h1 { font-size: 26px; }
            .header h2 { font-size: 20px; }
            .features-box { padding: 15px 10px; }
            .features-grid { flex-direction: column; gap: 0; }
            .features-list { width: 100%; }
            
            .footer-section {
                flex-direction: column;
                align-items: center;
                gap: 20px;
            }
            .profile-block, .contact-block, .wa-block {
                width: 100%;
            }
        }
    &lt;/style&gt;
&lt;/head&gt;
&lt;body&gt;

&lt;div class=&quot;flyer-container&quot;&gt;
    
    &lt;!-- Header Section --&gt;
    &lt;div class=&quot;header&quot;&gt;
        &lt;div class=&quot;logo-container&quot;&gt;
            &lt;!-- Placeholder for actual logo image --&gt;
            &lt;div class=&quot;logo-placeholder&quot;&gt;
                &lt;img src=&quot;https://placehold.co/80x80/ffffff/d4af37?text=MS+PROPERTI&quot; alt=&quot;Logo MS Properti&quot; style=&quot;width:100%; height:100%;&quot;&gt;
            &lt;/div&gt;
        &lt;/div&gt;
        &lt;h1&gt;RUMAH SUBSIDI&lt;/h1&gt;
        &lt;h2&gt;PESONA SAMBI RESIDENCE&lt;/h2&gt;
    &lt;/div&gt;

    &lt;!-- Features Section --&gt;
    &lt;div class=&quot;features-section&quot;&gt;
        &lt;div class=&quot;features-box&quot;&gt;
            &lt;h3&gt;Apa yang anda dapat ?&lt;/h3&gt;
            &lt;div class=&quot;features-grid&quot;&gt;
                &lt;ul class=&quot;features-list&quot;&gt;
                    &lt;li&gt;Tanah 6 x 10 m&lt;/li&gt;
                    &lt;li&gt;Rumah 30 m2&lt;/li&gt;
                    &lt;li&gt;Carport&lt;/li&gt;
                    &lt;li&gt;Halaman Belakang&lt;/li&gt;
                    &lt;li&gt;Bebas Desain +&lt;br&gt;Konsultasi Arsitek&lt;/li&gt;
                &lt;/ul&gt;
                &lt;ul class=&quot;features-list&quot;&gt;
                    &lt;li&gt;Sertifikat di Lokasi&lt;/li&gt;
                    &lt;li&gt;2 Ruang Tidur&lt;/li&gt;
                    &lt;li&gt;1 Kamar Mandi&lt;/li&gt;
                    &lt;li&gt;Garansi 3 Bulan&lt;/li&gt;
                    &lt;li&gt;Dibantu AKAD&lt;/li&gt;
                    &lt;li&gt;Design Bebas&lt;/li&gt;
                &lt;/ul&gt;
            &lt;/div&gt;
        &lt;/div&gt;
    &lt;/div&gt;

    &lt;!-- Gallery Section --&gt;
    &lt;div class=&quot;gallery-section&quot;&gt;
        &lt;!-- Main Image Placeholder --&gt;
        &lt;img src=&quot;https://placehold.co/600x300/e0e0e0/666666?text=Exterior+View&quot; alt=&quot;Exterior Rumah&quot; class=&quot;gallery-main-img&quot;&gt;
        
        &lt;div class=&quot;gallery-bottom-row&quot;&gt;
            &lt;!-- Left Image Placeholder --&gt;
            &lt;div class=&quot;gallery-half-img-container&quot;&gt;
                &lt;img src=&quot;https://placehold.co/300x250/d0d0d0/666666?text=Signing+Document&quot; alt=&quot;Proses Akad&quot; class=&quot;gallery-half-img&quot;&gt;
            &lt;/div&gt;
            
            &lt;!-- Right Image with Overlay Placeholder --&gt;
            &lt;div class=&quot;gallery-half-img-container&quot;&gt;
                &lt;img src=&quot;https://placehold.co/300x250/c0c0c0/666666?text=House+Detail&quot; alt=&quot;Detail Rumah&quot; class=&quot;gallery-half-img&quot;&gt;
                
                &lt;div class=&quot;location-tag&quot;&gt;
                    &lt;svg width=&quot;10&quot; height=&quot;10&quot; viewBox=&quot;0 0 24 24&quot; fill=&quot;none&quot; stroke=&quot;currentColor&quot; stroke-width=&quot;2&quot; stroke-linecap=&quot;round&quot; stroke-linejoin=&quot;round&quot;&gt;&lt;path d=&quot;M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z&quot;&gt;&lt;/path&gt;&lt;circle cx=&quot;12&quot; cy=&quot;10&quot; r=&quot;3&quot;&gt;&lt;/circle&gt;&lt;/svg&gt;
                    Sambi, Babadan, Boyolali
                &lt;/div&gt;
                
                &lt;div class=&quot;promo-overlay&quot;&gt;
                    &lt;h4&gt;🔥 PROMO SPEKTAKULER:&lt;br&gt;PUNYA RUMAH JADI MUDAH!&lt;/h4&gt;
                    &lt;ul class=&quot;promo-list&quot;&gt;
                        &lt;li&gt;&lt;span class=&quot;check-icon&quot;&gt;✅&lt;/span&gt; &lt;span&gt;Booking Fee: Hanya &lt;strong&gt;Rp 300.000&lt;/strong&gt;&lt;/span&gt;&lt;/li&gt;
                        &lt;li&gt;&lt;span class=&quot;check-icon&quot;&gt;✅&lt;/span&gt; &lt;span&gt;DP Ringan: Cukup &lt;strong&gt;Rp 1.000.000&lt;/strong&gt; saja!&lt;/span&gt;&lt;/li&gt;
                    &lt;/ul&gt;
                &lt;/div&gt;
            &lt;/div&gt;
        &lt;/div&gt;
    &lt;/div&gt;

    &lt;!-- Footer Section --&gt;
    &lt;div class=&quot;footer-section&quot;&gt;
        &lt;!-- Profile --&gt;
        &lt;div class=&quot;profile-block&quot;&gt;
            &lt;!-- Profile Image Placeholder --&gt;
            &lt;img src=&quot;https://placehold.co/150x150/555555/ffffff?text=Portrait&quot; alt=&quot;Rio Sunaryo&quot; class=&quot;profile-img&quot;&gt;
            &lt;div class=&quot;profile-name&quot;&gt;Rio Sunaryo&lt;/div&gt;
            &lt;div class=&quot;profile-title&quot;&gt;Kepala Marketing&lt;/div&gt;
        &lt;/div&gt;

        &lt;!-- Contact Info --&gt;
        &lt;div class=&quot;contact-block&quot;&gt;
            &lt;a href=&quot;#&quot; class=&quot;btn-hubungi&quot;&gt;HUBUNGI&lt;/a&gt;
            &lt;div class=&quot;phone-number&quot;&gt;0821-3613-8603&lt;/div&gt;
            &lt;a href=&quot;#&quot; class=&quot;website-link&quot;&gt;Kunjungi Website Kami&lt;/a&gt;
            &lt;div class=&quot;address-text&quot;&gt;Sambi, Babadan, Boyolali&lt;/div&gt;
        &lt;/div&gt;

        &lt;!-- WhatsApp CTA --&gt;
        &lt;div class=&quot;wa-block&quot;&gt;
            &lt;div class=&quot;wa-icon&quot;&gt;
                &lt;!-- Simple SVG for WhatsApp icon --&gt;
                &lt;svg viewBox=&quot;0 0 24 24&quot; xmlns=&quot;http://www.w3.org/2000/svg&quot;&gt;
                    &lt;path d=&quot;M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z&quot;/&gt;
                &lt;/svg&gt;
            &lt;/div&gt;
            &lt;div class=&quot;wa-text&quot;&gt;
                Klik
                &lt;span&gt;buat WA&lt;/span&gt;
            &lt;/div&gt;
        &lt;/div&gt;
    &lt;/div&gt;

&lt;/div&gt;

&lt;/body&gt;
&lt;/html&gt;
</code></pre></body>
</html>