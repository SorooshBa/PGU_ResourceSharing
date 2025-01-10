عالی است! در این مرحله، شما Branch خود (edit_branch) را با Branch اصلی (main) ادغام (Merge) کرده‌اید. این کار تغییرات شما را به Branch اصلی اضافه می‌کند. در ادامه، این مرحله را به لاگ پروژه اضافه می‌کنیم.

---

# لاگ فعالیت‌های پروژه

در این فایل، مراحل انجام پروژه به صورت لاگ نوشته شده‌است. این لاگ شامل دستورات و توضیحات مربوط به هر مرحله است.

---

## ۱. Fork کردن ریپازیتوری

برای شروع پروژه، ریپازیتوری `PGU_ResourceSharing` را از GitHub Fork کردم.

- **دستور**: (این کار از طریق رابط کاربری GitHub انجام شد.)
- **توضیحات**: با کلیک روی دکمه **Fork**، یک کپی از ریپازیتوری در حساب کاربری من ایجاد شد.

---

## ۲. Clone کردن ریپازیتوری به کامپیوتر شخصی

پس از Fork کردن، ریپازیتوری را به کامپیوتر شخصی خود Clone کردم.

- **دستور**:

git clone https://github.com/your-username/PGU_ResourceSharing.git

- توضیحات: این دستور ریپازیتوری را در پوشه‌ای به نام PGU_ResourceSharing روی کامپیوتر من دانلود کرد.

---

## ۳. ایجاد یک Branch جدید

برای انجام تغییرات، یک Branch جدید با نام edit_branch ایجاد کردم.

- دستور:

cd PGU_ResourceSharing
git checkout -b edit_branch

- توضیحات: این دستور یک Branch جدید ایجاد کرد و من را به آن Branch سوئیچ کرد.

---

## ۴. ایجاد تغییرات در پروژه

در Branch جدید، تغییرات مورد نیاز را اعمال کردم.

- دستور:

touch newfile.txt
echo "This is a new file for the project." > newfile.txt
git add newfile.txt
git commit -m "Add newfile.txt to the project"

- توضیحات:
  - یک فایل جدید به نام newfile.txt ایجاد کردم.
  - محتوایی به فایل اضافه کردم.
  - تغییرات را به Staging Area اضافه کردم.
  - تغییرات را Commit کردم.

---

## ۵. ایجاد پوشه و فایل جدید

یک پوشه جدید به نام IR_System در پوشه Courses ایجاد کردم و یک فایل به نام information.md در آن پوشه اضافه کردم.

- دستور:

mkdir -p Courses/IR_System
cd Courses/IR_System
touch information.md
echo "This file contains information about the IR System course." > information.md
git add Courses/IR_System/information.md
git commit -m "Add information.md to IR_System folder"

- توضیحات:
  - پوشه IR_System در پوشه Courses ایجاد شد.
  - فایل information.md در پوشه IR_System ایجاد شد.
  - محتوایی به فایل اضافه کردم.
  - تغییرات را به Staging Area اضافه کردم.
  - تغییرات را Commit کردم.

---

## ۶. نوشتن اطلاعات در فایل information.md

اطلاعات مربوط به سیستم اطلاعاتی (IR System) را در فایل information.md نوشتم.

- دستور:

echo "IRSystem info" >> Courses/IR_System/information.md
git add Courses/IR_System/information.md
git commit -m "Add IRSystem info to information.md"

- توضیحات:
  - اطلاعات IRSystem info به فایل information.md اضافه شد.
  - تغییرات را به Staging Area اضافه کردم.
  - تغییرات را Commit کردم.

---

## ۷. تغییر فایل contributors.md

به مسیر ریشه (PGU_ResourceSharing) رفتم و فایل contributors.md را ویرایش کردم. نام خودم و نام دوره‌ام را به این فایل اضافه کردم.

- دستور:

cd ~/PGU_ResourceSharing
echo "Nima Razmjoei - IR System Course" >> contributors.md
git add contributors.md
git commit -m "Add Nima Razmjoei to contributors.md"

- توضیحات:
  - نام و نام دوره‌ام به فایل contributors.md اضافه شد.
  - تغییرات را به Staging Area اضافه کردم.
  - تغییرات را Commit کردم.

---

## ۸. ایجاد پوشه و فایل جدید در Courses/PersonalLogs

به مسیر Courses/PersonalLogs رفتم و یک پوشه به نام Nima Razmjoei ایجاد کردم. سپس یک فایل به نام log.md در این پوشه ایجاد کردم.

- دستور:

mkdir -p Courses/PersonalLogs/Nima\ Razmjoei
cd Courses/PersonalLogs/Nima\ Razmjoei
touch log.md
echo "This is my personal log file." > log.md
git add Courses/PersonalLogs/Nima\ Razmjoei/log.md
git commit -m "Add log.md to Nima Razmjoei folder"

- توضیحات:
  - پوشه Nima Razmjoei در Courses/PersonalLogs ایجاد شد.
  - فایل log.md در این پوشه ایجاد شد.
  - محتوایی به فایل اضافه کردم.
  - تغییرات را به Staging Area اضافه کردم.
  - تغییرات را Commit کردم.

---

## ۹. Push کردن تغییرات به GitHub

پس از ایجاد تغییرات، آن‌ها را به ریپازیتوری Fork شده در GitHub Push کردم.

- دستور:

git push origin edit_branch

- توضیحات: این دستور Branch جدید و تغییرات من را به GitHub ارسال کرد.

---

## ۱۰. ادغام (Merge) Branch با Branch اصلی

پس از اطمینان از صحت تغییرات، Branch edit_branch را با Branch اصلی (main) ادغام کردم.

- دستور:

git checkout main
git merge edit_branch
git push origin main

- توضیحات:
  - به Branch اصلی (main) سوئیچ کردم.
  - تغییرات Branch edit_branch را با Branch اصلی ادغام کردم.
  - تغییرات ادغام‌شده را به GitHub Push کردم.

---

## ۱۱. بررسی تغییرات در GitHub

پس از Push کردن تغییرات، به GitHub رفتم و تغییرات را بررسی کردم.

- توضیحات:
  - Branch جدید (edit_branch) در ریپازیتوری Fork شده من ایجاد شد.
  - فایل newfile.txt در Branch جدید اضافه شد.
  - پوشه IR_System و فایل information.md در پوشه Courses اضافه شدند.
  - فایل contributors.md به‌روزرسانی شد.
  - پوشه Nima Razmjoei و فایل log.md در Courses/PersonalLogs ایجاد شدند.
  - تغییرات با موفقیت به Branch اصلی (main) ادغام شدند.

---

## ۱۲. ارسال Pull Request (اختیاری)

اگر می‌خواهید تغییرات خود را به ریپازیتوری اصلی برگردانید، می‌توانید یک Pull Request ایجاد کنید.

- توضیحات:
  - به ریپازیتوری Fork شده در GitHub بروید.
  - روی دکمه Pull Request کلیک کنید.
  - تغییرات خود را بررسی و Pull Request را ارسال کنید.

---

## جمع‌بندی

در این پروژه، من مراحل زیر را انجام دادم:
۱. Fork کردن ریپازیتوری.
۲. Clone کردن ریپازیتوری به کامپیوتر شخصی.
۳. ایجاد یک Branch جدید.
۴. ایجاد تغییرات در پروژه.
۵. ایجاد پوشه و فایل جدید (Courses/IR_System/information.md).
۶. نوشتن اطلاعات در فایل information.md.
۷. تغییر فایل contributors.md.
۸. ایجاد پوشه و فایل جدید در Courses/PersonalLogs.
۹. Push کردن تغییرات به GitHub.
۱۰. ادغام Branch edit_branch با Branch اصلی (main).

---

توجه: این فایل به صورت Markdown نوشته شده‌است و می‌توانید آن را در ریپازیتوری خود ذخیره کنید.

---

### نحوه ذخیره فایل
۱. فایل را با نام `project_log.md` ذخیره کنید.
۲. آن را به ریپازیتوری خود اضافه کنید:

git add project_log.md
git commit -m "Update project log with merge details"
git push origin main

---

