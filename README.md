# مكتبة أغلفة الكتب — CDN

**حالة المستودع:** أُزيلت جميع الأغلفة من هذا المستودع (`covers/`)، ولم يعد jsDelivr يقدّم أي غلاف منه.

الموقع لا يستخدم هذا المستودع حالياً؛ يعرض غلافاً متجهياً احتياطياً، ويمكن إضافة روابط صور كاملة من لوحة الإدارة عبر `updates.json`.

## إن أردت استخدامه لاحقاً
1. أضف ملفات `.webp` داخل مجلد `covers/`.
2. أنشئ خريطة `id,filename` وحدّث `covers.js` في موقع المكتبة.
3. انشر وسماً جديداً (`v5` مثلاً) واضبط `COVER_BASE` في `index.html` عبر:
   ```powershell
   python tools/finalize_site.py --domain cdn.jsdelivr.net/gh/alifadhil2030-eng/library-covers@v5 --map map.csv --prefix covers
   ```

> jsDelivr يخزّن الإصدارات في كاش طويل؛ استخدم وسماً أو اسم ملف جديداً عند كل تعديل.
