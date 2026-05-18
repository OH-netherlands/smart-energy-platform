<div dir="rtl">

# راهنمای مشارکت 🤝

اول از همه، از علاقه شما به کمک برای بهتر کردن Hyneto Energy Intelligence تشکر می‌کنیم!

## نحوه مشارکت

### 1️⃣ Report کردن مشکلات (Bug Report)

اگر مشکلی پیدا کردید:

1. **Issue جدید باز کنید**
2. **عنوان واضح بنویسید**: مثلاً "نمودار در Mobile نمایش نمی‌دهد"
3. **جزئیات مشخص کنید**:
   - مرورگر و نسخه
   - سیستم‌عامل
   - مراحل تکرار مشکل
   - رفتار مورد انتظار
   - رفتار واقعی

**مثال:**
```
## مشکل
نمودار مصرف در صفحه موبایل نمایش نمی‌دهد

## مرورگر
Chrome Mobile v125

## مراحل تکرار
1. دستگاه موبایل را مقلوب کنید
2. صفحه را Refresh کنید
3. نمودار نمایش نمی‌دهد

## رفتار مورد انتظار
نمودار باید در تمام اندازه‌ها نمایش داده شود

## رفتار واقعی
نمودار خالی است
```

### 2️⃣ ویژگی‌های جدید (Feature Request)

برای پیشنهاد ویژگی جدید:

1. **Discussions را بررسی کنید** تا مطمئن شوید که قبلاً پیشنهاد نشده
2. **Issue جدید با برچسب `enhancement` باز کنید**
3. **شرح واضح بنویسید**:
   - چرا این ویژگی مورد نیاز است؟
   - چگونه باید کار کند؟
   - مثال‌های عملی

### 3️⃣ Pull Request (PR)

#### قبل از شروع:
```bash
# Fork کنید (در گیت‌هاب)
# Clone کنید
git clone https://github.com/YOUR_USERNAME/hyneto-energy-intelligence.git
cd hyneto-energy-intelligence

# Branch جدید بسازید
git checkout -b feature/your-feature-name
```

#### بهترین عملکردها:

1. **یک ویژگی = یک Branch**
   - ❌ نه: `git checkout -b bugfix-everything`
   - ✅ بله: `git checkout -b fix/modal-animation-mobile`

2. **Commit messages واضح**
   ```
   ✅ بله:
   - "fix: correct chart responsiveness on mobile"
   - "feat: add new solar efficiency metric"
   - "docs: update installation guide"
   
   ❌ نه:
   - "fixed stuff"
   - "updates"
   - "asdf"
   ```

3. **کد مرتب و documented**
   ```javascript
   // ❌ نه:
   function f(a,b){return a+b}
   
   // ✅ بله:
   /**
    * محاسبه کل مصرف انرژی
    * @param {number} solar - مصرف خورشید
    * @param {number} grid - مصرف شبکه
    * @returns {number} مصرف کل
    */
   function calculateTotalConsumption(solar, grid) {
     return solar + grid;
   }
   ```

4. **Test کردن قبل از PR**
   - صفحه را در مرورگرهای مختلف بازی کنید
   - تغییرات را در موبایل تست کنید
   - Console را برای errors بررسی کنید

#### مراحل ارسال PR:

```bash
# تغییرات را commit کنید
git add .
git commit -m "feat: add machine efficiency calculator"

# به GitHub push کنید
git push origin feature/machine-efficiency

# در GitHub، Pull Request جدید باز کنید
# - عنوان واضح بنویسید
# - شرح تغییرات را اضافه کنید
# - Issues مرتبط را link کنید (#123)
```

**Template برای PR Description:**
```markdown
## توصیف تغییرات
نوع تغییر را مشخص کنید:

- [ ] Bug fix
- [ ] ویژگی جدید
- [ ] تغییر سبک (لایاوت، رنگ، فونت)
- [ ] مستندات

## توضیحات
تغییرات دقیق را توضیح دهید.

## مرتبط با Issue
Fixes #123
Closes #456

## Checklist
- [ ] کد من تمیز است
- [ ] اسناد به‌روز شده‌اند
- [ ] در موبایل تست شده است
- [ ] در دسکتاپ تست شده است
```

---

## استانداردهای کد 📐

### HTML
```html
<!-- ✅ بله -->
<div class="energy-source-card solar">
  <h2>پانل خورشیدی</h2>
</div>

<!-- ❌ نه -->
<div class="card">
  <h2>solar</h2>
</div>
```

### CSS
```css
/* ✅ بله */
.energy-source-card {
  background: linear-gradient(135deg, rgba(20, 33, 61, 0.8), rgba(15, 26, 41, 0.6));
  border: 1px solid var(--border-color);
  border-radius: 14px;
}

/* ❌ نه */
.card {
  background: #123;
  border: 1px solid;
}
```

### JavaScript
```javascript
// ✅ بله
function updateEnergyMetrics(sources) {
  const total = sources.reduce((sum, source) => sum + source.power, 0);
  return {
    total,
    timestamp: new Date(),
    renewable: (sources.solar / total) * 100
  };
}

// ❌ نه
function update(s) {
  let t = 0;
  for (let i = 0; i < s.length; i++) {
    t += s[i].power;
  }
  return t;
}
```

---

## سیستم برچسب‌ها 🏷️

- `bug`: مشکل در کارکرد
- `enhancement`: ویژگی جدید یا بهبود
- `documentation`: مستندات
- `good first issue`: مناسب برای شروع‌کنندگان
- `help wanted`: نیاز به کمک
- `question`: سوال
- `wontfix`: حل نخواهد شد

---

## برای شروع‌کنندگان 👶

اگر این اولین مرتبه‌ای است که در پروژه open-source مشارکت می‌کنید:

1. ⭐ **Star** کردن این پروژه
2. به پیدا کردن Issues با برچسب `good first issue`
3. روی مشکل کلیک کنید و فهمیدن آن را شروع کنید
4. اگر سوالی دارید، کامنت بگذارید
5. Branch جدید بسازید و شروع کنید!

**منابع مفید:**
- [Git Guide](https://git-scm.com/doc)
- [GitHub Hello World](https://guides.github.com/activities/hello-world/)
- [Markdown Guide](https://www.markdownguide.org/)

---

## کد رفتار 🤝

- **احترام**: تمام مشارکین و نظرات را احترام دهید
- **شفافیت**: در مورد اهداف و نیات صادق باشید
- **تحمل**: درک کنید که مردم نقاط نظر متفاوتی دارند
- **تمرکز**: روی بهتری پروژه تمرکز کنید

---

## سوالات متداول ❓

**Q: چقدر طول می‌کشد تا PR من merge شود؟**
A: معمولاً 2-7 روز، بسته به اندازه و پیچیدگی

**Q: اگر PR من رفع‌نشده باقی مانید چی؟**
A: بعد از 2 هفته بدون فعالیت، ممکن است بسته شود. دوباره کامنت بگذارید و دوباره باز خواهیم کرد

**Q: آیا باید signed CLA بفرستم؟**
A: خیر، برای پروژه Hyneto CLA نیاز نیست

---

## تماس 📧

- **GitHub Issues**: برای bugs و features
- **GitHub Discussions**: برای سوالات و ایده‌ها
- **Email**: contribute@hyneto.com

---

**تشکر از مشارکت شما! 🎉**

</div>
