# AI Response Evaluation - Case Study #01

## 📌 Task Overview
* **Domain:** Food & Culinary Marketing / Content Creation
* **Language:** Arabic (AR)
* **Task Type:** Side-by-Side (SdS) Model Evaluation

---

## 📝 User Prompt
> "اكتب لي خطة تسويقية بسيطة لمحل مخبوزات في القاهرة. الشروط: أن تكون الخطة في 3 نقاط فقط، تتضمن فكرة مسابقة على الفيسبوك، وأن لا تتجاوز الإجابة 60 كلمة."

---

## 🤖 Model Responses

### Model A
> * **التسويق الرقمي ومسابقة فيسبوك:** إطلاق مسابقة "شاركنا حبك للمخبوزات و اكسب" حيث يشارك المتابعون صور مخبوزاتهم مع إشارة لصفحة المحل لربح جائزة اسبوعية.
> * **الشراكات المحلية:** تقديم بوكسات فطار صغيرة للشركات والمكاتب القريبة بسعر خاص، مع عرض "اطلب 10 بوكسات واحصل على 2 مجانًا".
> * **العروض الموسمية:** تقديم خصم 15% على طلبات التوصيل للعملاء الجدد في القاهرة.

### Model B
> أهلًا بك، إليك خطة تسويقية لمحل المخبوزات:
> 
> * **عروض التذوق:** توزيع عينات طازجة للمارة لجذب الزبائن وتجربة المنتجات.
> * **مسابقة فيسبوك:** مشاركة منشور المحل مع الإشارة لأصدقاء للفوز بصندوق مخبوزات.
> * **خصومات الشركات:** استهداف المكاتب المجاورة بعروض إفطار صباحية مخصصة.
> * **إعلانات ممولة:** الترويج عبر منصات التواصل لجميع سكان المنطقة المجاورة.
> 
> أتمنى لك التوفيق.

---

## 📊 Evaluation Matrix

| Evaluation Criterion | Model A | Model B |
| :--- | :--- | :--- |
| **Instruction Following** | **Pass (Excellent):** Follows all explicit constraints (exactly 3 points, includes a Facebook contest, and stays under the 60-word limit). | **Fail:** Violates an explicit structural constraint by generating 4 points instead of the requested 3. |
| **Truthfulness & Logic** | **Pass:** Practical and logically sound marketing steps tailored for a local bakery. | **Pass:** Marketing suggestions are practical and logically sound. |
| **Formatting & Conciseness** | **Pass:** Direct, concise, and structured without any conversational filler. | **Minor Issue:** Adds unrequested conversational filler (introductory and closing phrases). |

---

## 🏆 Final Preference & Justification

* **Preference:** `Model A is Much Better Than Model B`

### Detailed Justification
> Model A strictly adhered to all explicit constraints: it provided exactly 3 marketing points, incorporated a Facebook contest idea, localized the context to Cairo, and remained concise at 55 words (well under the 60-word limit).
>
> Model B failed an explicit structural constraint by providing 4 bullet points instead of 3. Furthermore, it included unnecessary conversational filler ("أهلًا بك، إليك خطة تسويقية..." and "أتمنى لك التوفيق"), which compromises output conciseness.
>
> Because Model A demonstrates full constraint compliance while Model B violates structural instructions, Model A is preferred.
