ode (Python)

# Create the complete HTML file for IKEA Geopolitical Assessment

html_content = '''<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Geopolitical Assessment for IKEA | 1-5 Years</title>
    <meta name="description" content="Strategic geopolitical assessment for IKEA Retail (Ingka Group) and Inter IKEA, focusing on medium-term risks and opportunities.">
    <meta name="keywords" content="IKEA, Ingka Group, Inter IKEA, Geopolitical Assessment, Strategic Planning">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #fff;
            padding: 20px;
        }
        
        .container {
            max-width: 960px;
            margin: 0 auto;
        }
        
        h1 {
            color: #0058ab;
            font-size: 2.2em;
            margin-bottom: 10px;
            text-align: center;
            padding-bottom: 15px;
            border-bottom: 3px solid #ffcc00;
        }
        
        .subtitle {
            text-align: center;
            color: #666;
            margin-bottom: 40px;
            font-size: 0.95em;
        }
        
        .executive-summary {
            background-color: #f5f5f5;
            padding: 30px;
            margin-bottom: 40px;
            border-left: 5px solid #0058ab;
        }
        
        .executive-summary h2 {
            color: #0058ab;
            font-size: 1.6em;
            margin-bottom: 20px;
        }
        
        .executive-summary h3 {
            color: #333;
            font-size: 1.2em;
            margin-top: 20px;
            margin-bottom: 10px;
        }
        
        .executive-summary ul {
            margin-left: 20px;
            margin-bottom: 15px;
        }
        
        .executive-summary li {
            margin-bottom: 8px;
        }
        
        .recommendation {
            background-color: #fff3cd;
            padding: 15px;
            margin-top: 20px;
            border-left: 4px solid #ffcc00;
            font-weight: bold;
        }
        
        .section {
            margin-bottom: 20px;
            border: 1px solid #ddd;
            background-color: #fff;
        }
        
        .section-header {
            padding: 20px;
            cursor: pointer;
            background-color: #f9f9f9;
            border-bottom: 1px solid #ddd;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: background-color 0.2s;
        }
        
        .section-header:hover {
            background-color: #f0f0f0;
        }
        
        .section-header h2 {
            color: #0058ab;
            font-size: 1.4em;
            margin: 0;
        }
        
        .toggle-icon {
            font-size: 1.5em;
            color: #0058ab;
            font-weight: bold;
        }
        
        .section-content {
            padding: 25px;
            display: none;
        }
        
        .section-content.active {
            display: block;
        }
        
        .subsection {
            margin-bottom: 25px;
        }
        
        .subsection h3 {
            color: #0058ab;
            font-size: 1.2em;
            margin-bottom: 10px;
        }
        
        .subsection h4 {
            color: #333;
            font-size: 1.05em;
            margin-top: 15px;
            margin-bottom: 8px;
        }
        
        ul {
            margin-left: 25px;
            margin-bottom: 15px;
        }
        
        li {
            margin-bottom: 6px;
        }
        
        .region-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-top: 15px;
        }
        
        .region-box {
            background-color: #f9f9f9;
            padding: 15px;
            border-left: 3px solid #0058ab;
        }
        
        .region-box h4 {
            color: #0058ab;
            margin-bottom: 10px;
        }
        
        .scenario-box {
            background-color: #f0f7ff;
            padding: 15px;
            margin-bottom: 15px;
            border-left: 3px solid #0058ab;
        }
        
        .scenario-box h4 {
            color: #0058ab;
            margin-bottom: 8px;
        }
        
        .risk-item, .opportunity-item {
            margin-bottom: 12px;
            padding-left: 15px;
        }
        
        strong {
            color: #000;
        }
        
        @media (max-width: 768px) {
            .region-grid {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 1.8em;
            }
            
            .section-header h2 {
                font-size: 1.2em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Geopolitical Assessment for IKEA</h1>
        <div class="subtitle">
            Strategic Outlook for 1-5 Years | Ingka Group (Retail) & Inter IKEA (Supply Chain)
        </div>
        
        <div class="executive-summary">
            <h2>Executive Summary</h2>
            
            <h3>Top Risks (1-5 Years)</h3>
            <ul>
                <li><strong>Economic Volatility & Reduced Consumer Spending:</strong> Inflation and economic uncertainty directly impact discretionary purchases (Ingka) and increase operational costs (Inter IKEA).</li>
                <li><strong>Trade Wars & Tariff Escalation:</strong> Rising protectionism and tariffs on furniture and components increase product costs and complicate sourcing strategies (Inter IKEA).</li>
                <li><strong>Geopolitical Supply Chain Disruptions:</strong> Regional conflicts, sanctions, and political tensions threaten manufacturing hubs and logistics routes (Inter IKEA).</li>
                <li><strong>Regulatory Fragmentation:</strong> Divergent ESG, data privacy, and product standards across markets create compliance burdens for both retail operations (Ingka) and supply chain (Inter IKEA).</li>
            </ul>
            
            <h3>Top Opportunities (1-5 Years)</h3>
            <ul>
                <li><strong>Digital Transformation & Omnichannel Excellence:</strong> Accelerated e-commerce adoption and AI-driven personalization enhance customer experience and operational efficiency (Ingka).</li>
                <li><strong>Circular Economy Leadership:</strong> Growing consumer demand for sustainable, repairable products and buy-back/rental services creates competitive advantage (Ingka & Inter IKEA).</li>
                <li><strong>Supply Chain Diversification:</strong> Strategic shifts to nearshoring and multi-regional sourcing reduce geopolitical exposure and improve resilience (Inter IKEA).</li>
                <li><strong>Emerging Market Expansion:</strong> Strong growth potential in Asia, Latin America, and Africa with rising middle-class consumers seeking affordable home solutions (Ingka).</li>
            </ul>
            
            <div class="recommendation">
                <strong>Strategic Recommendation:</strong> IKEA must prioritize agility, supply chain diversification, digital innovation, and sustainability leadership to navigate geopolitical volatility and capitalize on evolving consumer demands over the next 1-5 years.
            </div>
        </div>
        
        <!-- Global Geopolitical Overview -->
        <div class="section">
            <div class="section-header" onclick="toggleSection('global')">
                <h2>🌍 Global Geopolitical Overview</h2>
                <span class="toggle-icon" id="icon-global">+</span>
            </div>
            <div class="section-content" id="content-global">
                <p>Key global trends shaping the 1-5 year outlook:</p>
                <ul>
                    <li><strong>Geopolitical Fragmentation:</strong> Shift from globalization to regionalization with competing economic blocs (US-China rivalry, EU autonomy). Impact: Trade barriers, tariffs, and "friendshoring" pressures.</li>
                    <li><strong>Economic Uncertainty:</strong> Persistent inflation, interest rate volatility, and uneven recovery impact consumer confidence and purchasing power.</li>
                    <li><strong>Climate & Sustainability Regulation:</strong> Accelerating ESG mandates (EU Green Deal, carbon border adjustments) require circular practices and transparent reporting.</li>
                    <li><strong>Technology & Data Governance:</strong> AI advancement alongside stricter data privacy laws (GDPR, regional variants) create both opportunities and compliance risks.</li>
                    <li><strong>Social & Political Instability:</strong> Rising inequality and political polarization influence consumer behavior and brand perception.</li>
                    <li><strong>Energy Transition:</strong> Volatile energy prices and shift to renewables impact operational costs and logistics.</li>
                </ul>
            </div>
        </div>
        
        <!-- Regional Analyses -->
        <div class="section">
            <div class="section-header" onclick="toggleSection('regions')">
                <h2>🗺️ Regional Geopolitical Landscapes</h2>
                <span class="toggle-icon" id="icon-regions">+</span>
            </div>
            <div class="section-content" id="content-regions">
                <div class="region-grid">
                    <div class="region-box">
                        <h4>Europe (EU, UK, Nordics, Eastern Europe)</h4>
                        <ul>
                            <li><strong>Ingka:</strong> Core market with high sustainability awareness; regulatory complexity around ESG and data; potential for circular retail leadership.</li>
                            <li><strong>Inter IKEA:</strong> Energy cost pressures; Eastern Europe manufacturing at risk from geopolitical tensions; need for supply chain resilience.</li>
                        </ul>
                    </div>
                    
                    <div class="region-box">
                        <h4>North America (USA, Canada, Mexico)</h4>
                        <ul>
                            <li><strong>Ingka:</strong> Large market with e-commerce growth; political polarization affects consumer sentiment; opportunity for smaller format stores.</li>
                            <li><strong>Inter IKEA:</strong> Tariff risks on imports; nearshoring opportunities in Mexico; USMCA trade dynamics.</li>
                        </ul>
                    </div>
                    
                    <div class="region-box">
                        <h4>Asia (China, India, Southeast Asia)</h4>
                        <ul>
                            <li><strong>Ingka:</strong> High-growth markets with digital-first consumers; need for localization and cultural sensitivity in brand messaging.</li>
                            <li><strong>Inter IKEA:</strong> Critical manufacturing hub facing US-China tensions; opportunity to diversify to Vietnam, India; complex regulatory environments.</li>
                        </ul>
                    </div>
                    
                    <div class="region-box">
                        <h4>Emerging Markets (Latin America, Africa)</h4>
                        <ul>
                            <li><strong>Ingka:</strong> Long-term growth potential; requires affordability focus and adaptable retail formats; infrastructure challenges.</li>
                            <li><strong>Inter IKEA:</strong> Sourcing opportunities for raw materials; logistics and political instability risks; currency volatility.</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Impact on Ingka Group -->
        <div class="section">
            <div class="section-header" onclick="toggleSection('ingka')">
                <h2>🏪 Impact on Ingka Group (Retail Operations)</h2>
                <span class="toggle-icon" id="icon-ingka">+</span>
            </div>
            <div class="section-content" id="content-ingka">
                <div class="subsection">
                    <h3>Consumer Behavior & Demand</h3>
                    <h4>Risks:</h4>
                    <ul>
                        <li>Economic downturns reduce discretionary spending on furniture</li>
                        <li>Shift towards essential purchases and delayed buying decisions</li>
                    </ul>
                    <h4>Opportunities:</h4>
                    <ul>
                        <li>Emphasize value proposition and affordability</li>
                        <li>Expand durable, repairable product lines and circular services (buy-back, repair)</li>
                    </ul>
                </div>
                
                <div class="subsection">
                    <h3>Market Access & Operations</h3>
                    <h4>Risks:</h4>
                    <ul>
                        <li>Potential market exit pressures due to sanctions or political tensions</li>
                        <li>Increased operational costs (energy, labor, rent)</li>
                    </ul>
                    <h4>Opportunities:</h4>
                    <ul>
                        <li>Flexible retail formats (city stores, planning studios, pick-up points)</li>
                        <li>Market expansion in high-growth emerging economies</li>
                    </ul>
                </div>
                
                <div class="subsection">
                    <h3>Digital Transformation</h3>
                    <h4>Opportunities:</h4>
                    <ul>
                        <li>Enhanced omnichannel experience with AI-driven personalization</li>
                        <li>Improved inventory management and customer insights through data analytics</li>
                        <li>Expansion of e-commerce and last-mile delivery capabilities</li>
                    </ul>
                    <h4>Risks:</h4>
                    <ul>
                        <li>Cybersecurity threats and data privacy compliance costs</li>
                        <li>Fragmented data regulations across markets (GDPR, CCPA, etc.)</li>
                    </ul>
                </div>
                
                <div class="subsection">
                    <h3>Brand & Reputation</h3>
                    <h4>Risks:</h4>
                    <ul>
                        <li>Association with controversial suppliers or geopolitical events</li>
                        <li>Failure to meet consumer expectations on sustainability and ethics</li>
                    </ul>
                    <h4>Opportunities:</h4>
                    <ul>
                        <li>Strengthen sustainability leadership as core brand differentiator</li>
                        <li>Deep local community engagement to build trust</li>
                    </ul>
                </div>
                
                <div class="subsection">
                    <h3>Regulatory Compliance</h3>
                    <h4>Risks:</h4>
                    <ul>
                        <li>Diverse and evolving ESG, consumer protection, and data privacy laws</li>
                        <li>Costs of compliance across multiple jurisdictions</li>
                    </ul>
                    <h4>Opportunities:</h4>
                    <ul>
                        <li>Proactive compliance
