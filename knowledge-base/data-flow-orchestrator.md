# 🤖 DATA FLOW ORCHESTRATOR - KORE KONTEXT

## PRIMARY FUNCTION
Automatically detect valuable content generated during conversations and orchestrate its storage in the correct repository structure.

---

## 🔍 AUTOMATIC CONTENT DETECTION

### CONTENT PATTERNS TO DETECT:

#### 📋 **STRATEGIC DOCUMENTS**
**Detection triggers:**
- "PRD", "Product Requirements", "product specifications"
- "Technical requirements", "technical specs", "system architecture"
- "Marketing strategy", "marketing plan", "go-to-market"
- "Business plan", "business strategy", "model canvas"
- "UVP", "USP", "value proposition", "competitive advantage"

**Automatic action:**
```
🤖 DETECTION: You've generated a [DOCUMENT_TYPE]

📁 SAVE SUGGESTION:
- Location: /active-projects/[CURRENT_PROJECT]/generated/[category]/
- File: [descriptive-name].md
- Reason: This document is fundamental for the project and should be preserved

Do you want me to save this document to the repository?
[Yes, save] [No] [Modify location]
```

#### 💡 **INSIGHTS AND DECISIONS**
**Detection triggers:**
- "Decision:", "We decided that", "The strategy will be"
- "Key insight:", "Important:", "We learned that"
- "Next steps:", "Action items", "TODO list"
- "Conclusion:", "In summary", "Main takeaway"

**Automatic action:**
```
🤖 DETECTION: You've made an important decision

📝 LOG SUGGESTION:
- Location: /active-projects/[CURRENT_PROJECT]/context/decisions-log.md
- Category: [Technical/Marketing/Strategic/Operational]
- Impact: [High/Medium/Low]

Do you want me to add this decision to the project log?
```

#### 🛠️ **CODE AND CONFIGURATIONS**
**Detection triggers:**
- Generated code blocks
- Tool configurations
- Automation scripts
- Custom templates

**Automatic action:**
```
🤖 DETECTION: You've generated code/configuration

⚙️ SAVE SUGGESTION:
- Location: /active-projects/[CURRENT_PROJECT]/generated/code/
- Type: [Frontend/Backend/Config/Script]
- Integration: [GitHub/VS Code/Deploy]

Do you want me to save this code to the project repository?
```

#### 📊 **ANALYSIS AND RESEARCH**
**Detection triggers:**
- Competitive analysis
- Market research  
- User/audience analysis
- Metrics and KPIs

**Automatic action:**
```
🤖 DETECTION: You've generated valuable analysis

📊 SAVE SUGGESTION:
- Location: /active-projects/[CURRENT_PROJECT]/generated/analyses/
- Category: [Market/Competitive/User/Technical]
- Update: [New document/Update existing]

Do you want me to preserve this analysis for future reference?
```

---

## 🗂️ INTELLIGENT LOCATION MAPPING

### CONTENT TYPES → AUTOMATIC LOCATIONS:

```yaml
# PROJECT DOCUMENTS
PRD/Requirements: /active-projects/[project]/generated/deliverables/
Technical Specs: /active-projects/[project]/generated/deliverables/
Marketing Strategy: /active-projects/[project]/generated/strategies/
Sales Strategy: /active-projects/[project]/generated/strategies/
Business Plan: /active-projects/[project]/generated/strategies/

# CODE AND ASSETS
Code/Scripts: /active-projects/[project]/generated/code/
Configurations: /active-projects/[project]/generated/config/
Assets/Creative: /active-projects/[project]/generated/assets/

# ANALYSIS AND RESEARCH
Market Research: /active-projects/[project]/generated/analyses/market/
Competitive Analysis: /active-projects/[project]/generated/analyses/competitive/
User Research: /active-projects/[project]/generated/analyses/user/
Technical Analysis: /active-projects/[project]/generated/analyses/technical/

# CONTEXT AND DECISIONS
Decisions: /active-projects/[project]/context/decisions-log.md (append)
Project Updates: /active-projects/[project]/context/project-context.md (update)
Expert Evolution: /active-projects/[project]/context/expert-profile.md (update)

# FRAMEWORK IMPROVEMENTS
New Templates: /framework/modules/[module]/templates/
New Prompts: /framework/modules/ai-prompts/templates/
Core Improvements: /framework/core/ or /framework/intelligence/
```

---

## 🤖 AUTOMATIC ORCHESTRATION FLOW

### STEP 1: REAL-TIME DETECTION
```
During conversation → Claude detects valuable content
↓
Automatically classifies content type
↓
Determines optimal location in structure
↓
Generates save suggestion
```

### STEP 2: USER VALIDATION  
```
🤖 "I've detected [CONTENT_TYPE]. 
   I suggest saving it to [LOCATION] because [REASON].
   Proceed?"

User: [Confirms/Modifies/Rejects]
```

### STEP 3: AUTOMATIC EXECUTION
```
If confirms → Use GitHub integration to:
- Create/update file in correct location
- Commit with descriptive message
- Update corresponding indices/logs
- Notify user of success
```

---

## 🔧 INSTRUCTIONS FOR CLAUDE

### INCLUDE IN SYSTEM PROMPT:

```markdown
## DATA FLOW ORCHESTRATION

Your work includes **automatically orchestrating** data flow:

1. **DETECT** when you generate valuable content (use defined patterns)
2. **CLASSIFY** content type automatically  
3. **MAP** to correct location in repo structure
4. **SUGGEST** save/update with clear value explanation
5. **EXECUTE** if user confirms (use GitHub integration)

### AUTOMATIC PROCESS:
- After generating content → Evaluate if valuable to preserve
- If valuable → Present save suggestion automatically
- Explain WHY it should be saved and WHERE
- If user confirms → Execute save with GitHub tools

### SUGGESTION FORMATS:
[Use templates defined in data-flow-orchestrator.md]

### AUTOMATIC COMMIT MESSAGES:
- "Add [type]: [brief-description] for [project]"
- "Update [document]: [main-change] for [project]"  
- "Create [analysis]: [key-insight] for [project]"
```

---

## 📊 DETECTION PATTERNS REFERENCE

### HIGH-VALUE CONTENT INDICATORS:
```
Structural documents:
- Length > 500 words with clear sections
- Contains specific requirements or specifications
- Includes actionable items or decisions
- References project goals or constraints

Strategic content:
- Contains analysis or recommendations
- Includes competitive or market insights
- Defines processes or methodologies
- Establishes project direction or priorities

Technical content:
- Code with significant functionality
- Configuration for production use
- Architecture or design decisions
- Integration or deployment instructions

Decision content:
- Clear decision statements
- Rationale for choices made
- Impact assessment
- Timeline or responsibility assignments
```

### LOW-VALUE CONTENT INDICATORS:
```
- Casual conversation or clarification
- Repeated information already documented
- Hypothetical scenarios without commitment
- Brief Q&A without strategic value
```

---

## 🔄 INTEGRATION WITH GITHUB TOOLS

### AUTOMATIC FUNCTIONS:
```
github:create_or_update_file
- For individual document creation/updates
- Automatic file naming conventions
- Descriptive commit messages

github:push_files  
- For multiple related files
- Batch operations for efficiency
- Consistent project structure maintenance

github:get_file_contents
- To check existing content before updates
- Avoid duplications
- Merge new information intelligently
```

### COMMIT MESSAGE TEMPLATES:
```
Document creation:
"Add [document-type]: [brief-description] for [project-name]"

Document updates:
"Update [document-name]: [main-change] for [project-name]"

Analysis creation:
"Create [analysis-type]: [key-finding] for [project-name]"

Decision logging:
"Log decision: [decision-summary] for [project-name]"

Code commits:
"Add [feature/fix]: [description] for [project-name]"
```

---

**OBJECTIVE: Seamlessly capture and organize all valuable project information while maintaining user control and repository quality.**