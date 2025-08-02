# 🔧 **SETUP GUIDE - KORE KONTEXT**

## 📋 **COMPLETE STEP-BY-STEP SETUP**

### **PREREQUISITES**
- ✅ Account on [Claude.ai](https://claude.ai) with Projects access
- ✅ Account on [GitHub](https://github.com) 
- ✅ Basic markdown knowledge
- ✅ 10 minutes of time

---

## 🚀 **STEP 1: PREPARE THE REPOSITORY**

### **1.1 Clone this Repository**
```bash
git clone https://github.com/KnuppeArt/kore-kontext.git
cd kore-kontext
```

### **1.2 Explore the Structure**
```bash
# Main directories
ls -la
# framework/     - Core framework files
# knowledge-base/ - Files for Claude Projects
# active-projects/ - Your project templates
```

---

## 🎯 **STEP 2: CONFIGURE YOUR FIRST PROJECT**

### **2.1 Create Project Folder**
```bash
# Duplicate template for your project
cp -r active-projects/template-new-project active-projects/my-first-project

# Personalize
cd active-projects/my-first-project
echo "# My First Project with Kore Kontext" > README.md
```

### **2.2 Prepare Context Files**
Edit `context/project-context.md`:
```markdown
# PROJECT CONTEXT

## BASIC INFORMATION
- **Name**: My First Project
- **Type**: [Startup/Ecommerce/Marketing/Development]
- **Industry**: [Specify your industry]
- **Stage**: [Idea/Validation/MVP/Growth]

## DESCRIPTION
[Briefly describe your project]

## OBJECTIVES
- [ ] Objective 1
- [ ] Objective 2
- [ ] Objective 3

## TIMELINE
- **Start**: [Date]
- **MVP Target**: [Date]
- **Launch**: [Date]
```

---

## 🤖 **STEP 3: CONFIGURE CLAUDE PROJECT**

### **3.1 Create the Claude Project**
1. Go to [Claude.ai](https://claude.ai)
2. Click **"Create Project"**
3. **Name**: `[Your Project] - Kore Kontext`
4. **Description**: `Project managed with Kore Kontext`

### **3.2 Upload Knowledge Base**
**MANDATORY files to upload:**
```
📁 Knowledge Base (3 core files)
├── kore-kontext-hybrid-system-prompt.md    # Main system prompt
├── data-flow-orchestrator.md               # Automatic orchestrator
└── project-classifier-complete.md          # Project classifier
```

### **3.3 Configure System Prompt**
Copy and paste in **Settings > Custom Instructions** the content from:
`knowledge-base/kore-kontext-hybrid-system-prompt.md`

---

## ⚙️ **STEP 4: FIRST TEST**

### **4.1 Functionality Test**
In your Claude Project, write:
```
"I want to create a [description of your project]"
```

**Example:**
```
"I want to create a mobile app for homemade food delivery"
```

### **4.2 Verify Expected Response**
Kore Kontext should respond with:
```
✅ AUTOMATIC ANALYSIS COMPLETED:
- Detected type: [Mobile App + Marketplace + Food Delivery]
- Suggested modules: [development + marketing + sales + ecommerce]
- Generated expert: [Food Delivery Product Manager]

🎯 AUTOMATIC CONFIGURATION READY:
[Configuration description]

Want to start NOW with this configuration, or prefer I ask you 
5 quick questions to optimize context?

[OPTIONS: "Start NOW" | "5 Quick Questions"]
```

---

## 🎯 **STEP 5: START WORKING**

### **5.1 Generate Your First Deliverable**
```
"Generate the initial PRD for this app"
```

### **5.2 Automatic Capture Test**
Kore Kontext should automatically detect and suggest:
```
🤖 AUTOMATIC DETECTION: I've generated a complete PRD

📁 SAVE SUGGESTION:
- Location: /active-projects/my-delivery-app/generated/deliverables/prd-mvp.md
- Reason: This PRD is fundamental for project development
- Action: Create new document

Shall I proceed to save it to the repository?
[Yes, save] [No] [Modify location]
```

---

## 🎯 **DAILY WORKFLOWS**

### **7.1 Typical Workflow**
```
1. Open project-specific Claude Project
2. Describe what you need to work on today
3. Kore Kontext (in expert mode) helps you as specialist
4. Generate documents, code, strategies, etc.
5. Automatically detects valuable content and suggests saving
6. Confirm and it syncs with GitHub automatically
7. Project context updates automatically
```

### **7.2 Multi-Project Usage**
```
Project 1: AgTech Startup → Claude Project: "AgTech MVP - Kore Kontext"
Project 2: Ecommerce Fashion → Claude Project: "Fashion Store - Kore Kontext"  
Project 3: Marketing Agency → Claude Project: "Agency Growth - Kore Kontext"

Each with specialized expert and independent context
```

---

## 🔍 **TROUBLESHOOTING**

### **Issue: Claude doesn't detect mode automatically**
**Solution:**
- Verify all knowledge base files are uploaded
- Check that system prompt was copied completely
- Clear project cache and restart conversation

### **Issue: Doesn't suggest saving content automatically**
**Solution:**
- Verify `data-flow-orchestrator.md` is in knowledge base
- Check that GitHub tools are available in project
- Try generating more specific content (PRD, technical specs, etc.)

---

## 📊 **SUCCESS METRICS**

### **Successful Setup if:**
- ✅ Claude Project responds in setup mode first time
- ✅ Automatically switches to expert mode after configuration  
- ✅ Detects and suggests saving content automatically
- ✅ Maintains context between conversations

### **Successful Usage if:**
- ✅ Reduce project setup time by 80%+
- ✅ Generate professional-quality documents quickly
- ✅ Don't lose valuable information between sessions
- ✅ Can manage multiple projects simultaneously
- ✅ Expert understands your industry and specific context

---

**🎉 Congratulations! You now have Kore Kontext working and ready to accelerate your projects.**