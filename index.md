 <!-- Key Risks Detailed -->
        <div class="collapsible-box">
            <div class="collapsible-header" onclick="toggleSection(this)">
                <div class="header-content">
                    <h2>Key Risks (Detailed)</h2>
                    <p class="summary-text">Critical risks separated by entity requiring immediate attention and mitigation strategies.</p>
                    <div class="tags"><span class="tag">#RiskManagement</span></div>
                </div>
                <button class="toggle-btn">+</button>
            </div>
            <div class="deep-dive-content">
                <h3><span class="entity-tag tag-ingka">Ingka Group Risks</span></h3>
                <ul>
                    <li><strong>Consumer Spending Decline:</strong> Economic downturns directly reduce furniture purchases.</li>
                    <li><strong>Market Access Restrictions:</strong> Political decisions forcing store closures or operational limits.</li>
                    <li><strong>Data Privacy Violations:</strong> Non-compliance with GDPR, CCPA, or emerging regulations leading to fines.</li>
                    <li><strong>Brand Perception Crisis:</strong> Association with controversial stances triggering boycotts.</li>
                </ul>
                <h3><span class="entity-tag tag-inter">Inter IKEA Risks</span></h3>
                <ul>
                    <li><strong>Tariff Escalation:</strong> Sharp increases in import duties on furniture and components.</li>
                    <li><strong>Supply Chain Disruptions:</strong> Geopolitical conflicts or climate events interrupting production.</li>
                    <li><strong>Single-Source Dependency:</strong> Over-reliance on specific countries creating vulnerability.</li>
                    <li><strong>Logistics Bottlenecks:</strong> Port congestion or shipping route closures delaying deliveries.</li>
                </ul>
            </div>
        </div>

        <!-- Key Opportunities Detailed -->
        <div class="collapsible-box">
            <div class="collapsible-header" onclick="toggleSection(this)">
                <div class="header-content">
                    <h2>Key Opportunities (Detailed)</h2>
                    <p class="summary-text">Strategic opportunities across retail and supply operations that can create competitive advantage.</p>
                    <div class="tags"><span class="tag">#Growth</span><span class="tag">#Innovation</span></div>
                </div>
                <button class="toggle-btn">+</button>
            </div>
            <div class="deep-dive-content">
                <h3><span class="entity-tag tag-ingka">Ingka Group Opportunities</span></h3>
                <ul>
                    <li><strong>Circular Retail Leadership:</strong> Expanding buy-back and repair services to meet sustainability demand.</li>
                    <li><strong>Digital Customer Experience:</strong> AI-driven personalization and seamless omnichannel integration.</li>
                    <li><strong>Emerging Market Expansion:</strong> Capturing growth in India and Southeast Asia with localized strategies.</li>
                    <li><strong>Flexible Retail Formats:</strong> Smaller urban stores reducing costs and increasing accessibility.</li>
                </ul>
                <h3><span class="entity-tag tag-inter">Inter IKEA Opportunities</span></h3>
                <ul>
                    <li><strong>Supply Chain Diversification:</strong> Multi-region sourcing reducing geopolitical risk.</li>
                    <li><strong>Nearshoring & Friendshoring:</strong> Bringing production closer to key markets.</li>
                    <li><strong>Sustainable Supply Chains:</strong> Investment in renewable materials and green logistics as a differentiator.</li>
                    <li><strong>Digital Supply Chain:</strong> AI-driven forecasting and real-time visibility improving efficiency.</li>
                </ul>
            </div>
        </div>

        <!-- Strategic Recommendations -->
        <div class="collapsible-box">
            <div class="collapsible-header" onclick="toggleSection(this)">
                <div class="header-content">
                    <h2>Strategic Recommendations</h2>
                    <p class="summary-text">Actionable steps for both Ingka Group and Inter IKEA to navigate challenges and capitalize on opportunities.</p>
                    <div class="tags"><span class="tag">#ActionPlan</span></div>
                </div>
                <button class="toggle-btn">+</button>
            </div>
            <div class="deep-dive-content">
                <h3><span class="entity-tag tag-ingka">Recommendations for Ingka Group</span></h3>
                <ul>
                    <li><strong>Accelerate Circular Retail:</strong> Expand buy-back and repair services across all markets.</li>
                    <li><strong>Invest in Digital Infrastructure:</strong> Enhance e-commerce platforms and AI-driven personalization.</li>
                    <li><strong>Strengthen Data Governance:</strong> Build robust compliance frameworks for GDPR, CCPA, etc.</li>
                    <li><strong>Localize Market Strategies:</strong> Empower regional teams to adapt offerings to local conditions.</li>
                </ul>
                <h3><span class="entity-tag tag-inter">Recommendations for Inter IKEA</span></h3>
                <ul>
                    <li><strong>Diversify Supply Base Urgently:</strong> Implement "China+1" strategy; invest in Vietnam, India, Mexico.</li>
                    <li><strong>Build Regional Supply Hubs:</strong> Create self-sufficient supply ecosystems in Americas, Europe, and Asia.</li>
                    <li><strong>Enhance Supply Chain Visibility:</strong> Deploy AI for real-time tracking and predictive risk management.</li>
                    <li><strong>Scenario Planning & Stress Testing:</strong> Regularly test supply chain resilience against geopolitical shocks.</li>
                </ul>
            </div>
        </div>

        <!-- Conclusion -->
        <div class="collapsible-box">
            <div class="collapsible-header" onclick="toggleSection(this)">
                <div class="header-content">
                    <h2>Conclusion & Outlook (1-5 Years)</h2>
                    <p class="summary-text">Final thoughts on navigating the geopolitical landscape for sustained success.</p>
                </div>
                <button class="toggle-btn">+</button>
            </div>
            <div class="deep-dive-content">
                <p>The geopolitical landscape over the next 1-5 years will be characterized by <strong>economic volatility, trade fragmentation, and accelerated sustainability demands</strong>. For IKEA, this environment presents both challenges and transformative opportunities.</p>
                <p><strong>Ingka Group</strong> must navigate reduced consumer spending while seizing the opportunity to lead in circular retail. <strong>Inter IKEA</strong> faces urgent pressure to diversify supply chains while managing rising costs.</p>
                <p>By aligning on sustainability, leveraging digital transformation, and maintaining agility, IKEA can emerge stronger and more resilient. Proactive adaptation to these geopolitical realities will determine IKEA's competitive position for the remainder of the decade.</p>
            </div>
        </div>

    </div> <!-- Closing container div -->

    <!-- JAVASCRIPT FOR TOGGLE FUNCTIONALITY -->
    <script>
        function toggleSection(headerElement) {
            const deepDiveContent = headerElement.nextElementSibling;
            const toggleBtn = headerElement.querySelector('.toggle-btn');

            if (deepDiveContent.classList.contains('active')) {
                deepDiveContent.classList.remove('active');
                toggleBtn.textContent = '+';
            } else {
                deepDiveContent.classList.add('active');
                toggleBtn.textContent = '−';
            }
        }
    </script>

</body>
</html>
