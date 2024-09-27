# KenLMPersianSpellingEditor
KenLM Paper https://aclanthology.org/W11-2123.pdf
Use DataSet [https://saied71.github.io/RohanAiLab/2021/09/03/Demo-datasets.html](https://huggingface.co/datasets/RohanAiLab/persian_news_dataset)

from datasets import load_dataset
ds = load_dataset("RohanAiLab/persian_news_dataset")


see more detail about DataSet here https://huggingface.co/docs/hub/datasets-usage


خلاصه‌ای از آنچه انجام شد و نتایج به دست آمده آمده است:
1. آموزش مدل KenLM:

    مدل بر روی داده‌های خبری فارسی که در Persian News Dataset ذخیره شده بود، آموزش داده شد.
    مدل زبانی به فرمت ARPA و سپس به باینری تبدیل شد.

2. استفاده از مدل برای امتیازدهی به جملات:

    از مدل برای امتیازدهی به جملات فارسی استفاده شد و نتایج آن را دریافت شد.
    جمله‌ی آزمایشی با امتیاز -24.176 ارزیابی شد.

3. پیشنهاد کلمات جایگزین:

    مدل با استفاده از امتیازدهی به کلمات مختلف بهترین کلمه را برای جمله انتخاب کرد.
    بهترین کلمه برای جمله‌ی "من به خانه ..." کلمه‌ی "رفتم" با امتیاز -19.269 بود.
