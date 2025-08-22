# All You Need to Know About CI/CD

## 📖 For Beginners

Let’s start with a simple story.  
Imagine you are building your **personal portfolio website**.  
Every time you make a small change (update a project, fix a typo, add a new skill), you have to:
- update your resume  
- add a new project  
- fix a typo  

You have to **unpublish the old site**, then **publish the new one**.  

⏳ This cycle wastes time 👉 This takes time.
🚨 Manual steps introduce mistakes 👉 You repeat the same steps again and again.  
⚡ Productivity drops 👉 Mistakes can happen.  


---

## 💡 Solution → CI/CD
That’s why we build **CI/CD** → to save time and reduce mistakes.

<img width="1676" height="263" alt="image" src="https://github.com/user-attachments/assets/012c529d-d6da-4dc1-a2c6-9edd2286ff7b" />

1. CI/CD ?

CI/CD = Continuous Integration / Continuous Delivery (or Deployment).
It’s the process of automating build, test, and release workflows.

2. Continuous Integration (CI)

Highlighted in yellow.

Means: build + test + verify.

Every time code is pushed (new feature, bug fix, etc.), CI automatically:

- Builds the code
- Runs tests
- Verifies everything still works

Goal → catch issues early and keep the main branch stable.

3. Continuous Delivery (CD)

Highlighted in blue.

After CI, the code is always ready to deploy.

But → a human decides when to push it live.

Example: CI pipeline prepares the build, runs tests, stores artifact → engineer presses “Deploy.”

4. Continuous Deployment (CD)

Also highlighted in blue.

After CI, code automatically goes live to users once it passes all tests.

No human button click needed.

Example: Push to main → CI runs → if green, it deploys straight to production.

5. Key Difference

Continuous Delivery → Ready for deployment, but manual release decision.
Continuous Deployment → Deployment is fully automated after tests.

👉 In short:

CI = build + test + verify
CD (Delivery) = package + ready to deploy (manual trigger)
CD (Deployment) = package + deploy + release (automatic to production)



## Level 1
<img width="1051" height="644" alt="image" src="https://github.com/user-attachments/assets/ca245474-4931-43bf-b16f-da04b0544120" />
Image source: ByteByteGo

## 🔄 Infinite Loop of DevOps
The pipeline is shown as an infinite loop because **CI/CD is continuous** — it never ends, it repeats with every code change.




---


## Level 2

