<div align="center">

# 🔗 URL Encoder / Decoder — أداة تشفير وفك تشفير الروابط

**تعمل على نظام Kali Linux و تطبيق Termux**

꧁ঔৣ☬ Muhannad Daher ☬ঔৣ꧂

---

![Version](https://img.shields.io/badge/Version-1.0-blue?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Kali_Linux-green?style=for-the-badge&logo=kalilinux)
![Platform](https://img.shields.io/badge/Platform-Android-green?style=for-the-badge&logo=android)
![Python](https://img.shields.io/badge/Python-3.x-yellow?style=for-the-badge&logo=python)
![License](https://img.shields.io/badge/License-MIT_License-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

---

**المحتويات:**

</div>

- [الوصف](#الوصف)
- [المميزات](#المميزات)
- [التثبيت على Termux](#التثبيت-على-termux)
- [التثبيت على Kali Linux](#التثبيت-على-kali-linux)
- [التشغيل](#التشغيل)
- [طريقة الاستخدام](#طريقة-الاستخدام)
- [مثال](#مثال)
- [المتطلبات](#المتطلبات)
- [إخلاء المسؤولية](#إخلاء-المسؤولية)
- [المطوّر](#المطوّر)

---

<div align="center" id="الوصف">

## 📌 الوصف

</div>

أداة شاملة لتشفير وفك تشفير النصوص والروابط بأشهر الطرق، مكتوبة بلغة Python وتعمل على Termux و Kali Linux. تدعم URL و Base64 و HTML و Hex مع تحليل الروابط الكاملة.

---

<div align="center" id="المميزات">

## ✨ المميزات

</div>

- 🔗 URL Encode / Decode (مع دعم + للمسافات)
- 🔐 Base64 Encode / Decode
- 🌐 HTML Encode / Decode
- 🔢 Hex Encode / Decode
- 🔍 تحليل رابط URL كامل (بروتوكول, نطاق, مسار, معاملات)
- ⚡ تشفير بكل الطرق دفعة واحدة
- 🌍 واجهة عربية بالكامل

---

<div align="center" id="التثبيت-على-termux">

## ⚙️ التثبيت

### Termux

</div>

**الخطوة 1 — تحديث النظام**
```bash
pkg update && pkg upgrade -y
```

**الخطوة 2 — تثبيت المتطلبات** *(لمرة واحدة فقط)*
```bash
pkg install python tor curl fontconfig rust -y
```
```bash
pip install requests pysocks arabic-reshaper
pip install python-bidi==0.4.2
```

**الخطوة 3 — تثبيت الخط العربي** *(لمرة واحدة فقط)*
```bash
curl -L "https://fonts.gstatic.com/s/notonaskharabic/v33/RrQ5bpV-9Dd1b1OAGA6M9PkyDuVBePeKNaxcsss0Y7bwvc-VaA.ttf" -o ~/.termux/font.ttf
termux-reload-settings
```

**الخطوة 4 — تنزيل الأداة**
```bash
curl -o $PREFIX/bin/mud_ue.py https://raw.githubusercontent.com/mmuhacker/mud-ue/main/mud_ue.py
```

**الخطوة 5 — إعطاء صلاحية التشغيل**
```bash
chmod +x $PREFIX/bin/mud_ue.py
```

**الخطوة 6 — إنشاء رابط الاختصار**
```bash
ln -sf $PREFIX/bin/mud_ue.py $PREFIX/bin/ue
```

**⚡ أو قم بكل شيء بأمر واحد مجمّع**
```bash
pkg update && pkg upgrade -y && pkg install python tor curl fontconfig rust -y && pip install requests pysocks arabic-reshaper && pip install python-bidi==0.4.2 && curl -L "https://fonts.gstatic.com/s/notonaskharabic/v33/RrQ5bpV-9Dd1b1OAGA6M9PkyDuVBePeKNaxcsss0Y7bwvc-VaA.ttf" -o ~/.termux/font.ttf && termux-reload-settings && curl -o $PREFIX/bin/mud_ue.py https://raw.githubusercontent.com/mmuhacker/mud-ue/main/mud_ue.py && chmod +x $PREFIX/bin/mud_ue.py && ln -sf $PREFIX/bin/mud_ue.py $PREFIX/bin/ue && ue
```

---

<div align="center" id="التثبيت-على-kali-linux">

### Kali Linux

</div>

**الخطوة 1 — تحديث النظام**
```bash
sudo apt update && sudo apt upgrade -y
```

**الخطوة 2 — تثبيت المتطلبات** *(لمرة واحدة فقط)*
```bash
pip install requests arabic-reshaper python-bidi==0.4.2 --break-system-packages
```

**الخطوة 3 — تنزيل الأداة**
```bash
sudo curl -o /usr/local/bin/mud_ue.py https://raw.githubusercontent.com/mmuhacker/mud-ue/main/mud_ue.py
```

**الخطوة 4 — إعطاء صلاحية التشغيل**
```bash
sudo chmod +x /usr/local/bin/mud_ue.py
```

**الخطوة 5 — إنشاء رابط الاختصار**
```bash
sudo ln -sf /usr/local/bin/mud_ue.py /usr/local/bin/ue
```

**⚡ أو قم بكل شيء بأمر واحد مجمّع**
```bash
sudo apt update && sudo apt upgrade -y && pip install requests arabic-reshaper python-bidi==0.4.2 --break-system-packages && sudo curl -o /usr/local/bin/mud_ue.py https://raw.githubusercontent.com/mmuhacker/mud-ue/main/mud_ue.py && sudo chmod +x /usr/local/bin/mud_ue.py && sudo ln -sf /usr/local/bin/mud_ue.py /usr/local/bin/ue && ue
```

---

<div align="center" id="التشغيل">

## 🚀 التشغيل

</div>

```bash
ue
```

**أو بالأمر الكامل**

```bash
mud_ue.py
```

---

<div align="center" id="طريقة-الاستخدام">

## 📖 طريقة الاستخدام


| الوضع | الوصف |
|-------|-------|
| `1` URL | تشفير/فك تشفير روابط URL |
| `2` Base64 | تشفير/فك تشفير Base64 |
| `3` HTML | تشفير/فك تشفير HTML |
| `4` Hex | تشفير/فك تشفير Hex |
| `5` تحليل رابط | تفكيك رابط URL كامل |
| `6` الكل دفعة | تشفير أو فك تشفير بكل الطرق مرة واحدة |

</div>

---

<div align="center" id="مثال">

## 💡 مثال

</div>


اختيارك: 6

أدخل النص: hello world

اختر الاتجاه: 1 (تشفير)
<div align="center">

  URL Encode:    hello%20world
  
  Base64:        aGVsbG8gd29ybGQ=
  
  HTML Encode:   hello world
  
  Hex:           68656c6c6f20776f726c64
  
  </div>
  
---


اختيارك: 5

أدخل الرابط: 

https://example.com/path?name=test&id=1#section

<div align="center">
  
  البروتوكول    https
  
  النطاق        example.com
  
  المسار        /path
  
  المعاملات     name=test&id=1
  
  الجزء         section

  المعاملات مفككة:
name = test
    
id   = 1

</div>

---

<div align="center" id="المتطلبات">

## 🔧 المتطلبات


| المتطلب | الوصف |
|---------|-------|
| Python 3.6+ | لغة البرمجة |
| arabic-reshaper | دعم النص العربي |
| python-bidi | اتجاه النص العربي |
| curl | تنزيل الأداة |

</div>

> ⚠️ **ملاحظة:** بدون تثبيت `arabic-reshaper` و `python-bidi` سيظهر النص العربي معكوساً ومتقطعاً.

---

<div align="center" id="إخلاء-المسؤولية">

## ⚖️ إخلاء المسؤولية

</div>

هذه الأداة مخصصة **لأغراض تعليمية فقط**.
لا تستخدمها لأغراض غير مشروعة.

---

<div align="center" id="المطوّر">

## 👨‍💻 المطوّر

**Muhannad Daher**

[![GitHub](https://img.shields.io/badge/GitHub-mmuhacker-black?style=for-the-badge&logo=github)](https://github.com/mmuhacker)

---

***Madarik Tools — صُنع بالعربية***

⭐ **إذا أعجبتك الأداة، لا تنسَ النجمة!** ⭐

</div>

