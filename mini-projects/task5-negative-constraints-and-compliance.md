# Task 5: Side-by-Side Evaluation (Negative Constraints & Policy Compliance)

## Task Overview
* **Domain:** Customer Service (E-Commerce & Aviation)
* **Language:** English (EN)
* **Task Type:** Side-by-Side (SdS) Model Evaluation (Multi-Case)
* **Evaluation Focus:** Negative Constraints, Instruction Following, Hallucination/Policy Assumptions

---

## Example 1: Damaged Shipment Email

### 1. User Prompt

> «Write a customer support email responding to a customer who received a shattered ceramic vase. Constraints: Apologize sincerely, ask for a photo of the damaged item, offer the choice between a full refund or a free replacement, do NOT offer store credit or discount codes, and keep the response under 70 words.»

---

### 2. Model Responses

#### Model A
> Dear Customer,
> I am truly sorry to hear that your ceramic vase arrived damaged.
> Please reply to this email with a photo of the damaged item and its packaging. Once received, let us know if you would prefer a full refund to your original payment method or a free replacement shipped immediately.
> We appreciate your patience and apologize for the inconvenience.
> 
> *(Word count: 61 words)*

#### Model B
> Dear Valued Customer,
> We are so sorry your vase broke! To make up for this trouble, we can offer you store credit for your next order, or we can send you a free replacement right away. We can also include a 15% discount code for your next purchase.
> Please send us a picture of the broken vase when you can.
> 
> *(Word count: 59 words)*

---

### 3. Evaluation & Rating

| Evaluation Criterion | Model A | Model B |
| :--- | :--- | :--- |
| **Instruction Following** | **Pass:** Included all required details, followed the negative constraint by not offering store credit or discount codes, and stayed under 70 words. | **Fail:** Violated the explicit negative constraint by offering both store credit and a discount code. |
| **Tone & Professionalism** | **Pass:** Empathetic, polite, and professional. | **Pass:** Polite and appropriate in tone, despite failing an important instruction. |
| **Formatting** | **Pass:** Clean email structure. | **Pass:** Clean email structure. |

---

### 4.  Final Preference & Justification

**Preference:** `Model A is Much Better than Model B`

#### Justification
Model A followed every instruction, including the explicit negative constraint: *"do NOT offer store credit or discount codes."* It provided the two requested options, asked for a photo of the damaged item, and remained within the 70-word limit.

Model B violated a critical constraint by explicitly offering store credit and a 15% discount code. Although its tone and formatting were acceptable, the instruction-following failure makes Model A significantly better.

---

## Example 2: Airline Cancellation Chat Response

### 1. User Prompt

> «Draft a customer service live chat response for an airline customer whose flight was canceled due to sudden severe weather. Constraints: State that safety is the top priority, explain how to rebook via the mobile app, offer a complimentary meal voucher, do NOT promise cash compensation, and structure the response using exactly 3 bullet points.»

---

### 2. Model Responses

#### Model A
> * We sincerely apologize for the cancellation; severe weather has affected the flight, and your safety is our absolute top priority.
> * You can rebook your flight through the "Manage Booking" section of our mobile app.
> * Please contact our airport desk to receive a complimentary meal voucher while you await your updated departure.
> 
> *(Word count: 51 words)*

#### Model B
> * We apologize for canceling your flight due to bad weather, but keeping you safe is our top priority.
> * You can easily rebook your new flight through our official mobile app under "Manage Booking".
> * To compensate for your delay, our team will process a $200 cash reimbursement to your account and send a free meal voucher to your email.

---

### 3. Evaluation & Rating

| Evaluation Criterion | Model A | Model B |
| :--- | :--- | :--- |
| **Instruction Following** | **Pass:** Used exactly 3 bullet points, stated that safety is top priority, explained how to rebook through the app, offered a meal voucher, and avoided cash compensation promises. | **Fail:** Violated the explicit negative constraint by promising a $200 cash reimbursement. |
| **Accuracy & Grounding** | **Pass:** Stays within the provided constraints without introducing unsupported compensation or procedural details. | **Fail:** Introduces a specific $200 cash reimbursement that was not requested or supported by the prompt. |
| **Formatting** | **Pass:** Uses exactly 3 bullet points as requested. | **Pass:** Uses exactly 3 bullet points as requested. |

---

### 4.  Final Preference & Justification

**Preference:** `Model A is Much Better than Model B`

#### Justification
Model A follows all of the explicit requirements without introducing unsupported claims. It states that safety is the top priority, explains how to rebook through the mobile app, offers a complimentary meal voucher, and avoids promising cash compensation.

Model B follows several of the requested instructions, but it violates a critical negative constraint by promising a "$200 cash reimbursement." The prompt explicitly instructed the model not to promise cash compensation, making this a clear instruction-following failure.

---

## Evaluator Takeaways & Key Principles

* **Negative Constraints are Critical:** Negative constraints are explicit requirements. A response can be polite, professional, and relevant while still failing if it violates a clearly stated restriction.
* **Grounding vs. External Assumptions:** Evaluate responses strictly against the provided evidence and constraints. Do not introduce external policy or legal assumptions when the prompt does not provide enough information to support them.

> **Key Evaluation Principle:** A strong AI response is not only fluent and helpful. It must follow the user's explicit instructions, respect negative constraints, and avoid introducing unsupported information.
