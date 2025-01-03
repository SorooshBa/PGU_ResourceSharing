# مستندات درس ساختمان داده

# 1. فورک کردن و کلون کردن ریپازتوری:

- فورک کردم به اکانت خودم
- در پاور شل آن را کلون کردم
- دستور:
  `  git clone https://github.com/MaralGoneWrong/PGU_ResourceSharing.git`

# 2. ساخت پوشه جدید به همراه فایل

- به پوشه Courses رفتم:

- ` cd PGU_ResourceSharing`

- ` cd Courses`

- در این پوشه فایل مربوط به درس ساختمان داده رو ساختم:

- ` mkdir "Data Structure"`

- سپس آن را باز کردم:

- ` cd "Data Structure"`

# 3. یک فایل Markdown ساختم

- چون در پاور شل بودم از دستور زیر استفاده کردم:

- ` New-Item -ItemType File DataS.md`

# 4. در آن فایل تغییرات مورد نظرم را انجام دادم

- دستور برای ثبت تغییرات:
- ` git add DataS.md`
- ` git commit -m "First Changes to Markdown adding new materials"`

# 5. برای ارسال تغییراتم push کردم

- دستور:
- ` git push origin main`

# 6. ساخت فایل برای مستندات

- به پوشه اصلی برگشتم
- ` cd ..`
- سپس به پوشه PersonalLogs رفتم:
- ` cd PersonalLogs`
- در آن یک فایل md برای ثبت مستندات ساختم
- ` New-Item -ItemType File log.md`
- در این فایل کارهایی که تا به حال انجام داده بودم را نوشتم وآن را commit و push کردم
- `git add log.md`
- `git commit -m "first time logging"`
- `git push origin main`
- در ادامه پروژه در این فایل تمام کارهایی که می‌کنیم را می‌نویسیم

# 7. اضافه کردن نام به فایل contributors

- به پوشه اصلی می‌رویم و فایل contributors را با vscode باز می‌کنیم
- نام خود را به لیست اضافه می‌کنیم
- تغییرات را commit و push می‌کنیم
- `git add contributors.md`
- `git commit -m "adding my name"`
- `git push origin main`

# 8. ساخت یک فایل در پوشه Data Structure برای اضافه کردن پی‌دی‌اف

- به فایل Data Structure می‌رویم و یک پوشه به نام refrence در آنجا می‌سازیم
- ` mkdir refrence`
- پی دی اف مورد نظر را آنجا کپی پیست می‌کنیم و سپس آن را به متریال اضافه می‌کنیم
- `git add refrence/analysis-slides.pdf`
- ` git commit -m "added my pdf to the folder"`
- سپس لینک آن را به DataS.md اضافه می‌کنیم
- ` [Analysis Slides](refrence\analysis-slides.pdf")`

- با دستور زیر تمام تغییرات را commit و push می‌کنیم
- `git add .`
- `git commit -m "added new pdf file " `
- `git push origin main`

# در آخر یک pull request ارسال کردم
