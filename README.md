Budget Predictor App

A mobile application built with React Native (Expo) that helps users track their expenses and predict overspending dates using simple analytics and visual charts.

Features

📊 Expense Tracking
Add, edit, and delete daily expenses with category, amount, and date.

💰 Budget Management
Set a monthly budget and monitor remaining balance.

🔮 Prediction Logic
AI-powered calculation to predict when you will exceed your budget:

"At this rate, you'll overspend by 20th of the month."

📈 Visual Insights

Pie chart for category-wise spending.

Line graph for daily spending trends.

💾 Local Data Storage
Uses AsyncStorage to save data securely on the device.

🌈 Beautiful UI
Modern, clean design using NativeWind (Tailwind for React Native).

Tech Stack
Layer	Technology
Frontend	React Native (Expo)
Navigation	React Navigation
State Storage	React Context API or Redux (Optional)
Local Storage	AsyncStorage
Charts	Victory Native / React Native SVG Charts
Styling	NativeWind (Tailwind)
Screenshots

(Add screenshots of your app here)

/assets/screenshots/
  ├── dashboard.png
  ├── add-expense.png
  └── insights.png

Project Structure
budget-predictor/
│
├── App.js
├── package.json
├── README.md
├── tailwind.config.js
│
├── components/
│   ├── ExpenseForm.js
│   ├── BudgetCard.js
│   └── PredictionAlert.js
│
├── screens/
│   ├── Dashboard.js
│   ├── AddExpense.js
│   └── Insights.js
│
└── assets/
    ├── icons/
    │   ├── food.png
    │   ├── transport.png
    │   └── bills.png
    └── screenshots/

Installation & Setup

Follow these steps to get the app running locally.

1. Prerequisites

Make sure you have installed:

Node.js
 (v18 or above)

Expo CLI

Git

Verify installations:

node -v
npm -v
git --version

2. Clone the Repository
git clone https://github.com/your-username/budget-predictor.git
cd budget-predictor

3. Install Dependencies
npm install


If you see a cross-env error on Windows, install it manually:

npm install cross-env

4. Start the Development Server
npx expo start


This will open Expo Developer Tools in your browser.

Scan the QR code using the Expo Go app on your phone.

5. Run on Emulator (Optional)

Android Emulator → Use Android Studio.

iOS Simulator → Requires Xcode (macOS only).

Usage

Set a Monthly Budget on the dashboard.

Add Expenses daily:

Amount

Category

Date

View prediction alerts to know when you might overspend.

Check Insights screen for trends and analytics.

Prediction Formula

The app uses a simple formula to forecast overspending:

Average Daily Spend = Total Spent ÷ Days Passed
Predicted Day = Total Budget ÷ Average Daily Spend


Example:

Total Budget: ₹15,000

Total Spent: ₹7,000

Day of Month: 10

Average Daily Spend = 7000 / 10 = 700
Predicted Day = 15000 / 700 = 21.4


Result: At this rate, you will overspend by day 21.

Available Scripts
Script	Description
npm start	Starts the app using Expo.
npm run dev	Starts with environment variables using cross-env.
npm run build	Builds the app for production.
Common Issues & Fixes
Issue: 'cross-env' is not recognized

Solution:

npm install cross-env


Or update package.json script for Windows:

"dev": "set EXPO_NO_TELEMETRY=true && expo start"

Issue: App won't load after installing NativeWind

Solution:

npx expo start -c


This clears Expo's cache.

Contributing

Fork the project.

Create a feature branch:

git checkout -b feature-name


Commit changes:

git commit -m "Add some feature"


Push to branch:

git push origin feature-name


Open a Pull Request.

License

This project is licensed under the MIT License.
See the LICENSE
 file for details.

Contact

Author: Jyoti Kumari
📧 Email: jyoti.kumari.098013@gmail.com
🔗 LinkedIn: https://www.linkedin.com/in/jyoti-kumari-35729125b/


