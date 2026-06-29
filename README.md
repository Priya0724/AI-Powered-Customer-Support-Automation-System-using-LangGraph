# AI-Powered-Customer-Support-Automation-System-using-LangGraph


## Project Information

**Project Title:** AI-Powered Customer Support Automation System using LangGraph

**Organization:** ABC Technologies

**Technology Stack:** Python, LangGraph, LangChain, SQLite, RAG

---

# 1. Project Overview

ABC Technologies is a SaaS company that provides cloud-based business management software to customers worldwide. The company receives thousands of support requests daily regarding product information, technical issues, billing problems, account management, and refund requests.

To improve customer support efficiency and reduce operational costs, an AI-Powered Customer Support Automation System has been developed using LangGraph. The system automatically classifies customer queries, routes them to appropriate departments, retrieves relevant information from company documents, maintains customer conversation history, supports human approval workflows, and generates final validated responses.

---

# 2. Project Objectives

The primary objectives of this project are:

- Automate customer support operations.
- Reduce response time.
- Route customer queries intelligently.
- Retrieve relevant information using RAG.
- Maintain customer conversation history.
- Implement human approval for critical requests.
- Validate responses using a supervisor agent.
- Demonstrate enterprise workflow automation using LangGraph.

---

# 3. Features Implemented

## ✓ Intent Classification

Customer queries are automatically classified into:

- Sales
- Technical Support
- Billing
- Account Management
- Memory Recall

---

## ✓ Conditional Routing using LangGraph

The system uses LangGraph conditional edges to route customer queries to the appropriate support department.

---

## ✓ Specialized Support Agents

### Sales Agent
Handles:

- Product information
- Subscription plans
- Pricing information

### Technical Support Agent
Handles:

- Application crashes
- Installation issues
- Login errors
- Configuration problems

### Billing Agent
Handles:

- Invoice requests
- Payment issues
- Refund requests

### Account Agent
Handles:

- Password reset
- Profile updates
- Account activation/deactivation

---

## ✓ Retrieval-Augmented Generation (RAG)

The system retrieves relevant information from company documents:

- Company Policy Document
- Pricing Guide
- Technical Manual
- FAQ Document

---

## ✓ SQLite Memory

Customer conversations are stored in SQLite memory.

Example:

Customer:
```
My name is David. I have a billing issue.
```

Later:

```
What was my previous support issue?
```

Response:

```
Your previous issue was: I have a billing issue.
```

---

## ✓ Human-in-the-Loop Approval

The following requests require human approval:

- Refund requests
- Subscription cancellation
- Account closure requests
- Compensation requests
- Escalation to management

---

## ✓ Supervisor Agent

The supervisor agent validates and improves responses before sending them to customers.

Example:

```
ABC Technologies Support:

Your refund request has been submitted.

Thank you for contacting us.
```

---

# 4. Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| LangGraph | Workflow Management |
| LangChain | AI Framework |
| SQLite | Conversation Memory |
| FAISS | Vector Database |
| HuggingFace Embeddings | Embedding Generation |
| PyPDFLoader | PDF Loading |
| Sentence Transformers | Text Embeddings |

---

# 5. Project Structure

```
CustomerSupportAutomation/

│
├── app.py
├── workflow.py
├── state.py
├── memory.py
├── supervisor.py
├── rag.py
│
├── agents/
│   ├── sales.py
│   ├── technical.py
│   ├── billing.py
│   └── account.py
│
├── documents/
│   ├── company_policy.pdf
│   ├── pricing_guide.pdf
│   ├── technical_manual.pdf
│   └── faq.pdf
│
├── database/
│   └── memory.db
│
├── screenshots/
│
├── workflow_diagram.png
│
└── README.md
```

---

# 6. LangGraph Workflow Architecture

```
START
   |
Intent Classification
   |
Conditional Routing
   |
Sales / Technical / Billing / Account / Memory
   |
RAG Retrieval
   |
Human Approval
   |
Supervisor Agent
   |
SQLite Memory
   |
END
```

---

# 7. Installation

Create virtual environment:

```bash
python -m venv .venv
```

Activate environment:

Windows:

```bash
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install langgraph
pip install langchain
pip install langchain-community
pip install sentence-transformers
pip install faiss-cpu
pip install pypdf
pip install grandalf
```

---

# 8. Running the Project

Run the application:

```bash
python app.py
```

Run the LangGraph workflow:

```bash
python workflow.py
```

---

# 9. Demonstration Queries

## Query 1

```
What are the pricing plans available for your software?
```

Expected Routing:

```
Sales Department
```

---

## Query 2

```
I forgot my account password.
```

Expected Routing:

```
Account Department
```

---

## Query 3

```
My application crashes whenever I upload a file.
```

Expected Routing:

```
Technical Support Department
```

---

## Query 4

```
I need a refund for my annual subscription.
```

Expected Routing:

```
Billing Department
→ Human Approval Required
```

---

## Query 5

```
What was my previous support issue?
```

Expected Routing:

```
Memory Recall
```

---

# 10. Assignment Tasks Completed

| Task | Description | Status |
|------|-------------|--------|
| Task 1 | Workflow Design | Completed |
| Task 2 | State Structure | Completed |
| Task 3 | Intent Classification | Completed |
| Task 4 | Conditional Routing | Completed |
| Task 5 | Specialized Agents | Completed |
| Task 6 | RAG Integration | Completed |
| Task 7 | SQLite Memory | Completed |
| Task 8 | Human-in-the-Loop | Completed |
| Task 9 | Supervisor Agent | Completed |
| Task 10 | Demonstration | Completed |

---

# 11. Outputs Demonstrated

The project successfully demonstrates:

- Intent Classification
- LangGraph Conditional Routing
- Specialized Agents
- Retrieval-Augmented Generation
- SQLite Memory Storage
- Memory Recall
- Human Approval Workflow
- Supervisor Validation
- Final Response Generation

---

# 12. Conclusion

The AI-Powered Customer Support Automation System successfully automates customer support operations using LangGraph. The system integrates workflow orchestration, retrieval-augmented generation, conversation memory, human approval workflows, and response supervision to create an efficient enterprise-grade customer support solution.

This project demonstrates practical applications of AI agents, workflow automation, and intelligent customer support systems.

---

