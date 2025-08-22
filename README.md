# All You Need to Know About CI/CD

## 📑 Table of Contents
1. [For Beginners](#for-beginners)  
   - [The Problems](#the-problems)  
   - [Solution → CI/CD](#-solution--cicd)  
   - [CI/CD Basics](#1-cicd-)  
   - [Continuous Integration](#2-continuous-integration-ci)  
   - [Continuous Delivery](#3-continuous-delivery-cd)  
   - [Continuous Deployment](#4-continuous-deployment-cd)  
   - [Key Difference](#5-key-difference)  
2. [Level 1 — CI/CD Cycle](#level-1--cicd-cycle)  
3. [Level 2 — Engineering Maturity](#level-2--engineering-maturity)  
4. [Real Projects](#-real-projects)  
5. [Thank You](#-thank-you)  

---

## For Beginners

Let’s start with a simple story.  
Imagine you are building your **personal portfolio website**.  

Every time you make a small change (update a project, fix a typo, add a new skill), you have to:  
- Update your resume  
- Add a new project  
- Fix a typo  

Then you must **unpublish the old site** and **publish the new one** again.  

### The Problems
- ⏳ Time wasted — repeating the same cycle  
- 🚨 Manual steps → mistakes introduced  
- ⚡ Productivity drops  

---

## 💡 Solution → CI/CD

That’s why we use **CI/CD** → to save time and reduce mistakes.

<p align="center">
  <img width="1676" height="263" alt="CI/CD Diagram" src="https://github.com/user-attachments/assets/012c529d-d6da-4dc1-a2c6-9edd2286ff7b" />
</p>

### 1. CI/CD ?
**CI/CD = Continuous Integration / Continuous Delivery (or Deployment).**  
It’s the process of automating **build, test, and release workflows**.

---

### 2. Continuous Integration (CI)  
*(highlighted in yellow in the diagram)*  

**Definition:** build + test + verify  

Every time code is pushed (new feature, bug fix, etc.), CI automatically:  
- Builds the code  
- Runs tests  
- Verifies everything still works  

➡️ Goal: catch issues early and keep the main branch stable.  

---

### 3. Continuous Delivery (CD)  
*(highlighted in blue in the diagram)*  

After CI, the code is **always ready to deploy**.  
But → a human decides **when** to push it live.  

Example: CI pipeline prepares the build, runs tests, stores artifact → engineer presses **Deploy**.  

---

### 4. Continuous Deployment (CD)  
*(also highlighted in blue in the diagram)*  

After CI, the code goes live **automatically** once tests pass.  
No manual button click needed.  

Example: Push to main → CI runs → if green ✅ → deploys to production.  

---

### 5. Key Difference
- **Continuous Delivery** → Ready for deployment (manual decision).  
- **Continuous Deployment** → Fully automated release after tests.  

👉 In short:  
- **CI** = build + test + verify  
- **CD (Delivery)** = package + ready to deploy (manual trigger)  
- **CD (Deployment)** = package + deploy + release (automatic to production)  

---

## Level 1 — CI/CD Cycle

🔄 The pipeline is shown as an infinite loop because **CI/CD is continuous**.  
It never ends — it repeats with every code change.  

📂 *For more Level 1 details → see Folder `Level-1`*  

---

## Level 2 — Engineering Maturity

**The difference between high-performing engineering orgs and slow ones? → CI/CD maturity.**

Most teams still:  
`push code → pray → debug production`  

Elite teams:  
**Automated pipelines that ship 100x faster with 90% fewer bugs.**

- ⚡ **Manual Build/Test/Deploy Overhead** → Velocity Bottleneck  
- ⚡ **CI/CD Automation** → 10x Engineering Productivity → **DORA Metrics Excellence**  

📂 *For more Level 2 details → see Folder `Level-2`*  

---

## 📂 Real Projects
For a **real-time project**, go to the `Projects` folder.  

---

# 🙏 Thank You
