# All You Need to Know About CI/CD

---

## 👶 For Beginners — The Story

Imagine you are building your **portfolio website**.  
Every time you make a change (add a project, fix a typo, update a skill):  

1. Unpublish the old site  
2. Publish the new one again  

### ❌ The Problems
- Time wasted ⏳  
- Manual steps cause mistakes 🚨  
- Repetition kills productivity ⚡  

---

## ✅ The Solution — CI/CD

Instead of doing everything manually, **CI/CD automates it**.  
You push code → pipeline does the rest.

<p align="center">
  <img width="1676" height="263" alt="CI/CD Diagram" src="https://github.com/user-attachments/assets/012c529d-d6da-4dc1-a2c6-9edd2286ff7b" />
</p>

---

## 🔎 What is CI/CD?

**CI/CD = Continuous Integration + Continuous Delivery/Deployment**  
It automates **build → test → release**.

---

### 🟨 1. Continuous Integration (CI)  
Every push → pipeline runs:  
- Build  
- Test  
- Verify  

➡️ Keeps the main branch stable.  

---

### 🟦 2. Continuous Delivery (CD)  
After CI → code is **always ready**.  
- Human decides when to deploy.  
- Example: engineer clicks “Deploy.”  

---

### 🟦 3. Continuous Deployment (CD)  
After CI → code goes live **automatically**.  
- No human button needed.  
- Example: push → tests pass → production.  

---

## ⚖️ Key Difference

- **Continuous Delivery** → Manual trigger to deploy  
- **Continuous Deployment** → Automatic deploy  

👉 In short:  
- **CI** = build + test + verify  
- **CD (Delivery)** = package + ready to deploy  
- **CD (Deployment)** = package + deploy + release  

---

## 🔄 Level 1 — CI/CD Loop

CI/CD is shown as an **infinite loop** because it repeats with every code change.  

📂 *See details in `Level-1` folder*  

---

## 🚀 Level 2 — Engineering Maturity

Bad teams:  
`push code → pray → debug in production`  

Great teams:  
Automated pipelines → **ship faster, fewer bugs.**  

- Manual workflows = bottleneck ⚡  
- CI/CD automation = 10x productivity 💡  

📂 *See details in `Level-2` folder*  

---

## 📂 Real Projects

Check the `Projects` folder for a working example.  

---

## 🙏 Thank You
