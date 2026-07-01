# HTML Notes 📚

هذا الملف يحتوي على ملخص لأهم عناصر HTML التي تعلمتها مع شرح بسيط لكل عنصر.

---

# 1. HTML Structure

```html
<!DOCTYPE html>
<html>
<head>
</head>
<body>
</body>
</html>
```

## شرح

- `<!DOCTYPE html>` يخبر المتصفح أن الصفحة تستخدم HTML5.
- `<html>` العنصر الأساسي الذي يحتوي على الصفحة بالكامل.
- `<head>` يحتوي على معلومات الصفحة.
- `<body>` يحتوي على المحتوى الظاهر للمستخدم.

---

# 2. Head Elements

```html
<meta charset="UTF-8">
<meta name="description" content="Description">
<title>My Project</title>
```

### الاستخدام

- `charset` لتحديد الترميز.
- `description` لوصف الصفحة.
- `title` عنوان الصفحة الذي يظهر في التبويب.

---

# 3. Text Elements

```html
<h1></h1>
<p></p>
<b></b>
<strong></strong>
<i></i>
<em></em>
<u></u>
<mark></mark>
<del></del>
<ins></ins>
```

### الفرق بينهم

| العنصر | الوظيفة |
|---------|----------|
| h1 | عنوان رئيسي |
| p | فقرة |
| b | خط عريض فقط |
| strong | خط عريض وله معنى مهم |
| i | خط مائل |
| em | تأكيد بمعنى مائل |
| u | خط أسفل النص |
| mark | تظليل |
| del | نص محذوف |
| ins | نص مضاف |

---

# 4. Links

```html
<a href="https://google.com">Google</a>
```

أهم الخصائص:

- href
- target
- title

وللانتقال داخل الصفحة:

```html
<a href="#section1"></a>

<p id="section1"></p>
```

---

# 5. Images

```html
<img src="" alt="">
```

خصائص مهمة:

- src
- alt
- width
- height

---

# 6. Lists

## Unordered List

```html
<ul>
<li></li>
</ul>
```

## Ordered List

```html
<ol>
<li></li>
</ol>
```

## Description List

```html
<dl>
<dt></dt>
<dd></dd>
</dl>

```

---

# 7. Tables

```html
<table>
<tr>
<th></th>
</tr>

<tr>
<td></td>
</tr>
</table>
```

تعلمت:

- table
- tr
- th
- td
- colspan

---

# 8. Span & HR

## span

لعزل جزء معين من النص لتطبيق CSS عليه.

```html
<span>Hello</span>
```

## hr

لرسم خط أفقي.

```html
<hr>
```

---

# 9. Semantic Elements

## ما هي Semantic Elements؟

الـ **Semantic Elements** هي عناصر في HTML اسمها يعبر عن وظيفتها داخل الصفحة، أي أن مجرد قراءة اسم العنصر تعرف ما هو محتواه.

مثلاً:

```html
<header>
<footer>
<nav>
<article>
<section>
```

من أسماء هذه العناصر يمكنك معرفة وظيفة كل جزء من الصفحة.

أما قبل HTML5، كان المطورون يستخدمون:

```html
<div id="header"></div>
<div id="menu"></div>
<div id="content"></div>
<div id="footer"></div>
```

كلها كانت عبارة عن `div` فقط، لذلك لم يكن المتصفح أو محركات البحث يعرف وظيفة كل جزء.

---

## لماذا نستخدم Semantic Elements؟

استخدام العناصر الدلالية يوفر عدة مميزات:

- يجعل الكود منظمًا وأسهل في القراءة.
- يسهل على أي مطور فهم المشروع.
- يساعد محركات البحث (SEO) على فهم محتوى الصفحة.
- يحسن تجربة مستخدمي برامج قراءة الشاشة (Accessibility).
- يجعل صيانة المشروع أسهل مع مرور الوقت.

---

## أشهر العناصر الدلالية

### 1. Header

يمثل رأس الصفحة أو رأس قسم معين.

غالبًا يحتوي على:

- شعار الموقع (Logo)
- اسم الموقع
- قائمة التنقل
- مربع البحث

مثال:

```html
<header>
    <h1>My Website</h1>
</header>
```

---

### 2. Nav

يمثل قائمة التنقل الخاصة بالموقع.

يحتوي عادة على روابط الانتقال بين الصفحات.

مثال:

```html
<nav>
    <a href="/">Home</a>
    <a href="/about">About</a>
    <a href="/contact">Contact</a>
</nav>
```

> يفضل استخدام `<nav>` فقط للروابط الأساسية الخاصة بالتنقل داخل الموقع.

---

### 3. Section

يمثل قسمًا من الصفحة يحتوي على موضوع معين.

مثال:

```html
<section>
    <h2>Latest News</h2>
    <p>News Content...</p>
</section>
```

يمكن أن تحتوي الصفحة على أكثر من Section.

---

### 4. Article

يمثل محتوى مستقل يمكن قراءته بمفرده.

مثل:

- مقال
- منشور Blog
- خبر
- تعليق مستخدم

مثال:

```html
<article>
    <h2>Learning HTML</h2>
    <p>HTML is the foundation of web development.</p>
</article>
```

---

### 5. Aside

يمثل محتوى جانبي مرتبط بالمحتوى الأساسي.

مثل:

- الإعلانات
- المقالات المقترحة
- آخر الأخبار
- معلومات الكاتب

مثال:

```html
<aside>
    <h3>Related Articles</h3>
</aside>
```

---

### 6. Figure

يستخدم لوضع صورة أو رسم أو جدول مع وصف له.

مثال:

```html
<figure>
    <img src="image.png" alt="HTML Logo">
    <figcaption>HTML Logo</figcaption>
</figure>
```

---

### 7. Figcaption

يكتب بداخله وصف للصورة الموجودة داخل `figure`.

مثال:

```html
<figcaption>
    HTML Logo
</figcaption>
```

---

### 8. Footer

يمثل الجزء السفلي من الصفحة.

غالبًا يحتوي على:

- حقوق النشر
- وسائل التواصل
- روابط مهمة
- معلومات التواصل

مثال:

```html
<footer>
    Copyright © 2026
</footer>
```

---

## مثال كامل

```html
<body>

<header>
    <h1>My Website</h1>
</header>

<nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
</nav>

<section>

    <article>
        <h2>First Article</h2>
        <p>Article Content...</p>
    </article>

    <article>
        <h2>Second Article</h2>
        <p>Article Content...</p>
    </article>

</section>

<aside>
    <h3>Popular Posts</h3>
</aside>

<footer>
    Copyright © 2026
</footer>

</body>
```

---

## الشكل التقريبي للصفحة

```
+----------------------------------+
|             Header               |
+----------------------------------+
|               Nav                |
+----------------------------------+
|                                  |
|            Section               |
|   +--------------------------+   |
|   |        Article           |   |
|   +--------------------------+   |
|   |        Article           |   |
|   +--------------------------+   |
|                                  |
+----------------------------------+
|             Aside                |
+----------------------------------+
|             Footer               |
+----------------------------------+
```

---

## هل الـ Semantic Elements تغير شكل الصفحة؟

**لا.**

هذه العناصر لا تضيف أي تصميم أو تنسيق تلقائي، بل وظيفتها هي إعطاء معنى وتنظيم للكود فقط.

يمكنك جعلها تبدو بأي شكل باستخدام CSS.

---

## ملخص سريع

| العنصر | الاستخدام |
|---------|------------|
| `header` | رأس الصفحة أو القسم |
| `nav` | روابط التنقل |
| `section` | قسم يحتوي على موضوع معين |
| `article` | محتوى مستقل يمكن قراءته وحده |
| `aside` | محتوى جانبي |
| `figure` | صورة أو رسم مع وصف |
| `figcaption` | وصف للصورة |
| `footer` | أسفل الصفحة |
---

# 10. Audio & Video

```html
<audio controls>

<source>

</audio>
```

```html
<video controls>

<source>

</video>
```

خاصية

```
controls
```

تظهر أدوات التشغيل.

---

# 11. Forms

```html
<form>

</form>
```

## أهم عناصر الإدخال

- text
- password
- email
- hidden
- color
- range
- number
- file
- search
- url
- date
- month
- time

---

# 12. Input Attributes

تعلمت استخدام:

| الخاصية | الوظيفة |
|----------|----------|
| name | اسم البيانات المرسلة |
| placeholder | نص مؤقت |
| required | إلزامي |
| autofocus | يبدأ المؤشر عليه |
| minlength | أقل عدد أحرف |
| maxlength | أكبر عدد أحرف |
| value | قيمة افتراضية |
| readonly | لا يمكن التعديل ويُرسل مع البيانات |
| disabled | لا يمكن التعديل ولا يُرسل |
| min | أقل قيمة |
| max | أكبر قيمة |
| step | مقدار الزيادة |

---

# 13. Radio Button

```html
<input type="radio">
```

يجب أن يكون لجميع الخيارات نفس

```html
name
```

حتى يمكن اختيار عنصر واحد فقط.

---

# 14. Checkbox

```html
<input type="checkbox">
```

يسمح باختيار أكثر من عنصر.

---

# 15. Select

```html
<select>

<option>

</select>
```

تعلمت:

- option
- optgroup
- multiple

---

# 16. Textarea

```html
<textarea></textarea>
```

لإدخال نصوص طويلة.

---

# 17. Buttons

```html
<input type="submit">

<input type="reset">
```

- submit لإرسال البيانات.
- reset لإعادة تعيين النموذج.

---

# أهم ما تعلمته

✅ كتابة هيكل صفحة HTML.

✅ استخدام عناصر النصوص.

✅ الروابط.

✅ الصور.

✅ القوائم.

✅ الجداول.

✅ العناصر الدلالية (Semantic HTML).

✅ الصوت والفيديو.

✅ إنشاء النماذج Forms.

✅ جميع أنواع Input الأساسية.

✅ Radio Buttons و Checkboxes.

✅ Select و Textarea.

✅ إرسال البيانات باستخدام Form.
