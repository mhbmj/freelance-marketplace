# مستند ساختار مدیریت پروژه در جیرا (Jira Project Backlog)
## پروژه: سامانه بازار کار فریلنسری (Freelance Marketplace)
**تیم:** مهتاب (Mahtab) | **درس:** آزمایشگاه مهندسی نرم‌افزار  

---

## ۱. اپیک‌ها (Epics)

### Epic 1: مدیریت کاربران، احراز هویت و پروفایل
* **Summary:** `User Management, Authentication & Profiles`
* **Description:** شامل کلیه نیازمندی‌ها و فرآیندهای ثبت‌نام، ورود با متدهای مختلف، تفکیک نقش کارفرما/فریلنسر و مدیریت پروفایل و پورتفولیو.

### Epic 2: چرخه حیات پروژه‌ها و مدیریت پیشنهادها
* **Summary:** `Project Lifecycle & Proposal Management`
* **Description:** شامل ثبت پروژه توسط کارفرما، دسته‌بندی و جستجوی پیشرفته توسط فریلنسرها، ارسال پروپوزال، بررسی پیشنهادها و انتخاب فریلنسر.

### Epic 3: پرداخت امن، قراردادها و ارزیابی
* **Summary:** `Escrow Payments, Contracting & Reviews`
* **Description:** ایجاد قرارداد، واریز وجه امانی در صندوق Escrow، پرداخت مرحله‌ای (Milestones)، آزادسازی وجه به فریلنسر و امتیازدهی دوطرفه.

---

## ۲. داستان‌های کاربر (User Stories)

### زیرمجموعه Epic 1:
1. **Story 1: ثبت‌نام با ایمیل یا پیامک و انتخاب نقش**
   * **Summary:** `User Registration & Role Selection`
   * **User Story:**
     > **As a** new user,  
     > **I want to** register using my email or phone number and choose whether I am a Client, Freelancer, or both,  
     > **So that** I can access the appropriate platform dashboard and tools.
   * **Acceptance Criteria:**
     - کاربر بتواند شماره موبایل یا ایمیل خود را وارد کند و کد تأیید دریافت نماید.
     - در فرم ثبت‌نام گزینه انتخاب نقش (Client / Freelancer) اجباری باشد.
     - رمز عبور باید حداقل ۸ کاراکتر و دارای پیچیدگی لازم باشد.
   * **Story Points:** 5

2. **Story 2: ساخت و ویرایش پروفایل و پورتفولیوی فریلنسر**
   * **Summary:** `Freelancer Profile & Portfolio Setup`
   * **User Story:**
     > **As a** freelancer,  
     > **I want to** add my title, bio, hourly rate, skills, and portfolio items,  
     > **So that** potential clients can evaluate my qualifications and past work.
   * **Acceptance Criteria:**
     - امکان افزودن حداقل ۵ مهارت از لیست پیش‌فرض یا تگ جدید.
     - امکان بارگذاری تصویر نمونه‌کار همراه با عنوان و توضیحات.
     - نمایش پیش‌نمایش عمومی پروفایل فریلنسر.
   * **Story Points:** 5

---

### زیرمجموعه Epic 2:
3. **Story 3: ثبت آگهی پروژه توسط کارفرما**
   * **Summary:** `Project Posting by Client`
   * **User Story:**
     > **As a** client,  
     > **I want to** create a new project post with title, description, skills, budget, and deadline,  
     > **So that** qualified freelancers can discover it and send proposals.
   * **Acceptance Criteria:**
     - فیلدهای عنوان، مهارت‌های مورد نیاز و محدوده بودجه اجباری باشند.
     - امکان ضمیمه کردن فایل راهنما (PDF/Word/ZIP تا سقف ۲۵ مگابایت).
     - ذخیره پیش‌نویس (Draft) قبل از انتشار نهایی.
   * **Story Points:** 5

4. **Story 4: جستجو و فیلتر پیشرفته پروژه‌ها**
   * **Summary:** `Advanced Project Search & Filtering`
   * **User Story:**
     > **As a** freelancer,  
     > **I want to** search projects by keywords and filter by skill, budget range, and recency,  
     > **So that** I can quickly find opportunities matching my expertise.
   * **Acceptance Criteria:**
     - فیلتر بر اساس تگ مهارت‌ها به صورت چندانتخابی.
     - فیلتر بر اساس بازه حداقل و حداکثر بودجه.
     - مرتب‌سازی بر اساس جدیدترین، بیشترین بودجه و کمترین تعداد پیشنهاد.
   * **Story Points:** 3

5. **Story 5: ارسال پیشنهاد همکاری (Proposal) توسط فریلنسر**
   * **Summary:** `Proposal Submission with Cover Letter`
   * **User Story:**
     > **As a** freelancer,  
     > **I want to** submit a proposal with my bid amount, delivery time, and cover letter,  
     > **So that** the client can consider me for the project.
   * **Acceptance Criteria:**
     - فریلنسر نتواند برای یک پروژه بیش از یک پیشنهاد فعال ارسال کند.
     - مبلغ پیشنهادی و زمان تخمینی باید اعتبارسنجی شوند (اعداد مثبت).
     - امکان الصاق نمونه‌کارهای مرتبط از پروفایل به پروپوزال.
   * **Story Points:** 5

6. **Story 6: بررسی، مقایسه و پذیرش پیشنهاد توسط کارفرما**
   * **Summary:** `Proposal Review and Freelancer Hiring`
   * **User Story:**
     > **As a** client,  
     > **I want to** view a list of received proposals, compare bids, and accept the best one,  
     > **So that** a formal contract is generated with the selected freelancer.
   * **Acceptance Criteria:**
     - نمایش لیست کامل فریلنسرهای متقاضی همراه با رتبه و قیمت پیشنهادی.
     - امکان رد پیشنهاد (Decline) با ارسال پیام خودکار مؤدبانه.
     - پذیرش پیشنهاد منجر به تغییر وضعیت پروژه به مرحله ایجاد قرارداد شود.
   * **Story Points:** 5

---

### زیرمجموعه Epic 3:
7. **Story 7: پرداخت امن و قفل وجه در صندوق Escrow**
   * **Summary:** `Escrow Milestone Funding`
   * **User Story:**
     > **As a** client,  
     > **I want to** deposit the milestone payment into a secure platform escrow account,  
     > **So that** the freelancer can start working with financial peace of mind.
   * **Acceptance Criteria:**
     - اتصال به درگاه پرداخت اینترنتی و شارژ حساب امانی پروژه.
     - ثبت رکورد مالی با شناسه رهگیری یکتا و تغییر وضعیت مایلستون به «تأمین مالی‌شده (Funded)».
     - ارسال نوتیفیکیشن فوری به فریلنسر مبنی بر مجاز بودن شروع کار.
   * **Story Points:** 8

8. **Story 8: آزادسازی وجه مایلستون و ثبت بازخورد دوطرفه**
   * **Summary:** `Milestone Release & Double-Blind Review`
   * **User Story:**
     > **As a** user (client or freelancer),  
     > **I want to** release completed milestone payments and exchange ratings/reviews,  
     > **So that** the financial cycle closes and our public reputation updates.
   * **Acceptance Criteria:**
     - کارفرما بتواند پس از بازبینی خروجی، دکمه «تأیید و آزادسازی وجه» را کلیک کند.
     - سیستم کارمزد پلتفرم را کسر کرده و خالص مبلغ را به کیف پول فریلنسر اضافه کند.
     - فرم امتیازدهی ۱ تا ۵ ستاره همراه با متن نظر فعال شود.
   * **Story Points:** 8

---

## ۳. وظایف فنی (Tasks)

1. **Task 1: راه‌اندازی ساختار بک‌اند جنگو و اتصال به PostgreSQL**
   * **Summary:** `Setup Django Architecture & PostgreSQL Database Connection`
   * **Description:** ساخت پروژه Django، ایجاد اپلیکیشن‌های اصلی (`accounts`, `projects`, `payments`) و اتصال تنظیمات پایگاه‌داده به دیتابیس `freelance_lab`.
   * **Component:** Backend / Database
   * **Status پیشنهادی روی برد:** `Done`

2. **Task 2: راه‌اندازی اولیه اپلیکیشن React و سیستم مسیریابی**
   * **Summary:** `Initialize React.js App with TailwindCSS and Router`
   * **Description:** ساخت اسکلت کلاینت با React و Vite، نصب پکیج‌های TailwindCSS و React Router و ساخت صفحات پایه داشبورد کارفرما و فریلنسر.
   * **Component:** Frontend
   * **Status پیشنهادی روی برد:** `In Progress`

3. **Task 3: پیکربندی مخزن گیت و ایجاد ساختار مستندات نیازمندی‌ها**
   * **Summary:** `Configure Git Workflow & Document Requirements Specification`
   * **Description:** تنظیم ریپازیتوری `freelance-marketplace`، مستندسازی نیازمندی‌های عملکردی و غیرعملکردی در `docs/requirements.md` و ادغام Pull Request.
   * **Component:** DevOps / Documentation
   * **Status پیشنهادی روی برد:** `Done`

---

## ۴. اسپرینت ۲: فاز طراحی و پیاده‌سازی پایگاه داده (Sprint 2: Database Design & Implementation)

این بخش منعکس‌کننده مراحل کامل انجام تکلیف دوم درس آزمایشگاه مهندسی نرم‌افزار در سیستم مدیریت پروژه جیرا است:

### Task 4: مدل‌سازی مفهومی، منطقی و تدوین نمودار ERD
* **Issue Key:** `FM-TASK-4`
* **Summary:** `Conceptual & Logical Data Modeling and ERD Diagram Design`
* **Description:** تحلیل کامل نیازمندی‌های داده‌ای، موجودیت‌ها (کاربران، مدیران، پروفایل‌ها، پروژه‌ها، پیشنهادها، مهارت‌ها و دسته‌بندی‌ها)، تعیین کاردینالیتی روابط و رسم نمودار استاندارد ERD.
* **Component:** Database / Architecture
* **Linked Stories:** `Story 1`, `Story 2`, `Story 4`, `Story 5`, `Story 6`
* **Status:** `Done`
* **Sub-tasks:**
  - `FM-SUB-4.1`: استخراج موجودیت‌ها، ویژگی‌ها و کلیدهای اصلی و خارجی
  - `FM-SUB-4.2`: مدل‌سازی رابطه ۱ به ۱ اختیاری مدیران سیستم (جدول `admins`)
  - `FM-SUB-4.3`: مدل‌سازی روابط چندبه‌چند با جداول واسط (`user_skills`, `project_categories`, `project_skills`)
  - `FM-SUB-4.4`: طراحی و تولید فایل تصویری نمودار ERD در `docs/erd.png` و سورس `docs/erd.puml`

### Task 5: پیاده‌سازی اسکریپت DDL و ساختار جداول پایگاه داده در PostgreSQL
* **Issue Key:** `FM-TASK-5`
* **Summary:** `PostgreSQL DDL Implementation, Tables, and Structural Constraints`
* **Description:** نگارش اسکریپت `database/schema.sql` جهت ساخت تمیز جداول، انواع داده دقیق، محدودیت‌های کلید اصلی/خارجی، رفتار ON DELETE، محدودیت‌های CHECK و ایندکس‌ها.
* **Component:** Database / Backend
* **Linked Stories:** `Story 1`, `Story 2`, `Story 4`
* **Status:** `Done`
* **Sub-tasks:**
  - `FM-SUB-5.1`: پیاده‌سازی جدول `users` با هش پسورد و اعتبارسنجی فرمت ایمیل و حذف منطقی (Soft Delete)
  - `FM-SUB-5.2`: پیاده‌سازی جداول `user_profiles`، `portfolios` و `certificates`
  - `FM-SUB-5.3`: پیاده‌سازی جداول پایه `categories` و `skills` و جداول واسط
  - `FM-SUB-5.4`: پیاده‌سازی جدول `projects` با محدودیت بودجه مثبت و وضعیت‌های چرخه حیات
  - `FM-SUB-5.5`: پیاده‌سازی جدول `proposals` با محدودیت یکتایی فریلنسر به ازای هر پروژه

### Task 6: اتوماسیون قواعد کسب‌وکار و یکپارچگی داده با Triggerها و توابع PL/pgSQL
* **Issue Key:** `FM-TASK-6`
* **Summary:** `Business Logic Automation using PostgreSQL Functions and Triggers`
* **Description:** پیاده‌سازی قواعد کسب‌وکار پیچیده و حیاتی پلتفرم که صرفاً با CHECKهای معمولی قابل اعمال نیستند.
* **Component:** Database / Business Logic
* **Linked Stories:** `Story 5`, `Story 6`
* **Status:** `Done`
* **Sub-tasks:**
  - `FM-SUB-6.1`: ایجاد ایندکس یکتایی شرطی (Partial Unique Index) جهت تضمین حداکثر یک پیشنهاد پذیرفته شده (`status = 'ACCEPTED'`)
  - `FM-SUB-6.2`: پیاده‌سازی تریگر `trg_check_project_admin` جهت منع ثبت پروژه توسط حساب‌های مدیر (قاعده ۱۰)
  - `FM-SUB-6.3`: پیاده‌سازی تریگر `trg_check_proposal_rules` جهت منع ارسال پیشنهاد توسط ادمین، پیشنهاد کارفرما روی پروژه خود، و محدودیت ثبت روی پروژه‌های OPEN
  - `FM-SUB-6.4`: پیاده‌سازی تریگر `trg_proposal_accepted` جهت تغییر خودکار وضعیت پروژه به `IN_PROGRESS` پس از پذیرش پیشنهاد
  - `FM-SUB-6.5`: پیاده‌سازی تریگرهای عمومی به‌روزرسانی فیلد `updated_at`

### Task 7: تولید داده‌های اولیه غنی و آزمایشی (Seed Data)
* **Issue Key:** `FM-TASK-7`
* **Summary:** `Comprehensive Seed Data Generation for Development & Testing`
* **Description:** تدوین فایل `database/seed.sql` منطبق با شرایط سناریوی عملیاتی پلتفرم جهت تست و مشاهده نتایج واقعی.
* **Component:** Database / QA
* **Linked Stories:** `Story 1`, `Story 4`, `Story 5`, `Story 6`
* **Status:** `Done`
* **Sub-tasks:**
  - `FM-SUB-7.1`: ثبت ۱ حساب مدیر سیستم، ۲ کارفرما، ۲ فریلنسر و حداقل ۱ کاربر با نقش دوطرفه (کارفرما/فریلنسر)
  - `FM-SUB-7.2`: ایجاد پروفایل‌ها، نمونه‌کارها و مدارک بین‌المللی مرتبط
  - `FM-SUB-7.3`: تعریف حداقل ۴ دسته‌بندی و ۷ مهارت تخصصی و انتساب آنها
  - `FM-SUB-7.4`: درج ۴ پروژه در وضعیت‌های مختلف (`OPEN`, `IN_PROGRESS`, `DRAFT`, `COMPLETED`)
  - `FM-SUB-7.5`: ثبت ۴ پیشنهاد معتبر و شبیه‌سازی فرآیند پذیرش پیشنهاد (تغییر وضعیت به ACCEPTED)

### Task 8: پیاده‌سازی کوئری‌های تحلیلی و عملیاتی پایگاه داده
* **Issue Key:** `FM-TASK-8`
* **Summary:** `Development of Key Operational and Analytical SQL Queries`
* **Description:** نگارش و بهینه‌سازی کوئری‌های SQL کاربردی در فایل `database/queries.sql` برای استفاده در APIها و داشبوردها.
* **Component:** Database / Query Optimization
* **Linked Stories:** `Story 3`, `Story 5`, `Story 6`
* **Status:** `Done`
* **Sub-tasks:**
  - `FM-SUB-8.1`: کوئری استخراج پروژه‌های باز به همراه اطلاعات کارفرما و دسته‌بندی
  - `FM-SUB-8.2`: کوئری واکشی پیشنهادهای یک پروژه مشخص با مشخصات فریلنسر
  - `FM-SUB-8.3`: کوئری گزارش آماری پروژه‌های هر کارفرما و تعداد پیشنهادهای دریافتی (GROUP BY / Aggregations)
  - `FM-SUB-8.4`: کوئری مهارت‌های مورد نیاز پروژه به صورت تجمیعی (STRING_AGG)
  - `FM-SUB-8.5`: کوئری‌های تکمیلی جستجوی پروژه‌ها بر اساس مهارت و گزارش جامع ۳۶۰ درجه فریلنسرها

### Task 9: طراحی اسکریپت آزمون اعتبارسنجی محدودیت‌ها (Constraints Test Suite)
* **Issue Key:** `FM-TASK-9`
* **Summary:** `Automated Database Constraints and Business Rules Verification Script`
* **Description:** تدوین اسکریپت `database/tests.sql` شامل سناریوهای آزمون منفی و مثبت با استفاده از بلوک‌های تراکنشی امن `DO $$` جهت احراز صحت تمامی محدودیت‌ها.
* **Component:** Database / QA & Verification
* **Linked Stories:** All Epics / Security & Rules
* **Status:** `Done`
* **Sub-tasks:**
  - `FM-SUB-9.1`: آزمون رد ایمیل تکراری و کلید خارجی نامعتبر
  - `FM-SUB-9.2`: آزمون رد مقادیر منفی یا صفر برای بودجه و مبالغ پیشنهادی
  - `FM-SUB-9.3`: آزمون رد پیشنهاد تکراری از یک فریلنسر برای یک پروژه
  - `FM-SUB-9.4`: آزمون منع ثبت پیشنهاد توسط کارفرما روی پروژه خودش
  - `FM-SUB-9.5`: آزمون منع فعالیت حساب‌های مدیر در ثبت پروژه و پیشنهاد
  - `FM-SUB-9.6`: آزمون منع ثبت پیشنهاد روی پروژه‌های غیر OPEN
  - `FM-SUB-9.7`: آزمون تضمین حداکثر یک پیشنهاد پذیرفته شده و تغییر خودکار وضعیت پروژه به IN_PROGRESS

