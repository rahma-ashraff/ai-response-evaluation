# AI Response Evaluation - Case Study #02

## 📌 Task Overview
* **Domain:** History & Science
* **Language:** English (EN)
* **Task Type:** Side-by-Side (SdS) Model Evaluation

---

## 📝 User Prompt
> "When did the Apollo 11 moon landing occur, and who were the three astronauts on board? Mention two primary lunar samples brought back, keeping your response concise."

---

## 🤖 Model Responses

### Model A
> The Apollo 11 moon landing occurred on July 20, 1969. The three crew members were Neil Armstrong, Buzz Aldrin, and Michael Collins. The mission brought back primary lunar samples including basalt rocks and lunar soil (regolith).

### Model B
> The Apollo 11 landing took place on July 20, 1975. The astronauts on board were Neil Armstrong, Yuri Gagarin, and Buzz Aldrin. They brought back moon rocks and alien fossils.

---

## 📊 Evaluation Matrix

| Evaluation Criterion | Model A | Model B |
| :--- | :--- | :--- |
| **Instruction Following** | **Pass (Excellent):** Addressed all sub-questions accurately while maintaining conciseness. | **Fail:** Failed to satisfy the prompt's core factual requirements despite attempting the structural parts. |
| **Truthfulness & Factuality** | **Pass (Accurate):** Fully accurate date (July 20, 1969), crew roster, and verified lunar samples. | **Fail (Severe Hallucination):** Contains critical factual errors (wrong year: 1975, wrong astronaut: Yuri Gagarin) and an unsupported/fabricated claim ("alien fossils"). |
| **Formatting & Tone** | **Pass:** Clear, direct, and concise structure. | **Pass (Structural):** Clear and concise layout, though completely invalidated by factual falsehoods. |

---

## 🏆 Final Preference & Justification

* **Preference:** `Model A is Much Better Than Model B`

### Detailed Justification
> Model A provided complete factual accuracy across all requested dimensions: the landing date (July 20, 1969), the three crew members (Armstrong, Aldrin, Collins), and legitimate lunar samples (basalt and regolith), all while remaining concise.
>
> Model B failed significantly across both instruction following and factuality. It generated severe hallucinations: stating the incorrect year (1975 instead of 1969), misidentifying Soviet cosmonaut Yuri Gagarin as an Apollo 11 astronaut, and making an unsupported/fabricated claim that astronauts returned with "alien fossils." In human preference evaluation benchmarks, severe factual hallucinations completely invalidate a model's response. Therefore, Model A is much better.
