# Hyneto Energy Intelligence 🌟

<div dir="rtl">

**سیستم هوشمند‌سازی انرژی صنعتی | Industrial Energy Intelligence Platform**

---

## 🎯 درباره پروژه

یک **دمو تعاملی، تمام‌عیار و حرفه‌ای** برای هوشمند‌سازی و نظارت بلادرنگ مصرف انرژی در صنایع و کارخانه‌ها.

### ✨ ویژگی‌های برجسته:

#### 🔋 **منابع انرژی چندگانه**
- ☀️ **پنل‌های خورشیدی** (Photovoltaic) - 120 kWp
- 🔌 **برق شبکه** (Grid Power) - 240 kW
- 🔋 **سیستم UPS** - Uninterruptible Power Supply
- 🔥 **ژنراتور دیزلی** - Backup Power
- **نمودارهای تعاملی** برای هر منبع

#### ⚙️ **10 دستگاه صنعتی واقع‌بینانه**
- کمپرسور (2 خط)
- دستگاه CNC (A & B)
- سیستم HVAC
- نوار نقاله
- ایستگاه جوشکاری
- پمپ آب
- سیستم روشنایی
- تهویه رنگ

#### 📊 **داشبورد جامع**
- **5 KPI اصلی**: مصرف فعلی، انرژی انباشته، سهم تجدیدپذیر، بهره‌وری، تعداد هشدارها
- **نمودارهای زنده**: تاریخچه مصرف ساعتی + توزیع منابع
- **معیارهای استاندارد صنعتی**:
  - PUE (Power Usage Effectiveness)
  - Carbon Footprint
  - Peak-to-Average Ratio
- **سیستم هشدار هوشمند** (بحرانی، اخطار، متوسط)

#### 🌍 **دو‌زبانه**
- 🇮🇷 فارسی (RTL)
- 🇬🇧 انگلیسی (LTR)
- تبدیل فوری در رابط‌کاربری

#### 📱 **واکنشگرا بر تمام دستگاه‌ها**
- موبایل (480px+)
- تبلت (768px+)
- دسکتاپ (1200px+)

#### 🎨 **طراحی حرفه‌ای**
- رنگ‌های متمایز برای هر منبع
- انیمیشن‌های ملایم
- Glassmorphism + Dark Mode
- رابط کاربری بدون بالا‌رفتگی

#### ⚡ **عملکرد بالا**
- بدون Framework (Vanilla JavaScript)
- بروزرسانی بلادرنگ هر 3 ثانیه
- Chart.js برای نمودارهای بهینه

---

## 🚀 شروع سریع

### 1️⃣ دانلود یا Clone کردن

```bash
git clone https://github.com/OpportunityHub-Hyneto/hyneto-energy-intelligence.git
cd hyneto-energy-intelligence
```

### 2️⃣ اجرا

**روش 1: مستقیم باز کردن فایل**
```bash
# فایل را در مرورگر باز کنید
open index.html
```

**روش 2: محلی با Server (توصیه‌شده)**
```bash
# Python 3
python -m http.server 8000

# یا Node.js (http-server)
npx http-server

# سپس به این آدرس بروید:
# http://localhost:8000
```

### 3️⃣ استفاده

- **سوئیچ زبان**: دکمه "فارسی / English" در گوشه‌ی بالا سمت راست
- **نمایش جزئیات**: روی KPI، منابع، یا دستگاه‌ها کلیک کنید
- **مشاهده بخش‌ها**: از سایدبار navigation استفاده کنید
- **پیشرو**: نمودارها و هشدارها بلادرنگ به‌روز می‌شوند

---

## 📂 ساختار پروژه

```
hyneto-energy-intelligence/
├── index.html              # فایل اصلی (تمام کد در یک فایل)
├── README.md              # این فایل
├── LICENSE                # مجوز MIT
├── CHANGELOG.md           # تاریخچه تغییرات
└── docs/                  # اسناد اضافی
    ├── FEATURES.md        # فهرست ویژگی‌ها
    ├── INSTALLATION.md    # راهنمای نصب
    └── API.md             # توثیق API (اختیاری)
```

---

## 🎓 نمایش برنامه

### 🎪 عملکرد‌های تعاملی:

| عملکرد | شرح |
|--------|------|
| **کلیک روی KPI** | باز شدن Modal با جزئیات |
| **کلیک روی منابع انرژی** | نمایش وضعیت و آمار |
| **کلیک روی دستگاه** | مشخصات تفصیلی ماشین |
| **سوئیچ زبان** | تغییر فوری تمام متن‌ها |
| **ناوبری سایدبار** | جهش صاف به بخش‌ها |

### 📊 داده‌های نمایشی:

تمام داده‌ها **بلادرنگ تولید می‌شوند** و شامل:
- مصرف دینامیکی دستگاه‌ها
- تشخیص خودکار ناهنجاری‌ها (5 نوع)
- تاریخچه حرارتی
- هشدارهای ترتیبی

---

## 🛠️ فناوری‌های استفاده‌شده

```
Frontend:
- HTML5
- CSS3 (Grid, Flexbox, Gradients, Animations)
- Vanilla JavaScript (ES6+)
- Chart.js 4.4.1 (نمودارها)
- GSAP 3.12.2 (انیمیشن‌ها)

Fonts:
- Vazirmatn (فارسی)
- Syne (انگلیسی)

Browser Support:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)
```

---

## 🎨 رنگ و Design System

### Color Palette:
```css
--accent-cyan: #00d4ff       /* آبی روشن */
--accent-blue: #2563eb       /* آبی تیره */
--accent-purple: #7c3aed     /* بنفش */
--accent-green: #10b981      /* سبز */
--alert-red: #ef4444         /* قرمز هشدار */
--warning-orange: #f97316    /* نارنجی */
--solar-yellow: #eab308      /* زرد خورشید */
--ups-purple: #a855f7        /* بنفش UPS */
--gen-orange: #f97316        /* نارنجی ژنراتور */
```

### Typography:
- **Display**: Syne 800 (عنوان‌ها)
- **Body**: Vazirmatn 400-600 (متن‌ها)
- **Mono**: Courier New (داده‌های عددی)

---

## 📈 اقتصادی‌سازی انرژی - مثال‌های عملی

### 🔍 کاربرد‌های عملی:
1. **نظارت بلادرنگ** → تشخیص مصرف اضافی
2. **بهینه‌سازی منابع** → ترجیح انرژی تجدیدپذیر
3. **پیشگویی و نگهداری** → جلوگیری از خرابی
4. **تقلیل هزینه** → کاهش صورت‌حساب برق
5. **پایداری محیطی** → کاهش CO₂

### 💰 بخش‌های قابل صرفه‌جویی:
- شناسایی دستگاه‌های تحت‌بار
- بهینه‌سازی جدول کاری
- بهره‌بری از انرژی تجدیدپذیر (خورشید)
- مدیریت UPS و دیزل

---

## 🔧 توسعه و Customization

### تغییر داده‌های نمایشی:

```javascript
// فایل: index.html (خط ~244-255)
const MACHINES = [
  { 
    id: 'M01', 
    name: 'دستگاه جدید', 
    baseline: 50, 
    max: 80 
  },
  // ... سایر دستگاه‌ها
];
```

### اضافه کردن منابع انرژی جدید:

```javascript
// فایل: index.html (خط ~312+)
energySources = {
  solar: { ... },
  grid: { ... },
  // منبع جدید:
  wind: { name: 'Wind', power: 50, max: 100 }
};
```

### تغییر رنگ‌ها:

```css
/* فایل: index.html (خط ~11-25) */
:root {
  --accent-cyan: #00d4ff;  /* رنگ جدید */
  --bg-primary: #08111f;
  /* ... */
};
```

---

## 📝 استانداردهای صنعتی

### PUE (Power Usage Effectiveness)
```
PUE = Total Facility Power / IT Equipment Power
تفسیر:
- 1.0 = کامل (غیرممکن)
- 1.5 = ممتاز
- 1.67 = متوسط
- 2.0+ = ضعیف
```

### Carbon Footprint
```
CO₂ = Energy (kWh) × Grid Emission Factor (0.436 kg/kWh in Iran)
```

### Peak-to-Average Ratio
```
PAR = Maximum Load / Average Load
نسبت‌های بالا = نوسانات شدید = نیاز برای مدیریت
```

---

## 🐛 مشکلات و خطاها

### مشکل: نمودارها نمایش نمی‌دهند
**راه‌حل:**
- بررسی کنسول (F12 → Console)
- اطمینان از اتصال اینترنت (CDN)
- Refresh صفحه (Ctrl+F5)

### مشکل: زبان فارسی درست نمایش نمی‌دهند
**راه‌حل:**
- فونت Vazirmatn نیاز به بارگذاری از Google Fonts
- بررسی اتصال و Cache

---

## 🤝 مشارکت و بهبود

ما خوشحال می‌شویم از مشارکت‌های شما!

1. **Fork** کردن این Repository
2. **Branch** جدید برای ویژگی: `git checkout -b feature/new-feature`
3. **Commit** تغییرات: `git commit -m 'Add new feature'`
4. **Push** به Branch: `git push origin feature/new-feature`
5. **Pull Request** ارسال

---

## 📄 مجوز

این پروژه تحت مجوز **MIT** منتشر شده است.

```
MIT License

Copyright (c) 2025 Opportunity Hub B.V. (Hyneto)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## 👨‍💼 درباره ما

**Hyneto** - Opportunity Hub B.V.

🌍 **مقر**: The Hague, Netherlands  
🌐 **وب‌سایت**: [hyneto.com](https://hyneto.com)  
📧 **ایمیل**: info@hyneto.com  
🔗 **GitHub**: [@opportunityhub-hyneto](https://github.com/OpportunityHub-Hyneto)

**ما در زمینه‌های زیر متخصص هستیم:**
- 🔌 هوشمند‌سازی انرژی صنعتی
- 🤖 اتوماسیون هوش‌مصنوعی
- ☁️ Infrastructure و Cloud
- 🌉 پل میان اروپا و خاورمیانه

---

## 📞 تماس و پشتیبانی

- **Issues**: برای گزارش مشکلات
- **Discussions**: برای سوالات و پیشنهادات
- **Email**: support@hyneto.com

---

## 🎉 قدردانی

تشکر از استفاده‌کنندگان و مشارکین ما!

</div>

---

**Built with ❤️ by Hyneto Team**

Last Updated: 2025-05-18
