Here are the **official links (papers / docs / repos)** for the three well-known ML platform projects from Google, Uber, and Netflix that inspired modern MLOps systems.

---

# 1️⃣ Google – TensorFlow Extended (TFX)

**Research paper (Google Research):**
🔗 [https://research.google/pubs/tfx-a-tensorflow-based-production-scale-machine-learning-platform/](https://research.google/pubs/tfx-a-tensorflow-based-production-scale-machine-learning-platform/)

**Official documentation:**
🔗 [https://www.tensorflow.org/tfx](https://www.tensorflow.org/tfx)

TFX is an **end-to-end ML production platform** used at Google to standardize ML pipelines including data validation, feature engineering, model training, evaluation, and deployment. ([TensorFlow][1])

**GitHub repo:**
🔗 [https://github.com/tensorflow/tfx](https://github.com/tensorflow/tfx)

Why it’s important:

* Modular ML pipeline components
* Data validation + model validation gates
* Production orchestration

This paper explains **how Google moved ML from research to production pipelines**. ([Google Research][2])

---

# 2️⃣ Uber – Michelangelo

**Engineering blog (Uber Engineering):**
🔗 [https://www.uber.com/blog/scaling-michelangelo/](https://www.uber.com/blog/scaling-michelangelo/)

Michelangelo is Uber’s internal **ML-as-a-service platform** that lets teams build, deploy, and operate machine-learning models at scale across the company. ([Digital Data Design Institute at Harvard][3])

It supports:

* training pipelines
* feature store
* model registry
* deployment
* monitoring

Uber runs **thousands of production ML models and millions of predictions per second** using the platform. ([Uber][4])

---

# 3️⃣ Netflix – Metaflow

**Official documentation:**
🔗 [https://docs.metaflow.org](https://docs.metaflow.org)

**GitHub repository:**
🔗 [https://github.com/Netflix/metaflow](https://github.com/Netflix/metaflow)

Metaflow is a Python framework created at Netflix to **turn data-science experiments into production workflows easily**. ([docs.metaflow.org][5])

Key ideas:

* simple Python workflow steps
* infrastructure abstraction
* experiment tracking
* scaling from notebook → production

Netflix uses it internally to run **thousands of ML workflows and large-scale data jobs**. ([GitHub][6])

---

# Quick comparison (very useful for your project)

| Platform            | Focus                   | Key Idea                     |
| ------------------- | ----------------------- | ---------------------------- |
| TFX (Google)        | Production ML pipelines | standardized ML lifecycle    |
| Michelangelo (Uber) | ML platform             | experiment → deployment      |
| Metaflow (Netflix)  | Workflow framework      | notebook → scalable workflow |

---

💡 **Important insight for your project**

All three systems solve **production ML pipelines**, but **none automatically convert notebooks into pipelines**.

That’s exactly the **gap your agentic system can fill**:

```
Notebook
   ↓
Pipeline Extraction Agent
   ↓
Code Refactor
   ↓
Workflow Generator
   ↓
Production Pipeline
```

---

✅ If you want, I can also show you **5 open-source projects that tried to solve “Notebook → Pipeline automation” but failed or remained incomplete**.

Those will give you **very strong inspiration for your agentic implementation.**

[1]: https://www.tensorflow.org/tfx?utm_source=chatgpt.com "TFX | ML Production Pipelines  |  TensorFlow"
[2]: https://research.google/pubs/tfx-a-tensorflow-based-production-scale-machine-learning-platform/?utm_source=chatgpt.com "TFX: A TensorFlow-Based Production-Scale Machine Learning Platform"
[3]: https://d3.harvard.edu/platform-digit/submission/uber-knows-you-how-data-optimizes-our-rides/?utm_source=chatgpt.com "Uber knows you: how data optimizes our rides - Digital Innovation and Transformation"
[4]: https://www.uber.com/en-JM/blog/scaling-michelangelo/?utm_source=chatgpt.com "Scaling Machine Learning at Uber with Michelangelo | Uber Blog"
[5]: https://docs.metaflow.org/introduction/what-is-metaflow?utm_source=chatgpt.com "What is Metaflow | Metaflow Docs"
[6]: https://github.com/Netflix/metaflow?utm_source=chatgpt.com "GitHub - Netflix/metaflow: Build, Manage and Deploy AI/ML Systems"
