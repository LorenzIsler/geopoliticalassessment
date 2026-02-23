 Create the complete HTML file with IKEA-style design, collapsible sections, and Inter IKEA content

html_content = """<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Geopolitical Assessment for IKEA Retail (Ingka Group)</title>
    <meta name="description" content="Comprehensive geopolitical assessment for IKEA Retail (Ingka Group), focusing on risks, opportunities, and strategic recommendations for global operations, targeting the Management Board.">
    <meta name="keywords" content="IKEA, Ingka Group, Inter IKEA, Retail, Geopolitical Assessment, Risk Management, Strategic Planning, Global Operations, Consumer Behavior, Sustainability, Digital Transformation">
    <meta name="author" content="Geopolitical Analysis Team">

    <!-- Open Graph / Social Media Tags -->
    <meta property="og:title" content="Geopolitical Assessment for IKEA Retail (Ingka Group)">
    <meta property="og:description" content="Comprehensive geopolitical assessment for IKEA Retail (Ingka Group), focusing on risks, opportunities, and strategic recommendations for global operations.">
    <meta property="og:type" content="article">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Noto IKEA', 'Noto Sans', Arial, sans-serif;
            line-height: 1.6;
            background-color: #f5f5f5;
            color: #111;
        }

        .header {
            background: linear-gradient(135deg, #0058ab 0%, #003d82 100%);
            color: white;
            padding: 40px 20px;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .header .subtitle {
            font-size: 1.1em;
            opacity: 0.9;
            margin-bottom: 5px;
        }

        .header .tagline {
            font-size: 0.95em;
            opacity: 0.8;
            font-style: italic;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Tags */
        .tags {
            text-align: center;
            margin: 20px 0;
        }

        .tags span {
            display: inline-block;
            background-color: #ffda1a;
            color: #111;
            padding: 6px 14px;
            border-radius: 20px;
            margin: 4px;
            font-size: 0.85em;
            font-weight: 600;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }

        /* Navigation Box */
        .nav-box {
            background: white;
            border-radius: 8px;
            padding: 25px;
            margin: 30px 0;
            box-shadow: 0 4px 12px rgba(0,0,0,0.08);
            border-top: 4px solid #0058ab;
        }

        .nav-box h2 {
            color: #0058ab;
            margin-bottom: 15px;
            font-size: 1.5em;
        }

        .nav-box ul {
            list-style: none;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 10px;
        }

        .nav-box li a {
            display: block;
            padding: 12px 15px;
            background: #f5f5f5;
            color: #0058ab;
            text-decoration: none;
            border-radius: 4px;
            transition: all 0.3s ease;
            font-weight: 600;
        }

        .nav-box li a:hover {
            background: #0058ab;
            color: white;
            transform: translateX(5px);
        }

        /* Executive Summary - Hero Box */
        .hero-box {
            background: linear-gradient(135deg, #e3f2fd 0%, #bbdefb 100%);
            border-radius: 12px;
            padding: 35px;
            margin: 30px 0;
            box-shadow: 0 6px 20px rgba(0,88,171,0.15);
            border-left: 8px solid #0058ab;
        }

        .hero-box h2 {
            color: #0058ab;
            font-size: 2em;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .hero-box .icon {
            font-size: 1.2em;
        }

        /* Content Boxes */
        .content-box {
            background: white;
            border-radius: 8px;
            padding: 30px;
            margin: 25px 0;
            box-shadow: 0 4px 12px rgba(0,0,0,0.08);
            border-top: 4px solid #0058ab;
        }

        .content-box h2 {
            color: #0058ab;
            font-size: 1.8em;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .content-box h3 {
            color: #333;
            font-size: 1.3em;
            margin-top: 20px;
            margin-bottom: 12px;
            padding-bottom: 8px;
            border-bottom: 2px solid #f5f5f5;
        }

        /* Highlight boxes */
        .highlight-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .highlight-card {
            background: #fff9e6;
            border-left: 5px solid #ffda1a;
            padding: 20px;
            border-radius: 6px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.06);
        }

        .highlight-card.risk {
            background: #ffebee;
            border-left-color: #d32f2f;
        }

        .highlight-card.opportunity {
            background: #e8f5e9;
            border-left-color: #388e3c;
        }

        .highlight-card h4 {
            color: #0058ab;
            font-size: 1.1em;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .highlight-card ul {
            list-style-type: none;
            padding-left: 0;
        }

        .highlight-card li {
            padding: 8px 0;
            padding-left: 20px;
            position: relative;
        }

        .highlight-card li:before {
            content: "▪";
            position: absolute;
            left: 0;
            color: #0058ab;
            font-weight: bold;
        }

        /* Deep Dive Toggle Button */
        .deep-dive-btn {
            background: #0058ab;
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 25px;
            font-size: 1em;
            font-weight: 600;
            cursor: pointer;
            margin: 20px 0;
            transition: all 0.3s ease;
            box-shadow: 0 4px 8px rgba(0,88,171,0.2);
        }

        .deep-dive-btn:hover {
            background: #003d82;
            transform: translateY(-2px);
            box-shadow: 0 6px 12px rgba(0,88,171,0.3);
        }

        .deep-dive-btn:active {
            transform: translateY(0);
        }

        .deep-dive-btn::after {
            content: " ▼";
            font-size: 0.8em;
        }

        .deep-dive-btn.active::after {
            content: " ▲";
        }

        /* Deep Dive Content */
        .deep-dive-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.5s ease;
        }

        .deep-dive-content.active {
            max-height: 5000px;
        }

        /* Regional Cards */
        .region-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .region-card {
            background: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            border-top: 4px solid #ffda1a;
            transition: transform 0.3s ease;
        }

        .region-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 16px rgba(0,0,0,0.15);
        }

        .region-card h3 {
            color: #0058ab;
            margin-top: 0;
            border-bottom: none;
        }

        /* Inter IKEA Label */
        .inter-ikea-label {
            display: inline-block;
            background: #ffda1a;
            color: #111;
            padding: 4px 12px;
            border-radius: 12px;
            font-size: 0.8em;
            font-weight: 700;
            margin-left: 10px;
            vertical-align: middle;
        }

        .ingka-label {
            display: inline-block;
            background: #0058ab;
            color: white;
            padding: 4px 12px;
            border-radius: 12px;
            font-size: 0.8em;
            font-weight: 700;
            margin-left: 10px;
            vertical-align: middle;
        }

        /* Lists */
        ul, ol {
            margin-left: 20px;
            margin-bottom: 15px;
        }

        li {
            margin-bottom: 8px;
        }

        strong {
            color: #0058ab;
            font-weight: 600;
        }

        /* Footer */
        .footer {
            background: #111;
            color: white;
            text-align: center;
            padding: 30px 20px;
            margin-top: 50px;
        }

        .footer p {
            opacity: 0.8;
            font-size: 0.9em;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .header h1 {
                font-size: 1.8em;
            }
            
            .highlight-grid, .region-grid {
                grid-template-columns: 1fr;
            }
        }

        /* Scroll behavior */
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body>

    <div class="header">
        <h1>🌍 Geopolitical Assessment for IKEA</h1>
        <div class="subtitle">Ingka Group Retail Operations & Inter IKEA System</div>
        <div class="tagline">Strategic Insights for the Global Management Board | FY25-FY30</div>
    </div>

    <div class="container">

        <div class="tags">
            <span>#IKEA</span>
            <span>#IngkaGroup</span>
            <span>#InterIKEA</span>
            <span>#Geopolitics</span>
            <span>#Retail</span>
            <span>#SupplyChain</span>
            <span>#Trade</span>
            <span>#Sustainability</span>
            <span>#RiskManagement</span>
            <span>#StrategicPlanning</span>
        </div>

        <!-- Navigation -->
        <div class="nav-box">
            <h2>📋 Quick Navigation</h2>
            <ul>
                <li><a href="#executive-summary">🚀 Executive Summary</a></li>
                <li><a href="#global-overview">🌍 Global Geopolitical Overview</a></li>
                <li><a href="#regional-landscapes">🗺️ Regional Landscapes</a></li>
                <li><a href="#retail-impact">⚙️ Impact on Retail (Ingka)</a></li>
                <li><a href="#supply-impact">📦 Impact on Supply & Trade (Inter IKEA)</a></li>
                <li><a href="#scenarios">🔮 Strategic Scenarios</a></li>
                <li><a href="#risks-opportunities">⚠️ Risks & Opportunities</a></li>
                <li><a href="#recommendations">🎯 Strategic Recommendations</a></li>
            </ul>
        </div>

        <!-- Executive Summary -->
        <div class="hero-box" id="executive-summary">
            <h2><span class="icon">🚀</span> Executive Summary: Key Insights</h2>
            
            <p style="font-size: 1.1em; line-height: 1.8; margin-bottom: 20px;">
                The global geopolitical landscape presents a <strong>complex and evolving environment</strong> for both <strong>Ingka Group's retail operations</strong> <span class="ingka-label">INGKA RETAIL</span> and <strong>Inter IKEA's supply chain, trade, and franchising systems</strong> <span class="inter-ikea-label">INTER IKEA</span>. External forces are increasingly shaping market dynamics, consumer behavior, regulatory frameworks, and global trade flows.
            </p>

            <div class="highlight-grid">
                <div class="highlight-card risk">
                    <h4>🔴 Top Risks</h4>
                    <ul>
                        <li><strong>Reduced Consumer Spending</strong> (Ingka): Economic downturns impacting discretionary purchases</li>
                        <li><strong>Supply Chain Disruptions</strong> (Inter IKEA): Geopolitical tensions, tariffs, and logistics bottlenecks</li>
                        <li><strong>Market Access Restrictions</strong>: Trade barriers and regulatory divergence</li>
                        <li><strong>Brand & Reputation Risks</strong>: Association with controversial suppliers or geopolitical events</li>
                    </ul>
                </div>

                <div class="highlight-card opportunity">
                    <h4>🟢 Key Opportunities</h4>
                    <ul>
                        <li><strong>Digital-First Innovation</strong> (Ingka): Omnichannel excellence and personalization</li>
                        <li><strong>Supply Chain Diversification</strong> (Inter IKEA): Multi-regional sourcing strategies</li>
                        <li><strong>Sustainability Leadership</strong>: Circular economy and ethical practices</li>
                        <li><strong>
