# Poppy Editor (Fork of GNU nano)

هذا المستودع يحتوي على سورس كود محرر **Poppy**، وهو نسخة معدلة (Fork) من محرر النصوص الشهير **GNU nano** (الإصدار 7.2).

## التعديلات التي تمت:
1. إضافة دعم قراءة ملفات PDF و DOCX عبر استدعاء سكربت Node.js خارجي (`converter.mjs`).
2. تغيير اسم البرنامج التنفيذي إلى `poppy`.
3. تعطيل ميزة إكمال أسماء المستخدمين (getpwent) لتعمل على Termux (Android).

## الترخيص:
هذا المشروع يخضع لترخيص **GNU GPL v3** (انظر ملف COPYING). يجب أن يبقى أي توزيع لهذا الكود مفتوح المصدر تحت نفس الترخيص.

## التجميع (Build):
```bash
./configure --prefix=$PREFIX
make
mv src/nano src/poppy
