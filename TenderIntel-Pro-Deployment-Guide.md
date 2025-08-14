# TenderIntel Pro - სრული განთავსების გზამკვლევი

## 📋 საჭირო მონაცემები

### Supabase Environment Variables
\`\`\`bash
NEXT_PUBLIC_SUPABASE_URL=https://hwnnwgeehqawxrecbwpw.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
SUPABASE_SERVICE_ROLE_KEY=[თქვენი service_role key]
NEXT_PUBLIC_SITE_URL=https://tender-intel-pro.vercel.app
\`\`\`

## 🚀 Vercel Deployment ნაბიჯები

### 1. GitHub Repository შემოწმება
✅ ყველა ფაილი ატვირთული უნდა იყოს:
- `app/` ფოლდერი
- `components/` ფოლდერი
- `lib/` ფოლდერი
- `scripts/` ფოლდერი
- `package.json`
- `next.config.mjs`

### 2. Vercel-ზე Deploy
1. გადადით [vercel.com](https://vercel.com)
2. დააჭირეთ "New Project"
3. აირჩიეთ "TenderIntel-Pro" repository
4. კონფიგურაცია:
   - **Framework Preset:** Next.js
   - **Root Directory:** ./
   - **Build Command:** (ავტომატური)
   - **Output Directory:** (ავტომატური)

### 3. Environment Variables დაყენება
**Environment Variables სექციაში დაამატეთ:**

| Key | Value |
|-----|-------|
| `NEXT_PUBLIC_SUPABASE_URL` | `https://hwnnwgeehqawxrecbwpw.supabase.co` |
| `NEXT_PUBLIC_SUPABASE_ANON_KEY` | `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...` |
| `SUPABASE_SERVICE_ROLE_KEY` | `[service_role key Supabase-იდან]` |
| `NEXT_PUBLIC_SITE_URL` | `https://tender-intel-pro.vercel.app` |

### 4. Deploy და შემოწმება
1. დააჭირეთ "Deploy"
2. დაელოდეთ build process-ს (2-5 წუთი)
3. შეამოწმეთ deployment URL

## 🗄️ Supabase Database Setup

### SQL Scripts (უკვე გაშვებული)
✅ `01_create_tables.sql` - ცხრილების შექმნა
✅ `02_seed_data.sql` - საწყისი მონაცემები
✅ `03_create_functions.sql` - ფუნქციები და triggers

### Test User Credentials
\`\`\`
Email: owner@local
Password: owner123
\`\`\`

## 🔧 Troubleshooting

### Build Errors
თუ "Module not found" შეცდომები გაქვთ:
1. შეამოწმეთ GitHub-ში `components/` ფოლდერი
2. დარწმუნდით რომ ყველა ფაილი ატვირთულია
3. Redeploy გააკეთეთ Vercel-ში

### Environment Variables Errors
1. შეამოწმეთ ყველა key სწორად არის დაწერილი
2. Values-ში არ უნდა იყოს დამატებითი spaces
3. Service Role Key-ი უნდა იყოს სრული (ძალიან გრძელი)

### Database Connection Issues
1. შეამოწმეთ Supabase Project Status
2. დარწმუნდით რომ SQL scripts გაშვებულია
3. შეამოწმეთ API Keys-ების სისწორე

## 📱 Application Features

### მთავარი ფუნქციები
- ✅ ქართული UI
- ✅ Mock Authentication System
- ✅ Dashboard Analytics
- ✅ Tenders Management
- ✅ Reports Generation
- ✅ AI Advisor
- ✅ Responsive Design

### გვერდები
- `/login` - შესვლა
- `/dashboard` - მთავარი dashboard
- `/tenders` - ტენდერების სია
- `/analytics` - ანალიტიკა
- `/advisor` - AI კონსულტანტი
- `/reports` - რეპორტები
- `/settings` - პარამეტრები

## 🔐 Authentication

### Mock System (MVP)
- Email: `owner@local`
- Password: `owner123`
- Role: `owner`

### Production Setup (მომავალში)
1. Supabase Auth-ის ჩართვა
2. Email Confirmation Setup
3. Password Reset Flow
4. Role-based Access Control

## 📊 Database Schema

### მთავარი ცხრილები
- `users` - მომხმარებლები
- `categories` - კატეგორიები (10 ცალი)
- `companies` - კომპანიები (5 სამთავრობო)
- `tenders` - ტენდერები
- `tender_documents` - დოკუმენტები
- `analytics_data` - ანალიტიკური მონაცემები
- `reports` - რეპორტები
- `user_settings` - მომხმარებლის პარამეტრები

## 🌐 Production URLs

### Vercel App
- **Main URL:** https://tender-intel-pro.vercel.app
- **Login:** https://tender-intel-pro.vercel.app/login
- **Dashboard:** https://tender-intel-pro.vercel.app/dashboard

### Supabase
- **Project URL:** https://hwnnwgeehqawxrecbwpw.supabase.co
- **Dashboard:** https://supabase.com/dashboard/project/hwnnwgeehqawxrecbwpw

## 📞 Support

### Common Issues
1. **White Screen:** Environment Variables არასწორია
2. **Build Errors:** Components ფაილები აკლია
3. **Database Errors:** SQL Scripts არ გაშვებულა
4. **Auth Errors:** Mock credentials არასწორია

### Next Steps
1. ✅ Production Deployment
2. 🔄 Real Data Integration (tenders.procurement.gov.ge)
3. 🔄 Advanced AI Features
4. 🔄 Email Notifications
5. 🔄 Multi-user Support

---

**შექმნილია:** TenderIntel Pro v1.0
**ბოლო განახლება:** 2025-01-14
**სტატუსი:** Production Ready 🚀
