# Shopping Cart Application

A modern, responsive e-commerce shopping cart application built with React, Redux Toolkit, and Tailwind CSS. This application fetches products from the Fake Store API and provides a seamless shopping experience with cart management functionality.

## Features

- **Product Catalog**: Browse products fetched from the Fake Store API
- **Shopping Cart**: Add and remove items from cart with real-time updates
- **Responsive Design**: Mobile-first design that works on all screen sizes
- **State Management**: Redux Toolkit for efficient state management
- **Toast Notifications**: User-friendly notifications for cart actions
- **Loading States**: Smooth loading experience with custom spinner
- **Dynamic Cart Counter**: Real-time cart item count in navigation

## Tech Stack

- **Frontend**: React 18
- **State Management**: Redux Toolkit
- **Styling**: Tailwind CSS
- **Routing**: React Router DOM
- **Icons**: React Icons (AI Icons, Font Awesome)
- **Notifications**: React Hot Toast
- **API**: Fake Store API

## Project Structure

```
src/
├── components/
│   ├── CartItem.jsx          # Individual cart item component
│   ├── Navbar.jsx            # Navigation bar with cart counter
│   ├── Product.jsx           # Product card component
│   ├── Spinner.jsx           # Loading spinner component
│   └── Spinner.css           # Spinner styles
├── pages/
│   ├── Cart.jsx              # Cart page with checkout functionality
│   └── Home.jsx              # Home page with product grid
├── redux/
│   ├── Store.jsx             # Redux store configuration
│   └── Slices/
│       └── CartSlice.jsx     # Cart state management
├── App.jsx                   # Main app component with routing
├── main.jsx                  # App entry point
├── index.css                 # Tailwind CSS imports
└── data.js                   # Static product data (backup)
```

## Installation & Setup

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd shopping-cart-app
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

## Key Components

### Cart Management

- **Add to Cart**: Products can be added to cart with instant feedback
- **Remove from Cart**: Items can be removed from both product view and cart page
- **Cart Persistence**: Cart state is maintained across page navigation
- **Total Calculation**: Automatic calculation of total amount

### UI/UX Features

- **Responsive Grid**: Products displayed in responsive grid layout
- **Hover Effects**: Smooth transitions and hover states
- **Loading States**: Custom spinner during API calls
- **Empty States**: Helpful messages when cart is empty
- **Toast Notifications**: Success/error messages for user actions

## API Integration

The app uses the [Fake Store API](https://fakestoreapi.com/) to fetch product data:

- **Endpoint**: `https://fakestoreapi.com/products`
- **Fallback**: Static product data available in `data.js`

## Cart Features

- **Real-time Updates**: Cart counter updates immediately
- **Item Management**: Add/remove items with visual feedback
- **Price Calculation**: Automatic total price calculation
- **Empty Cart Handling**: Graceful handling of empty cart state
- **Checkout Ready**: Structured for easy checkout integration
