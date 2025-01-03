
# مستندات فرآیندهای Git و GitHub

این فایل شامل تمامی مراحل و دستورات استفاده شده در طول انجام پروژه است.

---

## مرحله 1: ایجاد و کلون کردن ریپازیتوری

1. **Fork ریپازیتوری اصلی**:
   - از طریق رابط کاربری GitHub، ریپازیتوری اصلی پروژه را Fork کردم.
   - این کار به من اجازه داد که نسخه‌ای شخصی از پروژه داشته باشم.

2. **کلون ریپازیتوری Fork شده به سیستم محلی**:
   ```cmd
   git clone https://github.com/NazaninNiazi/PGU_ResourceSharing.git
   ```
   - `NazaninNiazi` نام کاربری GitHub من است.
   - این دستور، کپی پروژه را به سیستم محلی من انتقال داد.

---

## مرحله 2: ایجاد پوشه و فایل‌های مرتبط

1. **ورود به مسیر پروژه**:
   ```cmd
   cd PGU_ResourceSharing
   ```

2. **ایجاد پوشه جدید برای درس**:
   ```cmd
   mkdir AI
   ```

3. **ایجاد فایل Markdown برای درس**:
   ```cmd
   echo.> AI\overview.md
   ```

4. **اضافه کردن اطلاعات به فایل Markdown**:
   - شامل:
     - جزوات درسی
     - تمرین‌ها
     - پروژه
     - منابع آموزشی

---

## مرحله 3: ثبت تغییرات

1. **بررسی تغییرات انجام شده**:
   ```cmd
   git status
   ```
   - این دستور نشان می‌دهد که چه فایل‌هایی تغییر کرده‌اند.

2. **اضافه کردن فایل‌ها برای Commit**:
   ```cmd
   git add AI\overview.md
   ```

3. **ثبت تغییرات (Commit)**:
   ```cmd
   git commit -m "The AI lesson files have been added to overview"
   ```

---

## مرحله 4: ویرایش فایل `contributors.md`

1. **ویرایش فایل `contributors.md`**:
   ```cmd
   notepad contributors.md
   ```
   - اضافه کردن اطلاعات به جدول به فرمت زیر:
     ```markdown
   | نام درس  | نام و نام خانوادگی  | شماره |
   | :------------ |:---------------:| -----:|
   | مباحث ویژه یک      | علی باقریه | 1 |
   | هوش مصنوعی        | نازنین نیازی | 2|

     ```

2. **ثبت تغییرات**:
   ```cmd
   git add contributors.md
   git commit -m "I added my name and course name to contributors"
   ```

---

## مرحله 5: ساخت پوشه شخصی برای مستندسازی

1. **ایجاد پوشه برای مستندسازی شخصی**:
   - در ریشه ریپازیتوری، پوشه‌ای به نام `PersonalLogs` ایجاد کردم:
     ```cmd
     mkdir PersonalLogs
     ```

2. **ایجاد پوشه با نام کاربری**:
   - در داخل `PersonalLogs`، یک پوشه با نام `NazaninNiazi` ساختم:
     ```cmd
     mkdir PersonalLogs\NazaninNiazi
     ```

3. **ایجاد فایل مستندسازی (`log.md`)**:
   - فایل Markdown را در این پوشه ایجاد کردم:
     ```cmd
     echo.> PersonalLogs\NazaninNiazi\log.md
     ```

4. **اضافه کردن مستندات به `log.md`**:
   - تمامی دستورات و فرآیندهایی که انجام داده‌ام را به صورت کامل و مرتب در این فایل ثبت کردم.

5. **ثبت تغییرات**:
   ```cmd
   git add PersonalLogs\Nazanin Niazi\log.md
   git commit -m "Personal log for documentation created"
   ```

---

## مرحله 6: Push تغییرات به ریپازیتوری Fork شده

1. **ارسال تغییرات به ریپازیتوری Fork شده**:
   ```cmd
   git push origin main
   ```

---

## مرحله 7: Pull Request

1. **ایجاد Pull Request**:
   - به GitHub مراجعه کردم.
   - یک Pull Request ایجاد کردم که شامل:
     - توضیحات کامل تغییرات انجام شده.
     - اهمیت این تغییرات.

---