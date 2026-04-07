#  DealDrop

DealDrop is a full-stack web application that automates product price tracking across any website. Users can monitor price drops by simply pasting a product URL and setting a desired threshold. The system periodically checks prices and notifies users via email when a drop occurs.

---

## 🌐 Live Demo
👉 https://dealdroppro.vercel.app

---

## Features

- 🔗 Track products from **any website** using URL input  
- 📉 Set a **price threshold** and get notified on drops  
- ⏰ Automated **daily price checking (CRON job at 9:00 AM)**  
- 📧 **Email notifications** when price falls below threshold  
- 🔐 **Google OAuth 2.0 authentication** for quick onboarding  
- 📊 Interactive data visualization using **Recharts**  
- ⚡ Fully deployed on **Vercel**  

---

## 🛠️ Tech Stack

### Frontend
- React.js  
- Next.js  
- Tailwind CSS  
- Recharts  

### Backend
- Node.js  
- Express.js  

### Database & Auth
- Supabase (Auth + services)  

### Other Integrations
- Firecrawl API (for scraping product price data)  
- CRON Jobs (for scheduled automation)  
- Nodemailer (for email notifications)  

---

## ⚙️ How It Works

1. User logs in via **Google OAuth**
2. Pastes a product URL
3. Sets a desired price threshold
4. A scheduled CRON job runs daily at **9:00 AM**
5. Firecrawl API fetches the latest price
6. If price < threshold → Email alert is sent

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YashIsTheBest247/DeployDealDrop.git
cd dealdrop
```
### Install dependencies
```bash
npm install
```

### Setup Environment Variable
```bash
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
FIRECRAWL_API_KEY=your_firecrawl_api_key
EMAIL_USER=your_email
EMAIL_PASS=your_email_password
```

### Run server 
```bash
npm run dev
```

### Visit: http://localhost:3000
