# 🛍️ ThriftHub Marketplace - Setup Instructions

## 📦 What's Included
This ZIP file contains a complete, fully functional thrift store marketplace website with:

### ✨ Features
- **Three User Roles**: Admin, Seller, and Buyer dashboards
- **Buying System**: Shopping cart, checkout, order tracking
- **Rental System**: Daily pricing, security deposits, rental periods
- **Chat System**: Real-time messaging between users
- **Request System**: Buyers can request specific items
- **Authentication**: Role-based login/registration
- **Responsive Design**: Works on desktop and mobile

### 🎯 Demo Credentials
- **Admin**: admin@thrifthub.com / demo123
- **Seller**: seller@thrifthub.com / demo123
- **Buyer**: buyer@thrifthub.com / demo123

## 🚀 Quick Setup (5 minutes)

### Step 1: Prerequisites
Make sure you have installed:
- **Node.js** (version 18+) - Download from [nodejs.org](https://nodejs.org/)
- **npm** (comes with Node.js)

### Step 2: Extract & Setup
1. **Extract** the ZIP file to your desired location
2. **Open terminal/command prompt** in the extracted folder
3. **Install dependencies**:
   ```bash
   npm install
   ```

### Step 3: Run the Application
1. **Start the development server**:
   ```bash
   npm run dev
   ```
2. **Open your browser** and go to: `http://localhost:3000`

That's it! The marketplace is now running on your computer.

## 📁 Project Structure
```
thrifthub-marketplace/
├── src/
│   ├── app/                 # Pages (Next.js App Router)
│   │   ├── layout.tsx       # Global layout
│   │   ├── page.tsx         # Home page
│   │   ├── login/           # Login page
│   │   ├── register/        # Registration page
│   │   ├── admin/           # Admin dashboard
│   │   ├── seller/          # Seller dashboard
│   │   └── buyer/           # Buyer dashboard
│   ├── components/          # Reusable UI components
│   │   ├── Navigation.tsx   # Top navigation bar
│   │   ├── Chat.tsx         # Chat functionality
│   │   ├── ProductCard.tsx  # Product display cards
│   │   └── ui/              # Shadcn/ui components
│   ├── context/             # Global state management
│   │   └── UserContext.tsx  # User authentication context
│   └── lib/                 # Utility functions
├── public/                  # Static assets
├── package.json            # Project dependencies
└── README.md               # This file
```

## 🛠️ Technology Stack
- **Framework**: Next.js 15 with TypeScript
- **Styling**: Tailwind CSS + Shadcn/ui components
- **State Management**: React Context API
- **Authentication**: Simulated with localStorage
- **Data Storage**: Demo data with local state

## 🎮 How to Use

### As a Buyer:
1. Register/Login as a buyer
2. Browse items by category
3. Add items to cart or wishlist
4. Rent items with daily pricing
5. Request specific items you're looking for
6. Chat with sellers about products

### As a Seller:
1. Register/Login as a seller
2. Add new items for sale or rent
3. Manage your inventory
4. Handle orders and rental requests
5. Update order status
6. Customize your store profile

### As an Admin:
1. Login with admin credentials
2. Manage users and their permissions
3. Monitor transactions and disputes
4. Review reported content
5. View platform analytics

## 🔧 Troubleshooting

### Common Issues:
1. **Port already in use**: The app will automatically find an available port
2. **Dependencies error**: Try `npm install --legacy-peer-deps`
3. **Build errors**: Make sure you're using Node.js 18+

### Getting Help:
- Check the browser console for error messages
- Ensure all files were extracted properly
- Verify Node.js and npm are installed correctly

## 🚀 Next Steps

### For Development:
- The project uses demo data stored in component state
- To make it production-ready, integrate with:
  - Real authentication service (Auth0, Clerk, etc.)
  - Database (PostgreSQL, MongoDB, etc.)
  - File storage (AWS S3, Cloudinary, etc.)
  - Payment processing (Stripe, PayPal, etc.)
  - Real-time chat (Socket.io, Pusher, etc.)

### Customization:
- Modify colors and styling in `src/app/globals.css`
- Add new components in `src/components/`
- Extend functionality in the dashboard pages
- Add new user roles or permissions

## 📝 License
This project is created for educational and demonstration purposes.

---

**Enjoy your ThriftHub marketplace! 🎉**

For questions or support, refer to the code comments and component documentation.
