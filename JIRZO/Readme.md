# JIRZO - AI-Based Behavioral Risk Assessment for Adaptive Authentication

## 📌 Project Overview

This project explores the use of Artificial Intelligence in cybersecurity, specifically for improving the security of user authentication.

Traditional login systems mainly verify whether the username and password are correct. However, an attacker who obtains valid credentials may also be able to successfully log in.

The proposed system will investigate whether user login behavior can be analyzed using AI to identify potentially unusual login attempts.

Based on the risk associated with a login attempt, the system may be able to:

* Allow the login
* Request additional authentication such as MFA/OTP
* Temporarily block the login

The exact AI technique and implementation will be determined during the development of the project after learning the required AI and machine-learning concepts.

---

# 🎯 Problem Statement

A traditional authentication system generally works like this:

```text
Username + Password
        ↓
   Are credentials correct?
       ↓          ↓
      Yes         No
       ↓          ↓
   Allow Login   Reject
```

The problem is that valid credentials do not always mean that the person attempting the login is the legitimate account owner.

For example, an attacker may obtain a user's password through phishing or credential theft.

The attacker could then provide:

```text
Correct Username
+
Correct Password
```

and potentially pass traditional authentication.

The proposed project investigates whether additional behavioral information can help identify login attempts that appear unusual compared with a user's previous behavior.

---

# 💡 Proposed Solution

The proposed system will analyze selected login-related information and use AI to investigate whether a login attempt appears normal or unusual.

Possible information may include:

* Login time
* IP address
* Approximate location
* Browser
* Operating system
* Device information
* Failed login attempts
* Previous login history

The general idea is:

```text
              Login Attempt
                    ↓
          Collect Login Information
                    ↓
              AI Analysis
                    ↓
          Behavioral Assessment
                    ↓
             Risk Assessment
                    ↓
        ┌───────────┼───────────┐
        ↓           ↓           ↓
      Low Risk   Medium Risk  High Risk
        ↓           ↓           ↓
      Allow         MFA        Block
```

This diagram represents the **planned concept**. The final implementation may change as the project develops.

---

# 🎯 Project Objectives

The main objectives are:

1. Understand how Artificial Intelligence can be applied to cybersecurity.
2. Learn the basic concepts of Machine Learning.
3. Investigate how login behavior can be represented as data.
4. Explore whether AI can identify unusual authentication behavior.
5. Develop a prototype for risk-based authentication.
6. Use the risk assessment to support adaptive authentication decisions.
7. Document the complete learning and development process.

---

# 🔍 Initial Scope

The project will initially focus only on **authentication-related behavior**.

The system may consider a limited number of features, such as:

```text
Login Time
IP Address
Approximate Location
Browser
Device Information
Failed Login Attempts
Previous Login History
```

The project will **not initially attempt to monitor the user's entire computer or understand the user's psychological behavior**.

The exact features will be finalized after researching what information can realistically and ethically be collected by a web application.

---

# 🤖 AI Component

The AI component is currently in the **research and learning stage**.

The project will first cover the basic concepts of:

* Artificial Intelligence
* Machine Learning
* Dataset
* Features
* Training
* Model
* Prediction
* Model evaluation
* Behavioral analysis
* Anomaly detection

After learning these concepts, an appropriate AI/ML approach will be selected.

### Important

The project does not currently assume a specific algorithm.

The final algorithm will be selected based on:

* Understanding of the algorithm
* Suitability for the problem
* Available data
* Project complexity
* Course requirements

An existing machine-learning library may be used if appropriate.

---

# 📊 Possible Data

The project may use authentication-event data similar to:

```text
User ID
Login Time
IP Address
Location
Browser
Operating System
Device
Failed Attempts
Login Result
```

The final dataset has not yet been selected.

A synthetic or publicly available dataset may be considered depending on the requirements and availability.

Any dataset used in the final project will be documented.

---

# 🔐 Adaptive Authentication

The project will investigate the use of risk assessment to make authentication more adaptive.

The intended concept is:

### Low Risk

```text
Behavior appears normal
        ↓
Allow Login
```

### Medium Risk

```text
Some unusual behavior
        ↓
Request MFA/OTP
```

### High Risk

```text
Highly unusual behavior
        ↓
Temporarily restrict/block login
```

These decisions are part of the proposed design and will be implemented and tested only if they are achievable within the final project scope.

---

# 🏗️ Planned Development Process

The project will be developed gradually.

## Phase 1 — Understand the Problem

* [ ] Research authentication security
* [ ] Understand risks of stolen credentials
* [ ] Study behavioral authentication
* [ ] Study adaptive/risk-based authentication

## Phase 2 — Learn AI Fundamentals

* [ ] Learn AI basics
* [ ] Learn Machine Learning basics
* [ ] Understand datasets
* [ ] Understand features
* [ ] Understand training
* [ ] Understand models
* [ ] Understand predictions
* [ ] Learn basic model evaluation

## Phase 3 — Define the Data

* [ ] Decide which behavioral features are useful
* [ ] Determine how the data can be collected
* [ ] Select or create a dataset
* [ ] Document the dataset

## Phase 4 — Select AI Approach

* [ ] Research suitable AI/ML approaches
* [ ] Compare possible approaches
* [ ] Select an appropriate approach
* [ ] Document why it was selected

## Phase 5 — Develop Prototype

* [ ] Prepare data
* [ ] Implement AI component
* [ ] Analyze login behavior
* [ ] Generate risk assessment
* [ ] Implement authentication responses

## Phase 6 — Testing & Evaluation

* [ ] Create normal login scenarios
* [ ] Create unusual login scenarios
* [ ] Test AI predictions
* [ ] Analyze incorrect decisions
* [ ] Document results and limitations

---

# 📁 Planned Repository Structure

The repository structure will evolve as the project develops.

Initial structure:

```text
ai-behavior-risk/
│
├── README.md
│
├── docs/
│   └──
│
├── data/
│   └──
│
├── src/
│   └──
│
├── tests/
│   └──
│
└── requirements.txt
```

Additional files and folders will be added as the project develops.

---

# ⚠️ Current Limitations

At the current planning stage, the following have not yet been finalized:

* AI/ML algorithm
* Dataset
* Exact behavioral features
* Risk calculation method
* Risk thresholds
* Final technology stack
* Model evaluation method

These decisions will be made during development and documented in this repository.

---

# 📝 Documentation Approach

This repository will document the project from the beginning rather than only documenting the final result.

Documentation will include:

* Project research
* AI concepts learned
* Design decisions
* Dataset information
* Experiments
* Implementation
* Testing
* Results
* Problems encountered
* Limitations
* Future improvements

The goal is to maintain a record of **how the project was developed and what was learned during the process**.

---

# 📌 Current Status

**Status: 🟡 Planning / Learning**

The project idea has been selected.

The next step is to learn the fundamental concepts of Artificial Intelligence and Machine Learning before selecting the final AI approach.

No specific machine-learning algorithm has been selected yet.

---

# 🚀 Future Updates

As development progresses, this README will be updated with:

* Final requirements
* Final system architecture
* Selected dataset
* Selected AI/ML approach
* Implementation details
* Testing results
* Screenshots
* Demonstrations
* Final conclusions

The README will reflect the **actual implementation**, not just the original plan.

