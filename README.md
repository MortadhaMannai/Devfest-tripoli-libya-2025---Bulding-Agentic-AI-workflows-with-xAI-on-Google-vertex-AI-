# **Building Agentic AI Workflows with xAI on Vertex AI From Code to Action**
**DevFest Tripoli Libya 2025**
**By Eng. Manai Mohamed Mortadha**

---

## **Overview**

This repository contains the complete demo, code, and resources used in my DevFest Tripoli Libya 2025 session. The session explores how to design and deploy autonomous AI agents capable of perceiving information, reasoning with ML models, acting in real time, explaining their decisions, and running at cloud scale using Google Cloud Vertex AI.

The included demo is a local version of a production grade agentic workflow built to reflect real Vertex AI pipelines, decision orchestrators, and xAI tools.

---

# **Session Summary**

Agentic AI refers to AI systems that can:

• Gather information
• Interpret or predict
• Decide autonomously
• Take real actions
• Provide transparent explanations
• Maintain audit trails

This talk demonstrates how to build such systems end to end using Google Cloud Vertex AI, including:

• Decision pipelines
• Model serving
• xAI interpretability
• RAG based retrieval
• Automated agent actions

You will learn both the architectural patterns and the exact code required to deploy your own agent workflows.

---

# **Session Agenda**

## **1. Introduction**

• Why agentic AI matters today
• Where autonomous systems are used
• What makes AI trustworthy

## **2. Understanding Agentic Systems**

• Key components
• Decision flow patterns
• Perception to action loop
• Where xAI fits

## **3. Vertex AI Deep Dive**

• Workbench for development
• Pipelines for orchestration
• Endpoints for real time inference
• Built in explainability
• Scalable serving options

## **4. Building Autonomous Pipelines**

• Defining agent tasks
• Connecting data sources
• Handling realtime triggers
• Automating decisions

## **5. Integrating Explainable AI**

• Feature importance
• SHAP style reasoning
• Attributions
• Transparent inference

## **6. Using Vertex AI Models**

• Predictive logic
• RAG for more context
• Feedback loops for learning

## **7. Live Coding Demo**

• Build the agent step by step
• Model training
• Autonomous decision making
• Explanation outputs
• Logging and audit systems

## **8. Final Notes**

• Practical guidelines
• Deployment tips
• Learning paths
• Community connections

---

# **The Agent Demo

A Simple but Complete Agentic System**

This repository contains a hands on autonomous agent designed as a marketing assistant example. The workflow simulates real world enterprise agent behavior.

---

# **What the Agent Does**

## **Step 1. Collects Information**

The agent calls a mock API that provides new customer activity events.

Examples in real deployments:

• Sensor readings
• CRM activity
• Web tracking events
• Market movements
• Financial transactions

---

## **Step 2. Analyzes the Input**

The agent loads a trained model:

```
vertex_model.pkl
```

It predicts whether the user is likely to respond positively to a promotion.

---

## **Step 3. Explains Its Reasoning**

Explainability is generated using SHAP.

The agent creates visual and textual explanations including:

• Feature influence
• Top contributing factors
• Reasoning behind the decision

These explanations are stored in:

```
outputs/explanations/
```

---

## **Step 4. Acts Autonomously**

The agent makes a choice:

• Send email
• Update CRM
• Log follow up
• No action required

The chosen action is printed and logged.

---

## **Step 5. Audit Logging**

Every cycle is stored for transparency:

```
outputs/audit_logs/
```

This includes:

• Inputs
• Predictions
• Explanations
• Actions taken
• Timestamps

---

# **Why This Is an Agentic AI System**

The agent follows the full perception to action loop.

| Capability     | Description                                 |
| -------------- | ------------------------------------------- |
| Perception     | Gets new data from external sources         |
| Reasoning      | Predicts the best action                    |
| Explainability | Generates SHAP based explanations           |
| Action         | Takes a real autonomous step                |
| Logging        | Records full history for trust and auditing |

The demo is intentionally simple but aligns with enterprise agent patterns used in:

• Finance
• Retail
• Health
• Operations
• Customer engagement

---

# **Repository Structure**

```
devfest-agent-demo/
├── agent_demo.py        # Main agent loop
├── train_model.py       # Model training script
├── mock_api.py          # Simulated external data source
├── requirements.txt     # Dependencies
├── README.md
└── outputs/
    ├── audit_logs/
    └── explanations/
```

---

# **How to Run the Demo**

## **1. Install dependencies**

```bash
pip install -r requirements.txt
```

## **2. Train the model**

```bash
python train_model.py
```

## **3. Run the agent**

```bash
python agent_demo.py
```

You will see actions, predictions, and logs generated in real time.

---

# **How This Maps to Vertex AI**

This local demo is designed to scale into a full Vertex AI architecture:

| Local Demo        | Vertex AI Equivalent                   |
| ----------------- | -------------------------------------- |
| train_model.py    | Vertex AI Training                     |
| vertex_model.pkl  | Model Registry                         |
| agent_demo.py     | Cloud hosted Agent Workflow            |
| SHAP explanations | Vertex Explainable Predictions         |
| mock API          | Pub Sub, Cloud Functions, CRM webhooks |
| audit logs        | Cloud Logging, BigQuery                |

The same logic can be deployed to real production with pipelines and endpoints.

---

# **Speaker and Author**

**Eng. Manai Mohamed Mortadha**

Senior AI Engineer - Netflix , USA
Phd candidate in xAI - Saint Mary's university ,Canada
CEO and HEad of AI R&D Departement - MAN.AI
AI  Expert Consultant - Tegus USA
International AI Speaker
AI Expert Reviewer & Author - Packt Publishing UK

---

# **Connect with Me**

**Website**
[https://www.mann-ai.com](https://www.mann-ai.com](https://taplink.cc/manaimortadha))

**LinkedIn**
[https://linkedin.com/in/mannai-mortadha](https://linkedin.com/in/mannai-mortadha)

**GitHub**
[https://github.com/MortadhaMannai](https://github.com/MortadhaMannai)

**Leetcode**
[https://github.com/MortadhaMannai](https://github.com/MortadhaMannai](https://leetcode.com/u/mannaimortadha898/))

**Email**
[mannaimortadha898@gmail.com](mailto:mannaimortadha898@gmail.com)

