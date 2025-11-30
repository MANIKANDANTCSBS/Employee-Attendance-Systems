⚙️ Setup Instructions
1️⃣ Clone the repository
git clone <YOUR_REPO_URL>
cd attendance-tracker-pro-main

2️⃣ Install dependencies
npm install
# or
yarn install
# or
pnpm install

3️⃣ Create a .env file (optional, based on .env.example)
cp .env.example .env

🏃 How to Run
📌 Development Mode
npm run dev


Open the URL shown in the terminal (http://localhost:5173).

📌 Build for Production
npm run build
npm run preview

🔐 Seed Users (Demo Login Credentials)
Role	Email	Password
Employee	john@company.com
	password123
Manager	sarah@company.com
	password123

Mock attendance is auto-generated when the app starts.

🌱 Seed Data Location

Users: src/stores/authStore.ts → mockUsers

Attendance: src/stores/attendanceStore.ts → generateMockData()

Data is persisted in LocalStorage using Zustand

🔑 Environment Variables

Create a .env file in root (optional):

VITE_APP_NAME=Attendance Tracker Pro
VITE_API_BASE_URL=
VITE_USE_MOCK_DATA=true



📸 Screenshots

Add your own screenshots in the /screenshots folder.

![Login](./screenshots/login.png)
![Dashboard](./screenshots/dashboard.png)
![Team Calendar](./screenshots/calendar.png)
