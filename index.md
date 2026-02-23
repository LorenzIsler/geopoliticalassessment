# Create the complete HTML file for IKEA Geopolitical Assessment

html_content = '''<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IKEA Geopolitical Assessment 2026-2031</title>
    <meta name="description" content="Comprehensive geopolitical assessment for IKEA (Ingka Group & Inter IKEA), focusing on 1-5 year strategic planning.">
    <meta name="keywords" content="IKEA, Ingka Group, Inter IKEA, Geopolitical Assessment, Retail Strategy, Supply Chain">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Noto IKEA', 'Verdana', Arial, sans-serif;
            line-height: 1.6;
            color: #111;
            background-color: #f5f5f5;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* IKEA Header */
        header {
            background-color: #0058ab;
            color: white;
            padding: 30px 20px;
            text-align: center;
            margin-bottom: 30px;
        }
        
        header h1 {
            font-size: 2.5em;
            font-weight: 700;
            margin-bottom: 10px;
        }
        
        header p {
            font-size: 1.1em;
            opacity: 0.95;
        }
        
        .header-accent {
            height: 6px;
            background-color: #ffcc00;
            margin-top: 20px;
        }
        
        /* Tags */
        .tags {
            margin: 20px 0;
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            justify-content: center;
        }
        
        .tag {
            background-color: #fff;
            color: #0058ab;
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.85em;
            font-weight: 600;
            border: 2px solid #0058ab;
        }
        
        /* Executive Summary Box */
        .executive-summary {
            background: linear-gradient(135deg, #0058ab 0%, #0070d2 100%);
            color: white;
            padding: 30px;
            border-radius: 8px;
            margin-bottom: 40px;
            box-shadow: 0 4px 12px rgba(0,88,171,0.3);
        }
        
        .executive-summary h2 {
            font-size: 2em;
            margin-bottom: 20px;
            border-bottom: 3px solid #ffcc00;
            padding-bottom: 10px;
        }
        
        .executive-summary h3 {
            margin-top: 20px;
            margin-bottom: 10px;
            font-size: 1.3em;
        }
        
        .executive-summary ul {
            margin-left: 20px;
            margin-bottom: 15px;
        }
        
        .executive-summary li {
            margin-bottom: 8px;
        }
        
        .highlight-box {
            background-color: rgba(255, 204, 0, 0.2);
            border-left: 4px solid #ffcc00;
            padding: 15px;
            margin: 20px 0;
            border-radius: 4px;
        }
        
        /* Section Cards */
        .section-card {
            background-color: white;
            border-radius: 8px;
            padding: 25px;
            margin-bottom: 25px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            border-left: 5px solid #0058ab;
        }
        
        .section-card h2 {
            color: #0058ab;
            font-size: 1.8em;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .section-card h3 {
            color: #333;
            font-size: 1.3em;
            margin-top: 20px;
            margin-bottom: 10px;
        }
        
        /* Summary and Deep Dive */
        .summary {
            font-size: 1.05em;
            line-height: 1.8;
            color: #333;
            margin-bottom: 15px;
        }
        
        .deep-dive {
            display: none;
            margin-top: 20px;
            padding-top: 20px;
            border-top: 2px solid #f0f0f0;
        }
        
        .deep-dive.active {
            display: block;
        }
        
        .deep-dive-btn {
            background-color: #0058ab;
            color: white;
            border: none;
            padding: 12px 24px;
            font-size: 1em;
            font-weight: 600;
            border-radius: 25px;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 10px;
        }
        
        .deep-dive-btn:hover {
            background-color: #003d7a;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0,88,171,0.3);
        }
        
        .deep-dive-btn.active {
            background-color: #ffcc00;
            color: #111;
        }
        
        /* Regional Boxes */
        .region-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .region-box {
            background-color: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 6px rgba(0,0,0,0.08);
            border-top: 4px solid #0058ab;
        }
        
        .region-box h3 {
            color: #0058ab;
            margin-bottom: 12px;
            font-size: 1.2em;
        }
        
        /* Two Column Layout */
        .two-column {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-top: 20px;
        }
        
        .column-box {
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: 6px;
            border-left: 4px solid #0058ab;
        }
        
        .column-box.inter-ikea {
            border-left-color: #ffcc00;
        }
        
        .column-box h4 {
            color: #0058ab;
            margin-bottom: 12px;
            font-size: 1.1em;
        }
        
        .column-box.inter-ikea h4 {
            color: #d68000;
        }
        
        /* Lists */
        ul, ol {
            margin-left: 20px;
            margin-bottom: 15px;
        }
        
        li {
            margin-bottom: 8px;
        }
        
        /* Scenario Cards */
        .scenario-card {
            background: linear-gradient(to right, #f5f5f5, white);
            border-left: 5px solid #ffcc00;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 6px;
        }
        
        .scenario-card h3 {
            color: #0058ab;
            margin-bottom: 10px;
        }
        
        /* Risk/Opportunity Boxes */
        .risk-box {
            background-color: #fff5f5;
            border-left: 4px solid #dc3545;
            padding: 15px;
            margin-bottom: 15px;
            border-radius: 4px;
        }
        
        .opportunity-box {
            background-color: #f0f8ff;
            border-left: 4px solid #28a745;
            padding: 15px;
            margin-bottom: 15px;
            border-radius: 4px;
        }
        
        /* Footer */
        footer {
            background-color: #111;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 50px;
        }
        
        .footer-accent {
            height: 6px;
            background-color: #ffcc00;
            margin-bottom: 20px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .two-column {
                grid-template-columns: 1fr;
            }
            
            header h1 {
                font-size: 1.8em;
            }
            
            .region-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>🌍 IKEA Geopolitical Assessment</h1>
        <p>Strategic Outlook 2026-2031 | For the Global Management Board</p>
        <div class="header-accent"></div>
        <div class="tags">
            <span class="tag">#IngkaGroup</span>
            <span class="tag">#InterIKEA</span>
            <span class="tag">#GeopoliticalRisk</span>
            <span class="tag">#RetailStrategy</span>
            <span class="tag">#SupplyChain</span>
            <span class="tag">#1-5Years</span>
        </div>
    </header>

    <div class="container">
        
        <!-- EXECUTIVE SUMMARY -->
        <div class="executive-summary">
            <h2>🚀 Executive Summary</h2>
            <p style="font-size: 1.1em; margin-bottom: 20px;">The global geopolitical landscape over the next 1-5 years presents both significant challenges and strategic opportunities for IKEA. This assessment distinguishes between <strong>Ingka Group (Retail)</strong> and <strong>Inter IKEA (Supply Chain & Trade)</strong> to provide targeted strategic insights.</p>
            
            <div class="highlight-box">
                <strong>KEY INSIGHT:</strong> Economic volatility, regulatory fragmentation, and shifting trade dynamics will require agile, localized strategies while maintaining global brand coherence.
            </div>
            
            <h3>⚠️ Top Risks (2026-2031)</h3>
            <ul>
                <li><strong>Reduced Consumer Spending (Ingka):</strong> Economic downturns and inflation directly impact discretionary home furnishing purchases</li>
                <li><strong>Trade Barriers & Tariffs (Inter IKEA):</strong> Protectionism and geopolitical tensions increase costs and complexity in global sourcing</li>
                <li><strong>Regulatory Compliance Burden:</strong> Divergent ESG, data privacy, and product standards across markets</li>
                <li><strong>Supply Chain Disruptions (Inter IKEA):</strong> Continued volatility in logistics, raw materials, and manufacturing hubs</li>
            </ul>
            
            <h3>✅ Top Opportunities (2026-2031)</h3>
            <ul>
                <li><strong>Digital-First Retail (Ingka):</strong> Accelerated omnichannel innovation and personalized customer experiences</li>
                <li><strong>Sustainability Leadership:</strong> Circular economy models (buy-back, repair) as competitive advantage</li>
                <li><strong>Supply Chain Diversification (Inter IKEA):</strong> Strategic expansion into new manufacturing regions reduces single-point dependencies</li>
                <li><strong>Emerging Market Growth:</strong> Long-term consumer base expansion in Asia, Latin America, and Africa</li>
            </ul>
            
            <div class="highlight-box">
                <strong>STRATEGIC RECOMMENDATION:</strong> Prioritize agility, regional diversification, digital excellence, and unwavering sustainability commitment to navigate the 2026-2031 landscape successfully.
            </div>
        </div>

        <!-- GLOBAL OVERVIEW -->
        <div class="section-card">
            <h2>🌍 Global Geopolitical Overview</h2>
            <div class="summary">
                <p><strong>Summary:</strong> The 2026-2031 period will be characterized by increased fragmentation, economic uncertainty, climate pressures, and technological disruption. Five key trends will shape the operating environment for both Ingka Group and Inter IKEA.</p>
            </div>
            <button class="deep-dive-btn" onclick="toggleDeepDive('global-overview')">📊 Deep Dive</button>
            
            <div id="global-overview" class="deep-dive">
                <h3>1. Geopolitical Fragmentation & Competition</h3>
                <p><strong>Trend:</strong> Shift from hyper-globalization to regionalization, with distinct economic blocs forming (US-aligned, China-aligned, EU-autonomous). US-China rivalry continues to influence trade and technology.</p>
                <p><strong>Impact on Ingka:</strong> Consumer nationalism may influence purchasing decisions; need for culturally sensitive marketing.</p>
                <p><strong>Impact on Inter IKEA:</strong> Tariffs on finished goods, non-tariff barriers, and pressure to "friendshore" supply chains.</p>
                
                <h3>2. Economic Volatility & Consumer Confidence</h3>
                <p><strong>Trend:</strong> Persistent inflation, interest rate fluctuations, and uneven global recovery create economic uncertainty through 2031.</p>
                <p><strong>Impact on Ingka:</strong> Direct impact on discretionary spending; shift toward value, durability, and essential items.</p>
                <p><strong>Impact on Inter IKEA:</strong> Higher operational costs (energy, labor); pressure on margins; volatility in raw material prices.</p>
                
                <h3>3. Climate Change & Regulatory Pressure</h3>
                <p><strong>Trend:</strong> Accelerating climate impacts drive stricter environmental regulations (EU Green Deal expansion, carbon border adjustments, circular economy mandates).</p>
                <p><strong>Impact on Ingka:</strong> New requirements for product labeling, packaging, waste management; opportunity for circular retail leadership.</p>
                <p><strong>Impact on Inter IKEA:</strong> Compliance costs for sustainable materials; potential resource scarcity (timber, metals); green logistics investments.</p>
                
                <h3>4. Technological Disruption & Data Governance</h3>
                <p><strong>Trend:</strong> Rapid AI advancement, e-commerce evolution, and fragmented data privacy regulations (GDPR, CCPA variants globally).</p>
                <p><strong>Impact on Ingka:</strong> Opportunities for AI-driven personalization and operational efficiency; cybersecurity risks; complex data compliance.</p>
                <p><strong>Impact on Inter IKEA:</strong> Smart supply chain management; predictive analytics for demand forecasting; digital twins for logistics.</p>
                
                <h3>5. Social & Political Instability</h3>
                <p><strong>Trend:</strong> Rising inequality, political polarization
