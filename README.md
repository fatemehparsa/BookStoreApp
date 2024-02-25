







گزارش فاز اول پروژه نرم افزار فروشگاه کتاب

درس: نرم افزار1
طراح نرم افزار:  فاطمه پارسا
تاریخ: آبان 95









معرفی مسئله:
 طراحی نرم افزاری که فروش کتاب را به صورت مکانیزه انجام دهد. یعنی خریدار در سیستم کتاب مورد نظر خود را بر اساس نام نویسنده، نام کتاب و دیگر مشخصات آن پیدا میکند و شماره قفسه و ردیف کتاب برای فروشنده فرستاده میشود. خریدار  به صورت آنلاین در سیستم هزینه را پرداخت کند. و کتاب خود را از فروشنده تحویل می گیرد.
کاربرد دیگر این نرمافزاراین است که بر اساس سلیقه مشتری ها ی دارای اشتراک فروشگاه،  کتاب های جدید متناسب با سلیقه هر مشتری را پیشنهاد دهد. 
با توسعه این نرم افزار می توان به صورت آنلاین سفارش کتاب را دریافت و کتاب را برای خریدار ارسال کرد.
مشکلات سیستم انسانی:
در سیستم انسانی، خریدار باید برای یافتن کتاب مورد نظر خود از فروشنده کمک می خواست و تمام خریداران باید منتظر می ماندند تا فروشنده به ترتیب کتاب مورد نظر آنها را پیدا کند. و این روند بسیار زمان بر و خسته کننده بود. همچنین فروشنده باید محل تمام کتاب ها را به خاطر می سپرد تا بتواند به درستی مشتری ها  را راهنمایی کند. برای رفع این مشکلات و تسریع روند یافتن و خرید کتاب سیستم جدیدی را طراحی کرده ایم.
هدف: 
مدیریت فروشگاه کتاب به صورت کارآمد تر یعنی سریع تر  و جذابیت بیشتر برای خریداران. این اهداف با اتوماسیون فروش کتاب به دست می آید. اگر بخواهیم اهداف را به صورت جزئی تر بررسی کنیم به صورت زیر می باشد:
I.	 اطلاعات هر مشتری و خرید هایش ثبت می شوند و می توان با داده کاوی به علایق مشتری های دائم پی برد و به آنها کتاب های جدیدی پیشنهاد داد که مطابق با سلیقه آنها باشد.  با این روش هم فروش کتاب افزایش پیدا می کند و هم احساس رضایت در مشتری ایجاد می شود. 
II.	امکان جست و جو در تمام کتاب های موجود برای مشتری فراهم میشود.
III.	باعث ساده تر شدن روند یافتن کتاب و خرید آن میشود.
IV.	از سردرگمی مشتری ها در میان فروشگاه جلوگیری می شود.
V.	میتوان با ثبت کتاب هایی که خریداران جست و جو کرده اند و موجود نبوده است، لیست سفارش های فروشگاه را کامل کرد.

موارد کاربرد:
روش اول: کاربر هدف
هدف	کاربر
1.	بررسی موجود بودن کتاب مورد نظر
2.	ثبت کتاب انتخاب شده
3.	پرداخت هزینه کتاب	خریدار
1.	ثبت کتاب های جدید
2.	مشاهده لیست خرید مشتری و آدرس طبقه و ردیف کتاب ها
3.	بررسی فیش واریز
4.	اعلام کتاب های انتخاب شده به همراه آدرس به فروشنده 2	فروشنده 1
آماده کردن کتاب های اعلام شده 	فروشنده 2
1.	تهیه کتاب های جدید الانتشار
2.	تهیه کتاب هایی که موجودی آنها در حال تمام شدن است
3.	تهیه کتاب های ناموجودی که مشتریان درخواست داشته اند	مسئول خرید
1.	بررسی امور مالی ماهانه
2.	بررسی روند کار مسئول خرید و فروشنده
3.	بررسی کسری انبار 
4.	مدیر فروشنده جدید استخدام می کند.
5.	مدیر مسئول خرید جدید استخدام می کند.	مدیر فروشگاه
	
	
	

روش دوم: CRUD
موجودیت ها: کتاب _مدیر_فروشنده_مسئول خرید
کتاب: ثبت_ مشاهده_ ویرایش_ حذف
مدیر : ثبت_ مشاهده_ ویرایش_ حذف
فروشنده: ثبت_ مشاهده_ ویرایش_ حذف
مسئول خرید: ثبت_ مشاهده_ ویرایش_ حذف

روش تجزیه رویداد:
رویداد خارجی:
•	فروشنده 1 وارد حساب کاربری خود می شود.
•	فروشنده 1 کتاب جدید را ثبت می کند.
•	فروشنده 1 کتابی را حذف یا ویرایش میکند.
•	فروشنده 1 لیست کتاب های انتخابی مشتری را نگاه می کند.
•	فروشنده 1 آدرس کتاب را به فروشنده 2 می دهد.
•	مدیر وارد حساب کاربری خود می شود.
•	مدیر فروشنده جدید استخدام می کند.
•	مدیر مسئول خرید جدید استخدام می کند.
•	بررسی امور مالی ماهانه را انجام می دهد.
•	بررسی روند کار مسئول خرید و فروشنده را انجام می دهد.
•	بررسی کسری انبار را انجام می دهد.
•	مسئول خرید کتاب های جدید الانتشار را تهیه می کند.
•	مسئول خرید  کتاب هایی که موجودی آنها در حال تمام شدن است را تهیه می کند.
•	مسئول خرید کتاب های ناموجودی که مشتریان درخواست داشته اند را تهیه می کند.
•	مشتری ثبت نام می کند
•	مشتری لیست کتاب ها ی پیشنهادی را مشاهده می کند
•	مشتری در کتاب ها جست و جو می کند
•	مشتری کتاب های مورد نظرش را انتخاب میکند.
رویداد زمانی:
•	زمان گزارش ماهانه به مدیر فرا می رسد.
•	زمان OFF  سالانه فرا می رسد.
•	رویداد وضعیت:
•	موجودی کتابی کمتر از حد نساب می شود.
•	میزان امتیاز یک مشتری بیشتر از حد نساب می شود.
لیست موارد کاربرد:
•	افزودن مدیر جدید
•	ویرایش مدیر
•	افزودن کتاب جدید
•	ویرایش اطلاعات کتاب
•	حذف کتاب
•	افزودن فروشنده جدید
•	ویرایش مشخصات فروشنده
•	حذف فروشنده
•	افزودن مسئول خرید جدید
•	ویرایش مشخصات مسئول خرید
•	حذف مسئول خرید
•	ورود به حساب کاربری
•	ثبت نام مشتری
•	مشاهده کتاب های پیشنهادی
•	جست و جو در کتاب ها
•	انتخاب کتاب
•	پرداخت هزینه
•	مشاهده آدرس کتاب
•	ثبت کتاب جدید
شرح موارد کاربرد:
1.	مورد کاربرد: پرداخت هزینه
بازیگر: مشتری
جریان اصلی: 
1.	مشتری وارد صفحه پرداخت می شود 
2.	 مشخصات کارت خود را وارد می کند
3.	دکمه تایید را می زند
4.	سیستم نتیجه را اعلام می کند
جریان استثنا: اگر عملیات موفقیت امیز نبود سیستم پیامی را نمایش می دهد و کاربر باید دوباره اقدام کند
2.	مورد کاربرد: ثبت نام مشتری
بازیگر: مشتری
جریان اصلی: 
1.	مشتری وارد سیستم می شود سیستم صفحه ثبت نام را می آورد
2.	مشتری مشخصات خود را ثبت می کند
3.	دکمه تایید را می زند
4.	سیستم مشخصات را ثبت می کند
جریان استثنا: اگر نام کاربری قبلا ثبت شده باشد سیستم از کاربر می خواهد که آن را عوض کند.

3.	 مورد کاربرد: ثبت کتاب
بازیگر: فروشنده 1
جریان اصلی: 
1.	 فروشنده وارد حساب کاربری خود می شود
2.	قسمت اضافه کردن کتاب را باز می کند
3.	مشخصات کتاب را می نویسد
4.	دکمه ثبت را می زند
5.	سیستم پیام موفقیت ثبت را می دهد
جریان استثنا: ندارد
4.	مورد کاربرد: جست و جو در کتاب ها
بازیگر: مشتری
جریان اصلی:
1.	مشتری صفحه جست و جو را باز می کند
2.	عبارت مورد نظر برای جست و جو را می نویسد
3.	دکمه جست و جو را میزند
4.	سیستم از پایگاه داده اطلاعات را بررسی می کند
5.	سیستم نتیجه را به صورت لیستکتاب ها و آدرسشان اعلام میکند
6.	کاربر دوباره جست و جو می کند یا دکمه خروج را می زند
جریان استثنا: ندارد
5.	مورد کاربرد: مشاهده لیست کتابها
بازیگر: مدیر فروشگاه
1.	مدیر وارد حساب کاربری خود می شود.
2.	مشاهده لیست را انتخاب می کند
3.	سیستم جزییات لیست را نشان می دهد
جریان استثنا: ندارد
پروتوتایپ:
 
 
 
 
 
 
 
 
