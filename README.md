# روبوت محادثة لمساعدة الطلاب في دورة Building AI

## Summary

يهدف هذا المشروع إلى بناء روبوت محادثة تفاعلي (Chatbot) باستخدام لغة Python لمساعدة الطلاب الجدد في الإجابة على الأسئلة الشائعة (FAQ) حول دورة **"Building AI"** المقدمة من جامعة هلسنكي و Reaktor.

يعتمد الروبوت على منهجية **استرجاع المعلومات (Retrieval-Based)** حيث يقوم بمطابقة أسئلة المستخدم مع قاعدة بيانات محددة من النوايا والإجابات (Intents and Responses) لتقديم ردود سريعة ودقيقة. الهدف هو تطبيق مفاهيم معالجة اللغات الطبيعية الأساسية التي تم تعلمها في الدورة.

## Features

1.  **تصنيف النوايا:** يحلل سؤال المستخدم لتحديد النية (Intent) الكامنة وراءه (مثل: `Project_Submission`، `Peer_Review`، `Course_Details`).
2.  **التطابق عبر TF-IDF:** يستخدم خوارزمية **TF-IDF (Term Frequency-Inverse Document Frequency)** لقياس **تشابه جيب التمام (Cosine Similarity)** بين المدخلات والأنماط المخزنة.
3.  **دقة في الردود:** يوفر إجابات مباشرة وموثوقة حول آليات القبول ومتطلبات التسليم وخطوات مراجعة الأقران.

## Technologies Used

| الأداة/المكتبة | الاستخدام |
| :--- | :--- |
| **Python** | لغة البرمجة الأساسية. |
| **Pandas** | تنظيم وهيكلة بيانات النوايا والإجابات. |
| **Scikit-learn** | تطبيق **TF-IDF** و **Cosine Similarity** لإيجاد التطابق. |

## How to Run

للتشغيل محلياً، اتبع الخطوات التالية:

1.  **استنساخ المستودع (Clone the Repository):**
    ```bash
    git clone [https://github.com/bella976/Ghatbot](https://github.com/bella976/Ghatbot)
    ```
2.  **تثبيت المكتبات:**
    ```bash
    pip install pandas scikit-learn
    ```
3.  **تشغيل الروبوت:**
    ```bash
    python chatbot.py 
    ```
