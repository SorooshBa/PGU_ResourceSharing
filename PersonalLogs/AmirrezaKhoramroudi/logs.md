مرحله 1 :
کلون کردن ریپازیتوری با دستور زیر :
ابتدا جایی که میخوایم پوشه در اون قرار بگیرد را با این دستور اجرا میکنیم :
cd C:\Users\amirk>cd C:\Users\amirk\OneDrive\Documents\KargahProject
سپس با دستور زیر ریپازیتوری را کلون میکنیم :
git clone https://github.com/AmirKhoram771/PGU_ResourceSharing.git
البته در گیت هاب یک کپی از ریپازیتوری به حساب کاربری خود ایجاد میکنیم
مرحله 2 :
دستورات زیر را در کامند پرامپت اجرا میکنیم :
cd PGU_ResourceSharing
cd Courses
برای رفتن در پوشه ای که میخوایم پوشه درس مربوطه رو در اون درست کنیم.
سپس با دستور زیر پوشه ای برای درس اقتصاد مهندسی درست میکنیم
mkdir PGU_EconomyEngineering
در داخل این پوشه یک فایل برای درس ایجاد میکنیم
markdown file :
type nul > notes.md
سپس با دستور زیر میتوانیم در داخل این فایل یک خط بنویسیم :
echo "This is the first line of notes" > notes.md
و یا میتوانیم فایل را باز کنیم و محتوای مورد نظر را بنویسیم و برای ثبت آن دستورات زیر را اجرا میکنیم
git add notes.md
git commit -m "توضیح تغییری که انجام شده" 
مرحله 3 :
ویرایش فایل 