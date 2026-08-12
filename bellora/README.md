# Bellora — بلّورا

**Merchant documentation for the Bellora Salla theme · Version 1.0.0**

[English](#english) · [العربية](#العربية)

---

<a id="english"></a>
## English

### About Bellora

Bellora is a premium storefront theme for Salla built around a glass-inspired visual system, responsive product presentation, optional 3D experiences, and merchant-controlled design settings. It keeps Salla's native commerce flows while adding a distinctive storefront layer for desktop and mobile.

### Quick start

After installing Bellora, open the Salla theme customizer and configure the global Design System first. Then configure the header, homepage components, product presentation, and footer. Preview the store on both mobile and desktop before publishing your changes.

### Design System settings

Bellora exposes the following global controls in the theme customizer:

| Setting | Options | Purpose |
|---|---|---|
| Glass intensity | Subtle / Medium / Immersive | Controls the strength of Bellora's glass surfaces and blur |
| Animation intensity | Off / Subtle / Full | Controls decorative motion and transitions |
| Reduced effects mode | On / Off | Disables blur, motion, and optional visual effects for a calmer presentation |
| 3D effects | On / Off | Master switch for optional 3D/effect experiences |
| Liquid transitions | On / Off | Enables the optional liquid-style hero transition |
| Container width | Standard / Wide / Full width | Controls the maximum content width |
| Corner style | Sharp / Soft / Rounded | Controls the global corner-radius system |
| Spacing density | Compact / Comfortable / Spacious | Controls the overall spacing rhythm |
| Dark mode | On / Off | Allows the storefront to start in Bellora's dark appearance |

Bellora also respects reduced-motion and reduced-effects conditions so decorative effects can fall back without blocking shopping functionality.

### Header and navigation

The header supports Salla's native navigation and account flows with Bellora styling. Available presentation options include a sticky header, transparent-header treatment, announcement bar, important links, and the additional menu area. On mobile, Bellora uses a dedicated bottom navigation bar for fast access to core store destinations.

### Homepage components

Bellora includes the standard Salla content building blocks plus Bellora-specific presentation options. For the clearest homepage, use one primary hero treatment and arrange the remaining components around the store's merchandising priorities.

Common Bellora homepage experiences include:

- classic and enhanced hero/banner sliders;
- Interactive Glass Slider with optional 3D model support;
- quick links and category navigation;
- featured, latest, and selected product sections;
- Flash Deals with countdown and responsive navigation;
- banners, video sections, testimonials, brands, blog articles, and store features.

### Interactive Glass Slider and 3D models

The Interactive Glass Slider can combine responsive images, text, calls to action, and an optional 3D model.

For each slide:

1. Add the desktop image and, when available, a dedicated mobile image.
2. Add the slide title, description, button text, and destination URL as needed.
3. To display a model, provide a **public HTTPS `.glb` or `.gltf` URL** that the visitor's browser can access.
4. Ensure the model host permits browser access with appropriate CORS headers.
5. Keep a normal slide image configured. Bellora uses the image as the visual fallback while the 3D model loads or when 3D effects are unavailable.

Bellora uses Google's `<model-viewer>` for interactive model presentation. Supported devices can receive camera controls, auto-rotation, and available AR modes. The optional liquid transition is a separate image-transition effect and does not replace the model viewer.

### Product page

Bellora keeps Salla's native product data and purchase controls while providing a dedicated product-detail layout. Depending on the product and store configuration, the page can include:

- product gallery, video, and Salla-provided 3D media;
- product variants and option images;
- sale pricing and discount presentation;
- wishlist and social sharing;
- quantity selection and native add-to-cart flow;
- sticky mobile purchase controls;
- image zoom;
- product and collection breadcrumbs;
- notify-when-available behavior for unavailable products.

For product 3D media, configure the product's 3D image/model through Salla. When a valid model is present and Bellora's 3D effects are enabled, the product gallery can offer Gallery / 3D viewing with the product image retained as a fallback.

### Product cards and wishlist

Bellora product cards preserve Salla product state, pricing, availability, and wishlist behavior. On mobile, the wishlist control remains directly visible and is positioned within the card's media area so it does not cover the product title or commerce information.

### Flash Deals

The Flash Deals component supports grid and horizontally navigable presentations with a countdown when an expiry date is configured. Product source, availability, pricing, wishlist state, and product-card behavior remain Salla-owned.

### Light, dark, RTL, and mobile behavior

Bellora is designed for Arabic and English storefronts and supports RTL/LTR layouts. Glass surfaces and contrast adapt to light and dark modes. Responsive behavior is built for mobile storefront use, including touch-friendly controls, mobile navigation, responsive product cards, and mobile purchase controls.

### Accessibility and reduced effects

If a customer requests reduced motion, or the store uses Bellora's Reduced Effects mode, decorative motion and heavy visual effects are reduced or disabled. Commerce controls, navigation, product information, and purchase flows remain available.

### Troubleshooting

**A 3D model does not appear**

- Confirm Bellora's 3D effects setting is enabled.
- Confirm the model URL is public HTTPS and ends in `.glb` or `.gltf` where a direct model URL is required.
- Confirm the model server permits cross-origin browser requests.
- Check whether Reduced Effects or a browser/device accessibility preference is suppressing optional effects.
- Keep the configured image fallback; customers should never depend on the 3D model to understand the slide or product.

**The storefront looks different in dark mode**

This is expected. Bellora changes its glass tint, contrast, borders, and shadows for dark surfaces while preserving the selected glass-intensity setting.

**An animation is missing on a device**

Optional animation can be reduced by the merchant setting, reduced-motion preferences, reduced-effects policy, or device/runtime capability. This does not disable the underlying store function.

### Recommended pre-publish check

Before publishing customizer changes, check the home page, one product with variants, one discounted product, one unavailable product/variant, cart, search, account navigation, and the footer on both mobile and desktop. Also verify Arabic/RTL and English/LTR if both languages are enabled.

### Support

For Bellora theme support, contact **screenprotectiontv@gmail.com**. Support requests are normally handled within **two business days**.

---

<a id="العربية"></a>
## العربية

### عن بلّورا

بلّورا هو قالب متجر مميز لمنصة سلة، يعتمد على تصميم زجاجي حديث، وتجربة متجاوبة للجوال والكمبيوتر، ودعم اختياري لتجارب العرض ثلاثي الأبعاد. يحافظ القالب على وظائف سلة الأساسية للمنتجات والسلة والشراء، ويضيف طبقة تصميم متكاملة يمكن للتاجر التحكم بها من إعدادات القالب.

### البدء السريع

بعد تثبيت بلّورا، افتح تخصيص القالب في سلة وابدأ بإعداد **نظام التصميم**، ثم اضبط الهيدر ومكونات الصفحة الرئيسية وصفحة المنتج والفوتر. قبل نشر التغييرات، راجع المتجر على الجوال والكمبيوتر.

### إعدادات نظام التصميم

يوفر بلّورا إعدادات عامة تشمل:

| الإعداد | الخيارات | الوظيفة |
|---|---|---|
| شدة الزجاج | خفيف / متوسط / غامر | التحكم في شفافية وضبابية الأسطح الزجاجية |
| شدة الحركة | إيقاف / خفيفة / كاملة | التحكم في الحركات والانتقالات الزخرفية |
| وضع تقليل المؤثرات | تشغيل / إيقاف | تقليل الضبابية والحركة والمؤثرات الاختيارية |
| مؤثرات 3D | تشغيل / إيقاف | المفتاح الرئيسي للتجارب ثلاثية الأبعاد والمؤثرات الاختيارية |
| الانتقالات السائلة | تشغيل / إيقاف | تشغيل تأثير الانتقال السائل الاختياري في البانر |
| عرض المحتوى | قياسي / واسع / كامل | تحديد أقصى عرض لمحتوى المتجر |
| شكل الزوايا | حاد / ناعم / دائري | التحكم في استدارة الزوايا في القالب |
| كثافة المسافات | مدمج / مريح / واسع | التحكم في المسافات العامة بين العناصر |
| الوضع الداكن | تشغيل / إيقاف | بدء المتجر بالمظهر الداكن عند اختياره |

### الهيدر والتنقل

يدعم الهيدر تنقل سلة وحساب العميل مع تصميم بلّورا، ويمكن استخدام الهيدر الثابت أو الشفاف، وشريط الإعلان، والروابط المهمة والقائمة الإضافية. على الجوال يوفر بلّورا شريط تنقل سفلي للوصول السريع إلى أقسام المتجر الأساسية.

### مكونات الصفحة الرئيسية

يمكن استخدام مكونات سلة الأساسية مع مكونات وتصاميم بلّورا، ومنها:

- سلايدر البانرات التقليدي والمحسن؛
- **Interactive Glass Slider** مع دعم اختياري لموديلات 3D؛
- الروابط السريعة والأقسام؛
- المنتجات المميزة والأحدث والمختارة؛
- العروض السريعة مع عداد ونظام تنقل متجاوب؛
- البانرات والفيديو والتقييمات والعلامات التجارية والمقالات ومميزات المتجر.

يفضل استخدام بانر رئيسي واحد واضح ثم ترتيب بقية المكونات حسب أولوية المنتجات والمحتوى.

### السلايدر الزجاجي وموديلات 3D

يمكن للسلايدر الزجاجي دمج الصور والنصوص وأزرار الدعوة للإجراء مع موديل ثلاثي الأبعاد اختياري.

عند إضافة موديل:

1. أضف صورة للكمبيوتر وصورة منفصلة للجوال إن توفرت.
2. أضف العنوان والوصف ونص الزر والرابط حسب الحاجة.
3. استخدم رابط HTTPS عام ومباشر لملف `.glb` أو `.gltf` عند طلب رابط موديل مباشر.
4. تأكد أن خادم الملف يسمح بتحميله من المتصفح عبر CORS.
5. احتفظ بصورة البانر العادية؛ فهي تعمل كصورة بديلة أثناء تحميل الموديل أو عند عدم توفر 3D.

يستخدم بلّورا Google `<model-viewer>` لعرض الموديلات التفاعلية. وعلى الأجهزة المدعومة يمكن استخدام التحكم بالكاميرا والدوران التلقائي وخيارات الواقع المعزز المتاحة. الانتقال السائل تأثير منفصل خاص بانتقال الصور ولا يستبدل عارض الموديل.

### صفحة المنتج

يحافظ بلّورا على بيانات المنتج وأدوات الشراء الأصلية من سلة، ويمكن أن تتضمن صفحة المنتج بحسب إعدادات المتجر والمنتج:

- معرض الصور والفيديو ومحتوى 3D المضاف في سلة؛
- الخيارات والمتغيرات وصور الخيارات؛
- السعر قبل وبعد الخصم؛
- المفضلة والمشاركة؛
- الكمية والإضافة إلى السلة؛
- شريط شراء ثابت على الجوال؛
- تكبير الصور؛
- مسار التنقل للمنتج والتصنيف؛
- تنبيه توفر المنتج عند نفاد المخزون.

إذا كان المنتج يحتوي على موديل 3D صالح وكانت مؤثرات 3D مفعلة، يمكن للمعرض إظهار خيار للتبديل بين المعرض والعرض ثلاثي الأبعاد، مع الاحتفاظ بصورة المنتج كخيار بديل.

### بطاقات المنتجات والمفضلة

تحافظ بطاقات بلّورا على حالة المنتج والسعر والتوفر والمفضلة من سلة. على الجوال يبقى زر المفضلة ظاهرًا مباشرة داخل منطقة صورة المنتج بدون تغطية اسم المنتج أو معلومات السعر والشراء.

### العروض السريعة

يدعم قسم العروض السريعة العرض الشبكي أو التنقل الأفقي، مع عداد عند تحديد تاريخ انتهاء. مصدر المنتجات والسعر والتوفر والمفضلة تظل مرتبطة بوظائف سلة الأصلية.

### العربية والإنجليزية والجوال

بلّورا مصمم لدعم العربية RTL والإنجليزية LTR. تتغير درجات الزجاج والحدود والظلال تلقائيًا حسب الوضع الفاتح أو الداكن. كما أن عناصر التنقل والبطاقات وأدوات الشراء مهيأة للاستخدام باللمس على الجوال.

### سهولة الاستخدام وتقليل المؤثرات

عند تفعيل تقليل المؤثرات أو عندما يطلب جهاز العميل تقليل الحركة، يتم تخفيف أو إيقاف المؤثرات الزخرفية الثقيلة. تظل وظائف التنقل ومعلومات المنتجات والسلة والشراء متاحة بشكل طبيعي.

### حل المشاكل

**موديل 3D لا يظهر**

- تأكد من تفعيل مؤثرات 3D في إعدادات بلّورا.
- تأكد أن رابط الموديل HTTPS عام ومباشر وأن الصيغة صحيحة.
- تأكد أن خادم الملف يسمح بطلبات CORS.
- تحقق من عدم تفعيل وضع تقليل المؤثرات أو إعدادات جهاز تقلل المؤثرات الاختيارية.
- احتفظ دائمًا بصورة بديلة للبانر أو المنتج.

**المظهر مختلف في الوضع الداكن**

هذا طبيعي. بلّورا يغير لون الزجاج والتباين والحدود والظلال ليناسب الخلفية الداكنة مع الحفاظ على شدة الزجاج المختارة.

**بعض الحركات لا تظهر على جهاز معين**

يمكن تقليل المؤثرات بسبب إعداد القالب أو تفضيلات تقليل الحركة أو قدرات الجهاز والمتصفح. الوظيفة الأساسية للعنصر لا تتوقف بسبب ذلك.

### فحص مقترح قبل النشر

قبل نشر تغييرات القالب، راجع الصفحة الرئيسية، ومنتجًا يحتوي على خيارات، ومنتجًا عليه خصم، ومنتجًا أو خيارًا نافدًا، والسلة والبحث والحساب والفوتر على الجوال والكمبيوتر. وإذا كان المتجر ثنائي اللغة، راجع العربية RTL والإنجليزية LTR.

### الدعم

للدعم الخاص بقالب بلّورا: **screenprotectiontv@gmail.com**. يتم التعامل مع طلبات الدعم عادة خلال **يومي عمل**.

---

**Bellora / بلّورا · Merchant Documentation · v1.0.0**
