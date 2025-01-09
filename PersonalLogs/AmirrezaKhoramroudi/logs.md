برای کلون کردن ریپازیتوری ابتدا به پوشه‌ای که می‌خواهیم پروژه در آن ذخیره شود می‌رویم با دستور `cd C:\Users\amirk\OneDrive\Documents\KargahProject` سپس با استفاده از دستور `git clone https://github.com/AmirKhoram771/PGU_ResourceSharing.git` ریپازیتوری را کلون می‌کنیم. در GitHub نیز یک کپی از ریپازیتوری در حساب کاربری خود ایجاد می‌کنیم.

برای کار با پوشه‌ها و فایل‌های پروژه، ابتدا وارد پوشه اصلی پروژه شده و سپس به پوشه `Courses` می‌رویم با دستور `cd PGU_ResourceSharing` و `cd Courses`. حالا می‌توانیم برای درس اقتصاد مهندسی یک پوشه جدید بسازیم. دستور `mkdir PGU_EconomyEngineering` برای ساخت پوشه و دستور `type nul > notes.md` برای ایجاد فایل یادداشت‌ها استفاده می‌شود. برای نوشتن اولین خط در فایل `notes.md` از دستور `echo "This is the first line of notes" > notes.md` استفاده می‌کنیم. اگر بخواهیم فایل را باز کرده و محتویات مورد نظر را بنویسیم، پس از اعمال تغییرات از دستورات `git add notes.md`، `git commit -m "توضیح تغییری که انجام شده"` و `git push origin main` برای ذخیره و ارسال تغییرات به GitHub استفاده می‌کنیم.

سپس برای ثبت نام خود در فایل `contributors.md` که در ریشه پروژه قرار دارد، ابتدا به پوشه اصلی پروژه برمی‌گردیم. بعد از ویرایش فایل، دستورات `git add contributors.md` و `git commit -m "new contributors added"` را اجرا کرده و در نهایت تغییرات را با دستور `git push origin main` به ریپازیتوری ارسال می‌کنیم.

برای مستندسازی دستورات، ابتدا در پوشه `PersonalLogs`، یک پوشه جدید به نام خودمان ایجاد می‌کنیم. دستور `mkdir AmirKhoram` و سپس `type nul > log.md` برای ساخت فایل مستندسازی استفاده می‌شود. مراحل انجام شده را در این فایل مستند می‌کنیم.

اگر بخواهیم فایل‌های PDF مرتبط با درس را اضافه کنیم، ابتدا پوشه‌ای به نام `PDFs` ایجاد کرده و فایل‌ها را به آن منتقل می‌کنیم. دستورات زیر برای اضافه کردن فایل‌های PDF استفاده می‌شود:
mkdir PDFs move path_to_the_pdf destination_path git add Courses/EngineeringEconomics/PDFs/*.pdf git commit -m "Added PDF resources for Engineering Economics" git push origin main


برای لینک دادن به فایل‌ها در فایل Markdown می‌توانیم از فرمت زیر استفاده کنیم:
```markdown
1. [جزوه](Courses/EngineeringEconomics/PDFs/pdf1.pdf)
اگر فایل‌های PDF بزرگتر از 50 مگابایت باشند، می‌توانیم از Git LFS استفاده کنیم. دستورات زیر برای نصب و استفاده از Git LFS به‌کار می‌رود:


git lfs install
git lfs track "*.pdf"
git add .gitattributes
git add Courses/EngineeringEconomics/PDFs/*.pdf
git commit -m "Added large PDF resources using Git LFS"
git push origin main
برای هر پوشه‌ای که ایجاد کرده‌ایم، می‌توانیم یک فایل README.md بسازیم تا توضیحات و محتوای مربوطه را درج کنیم. برای مثال:


echo "# Engineering Economics" > README.md
echo "This directory contains resources, notes, and exercises related to the Engineering Economics course taught by Dr. Soltani." >> README.md
git add README.md
git commit -m "Added README for Engineering Economics course"
git push origin main
اگر بخواهیم تمرینات را در یک شاخه جدید اضافه کنیم، ابتدا شاخه جدیدی به نام exercises ایجاد کرده و فایل تمرینات را می‌سازیم. پس از اتمام کار، شاخه تمرینات را به شاخه اصلی پروژه ادغام می‌کنیم و شاخه تمرینات را حذف می‌کنیم. دستورات زیر برای این مراحل استفاده می‌شود:


git checkout -b exercises
type nul > exercise1.md
git add exercise1.md
git commit -m "Added exercise 1"
git checkout main
git merge exercises
git branch -d exercises
git push origin main
برای مدیریت نسخه‌های پروژه، از تگ‌ها استفاده می‌کنیم. هر زمان که یک نسخه کامل از پروژه داشته باشیم، می‌توانیم یک تگ ایجاد کنیم تا تاریخچه نسخه‌های مختلف پروژه ذخیره شود. به عنوان مثال:


git tag -a v1.0 -m "First complete version"
git push origin v1.0
دستورات کلی برای ایجاد پوشه‌ها، فایل‌ها، و ارسال تغییرات به GitHub به شرح زیر است:

برای رفتن به پوشه‌ای: cd <path>
برای ساخت پوشه جدید: mkdir <name>
برای ساخت فایل جدید: type nul > <name>.md
برای ذخیره تغییرات: git add <name>.md و git commit -m "<message>"
برای ارسال تغییرات به GitHub: git push origin <branch>
برای جابجا کردن فایل‌ها: move <path> <destination>
برای دیدن وضعیت فایل ها : git status
برای بررسی تغییرات فایل ها : git diff

