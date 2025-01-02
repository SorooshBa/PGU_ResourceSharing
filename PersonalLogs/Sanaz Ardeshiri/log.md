# مراحل انجام پروژه

1. **نصب Git**
   - ابتدا Git را از سایت رسمی آن نصب کردم:
     [https://git-scm.com/downloads](https://git-scm.com/downloads)

2. **نصب GitHub Desktop**
   - سپس GitHub Desktop را نصب کردم.

3. **کلون کردن ریپازیتوری**
   - با دستور زیر ریپازیتوری گفته شده را کلون کردم:
     ```bash
     git clone https://github.com/SorooshBa/PGU_ResourceSharing
     ```

4. **فورک کردن ریپازیتوری**
   - با گزینه‌ی **Fork**، ریپازیتوری را فورک کردم.

5. **ویرایش فایل contributors.md**
   - محتویات فایل `contributors.md` را تغییر دادم.
   - سپس با دستور زیر فایل را به Stage بردم:
     ```bash
     git add -A
     ```
   - و با دستور زیر کامیت کردم:
     ```bash
     git commit -m "Added sanax ardeshiri info and selected course"
     ```

6. **ایجاد پوشه Advanced Programming**
   - پوشه‌ی `Advanced Programming` را ایجاد کردم.
   - فایل `Notes.md` را ایجاد کردم.
   - سپس با دستور زیر فایل را به Stage بردم:
     ```bash
     git add -A
     ```
   - و با دستور زیر کامیت کردم:
     ```bash
     git commit -m "create Advanced Programming folder and notes.md"
     ```

7. **ایجاد پوشه references**
   - پوشه‌ی `references` را ایجاد کردم.
   - درون آن دو کتاب به‌عنوان منبع درس اضافه کردم.
   - سپس با دستور زیر کتاب‌ها را به Stage بردم:
     ```bash
     git add -A
     ```
   - و با دستور زیر کامیت کردم:
     ```bash
     git commit -m "create references folder and add two reference : 1-Java how to program 2-Thinking in java"
     ```

8. **ویرایش فایل Notes.md**
   - فایل `Notes.md` را کامل کردم.
   - سپس با دستور زیر به Stage بردم:
     ```bash
     git add -A
     ```
   - و با دستور زیر کامیت کردم:
     ```bash
     git commit -m "Write notes.md file"
     ```

9. **رفع مشکل کامیت**
   - تغییرات را Push کردم و متوجه شدم کامیت آخر فایل `Notes.md` مشکلی دارد.
   - با فلگ `--amend` تغییرات فعلی را با کامیت قبلی منتشر کردم:
     ```bash
     git commit --amend --no-edit
     ```
   - اما کانفلیکت رخ داد.
   - کانفلیکت‌ها را به‌صورت دستی در فایل `Notes.md` رفع کردم و مجدداً Push کردم.

10. **ایجاد پوشه PersonalLogs**
    - در پوشه‌ی `PersonalLogs`، پوشه‌ی خودم را ایجاد کردم.
    - فایل `log.md` را ایجاد کردم.
    - سپس با دستور زیر فایل را به Stage بردم:
      ```bash
      git add -A
      ```
    - و با دستور زیر کامیت کردم:
      ```bash
      git commit -m "Create log.md file in PersonalLogs\\Sanaz Ardeshiri"
      ```

11. **تغییر پیام کامیت دارای غلط املایی**
    - متوجه شدم در یکی از کامیت‌ها پیام کامیت دارای غلط املایی است:
      ```text
      git commit -m "Added sanax ardeshiri info and selected course"
      ```
    - هش کامیت را با دستور زیر به دست آوردم:
      ```bash
      git log
      ```
    - سپس با دستور زیر ویرایش پیام کامیت را انجام دادم:
      ```bash
      git rebase -i aec1d114~1
      ```
    - در فایل بازشده، `Pick` را به `Reword` تغییر دادم.
    - سپس پیام کامیت را تغییر دادم. پس از ذخیره‌سازی، هش کامیت تغییر کرد..

	- با دستور git rebase --continue عملیات را نهایی کردم
12. **کامیت نهایی و ارسال Pull Request**
    - در فایل `log.md` تغییرات نهایی را ذخیره کردم.
    - سپس با دستورات زیر کامیت و Push کردم:
      ```bash
      git add -A
      git commit -m "Write log.md file"
      git push
      ```
    - در نهایت یک **Pull Request** به ریپازیتوری اصلی ارسال کردم.
