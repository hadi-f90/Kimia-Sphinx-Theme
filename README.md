#  قالب زمینه‌ی فارسی کیمیا برای  اسفینکس 
‍`(دسترسی زودهنگام-در دست توسعه)`

__کیمیا__ قالبی برای تولید محتوا با [اسفینکس](sphinx.org) به صورت صفحات  وب ایستا است. 

در اصل، این قالب همان قالب پروژه‌ی [ریبرگ](reeborg.ca) است که برای بخش کتاب [پروژه‌ی ریبرگ فارسی](https://book.reeborg.ir) فارسی سازی شده است. 

شما هم می‌توانید آن را برای تولید محتوا و یا وب‌گاه‌های ایستا به کار ببرید.

## درباره‌ی قالب
وقتی داشتم بخش کتاب پروژه‌ی ریبرگ را ترجمه می‌کردم؛ دنبال یک قالب فارسی برایش بودم. ولی، بر خلاف انبوه قالب‌های ساخته شده برای زبان‌های پایه‌ی لاتین، برایش به فارسی و دیگر زبان‌های راست به چپ مانند عربی، به جز پروژه‌ی مینو و [خواندن مستندات](readthedoc.org)  قالب دیگری پیدا نکردم.
 
 چیزی که از سازندگان آن قالب شنیدم این بود که احتمالاً با زبان‌های راست به چپ مشکلی نداشته باشد؛ ولی مطمئن نیستم.
 بعد از چندین بار تلاشو آزمون و خطا متوجّه شدم دو قالب‌های قبل آن چیزی که می‌خواستم نبودند. از طرفی هم دلم می‌خواست یک قالب به قالب‌های موجود اضافه کنم. بنابراین، تلاش کردم با دانش محدودم در زمینه‌ی توسعه صفحات وب ،همان قالب اصلی پروژه‌ی ریبرگ را برای فارسی بهینه کنم که احتمالاً در باقی زبان‌های راست به چپ هم درست کار کند.این قالب را فعلاً با نام قالب فارسی کیمیا منتشر کرده‌ام (اگر نام بهتر سراغ دارید پشنهاد بدهید).

## ساختار و طرز استفاده 
ساختار پوشه‌ها همان طوری که باید در یک پروژه‌ی مستندات باشد، از قبل مرتّب شده (احتمالاً کمی تمیزکاری لازم داشته باشید). از طرفی قالب‌هایی که قرار است بر اساس آن‌ها فایل‌های منبع تدوین شوند؛ در پوشه‌ی 

    theme
قرار دارند. اصل کار شما با آن‌‌هاست. ولی از آن‌جایی که این قالب خودش بر اساس یکی دو قالب پایه‌ای دیگر داخل سیستم اسفینکس هست -که پیدا کردنش شاید برای شما دردسر داشته باشد. برای همین، من آن‌ها را برای شما جدا کرده‌ام (البتّه، اگر آن‌ها را ویرایش کنید؛ باز باید سرجای خودشان درون پوشه‌ی اسفینکس برگردانید و یا درون فایل تنظیمات آدرس دهی کنید تا تغییرات شما اعمال شود.). اگر به این مرحله رسیدید و نیاز به کمک داشتید پیام بگذارید؛ شاید بتوانم شما را راهنمایی کنم. 

بعد از این مرحله، تمام کاری که شما برای دیدن خروجی باید انجام بدهید این است که دستور 

    make html
را در محیط خط‌فرمان از مسیر همین پوشه وارد کنید.

 با وارد کردن این دستور، روند تبدیل فایل های منبع به صفحات وبا ایستا از داخل فایل ساخت پروژه شروع می‌شود.
بسته به سیستم عامل یکی از یکی از این دو تا فایل اجرا می‌شود:

    make یا make.bat
 البتّه، اگر از اجرا بد افزار نگرانید؛ با نگاهی به داخل فایل‌های سازنده، خیلی زود متوجّه می‌شوید؛ این فرمان فقط فایلی بوده که مدیر محتوای اسفینکس رو شروع می‌کرده تا فایل‌های منبع را به خروجی صفحات وب تبدیل کند.
برای دیدن فهرست قالب و پسوندهای پشتیبانی شده‌ی فایل‌های منبع به مستندات اسفینکس نگاهی بیاندازید.

اگر دلتان خواست هر کدام از آن‌ها را استفاده کنید؛ از قبل باید در فایل تنظیمات‌پروژه‌یتان  همان را به جای پیش‌فرض تعریف کنید.

اگر در طول کار ساختار فایل‌ها و پوشه‌ها به هم ریخت، می توانید فایل زیپ

    Testing_doc.zip 
را باز کنیدو یا انباره رو دوباره از همین‌جا بگیرید.

