# Task 4: Single-Response Evaluation (Instruction Following & Policy Assumptions)

## Task Overview
* **Domain:** Customer Service / Online Retail
* **Language:** English (EN)
* **Task Type:** AI Response Evaluation (Single Response)
* **Evaluation Focus:** Instruction Following, Relevance, Empathy, Accuracy, and Completeness

---

## 1. User Prompt

> «I received my package today, but the product is damaged. I want a refund, not a replacement. What should I do?»

---

## 2. AI Response

> «We're sorry that your product arrived damaged. We can send you a replacement immediately. Please send us a photo of the damaged item and we'll arrange the replacement for you.»

---

## 3. Evaluation

**Overall Assessment**
The response is polite and recognizes the damaged product, but it fails to follow the customer's explicit request for a refund and instead offers a replacement. The primary issue is ignoring explicit user constraints.

**Errors Identified**

1. **Failure to Follow the Customer's Request**
   * **Description:** The customer specifically requested a refund rather than a replacement. The AI responds by offering only a replacement.
   * **Error Type:** Instruction Following
   * **Severity:** High

2. **Incomplete Resolution**
   * **Description:** The response does not explain what the customer should do to request a refund or what information may be needed to proceed.
   * **Error Type:** Helpfulness / Completeness
   * **Severity:** Medium

3. **Unsupported Policy Assumption**
   * **Description:** The AI states that a replacement can be arranged immediately, even though no company return, replacement, or refund policy is provided in the prompt context.
   * **Error Type:** Unsupported Assumption
   * **Severity:** Medium

---

## 4. What the Model Did Well

* Acknowledged the damaged item promptly.
* Used an appropriate, sympathetic, and professional tone.
* Requested a photo, which is relevant for documenting the physical damage.

---

## 5. Improved Response

> «I'm sorry that your product arrived damaged. Since you'd prefer a refund rather than a replacement, please contact the support team to request a refund and ask about the required steps.
> 
> Keep the damaged item and its packaging, and provide a photo of the damage if requested. The support team can confirm the refund process and any applicable requirements.»

---

## 6. Evaluation Scores

| Criterion | Score |
| :--- | :---: |
| Instruction Following | 2/5 |
| Relevance | 4/5 |
| Empathy & Tone | 4/5 |
| Accuracy | 3/5 |
| Completeness | 3/5 |
| **Overall Score** | **3.0/5** |

---

## 7. Key Evaluation Insight

The AI recognized the customer's problem and maintained a polite tone, but it failed to address the customer's actual request for a refund. It also introduced a replacement option without having any information about the company's actual refund or replacement policy.

**Evaluator Takeaway:**
> *A customer-service AI should prioritize the customer's explicit request and avoid assuming company policies that are not provided in the available information.*

A response can be polite and relevant while still failing the most important requirement: following the customer's explicit instruction.
