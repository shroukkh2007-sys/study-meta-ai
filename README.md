# Study Meta AI (نسخة احتياطية)

نسخة طبق الأصل من التطبيق، بتشتغل على Streamlit.

## التشغيل محلياً
```
pip install -r requirements.txt
streamlit run app.py
```

## النشر على Streamlit Cloud
1. ارفعي الفولدر ده كله على ريبو GitHub جديد.
2. من Streamlit Cloud اعملي App جديد واختاري `app.py`.
3. من Settings > Secrets الصقي محتوى `.streamlit/secrets.toml.example` وحطي مفتاح Gemini جديد (من حساب Google تاني لو الليميت قفل على المفتاح القديم).

## ملاحظات
- فولدر `seed/` اختياري: حطي فيه ملفات PDF للدروس وهتتضاف للمكتبة أول تشغيل.
- قاعدة البيانات `studymeta.db` بتتعمل تلقائي وبتبدأ فاضية. لو عايزة نفس الطلاب والدروس القديمة انسخي الملف القديم جنب `app.py`.
- على Streamlit Cloud الملف ده بيتمسح لما التطبيق يعيد التشغيل.
