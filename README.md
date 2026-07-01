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

تعلمت استخدام:

```html
<header>
<nav>
<section>
<footer>
<figure>
<figcaption>
```

وهي تجعل الصفحة أكثر تنظيماً وأسهل لمحركات البحث.

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
