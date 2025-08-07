# PM Cursor Generator

AI-powered Product Management document generator using **Cursor Project Rules** for seamless integration with Cursor's AI capabilities.

## 🎯 Overview

This project provides a modern approach to PM document generation by leveraging Cursor's **Project Rules** system. Instead of complex command palettes, users can simply ask Cursor's AI to create documents, and the AI will follow the predefined templates and product context.
Note that the Cursor Rules now follow this paradigm, as defined here: https://docs.cursor.com/en/context/rules#can-rules-reference-other-rules-or-files

## 🚀 Key Features

### ✅ **Project Rules Integration**
- Uses Cursor's native `.cursor/rules/` system
- Product context automatically included in all AI conversations
- Template instructions guide AI document creation
- No complex command palette needed

### ✅ **AI-First Approach**
- Simply ask Cursor AI: "Create a PRD for login feature"
- AI automatically applies relevant templates
- Product context is always included
- Natural language interaction

### ✅ **Document Types**
- **PRD (Product Requirements Document)**
- **User Stories**
- **User Personas**
- **Product Roadmaps**
- **Epics Generator**
- **RICE Prioritization**
- **User Journey**
- **Lean Canvas (Product Strategy)**
- **Product Positioning (Elevator Pitch)**
- **KPI to Revenue Connector**
- **Risk Analysis**

### ✅ **Smart File Management**
- Automatic `/product-documents/` folder creation
- Unique document IDs with timestamps
- Documents are ready for immediate use

## 📁 Project Structure

```
pm-cursor-generator/
├── .cursor/rules/           # Cursor Project Rules
│   ├── product-context.mdc  # Product context (*always* applied)
│   ├── context-generator.mdc    # helps generate your product context
│   ├── prd-template.mdc    # PRD creation instructions
│   ├── user-story-template.mdc
│   ├── persona-template.mdc
│   ├── roadmap-template.mdc
│   ├── epic-generator-template.mdc
│   ├── rice-analysis-template.mdc
│   ├── user-journey-template.mdc
│   ├── lean-canvas-template.mdc
│   ├── product-positioning.mdc
│   ├── kpi-revenues-template.mdc
│   └── risk-analysis-template.mdc
├── product-documents/      # Generated documents (output)
├── alternate-templates/    # alternate versions of templates
|   ├── alternate_read.me  
|   └── etc....
├── helper-docs/    # helper documentation and examples
|   ├── example-product-context.md    # an example of what this should look like  
|   └── etc....     # *.txt files that can add extra information for templates
└── README.md
```

## 🛠️ Installation & Setup

### 1. Download this repo to a new folder for your project
All you need are the directories - no installation required (other than Cursor itself)

### 2. **Configure Product Context**
Edit `.cursor/rules/product-context.mdc` with your product information:

You can check out the helper-docs/example-product-context.md for an example

#### ALTERNATIVE AUTOMATED CONFIGURATION SOLUTION:
You can use the AI to help generate your product-context:
To do this, you need to MANUALLY type in @context-generator.mdc and ask it for help (you can provide a 1-liner of the product, or it will ask you for it)
It will then generate data for the product-context, which you can manually paste into the product-context.mdc file

### 3. **Usage**

#### AI Commands
Simply ask Cursor AI:
- "Create a PRD for user authentication"
- "Generate user stories for checkout process"
- "Make a persona for our target users"
- "Create a roadmap for Q1 features"


## 🎯 How It Works

### **1. Project Rules Integration**
The `.cursor/rules/` files provide:
- **Product Context**: Always included in AI conversations
- **Template Instructions**: Guide AI on document structure
- **Writing Guidelines**: Ensure consistent quality

### **2. AI-Powered Creation**
When you ask Cursor AI to create a document:
1. AI reads the product context from Project Rules
2. AI applies relevant template instructions
3. AI generates structured content
4. AI creates the file with proper naming

### **3. Smart File Management**
- Creates `/product-documents/` folder automatically
- Maintains unique document IDs with timestamps
- Documents are ready for immediate use


## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Add new template rules in `.cursor/rules/`
4. Update documentation as needed
5. Submit a pull request

## 📄 License

MIT License - see LICENSE file for details.

---

**🎯 The future of PM document generation is AI-first, context-aware, and seamlessly integrated with your development workflow.** 
Copyright (c) 2025 Ze'ev Abrams (ZeevAbrams)