<div align="center">

<img src="https://upload.wikimedia.org/wikipedia/commons/3/38/Arduino_Uno_-_R3.jpg" width="180" style="border-radius:16px" alt="Arduino UNO"/>

<br/>

# ⚡ دليل برمجة الأردوينو ⚡ 

### صفحة تعليمية تفاعلية لورشة أردوينو — من الصفر إلى أول مشروع ذكي

<br/>

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-hoqsyber.github.io-00c8ff?style=for-the-badge&logoColor=white)](https://hoqsyber.github.io/intro-to-Arduino/)
[![HTML](https://img.shields.io/badge/HTML5-Pure-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://hoqsyber.github.io/intro-to-Arduino/)
[![CSS](https://img.shields.io/badge/CSS3-Animated-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://hoqsyber.github.io/intro-to-Arduino/)
[![Arduino](https://img.shields.io/badge/Arduino-Compatible-00979D?style=for-the-badge&logo=arduino&logoColor=white)](https://www.arduino.cc)
[![License](https://img.shields.io/badge/License-MIT-7b2fff?style=for-the-badge)](LICENSE)

<br/>

> **"كلما واجهت مشاكل أكثر، اكتسبت خبرة أكبر"** 💪

</div>

---

## 📌 نظرة عامة

هذه الصفحة هي **رفيقك الرقمي** خلال ورشة الأردوينو — مصممة بعناية لتكون مرجعاً شاملاً وتفاعلياً يأخذك من أول LED تُشغله حتى بناء نظام إنذار ذكي حقيقي.

```
📦 intro-to-Arduino
 ┣ 📄 index.html       ← الصفحة التعليمية الكاملة
 ┗ 📄 README.md        ← أنت هنا
```

---

## 🗂️ محتويات الصفحة

| # | القسم | الوصف |
|---|-------|--------|
| 01 | 🚀 **البداية** | تحميل Arduino IDE وكيفية استخدام الصفحة |
| 02 | 🔩 **القطع الإلكترونية** | تعرّف على كل قطعة بصورة وشرح تفصيلي |
| 03 | 🖥️ **Arduino IDE** | جولة كاملة في بيئة التطوير + القواعد الذهبية |
| 04 | 🔬 **التمارين التطبيقية** | 4 تمارين متدرجة من السهل للمركّب |
| 05 | 📋 **Cheat Sheet** | جميع الأوامر الأساسية في مكان واحد |
| 06 | 🛠️ **حل المشاكل** | أكثر 6 مشاكل شيوعاً وحلولها |
| 07 | 🌟 **بعد الورشة** | أفكار مشاريع + موارد للتعلم |

---

## 🔬 التمارين التطبيقية

<table>
<tr>
<td width="50%">

### 🟢 تمرين 01 — تشغيل LED
**المستوى:** سهل

تعلّم كيف تتحكم في نور بسيط — أساس كل شيء في الأردوينو.

```cpp
digitalWrite(ledPin, HIGH); // تشغيل
delay(1000);
digitalWrite(ledPin, LOW);  // إطفاء
delay(1000);
```

</td>
<td width="50%">

### 🔵 تمرين 02 — تشغيل Buzzer
**المستوى:** سهل

نفس مبدأ الـ LED — لكن بالصوت هذي المرة!

```cpp
digitalWrite(buzzerPin, HIGH); // صوت
delay(1000);
digitalWrite(buzzerPin, LOW);  // صمت
delay(1000);
```

</td>
</tr>
<tr>
<td width="50%">

### 🟡 تمرين 03 — حساس المسافة
**المستوى:** متوسط

اقرأ البيئة المحيطة باستخدام الموجات فوق الصوتية 📡

```cpp
duration = pulseIn(echoPin, HIGH);
distance = duration * 0.034 / 2;
Serial.println(distance);
```

</td>
<td width="50%">

### 🔴 تمرين 04 — نظام إنذار ذكي
**المستوى:** مركّب 🏆

دمج LED أحمر + أخضر + Buzzer + حساس مسافة في مشروع واحد متكامل!

```cpp
if (distance <= 15) {
  // تنبيه! جسم قريب
  digitalWrite(redLED, HIGH);
  digitalWrite(buzzer, HIGH);
}
```

</td>
</tr>
</table>

---

## ⚡ القطع المستخدمة

| القطعة | الوظيفة | الكمية |
|--------|---------|--------|
| 🤖 Arduino UNO | العقل الرئيسي للمشروع | 1 |
| 🔲 Breadboard | لوحة التوصيل بدون لحام | 1 |
| 💡 LED أخضر | مؤشر الحالة الآمنة | 1 |
| 💡 LED أحمر | مؤشر التنبيه | 1 |
| 🔊 Active Buzzer | صوت الإنذار | 1 |
| 📡 HC-SR04 | حساس المسافة بالموجات الصوتية | 1 |
| ⚡ مقاومة 220Ω | حماية الأنوار من التيار العالي | 3 |
| 🔌 أسلاك توصيل | ربط القطع ببعضها | متعدد |

---

## 🚀 كيفية التشغيل

**الطريقة الأولى — مباشرة من المتصفح:**

```bash
# افتح الرابط مباشرة
https://hoqsyber.github.io/intro-to-Arduino/
```

**الطريقة الثانية — تشغيل محلي:**

```bash
# 1. استنسخ المشروع
git clone https://github.com/HOQsyber/intro-to-Arduino.git

# 2. افتح المجلد
cd intro-to-Arduino

# 3. افتح الملف في المتصفح
start index.html        # Windows
open index.html         # Mac
xdg-open index.html     # Linux
```

> لا يحتاج إلى خادم أو مكتبات خارجية — يعمل مباشرة في المتصفح ✅

---

## ✨ مميزات الصفحة

- 🌙 **تصميم داكن** احترافي مريح للعين
- 📱 **متجاوب** — يعمل على الجوال والكمبيوتر
- ⚡ **أكواد قابلة للنسخ** بنقرة واحدة
- 🖼️ **صور حقيقية** لكل قطعة إلكترونية
- 🎯 **تحديات إضافية** في نهاية كل تمرين
- 🛠️ **دليل حل المشاكل** للأخطاء الشائعة
- 🔢 **شريط تقدم** يتتبع موضعك في الصفحة
- ✨ **أنيميشن** عند التمرير لتجربة سلسة

---


---

## 💡 مشاريع مقترحة بعد الورشة

<table>
<tr>
<th>المستوى</th>
<th>المشروع</th>
<th>القطع المطلوبة</th>
</tr>
<tr>
<td>🟢 مبتدئ</td>
<td>إشارة مرور بـ 3 أنوار</td>
<td>3x LED + أسلاك</td>
</tr>
<tr>
<td>🟢 مبتدئ</td>
<td>ميزان حرارة رقمي</td>
<td>DHT11 + شاشة LCD</td>
</tr>
<tr>
<td>🟡 متوسط</td>
<td>نظام ري آلي للنباتات</td>
<td>حساس رطوبة + مضخة</td>
</tr>
<tr>
<td>🟡 متوسط</td>
<td>مفتاح إضاءة بالتصفيق</td>
<td>حساس صوت + ريلاي</td>
</tr>
<tr>
<td>🔴 متقدم</td>
<td>سيارة ذاتية التجنّب</td>
<td>HC-SR04 + محركات + L298N</td>
</tr>
<tr>
<td>🔴 متقدم</td>
<td>منزل ذكي عبر الجوال</td>
<td>ESP8266 + تطبيق</td>
</tr>
</table>

---

## 📚 موارد التعلم

**المواقع:**
- 🌐 [arduino.cc](https://www.arduino.cc) — الموقع الرسمي
- 🎮 [tinkercad.com](https://www.tinkercad.com) — محاكاة الدوائر
- 📖 [randomnerdtutorials.com](https://randomnerdtutorials.com) — دروس شاملة

**يوتيوب عربي:**
- 📺 أكاديمية الأردوينو
- 📺 Arduino بالعربي

**يوتيوب إنجليزي:**
- 📺 Paul McWhorter
- 📺 DroneBot Workshop

---

## 👨‍💻 صاحب المشروع

<div align="center">

**Hashim Omar Alqassab**

[![GitHub](https://img.shields.io/badge/GitHub-HOQsyber-181717?style=for-the-badge&logo=github)](https://github.com/HOQsyber)

*طالب علوم حاسب — جامعة الإمام عبدالرحمن بن فيصل*

</div>

---

<div align="center">

⭐ إذا أفادك المشروع، لا تنسَ تعطيه نجمة!

</div>
