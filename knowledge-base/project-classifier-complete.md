# 🔍 PROJECT CLASSIFIER - KORE KONTEXT

## PRIMARY FUNCTION
Automatically detect project type, industry, and necessary modules based on user input.

---

## 🎯 TYPE DETECTION PATTERNS

### 🚀 STARTUP/SAAS
**Primary keywords:**
- app, application, platform, saas, software
- startup, venture, mvp, digital product
- users, subscribers, scalable, technology

**Secondary keywords:**
- dashboard, analytics, integration, api
- freemium, subscription, recurring revenue
- user experience, product-market fit

**Modules to activate:**
- ✅ core-project (universal base)
- ✅ development (technical MVP)
- ✅ marketing-digital (user acquisition)
- ✅ sales (B2B if applicable)
- ❌ ecommerce (unless marketplace)

**Generated expert:**
- "Startup Product Manager" 
- "SaaS Growth Lead"
- "Technical Product Manager"

---

### 🛒 ECOMMERCE
**Primary keywords:**
- store, shopify, ecommerce, online store
- products, sell, inventory, catalog
- payments, shipping, fulfillment

**Secondary keywords:**
- conversion, checkout, abandoned cart
- product photography, marketplace
- dropshipping, retail, wholesale

**Modules to activate:**
- ✅ ecommerce (store configuration)
- ✅ marketing-digital (traffic acquisition)
- ✅ content-creative (product content)
- ✅ sales (conversion optimization)
- ❌ development (unless custom features)

**Generated expert:**
- "Ecommerce Growth Specialist"
- "Shopify Store Manager" 
- "Digital Commerce Strategist"

---

### 📱 DIGITAL MARKETING
**Primary keywords:**
- marketing, campaign, content, social media
- ads, advertising, social media, influencer
- brand, awareness, engagement, audience

**Secondary keywords:**
- instagram, facebook, tiktok, youtube
- seo, content marketing, email marketing
- conversion, leads, funnel, analytics

**Modules to activate:**
- ✅ marketing-digital (complete strategy)
- ✅ content-creative (content creation)
- ✅ sales (lead conversion)
- ❌ development (unless landing pages)
- ❌ ecommerce (unless selling products)

**Generated expert:**
- "Digital Marketing Strategist"
- "Content Marketing Manager"
- "Social Media Growth Specialist"

---

### 💻 DEVELOPMENT
**Primary keywords:**
- code, programming, development, software
- website, app, system, technical, programming
- frontend, backend, database, api

**Secondary keywords:**
- react, python, javascript, framework
- architecture, scalability, performance
- testing, deployment, ci/cd, devops

**Modules to activate:**
- ✅ development (complete)
- ✅ documentation (technical docs)
- ✅ core-project (requirements)
- ❌ marketing (unless product launch)
- ❌ sales (unless B2B software)

**Generated expert:**
- "Senior Software Engineer"
- "Technical Lead"
- "Full-Stack Developer"

---

### 🌱 AGTECH
**Primary keywords:**
- agriculture, farm, agricultural, agritech
- sensors, iot, crops, crop, soil
- agricultural technology, precision farming

**Secondary keywords:**
- monitoring, irrigation, livestock
- yield optimization, farm management
- agricultural data, rural, farmers

**Modules to activate:**
- ✅ development (IoT/hardware)
- ✅ marketing-digital (B2B agriculture)
- ✅ sales (enterprise agriculture)
- ✅ core-project (complex requirements)

**Generated expert:**
- "AgTech Product Manager"
- "Agricultural IoT Specialist" 
- "Farm Technology Consultant"

---

### 💰 FINTECH
**Primary keywords:**
- fintech, financial, finance, banking
- payments, crypto, blockchain, wallet
- lending, investment, trading, finance

**Secondary keywords:**
- compliance, regulatory, security
- transactions, digital banking, neobank
- financial services, risk management

**Modules to activate:**
- ✅ development (security critical)
- ✅ sales (B2B financial)
- ✅ documentation (compliance)
- ✅ core-project (regulatory requirements)

**Generated expert:**
- "FinTech Product Manager"
- "Financial Technology Strategist"
- "Digital Banking Specialist"

---

## 🔄 CLASSIFICATION LOGIC

### STEP 1: KEYWORD ANALYSIS
```python
# Pseudocode of the process
def classify_project(user_input):
    keywords = extract_keywords(user_input)
    
    # Score each project type
    startup_score = count_matches(keywords, STARTUP_KEYWORDS)
    ecommerce_score = count_matches(keywords, ECOMMERCE_KEYWORDS)
    marketing_score = count_matches(keywords, MARKETING_KEYWORDS)
    # ... etc
    
    # Determine primary type
    primary_type = max_score_type(scores)
    
    return primary_type
```

### STEP 2: CONTEXT ANALYSIS
- Analyze input length and detail
- Detect mentions of timeline, budget, team
- Identify specific pain points
- Evaluate user's experience level

### STEP 3: MODULE ACTIVATION
- Activate core modules according to detected type
- Consider common combinations
- Adjust according to detected complexity
- Prioritize modules according to context

### STEP 4: EXPERT GENERATION
- Combine necessary expertise
- Personalize according to specific industry
- Adjust personality according to target (B2B vs B2C)
- Consider relevant background

---

## 📊 CONFIDENCE SCORING

### HIGH CONFIDENCE (>80%)
- Multiple clear keyword matches
- Specific industry detected
- Obvious project type
- Proceed with automatic configuration

### MEDIUM CONFIDENCE (40-80%)
- Some keyword matches
- General type detected but ambiguous
- Offer refinement with 5 questions

### LOW CONFIDENCE (<40%)
- Few or no keyword matches
- Very vague or abstract input
- Activate explorer mode with open questions

---

## 🔧 USAGE INSTRUCTIONS

### FOR SYSTEM PROMPT:
```markdown
When receiving user input:

1. EXTRACT keywords from input
2. APPLY scoring using these patterns
3. DETERMINE primary type + specific industry  
4. CALCULATE confidence score
5. ACTIVATE appropriate modules
6. GENERATE specialized expert
7. PRESENT analysis to user
```

### EXAMPLE OUTPUT:
```
✅ AUTOMATIC ANALYSIS:
- Detected type: Startup SaaS (confidence: 85%)
- Industry: FinTech - Digital Payments  
- Complexity: Medium-High (regulatory requirements)
- Modules: development + sales + documentation + core-project
- Expert: "FinTech Product Manager with compliance expertise"
```

---

**FINAL OBJECTIVE:** Automatically detect complete project context to activate optimal framework configuration without manual user intervention.