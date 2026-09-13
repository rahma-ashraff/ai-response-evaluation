---

# Mini Projects Case Study 3: AI Response Evaluation

* **Language:** Egyptian Arabic
* **Domain:** Customer Support
* **Task Type:** AI Response Evaluation
* **Evaluation Focus:** Instruction Following, Factual Accuracy, Tone, Relevance, and Completeness

---

### 1. User Prompt

> «أنا طلبت أوردر من الموقع من 5 أيام، وكان المفروض يوصل خلال 2 لـ3 أيام. لحد دلوقتي الأوردر موصلش، ولما بدخل أتابعه بيظهرلي "Out for Delivery". ممكن أعرف الأوردر هيوصل إمتى؟»

**Required Behavior**
The response should:
* Respond in natural Egyptian Arabic.
* Acknowledge the delivery delay.
* Avoid inventing an exact delivery time.
* Explain that "Out for Delivery" generally means the package is with the delivery carrier and is in the final delivery stage.
* Clearly communicate uncertainty about the exact arrival time.
* Provide a useful next step for the customer.

---

### 2. AI Response

> «أوردر حضرتك هيوصل النهارده الساعة 6 مساءً بالضبط، لأن حالة الأوردر بتقول Out for Delivery. لو موصلش الساعة 6، تواصلي مع شركة الشحن عشان تعرفي سبب التأخير.»

---

### 3. Evaluation

**Overall Assessment**
The response is understandable, relevant, and uses a natural conversational tone. However, it introduces an unsupported exact delivery time and incorrectly treats the "Out for Delivery" status as a guarantee of delivery at 6 PM. The main issue is factual grounding, not language quality.

**Errors Identified**

1. **Unsupported Specificity**
   * **Description:** The model claims that the order will arrive exactly at 6 PM, even though no information in the prompt supports this claim.
   * **Error Type:** Factual Grounding
   * **Severity:** High

2. **Misinterpretation of Order Status**
   * **Description:** "Out for Delivery" generally indicates that the package is with the delivery carrier and is in the final delivery stage. It does not guarantee a specific delivery time.
   * **Error Type:** Factual Interpretation
   * **Severity:** Medium

3. **Missing Uncertainty Handling**
   * **Description:** The response should explicitly acknowledge that the exact arrival time cannot be determined from the available information.
   * **Error Type:** Instruction Following / Uncertainty Handling
   * **Severity:** Medium

---

### 4. What the Model Did Well

* Used understandable and natural Egyptian Arabic.
* Directly addressed the customer's question.
* Maintained an appropriate customer-support tone.
* Provided a reasonable next step by suggesting contact with the shipping company.

---

### 5. Improved Response

> «معلش على التأخير، خصوصًا إن ميعاد التوصيل المتوقع كان من 2 لـ3 أيام.
> 
> حالة Out for Delivery معناها غالبًا إن الأوردر مع شركة الشحن وفي مرحلة التوصيل الأخيرة، لكن الحالة دي لوحدها مش بتحدد ميعاد وصول دقيق.
> 
> بما إن الأوردر متأخر عن المدة المتوقعة، الأفضل تتابعي مع شركة الشحن أو خدمة العملاء عشان تعرفي آخر تحديث على الأوردر وميعاد التوصيل المتوقع.»

**Why This Response Is Better**
The improved response:
* Acknowledges the delay without over-apologizing.
* Correctly interprets the "Out for Delivery" status.
* Does not invent an exact delivery time.
* Clearly communicates uncertainty.
* Gives the customer a practical next step.
* Remains natural and conversational in Egyptian Arabic.

---

### 6. Evaluation Scores

| Criterion | Score |
| :--- | :---: |
| Instruction Following | 3/5 |
| Factual Accuracy | 2/5 |
| Relevance | 5/5 |
| Tone | 5/5 |
| Completeness | 4/5 |
| **Overall Score** | **3.5/5** |

**Score Rationale**
The response performs well in tone, relevance, and general communication, but the unsupported claim about an exact delivery time is a significant factual-grounding error. Because the prompt explicitly required the model not to invent an exact delivery time, the Instruction Following score is also reduced.

---

### 7. Key Evaluation Insight

A response can be fluent, natural, and helpful in tone while still being factually ungrounded. In this example, the model correctly recognized that "Out for Delivery" is relevant to the delivery status, but it went beyond the available evidence by inventing a specific arrival time.

**Evaluator Takeaway:**
> *The model should not infer or invent information that is not present in the prompt or supported by the available order status.* 

This is particularly important in customer-support scenarios, where confident but unsupported information can create incorrect expectations and negatively affect the customer's experience.
