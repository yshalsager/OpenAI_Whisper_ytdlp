# تفريغ الصوتيات بواسطة OpenAI Whisper

<div dir="rtl">
<a href="https://colab.research.google.com/github/yshalsager/OpenAI_Whisper_ytdlp/blob/master/OpenAI_Whisper_ar_ytdlp.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="فتح في جوجل كولاب"/></a>

## حول هذا المِلَفّ
  
  - هذا المِلَفّ هو دفتر على جوجل كولاب يمكنك من تفريغ الصوتيات والمرئيات بواسطة [OpenAI Whisper](https://github.com/openai/whisper) و[faster-whisper](https://github.com/guillaumekln/faster-whisper/) أو حزمة [cohere-transcribe-arabic](https://github.com/AliOsm/cohere-transcribe-arabic-batch-inference). يمكن عبر هذا المِلَفّ تفريغ الملفات المحلية بعد رفعها أو تفريغ مقاطع وقوائم تشغيل يوتيوب.
  - خيار Cohere يدعم العربية والإنجليزية فقط، ويتطلب قبول شروط النموذج على Hugging Face وتوفير صلاحية الوصول للحساب المستخدم في كولاب. الإعداد الافتراضي يستخدم fp16 وتوقيت المقاطع ليعمل على كولاب المجاني مع بطاقة T4 غالبا.
  - حسب [تقرير المقارنة](https://pkrujqfyzo7l3tnykd8csnmkqsy4d33c.pastehtml.dev)، كان Cohere أفضل إجمالا وفي العربية الفصحى والكلاسيكية، بينما كان Wit.ai أفضل قليلا في تجميعة اللهجات الثقيلة. توجد أيضا [مقارنة سماعية مباشرة](https://rhykxn852pkyiiq5340bci70rz2m5x6i.pastehtml.dev).
  
## كيفية الاستخدام
  
1. شغل خطوة "اﻹعداد".
2. اختر نمط التشغيل: يوتيوب أو مِلَفّ محلي.
    - إذا اخترت local لتفريغ مِلَفّ ترفعه بنفسك، شغل خطوة اﻹعداد أولا ثم ارفع المِلَفّ إلى مجلد download.
    - إذا اخترت يوتيوب ضع رابط المقطع أو قائمة التشغيل في youtube_urls
    - يمكنك تحديد بداية ونهاية قائمة التشغيل من الخيارين التاليين.
3. اختر لغة المِلَفّ.
4. اختر محرك التفريغ. عند اختيار Whisper اختر النموذج المستخدم في التفريغ، large يعطي أفضل نتائج لكن أبطأ. عند اختيار Cohere فالخيار الافتراضي ينتج ملفات txt وsrt وvtt بتوقيت تقريبي سريع، ويستخدم fp16 المناسب لكولاب المجاني.
5. شغل خطوة "التفريغ".
</div>
