My Sales Pro – FM Foods Edition
ابتدائی Android Studio پروجیکٹ (Version 0.1.0)

اس پروجیکٹ میں:
- Room مقامی ڈیٹا بیس (آف لائن بنیاد)
- کسٹمر ریکارڈ
- آپ کی فراہم کردہ 12 ابتدائی مصنوعات اور Box ریٹس
- ایک آرڈر میں متعدد مصنوعات
- Cash / Credit / Partial کی بنیادی منطق
- کسٹمر لیجر، اضافی وصولی اور آرڈر ہسٹری کی بنیاد

اہم:
یہ سورس کوڈ ہے، تیار شدہ APK نہیں۔ اسے Android Studio میں کھول کر Gradle Sync اور Build کرنا ہوگا۔
پہلی بار کاروباری استعمال سے پہلے مکمل ٹیسٹنگ ضروری ہے۔
ابھی باقی:
- محفوظ PIN hashing/lock screen
- ریٹرن فارم اور order-line کے خلاف return quantity کی validation
- JSON/CSV backup & restore
- مصنوعات/ریٹس اور مارکیٹنگ ایریاز کی مکمل ایڈیٹنگ
- مکمل رپورٹس، رسید اور تاریخ/وقت کی فارمیٹنگ
- automated tests اور APK signing

Build:
1. Android Studio میں اس فولڈر کو Open کریں۔
2. JDK 17 اور Android SDK 35 منتخب کریں۔
3. Gradle Sync کریں۔
4. Build > Build Bundle(s) / APK(s) > Build APK(s)


موبائل سے GitHub پر APK بنانے کا طریقہ:
1. GitHub پر نیا Repository بنائیں، نام MySalesPro رکھیں اور Public یا Private منتخب کریں۔
2. اس ZIP کو فون میں Extract کریں۔
3. Extract شدہ پروجیکٹ کی تمام فائلیں اور .github فولڈر Repository کی main branch میں اپ لوڈ کریں۔
4. GitHub میں Actions کھولیں؛ اگر workflow پہلی بار نظر نہ آئے تو main branch میں فائلیں commit کریں۔
5. "Build My Sales Pro APK" workflow کھول کر "Run workflow" دبائیں۔
6. کامیاب build کے بعد workflow کے نیچے Artifacts میں MySalesPro-debug-APK ڈاؤن لوڈ کریں۔
7. ZIP کھول کر app-debug.apk فون میں انسٹال کریں۔

نوٹ: یہ Debug APK ہوگی، Play Store کی signed release نہیں۔ Build کامیاب ہونے اور فون پر انسٹال ہونے کی ضمانت پہلے سے نہیں دی جا سکتی؛ GitHub Actions کے نتیجے یا error کی تصویر بھیجیں تاکہ مسئلہ درست کیا جا سکے۔
