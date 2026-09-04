# Platform Team Goals

## Core Mission
- Listen to developers and be empathetic – understand their pain points, workflows, and needs through interviews, surveys, and usage analytics
- Reduce cognitive load on developers – handle infrastructure complexity so developers can focus on their core competency: writing business features
- Treat application development teams as customers and work with them to define best practices

## Developer Productivity & Experience
- Make it effortless for developers to build, test, and ship – remove as much friction as possible from the development lifecycle
- Reduce onboarding time – templatize development environments and workflows so new engineers can start contributing on day one
- Enable "day one" productivity – provide templates for common application types (Go, Java, Python, React) so developers can start committing code immediately
- Improve developer experience – ensure development environments are easy to set up, reduce onboarding time for new developers, and use modern, enjoyable technologies
- Guide teams to write unit tests, integration tests, end-to-end tests, and API tests with platform test infrastructure to make testing easier for developers

## Platform Design & Engineering
- Design, build, and maintain infrastructure and tools that support software development and deployment
- Abstract away infrastructure complexity – hide the complexity of modern cloud-native tooling (Kubernetes, Terraform, Helm, YAML, etc.) so developers can focus on application code
- Provide standardized tools and frameworks to streamline the development process and reduce cognitive load on developers
- Build reusable infrastructure modules (blueprints) – create Terraform modules for common patterns that bake in security, networking, and observability, enabling rapid, consistent onboarding
- Provide building blocks (constructs) with baked-in best practices – create reusable, versioned infrastructure components (e.g., using CDK constructs) that include company-specific policies, encryption standards, security defaults, and compliance requirements
- Publish versioned infrastructure packages – release platform components as versioned packages (e.g., via NuGet, Maven) so teams can consume them like any other dependency, with semantic versioning and release notes
- Standardize the tools and services needed for applications' non-functional requirements (CI/CD, version control, runtime, logging, monitoring, security) across all product teams
- Provide a centralized observability stack – offer shared logging, telemetry, and tracing services so all apps emit data in a consistent way for health monitoring and debugging

## Governance & Best Practices
- Standardize, but enable flexibility – establish opinionated defaults and "golden paths" for core capabilities while allowing necessary room for customization, clearly documenting which areas are negotiable
- Embed best practices and guardrails via Infrastructure as Code (IaC) – create reusable templates with baked-in security, compliance, monitoring, and configuration standards, while still allowing team-specific parameters
- Establish patterns and practices – define consistent approaches for code structure, layer interactions, service communication, and other cross-cutting concerns
- Balance standardization with autonomy – enforce guardrails and consistency where needed, but allow teams the freedom to customize their usage within the platform's boundaries
- Offer flexibility and choice – don't lock teams into a single tool; instead, support multiple standardized options and integrate new tools upon request when they provide value

## Security & Compliance
- Implement security and compliance by default – bake security, governance, and compliance into the platform from the start so teams don't have to think about it
- Maintain security, compliance, and consistency – ensure all platform services meet organizational security policies and regulatory requirements, and provide audit trails and compliance visibility for governance teams

## Reliability & Scalability
- Ensure scalability and flexibility – design infrastructure that can handle increasing workloads and use automation/cloud technologies for seamless scaling
- Guarantee reliability and stability – implement robust monitoring, automated backups, and disaster recovery mechanisms

## Cost Optimization
- Provide cost optimization through the platform – enforce cost-efficient defaults (auto-scaling, resource limits) and track cost savings as a key metric

## Team Composition & Culture
- Have engineers with both development and systems experience – ideal platform engineers have strong programming skills plus operational experience (OS, networking, distributed systems, monitoring)
- Have a stable, dedicated team – the platform team should be a permanent, ongoing team, not a temporary group that disbands after building something
- Blend three skill sets on the team – software engineering (to build abstractions), system skills (to operate reliably), and product/customer empathy (to focus on user needs)
- Avoid being a ticket-taker or bureaucratic bottleneck – don't become a process-heavy team that says "no"; be an enabler that solves problems for developers

## Operations & Maintenance
- Reduce migration pain for application teams – handle upgrades, security patches, and migrations (EKS upgrades, Python version updates) within the platform rather than pushing that work to development teams
- Define and maintain the technology roadmap – guide the organization's technical direction and ensure alignment across teams
- Make strategic technology decisions – answer high-level questions like monolith vs. microservices, cloud provider selection, and other architectural choices
- Evaluate, choose, and integrate third-party tools and services so developers don't have to evaluate them individually

## Collaboration & Support
- Collaborate closely with application teams – understand their pain points, bottlenecks, and workflows, and prioritize platform features that genuinely reduce their cognitive load
- Work with infrastructure/cloud teams – partner with cloud, on-premise, and security teams to leverage their expertise and ensure the platform runs on a solid, well-managed foundation
- Provide clear documentation and support – offer onboarding guides, troubleshooting resources, and responsive support channels to help developers effectively use the platform
- Facilitate collaboration and knowledge sharing across teams – provide technical guidance and promote cross-functional collaboration
- Drive continuous improvement – explore new technologies, tools, and practices to enhance the platform

## Product Mindset
- Continuously develop the platform as a product – treat the internal developer platform like a product with its own roadmap, releases, feature additions, bug fixes, and iterative improvements based on user feedback
- Treat the entire software delivery toolchain as a product – bring isolated DevOps, CI/CD, and operations tooling into a cohesive platform, delivered as a product to internal developers

## Measurement
- Measure migration pain reduction – track how much effort the platform saves teams during upgrades and migrations
-----------
# اهداف تیم پلتفرم

## مأموریت اصلی
- به توسعه‌دهندگان گوش دهید و همدل باشید – درک نقاط درد، جریان‌های کاری و نیازهای آن‌ها از طریق مصاحبه، نظرسنجی و تحلیل استفاده
- کاهش بار شناختی بر روی توسعه‌دهندگان – مدیریت پیچیدگی زیرساخت تا توسعه‌دهندگان بتوانند بر روی تخصص اصلی خود تمرکز کنند: نوشتن ویژگی‌های کسب‌وکاری
- با تیم‌های توسعه‌دهنده به عنوان مشتری رفتار کنید و برای تعیین بهترین شیوه‌ها با آن‌ها همکاری کنید

## بهره‌وری و تجربه توسعه‌دهنده
- ساخت، تست و انتشار نرم‌افزار را برای توسعه‌دهندگان بی‌دردسر کنید – تا حد امکان اصطکاک را از چرخه عمر توسعه حذف کنید
- کاهش زمان ورود به پروژه (Onboarding) – محیط‌ها و جریان‌های کاری توسعه را الگوسازی کنید تا مهندسان جدید از روز اول بتوانند مشارکت کنند
- قابلیت بهره‌وری "از روز اول" را فراهم کنید – الگوهایی برای انواع رایج اپلیکیشن‌ها (Go، Java، Python، React) ارائه دهید تا توسعه‌دهندگان بتوانند بلافاصله کدنویسی را شروع کنند
- بهبود تجربه توسعه‌دهنده – اطمینان از راه‌اندازی آسان محیط‌های توسعه، کاهش زمان ورود به پروژه برای توسعه‌دهندگان جدید، و استفاده از فناوری‌های مدرن و لذت‌بخش
- راهنمایی تیم‌ها برای نوشتن تست‌های واحد، تست‌های یکپارچه‌سازی، تست‌های سرتاسری و تست‌های API با استفاده از زیرساخت تست پلتفرم برای آسان‌تر کردن نوشتن تست برای توسعه‌دهندگان

## طراحی و مهندسی پلتفرم
- طراحی، ساخت و نگهداری زیرساخت و ابزارهایی که از توسعه و استقرار نرم‌افزار پشتیبانی می‌کنند
- انتزاع پیچیدگی زیرساخت – پنهان کردن پیچیدگی ابزارهای مدرن ابری-بومی (Kubernetes، Terraform، Helm، YAML و غیره) تا توسعه‌دهندگان بتوانند بر روی کد اپلیکیشن تمرکز کنند
- ارائه ابزارها و چارچوب‌های استاندارد برای ساده‌سازی فرآیند توسعه و کاهش بار شناختی بر روی توسعه‌دهندگان
- ساخت ماژول‌های زیرساخت قابل استفاده مجدد (الگوهای ساختمانی) – ایجاد ماژول‌های Terraform برای الگوهای رایج که امنیت، شبکه‌سازی و قابلیت مشاهده را در خود دارند و امکان ورود سریع و یکپارچه به پروژه را فراهم می‌کنند
- ارائه بلوک‌های ساختمانی با بهترین شیوه‌های تعبیه‌شده – ایجاد مؤلفه‌های زیرساخت قابل استفاده مجدد و نسخه‌گذاری شده (مثلاً با استفاده از CDK constructs) که شامل سیاست‌های مختص شرکت، استانداردهای رمزنگاری، پیش‌فرض‌های امنیتی و الزامات انطباق است
- انتشار بسته‌های زیرساخت نسخه‌گذاری شده – انتشار مؤلفه‌های پلتفرم به عنوان بسته‌های نسخه‌گذاری شده (مثلاً از طریق NuGet، Maven) تا تیم‌ها بتوانند مانند هر وابستگی دیگری از آن‌ها استفاده کنند، با نسخه‌گذاری معنایی و یادداشت‌های انتشار
- استانداردسازی ابزارها و خدمات مورد نیاز برای نیازمندی‌های غیرعملکردی اپلیکیشن‌ها (CI/CD، کنترل نسخه، محیط اجرا، لاگ‌گیری، نظارت، امنیت) در تمام تیم‌های محصول
- ارائه پشته مشاهده‌پذیری متمرکز – ارائه خدمات لاگ‌گیری، تلمتری و ردیابی مشترک تا همه اپلیکیشن‌ها داده‌ها را به روشی یکپارچه برای نظارت بر سلامت و اشکال‌زدایی انتشار دهند

## حاکمیت و بهترین شیوه‌ها
- استانداردسازی، اما امکان انعطاف‌پذیری – ایجاد پیش‌فرض‌های نظرپایه و "مسیرهای طلایی" برای قابلیت‌های اصلی و در عین حال اجازه دادن به سفارشی‌سازی در صورت نیاز، با مستندسازی واضح حوزه‌های قابل مذاکره
- تعبیه بهترین شیوه‌ها و راهنماها از طریق زیرساخت به‌عنوان کد (IaC) – ایجاد الگوهای قابل استفاده مجدد با امنیت، انطباق، نظارت و استانداردهای پیکربندی تعبیه‌شده، و در عین حال اجازه دادن به پارامترهای مختص تیم
- ایجاد الگوها و شیوه‌ها – تعریف رویکردهای یکپارچه برای ساختار کد، تعاملات لایه‌ها، ارتباطات بین سرویس‌ها و سایر دغدغه‌های افقی
- تعادل بین استانداردسازی و خودمختاری – اعمال راهنماها و یکپارچگی در جایی که نیاز است، اما اجازه دادن به تیم‌ها برای سفارشی‌سازی استفاده خود در محدوده پلتفرم
- ارائه انعطاف‌پذیری و انتخاب – تیم‌ها را به یک ابزار واحد محدود نکنید؛ در عوض، از گزینه‌های استاندارد متعدد پشتیبانی کنید و ابزارهای جدید را در صورت درخواست و زمانی که ارزش افزوده دارند، یکپارچه کنید

## امنیت و انطباق
- اجرای امنیت و انطباق به‌صورت پیش‌فرض – تعبیه امنیت، حاکمیت و انطباق در پلتفرم از ابتدا تا تیم‌ها مجبور نباشند به آن فکر کنند
- حفظ امنیت، انطباق و یکپارچگی – اطمینان از اینکه تمام خدمات پلتفرم با سیاست‌های امنیتی و الزامات نظارتی سازمان مطابقت دارند، و ارائه مسیرهای حسابرسی و دید انطباق برای تیم‌های حاکمیت

## قابلیت اطمینان و مقیاس‌پذیری
- تضمین مقیاس‌پذیری و انعطاف‌پذیری – طراحی زیرساخت که بتواند حجم کار فزاینده را مدیریت کند و استفاده از اتوماسیون/فناوری‌های ابری برای مقیاس‌پذیری یکپارچه
- تضمین قابلیت اطمینان و پایداری – پیاده‌سازی نظارت قوی، پشتیبان‌گیری خودکار و مکانیسم‌های بازیابی پس از فاجعه

## بهینه‌سازی هزینه
- ارائه بهینه‌سازی هزینه از طریق پلتفرم – اعمال پیش‌فرض‌های کارآمد از نظر هزینه (مقیاس‌پذیری خودکار، محدودیت‌های منابع) و پیگیری صرفه‌جویی در هزینه به عنوان یک معیار کلیدی

## ترکیب تیم و فرهنگ
- داشتن مهندسین با تجربه هم در توسعه و هم در سیستم‌ها – مهندسان ایده‌آل پلتفرم دارای مهارت‌های برنامه‌نویسی قوی به همراه تجربه عملیاتی (سیستم‌عامل، شبکه، سیستم‌های توزیع‌شده، نظارت) هستند
- داشتن تیم پایدار و اختصاصی – تیم پلتفرم باید یک تیم دائمی و مستمر باشد، نه یک گروه موقت که پس از ساختن چیزی منحل شود
- ترکیب سه مجموعه مهارت در تیم – مهندسی نرم‌افزار (برای ساختن انتزاعات)، مهارت‌های سیستمی (برای عملکرد قابل اطمینان)، و همدلی محصول/مشتری (برای تمرکز بر نیازهای کاربر)
- اجتناب از نقش یک پذیرنده درخواست یا گلوگاه بوروکراتیک – تبدیل به تیمی پر از فرآیند نشوید که "نه" می‌گوید؛ بلکه یک توانمندساز باشید که مشکلات را برای توسعه‌دهندگان حل می‌کند

## عملیات و نگهداری
- کاهش درد مهاجرت برای تیم‌های اپلیکیشن – انجام ارتقاءها، وصله‌های امنیتی و مهاجرت‌ها (ارتقاء EKS، به‌روزرسانی نسخه Python) در داخل پلتفرم به جای اینکه آن کار را به تیم‌های توسعه محول کنید
- تعریف و حفظ نقشه راه فناوری – هدایت جهت‌گیری فنی سازمان و اطمینان از همسویی بین تیم‌ها
- اتخاذ تصمیمات استراتژیک فناوری – پاسخ به سوالات سطح بالا مانند یکپارچه در مقابل میکروسرویس‌ها، انتخاب ارائه‌دهنده ابر، و سایر انتخاب‌های معماری
- ارزیابی، انتخاب و یکپارچه‌سازی ابزارها و خدمات شخص ثالث تا توسعه‌دهندگان مجبور نباشند هر کدام را به صورت جداگانه ارزیابی کنند

## همکاری و پشتیبانی
- همکاری نزدیک با تیم‌های اپلیکیشن – درک نقاط درد، گلوگاه‌ها و جریان‌های کاری آن‌ها، و اولویت‌بندی ویژگی‌های پلتفرم که واقعاً بار شناختی آن‌ها را کاهش می‌دهند
- کار با تیم‌های زیرساخت/ابر – مشارکت با تیم‌های ابر، داخلی و امنیتی برای بهره‌گیری از تخصص آن‌ها و اطمینان از اجرای پلتفرم بر روی یک پایه مستحکم و با مدیریت خوب
- ارائه مستندات و پشتیبانی واضح – ارائه راهنماهای ورود به پروژه، منابع عیب‌یابی و کانال‌های پشتیبانی پاسخگو برای کمک به توسعه‌دهندگان در استفاده مؤثر از پلتفرم
- تسهیل همکاری و اشتراک دانش بین تیم‌ها – ارائه راهنمایی فنی و ترویج همکاری بین‌فункциональی
- هدایت بهبود مستمر – بررسی فناوری‌ها، ابزارها و شیوه‌های جدید برای بهبود پلتفرم

## ذهنیت محصول
- توسعه مستمر پلتفرم به عنوان یک محصول – با پلتفرم توسعه‌دهنده داخلی مانند یک محصول با نقشه راه، انتشارات، افزودن ویژگی‌ها، رفع اشکال و بهبودهای تدریجی مبتنی بر بازخورد کاربر رفتار کنید
- رفتار با کل زنجیره ابزار تحویل نرم‌افزار به عنوان یک محصول – گرد هم آوردن ابزارهای منزوی DevOps، CI/CD و عملیات در یک پلتفرم منسجم، که به عنوان یک محصول به توسعه‌دهندگان داخلی ارائه می‌شود

## اندازه‌گیری
- اندازه‌گیری کاهش درد مهاجرت – پیگیری میزان تلاشی که پلتفرم در طول ارتقاءها و مهاجرت‌ها برای تیم‌ها صرفه‌جویی می‌کند