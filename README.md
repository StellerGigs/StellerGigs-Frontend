# StellerGigs-Frontend


  Stellar Gigs — Frontend

 Overview
This is the **frontend application** for Stellar Gigs, built with React to deliver a fast, intuitive, and seamless user experience for freelancers and clients interacting with the platform.
The frontend communicates with a Python (FastAPI) backend and integrates with the Stellar network for real-time payment interactions.

---

## 🎯 Responsibilities
The frontend handles:
- User interface and experience (UI/UX)
- Wallet connection and interaction
- Payment link generation
- Displaying transaction data
- Communicating with backend APIs
- Real-time user feedback and updates

---

## ✨ Features

### 🏠 Landing Page
- Project introduction
- Call-to-action for users to get started

---

### 🔐 Wallet Integration
- Connect to Stellar-compatible wallets
- Display wallet address and balance

---

### 🔗 Payment Link Creation
- Input amount and details
- Generate shareable payment links

---

### 💳 Payment Page
- Client-facing page for completing payments
- Displays payment details clearly

---

### 📊 Dashboard
- Overview of:
  - Total earnings
  - Pending payments
  - Completed transactions

---

### 📜 Transaction History
- List of all payments
- Status indicators (pending, completed)

---

## 🧱 Tech Stack

- ⚛️ React  
- 🎨 Tailwind CSS  
- 🌐 Fetch API / Axios  
- 🔗 Stellar SDK (frontend usage where applicable)  

---

## 📁 Project Structure

```

client/
│
├── src/
│   ├── components/        # Reusable UI components
│   │   ├── Navbar.jsx
│   │   ├── PaymentCard.jsx
│   │   └── DashboardStats.jsx
│
│   ├── pages/             # Application pages
│   │   ├── Home.jsx
│   │   ├── Dashboard.jsx
│   │   ├── CreatePayment.jsx
│   │   └── PaymentPage.jsx
│
│   ├── hooks/             # Custom React hooks
│   │   ├── useWallet.js
│   │   └── usePayments.js
│
│   ├── services/          # API & blockchain logic
│   │   ├── api.js
│   │   └── stellarService.js
│
│   ├── utils/             # Helper functions
│   │   └── formatCurrency.js
│
│   ├── App.jsx
│   └── main.jsx
│
├── public/
├── package.json
└── tailwind.config.js

````

---

## ⚙️ Getting Started

### 📦 Prerequisites

- Node.js (v18+)
- npm or yarn

---

### 🚀 Installation

```bash
git clone https://github.com/your-username/stellar-gigs.git
cd stellar-gigs/client
npm install
````

---

### ▶️ Run Development Server

```bash
npm run dev
```

App will be available at:

```
http://localhost:5173
```

---

## 🔗 API Integration

The frontend communicates with the backend via REST APIs.

Example:

```js
fetch("http://localhost:8000/api/payments", {
  method: "GET"
});
```

---

## 🔐 Environment Variables

Create a `.env` file in the `client/` directory:

```
VITE_API_URL=http://localhost:8000
VITE_STELLAR_NETWORK=testnet
```

---

## 🧩 Key Concepts

### State Management

* React hooks (`useState`, `useEffect`)
* Custom hooks for reusable logic

---

### Component Design

* Reusable and modular components
* Separation of concerns

---

### API Communication

* Centralized API service (`services/api.js`)
* Handles all backend requests

---

## 🎨 UI/UX Principles

* Clean and minimal interface
* Mobile-first responsive design
* Accessible components
* Clear feedback for user actions

---

## 🧪 Future Improvements

* Dark mode support
* Real-time updates (WebSockets)
* Improved wallet integrations
* Better error handling and notifications

---

## 🤝 Contribution Guide

We welcome contributions!

### 🟢 Beginner

* Build UI components
* Improve styling
* Fix layout issues

### 🟡 Intermediate

* Connect API endpoints
* Implement features

### 🔴 Advanced

* Optimize performance
* Improve architecture

---

### 🛠️ How to Contribute

1. Fork the repo
2. Create a branch

   ```
   git checkout -b feature/frontend-feature
   ```
3. Make changes
4. Submit a Pull Request




