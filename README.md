# 🎓 EduMind AI 2.0

EduMind AI is an advanced AI-powered learning platform designed to make studying smarter, more engaging, and personalized.  
Built with **React + Supabase + Paystack + OpenAI GPT**, it integrates intelligent chat learning, flashcards, and progress tracking.

---

## 🚀 Features

### 🧠 Core AI Functions
- GPT-powered conversational tutor for any topic  
- Smart flashcard generator  
- Voice reading (Text-to-Speech)  
- Analytics dashboard for learning progress

### 🔐 User Management
- Secure signup/login (Supabase Auth)  
- Profile & settings pages  
- Session management and logout

### 💳 Subscription System
- Paystack integration  
- Monthly/yearly plans in responsive pricing table  
- Webhook verification  
- Access control for premium users

### 💾 Backend
- Supabase (PostgreSQL + Auth + Edge Functions)  
- Paystack webhooks + GPT API connections

### ⚡ Tech Stack
React 18 • Tailwind CSS • Framer Motion • Recharts  
Supabase • Paystack • OpenAI • Vercel / Expo  

---

## 🧩 Folder Structure
EduMind-AI/
├── src/components/{ChatAssistant,Flashcards,Dashboard,Pricing,Auth}/  
├── src/pages/{index,dashboard,pricing,login,signup}.tsx  
├── src/lib/{supabaseClient,paystack,openai}.ts  
├── supabase/{schema.sql,functions/}  
└── .env.local

---

## ⚙️ Environment Variables
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
PAYSTACK_SECRET_KEY=your_paystack_secret_key
NEXT_PUBLIC_PAYSTACK_PUBLIC_KEY=your_paystack_public_key
OPENAI_API_KEY=your_openai_api_key

---

## 🪄 Installation
```bash
git clone https://github.com/yourusername/edumind-ai.git
cd edumind-ai
npm install
npm run dev
💰 Payment Flow
1️⃣ User picks plan
2️⃣ Paystack checkout opens
3️⃣ Webhook verifies payment
4️⃣ Supabase updates subscription
5️⃣ Premium access unlocked

🧠 AI Chat Flow
User → GPT via Edge Function → Supabase log → Real-time chat update

📊 Database Tables
profiles
| id | full_name | email | avatar_url | created_at |

subscriptions
| id | user_id | plan | amount | status | created_at |

🧩 Roadmap
 Quiz generation

 AI note summarizer

 Mobile push notifications

 EduMind mobile app launch
```
👨🏽‍💻 Author
Karl Seyram (DJ VALENCY)
Pentester | AI Engineer | EduMind Creator 🇬🇭

🪶 License
MIT © 2025 Karl Seyram
