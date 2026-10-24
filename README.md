# Reabetswemodubu.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ThreadCraft | Platform for Fashion Designers & Apparel Creators</title>
    <style>
        /* Modern Reset & Base Typography */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            color: #1a1a1a;
            background-color: #fafafa;
            line-height: 1.6;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        /* Top Announcement / Creator Banner */
        .creator-bar {
            background-color: #0f172a;
            color: #e2e8f0;
            text-align: center;
            padding: 10px;
            font-size: 0.85rem;
            letter-spacing: 0.5px;
        }

        .creator-bar a {
            color: #38bdf8;
            font-weight: 600;
            text-decoration: underline;
        }

        /* Navigation */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 6%;
            background: #ffffff;
            border-bottom: 1px solid #e2e8f0;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 1.6rem;
            font-weight: 800;
            letter-spacing: -0.5px;
            color: #0f172a;
        }

        .logo span {
            color: #6366f1;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 32px;
        }

        nav a {
            font-size: 0.95rem;
            font-weight: 500;
            color: #475569;
            transition: color 0.2s;
        }

        nav a:hover {
            color: #6366f1;
        }

        .nav-actions {
            display: flex;
            align-items: center;
            gap: 16px;
        }

        .btn-link {
            font-size: 0.95rem;
            font-weight: 600;
            color: #475569;
            padding: 10px 16px;
        }

        .btn-primary {
            display: inline-block;
            padding: 10px 22px;
            background: #6366f1;
            color: #ffffff;
            font-size: 0.95rem;
            font-weight: 600;
            border-radius: 8px;
            border: none;
            cursor: pointer;
            transition: background 0.2s, transform 0.1s;
        }

        .btn-primary:hover {
            background: #4f46e5;
        }

        .btn-outline {
            display: inline-block;
            padding: 10px 22px;
            background: transparent;
            color: #0f172a;
            font-size: 0.95rem;
            font-weight: 600;
            border-radius: 8px;
            border: 1px solid #cbd5e1;
            cursor: pointer;
            transition: border-color 0.2s, background 0.2s;
        }

        .btn-outline:hover {
            border-color: #0f172a;
            background: #f1f5f9;
        }

        /* Hero Section */
        .hero {
            display: grid;
            grid-template-columns: 1fr 1fr;
            align-items: center;
            padding: 80px 6%;
            gap: 60px;
            background: linear-gradient(135deg, #f8fafc 0%, #f1f5f9 100%);
        }

        .hero-text h1 {
            font-size: 3.2rem;
            line-height: 1.15;
            font-weight: 800;
            color: #0f172a;
            margin-bottom: 20px;
            letter-spacing: -1px;
        }

        .hero-text p {
            font-size: 1.15rem;
            color: #475569;
            margin-bottom: 32px;
            max-width: 520px;
        }

        .hero-btns {
            display: flex;
            gap: 16px;
        }

        .hero-image {
            position: relative;
        }

        .hero-image img {
            width: 100%;
            height: 480px;
            object-fit: cover;
            border-radius: 16px;
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }

        /* Digital Design Studio Tools Section */
        .features {
            padding: 90px 6%;
            background: #ffffff;
        }

        .section-header {
            text-align: center;
            max-width: 640px;
            margin: 0 auto 60px;
        }

        .section-header h2 {
            font-size: 2.2rem;
            font-weight: 700;
            color: #0f172a;
            margin-bottom: 12px;
            letter-spacing: -0.5px;
        }

        .section-header p {
            color: #64748b;
            font-size: 1.05rem;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 32px;
        }

        .feature-card {
            background: #f8fafc;
            border: 1px solid #e2e8f0;
            border-radius: 12px;
            padding: 32px;
            transition: transform 0.2s, box-shadow 0.2s;
        }

        .feature-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 12px 20px -5px rgba(0, 0, 0, 0.05);
        }

        .feature-icon {
            width: 48px;
            height: 48px;
            background: #e0e7ff;
            color: #6366f1;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.4rem;
            font-weight: bold;
            margin-bottom: 20px;
        }

        .feature-card h3 {
            font-size: 1.25rem;
            color: #0f172a;
            margin-bottom: 10px;
        }

        .feature-card p {
            color: #64748b;
            font-size: 0.95rem;
        }

        /* Showcase / Community Creations */
        .showcase {
            padding: 90px 6%;
            background: #fafafa;
        }

        .showcase-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .creation-card {
            background: #ffffff;
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid #e2e8f0;
        }

        .creation-img {
            width: 100%;
            height: 360px;
            object-fit: cover;
            display: block;
        }

        .creation-info {
            padding: 20px;
        }

        .creation-title {
            font-size: 1.1rem;
            font-weight: 700;
            color: #0f172a;
            margin-bottom: 6px;
        }

        .designer-meta {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-top: 12px;
        }

        .avatar {
            width: 32px;
            height: 32px;
            border-radius: 50%;
            object-fit: cover;
        }

        .designer-name {
            font-size: 0.88rem;
            color: #475569;
            font-weight: 500;
        }

        .tags {
            display: flex;
            gap: 8px;
            margin-top: 12px;
        }

        .tag {
            font-size: 0.75rem;
            background: #f1f5f9;
            color: #475569;
            padding: 4px 10px;
            border-radius: 20px;
            font-weight: 500;
        }

        /* Supply & Fabrics Hub */
        .hub-banner {
            margin: 0 6% 90px;
            background: #0f172a;
            color: #ffffff;
            border-radius: 20px;
            padding: 60px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 40px;
        }

        .hub-content h2 {
            font-size: 2.2rem;
            font-weight: 700;
            margin-bottom: 16px;
        }

        .hub-content p {
            color: #94a3b8;
            font-size: 1.1rem;
            max-width: 560px;
            margin-bottom: 24px;
        }

        /* Footer */
        footer {
            background: #ffffff;
            border-top: 1px solid #e2e8f0;
            padding: 60px 6% 30px;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: 2fr repeat(3, 1fr);
            gap: 40px;
            margin-bottom: 50px;
        }

        .footer-brand p {
            color: #64748b;
            margin-top: 12px;
            max-width: 300px;
            font-size: 0.95rem;
        }

        .footer-col h4 {
            font-size: 0.95rem;
            font-weight: 700;
            color: #0f172a;
            margin-bottom: 18px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .footer-col ul {
            list-style: none;
        }

        .footer-col ul li {
            margin-bottom: 10px;
        }

        .footer-col a {
            color: #64748b;
            font-size: 0.9rem;
            transition: color 0.2s;
        }

        .footer-col a:hover {
            color: #6366f1;
        }

        .copyright {
            text-align: center;
            color: #94a3b8;
            font-size: 0.85rem;
            padding-top: 30px;
            border-top: 1px solid #f1f5f9;
        }

        /* Responsive Breakpoints */
        @media (max-width: 900px) {
            .hero {
                grid-template-columns: 1fr;
                text-align: center;
                padding: 60px 5%;
            }

            .hero-text p {
                margin-left: auto;
                margin-right: auto;
            }

            .hero-btns {
                justify-content: center;
            }

            .hub-banner {
                flex-direction: column;
                text-align: center;
                padding: 40px 24px;
            }

            .footer-grid {
                grid-template-columns: 1fr 1fr;
            }

            nav ul {
                display: none;
            }
        }
    </style>
</head>
<body>

    <!-- Creator Hub Announcement Bar -->
    <div class="creator-bar">
        🎨 <strong>Spring Design Challenge:</strong> Submit your 3D digital patterns by May 15 to win $5,000 in production support. <a href="#">Enter Challenge</a>
    </div>

    <!-- Header Navigation -->
    <header>
        <div class="logo">Thread<span>Craft</span></div>
        <nav>
            <ul>
                <li><a href="#">Design Studio</a></li>
                <li><a href="#">Pattern Library</a></li>
                <li><a href="#">Fabric Sourcing</a></li>
                <li><a href="#">Community Marketplace</a></li>
            </ul>
        </nav>
        <div class="nav-actions">
            <a href="#" class="btn-link">Sign In</a>
            <a href="#" class="btn-primary">Start Designing</a>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-text">
            <h1>Bring Your Apparel Designs From Sketch to Screen.</h1>
            <p>The ultimate platform for fashion creators. Access digital drafting tools, source sustainable fabrics, collaborate with patternmakers, and launch your clothing line.</p>
            <div class="hero-btns">
                <a href="#" class="btn-primary">Launch Studio Tool</a>
                <a href="#" class="btn-outline">Explore Marketplace</a>
            </div>
        </div>
        <div class="hero-image">
            <img src="https://images.unsplash.com/photo-1558769132-cb1aea458c5e?q=80&w=1000&auto=format&fit=crop" alt="Fashion designer working on clothing patterns">
        </div>
    </section>

    <!-- Design Suite / Feature Highlights -->
    <section class="features">
        <div class="section-header">
            <h2>Built for Apparel Creators</h2>
            <p>Everything independent fashion designers, tailors, and garment makers need to streamline their creative process.</p>
        </div>

        <div class="feature-grid">
            <div class="feature-card">
                <div class="feature-icon">📐</div>
                <h3>Digital Pattern Drafting</h3>
                <p>Convert sketches into precise 2D vector patterns or export industry-standard DXF files for cutting.</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon">🧵</div>
                <h3>3D Garment Fitting</h3>
                <p>Visualize fabrics, drape, and sizing on customizable 3D avatars before cutting a single yard of cloth.</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon">🌿</div>
                <h3>Textile & Trim Sourcing</h3>
                <p>Connect directly with verified eco-friendly mills, low-minimum fabric suppliers, and haberdasheries.</p>
            </div>
            <div class="feature-card">
                <div class="feature-icon">🛍️</div>
                <h3>Pattern Marketplace</h3>
                <p>Sell downloadable PDF sewing patterns, tech packs, or design licenses directly to global creators.</p>
            </div>
        </div>
    </section>

    <!-- Designer Showcase / Community Gallery -->
    <section class="showcase">
        <div class="section-header">
            <h2>Trending Designer Creations</h2>
            <p>Explore original clothing concepts, tech packs, and sewing patterns uploaded by community designers.</p>
        </div>

        <div class="showcase-grid">
            <!-- Card 1 -->
            <div class="creation-card">
                <img class="creation-img" src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?q=80&w=800&auto=format&fit=crop" alt="Minimalist Jacket Design">
                <div class="creation-info">
                    <div class="creation-title">Minimalist Sculpted Blazer</div>
                    <div class="tags">
                        <span class="tag">Outerwear</span>
                        <span class="tag">PDF Pattern</span>
                    </div>
                    <div class="designer-meta">
                        <img class="avatar" src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?q=80&w=100&auto=format&fit=crop" alt="Elena Rostova">
                        <span class="designer-name">by Elena Rostova</span>
                    </div>
                </div>
            </div>

            <!-- Card 2 -->
            <div class="creation-card">
                <img class="creation-img" src="https://images.unsplash.com/photo-1509631179647-0177331693ae?q=80&w=800&auto=format&fit=crop" alt="Draped Silk Dress Design">
                <div class="creation-info">
                    <div class="creation-title">Asymmetric Draped Dress</div>
                    <div class="tags">
                        <span class="tag">Eveningwear</span>
                        <span class="tag">3D Render</span>
                    </div>
                    <div class="designer-meta">
                        <img class="avatar" src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?q=80&w=100&auto=format&fit=crop" alt="Marcus Chen">
                        <span class="designer-name">by Marcus Chen</span>
                    </div>
                </div>
            </div>

            <!-- Card 3 -->
            <div class="creation-card">
                <img class="creation-img" src="https://images.unsplash.com/photo-1576995853123-5a10305d93c0?q=80&w=800&auto=format&fit=crop" alt="Upcycled Denim Streetwear">
                <div class="creation-info">
                    <div class="creation-title">Patchwork Utility Overshirt</div>
                    <div class="tags">
                        <span class="tag">Streetwear</span>
                        <span class="tag">Upcycled</span>
                    </div>
                    <div class="designer-meta">
                        <img class="avatar" src="https://images.unsplash.com/photo-1517841905240-472988babdf9?q=80&w=100&auto=format&fit=crop" alt="Amara Okafor">
                        <span class="designer-name">by Amara Okafor</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Manufacturing & Sourcing Banner -->
    <div class="hub-banner">
        <div class="hub-content">
            <h2>Ready to manufacture your capsule collection?</h2>
            <p>Find small-batch apparel manufacturers, ethical seamstresses, and sampling studios that match your brand values.</p>
            <a href="#" class="btn-primary" style="background: #38bdf8; color: #0f172a;">Find Manufacturers</a>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="footer-grid">
            <div class="footer-brand">
                <div class="logo">Thread<span>Craft</span></div>
                <p>Empowering fashion designers, patternmakers, and garment creators worldwide with modern design tools and community.</p>
            </div>
            <div class="footer-col">
                <h4>Design Tools</h4>
                <ul>
                    <li><a href="#">3D Garment Studio</a></li>
                    <li><a href="#">Pattern Generator</a></li>
                    <li><a href="#">Tech Pack Builder</a></li>
                    <li><a href="#">Color Palette Studio</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h4>Marketplace</h4>
                <ul>
                    <li><a href="#">Buy Sewing Patterns</a></li>
                    <li><a href="#">Sell Your Designs</a></li>
                    <li><a href="#">Fabric Directory</a></li>
                    <li><a href="#">Trim & Hardware</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h4>Community</h4>
                <ul>
                    <li><a href="#">Designer Forum</a></li>
                    <li><a href="#">Design Competitions</a></li>
                    <li><a href="#">Manufacturer Match</a></li>
                    <li><a href="#">Creator Blog</a></li>
                </ul>
            </div>
        </div>
        <div class="copyright">
            &copy; 2026 ThreadCraft Inc. Designed for clothing designers worldwide.
        </div>
    </footer>

</body>
</html>
