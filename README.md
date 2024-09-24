# Sushi Cult

Sushi Cult is a Flutter-based application designed for sushi lovers who want a convenient and enjoyable way to order their favorite sushi dishes. The app provides a seamless user experience with an attractive interface and intuitive navigation.

## Table of Contents

- [Features](#features)
- [Architecture](#architecture)
- [Models](#models)
- [Pages](#pages)
- [State Management](#state-management)
- [Getting Started](#getting-started)

## Features

- **User-Friendly Interface**: The app is designed with a clean and modern UI, making it easy for users to browse through the menu and place orders.
- **Menu Display**: A dynamic menu showcasing various sushi dishes, allowing users to select their favorites.
- **Cart Functionality**: Users can add items to their cart, review their selections, and proceed to checkout.
- **Responsive Design**: The app is optimized for both mobile and tablet devices, ensuring a smooth experience across different screen sizes.

## Architecture

The Sushi Cult app follows a structured architecture that enhances maintainability and scalability. It utilizes the Model-View-ViewModel (MVVM) pattern, which separates the business logic from the UI components, allowing for easier testing and code management.

### Main Components

- **Models**: Represents the data structure of the application (e.g., `Shop`, `MenuItem`).
- **Views**: Contains the UI components, including the introduction page, menu page, and cart page.
- **Providers**: Manages the state of the application, enabling communication between different parts of the app.

## Models

### Shop
The `Shop` model serves as the central data repository for the application. It manages the list of menu items, the user's cart, and other essential functionalities.

#### Key Properties:
- **menuItems**: A list of available sushi items.
- **cartItems**: A list of items added to the user's cart.
  
#### Methods:
- **addItemToCart(MenuItem item)**: Adds the selected menu item to the cart.
- **removeItemFromCart(MenuItem item)**: Removes the specified item from the cart.
- **clearCart()**: Empties the cart, allowing users to start fresh.

## Pages

### IntroPage
The entry point of the application, presenting a welcoming introduction to users. This page typically includes branding elements and navigational prompts.

### MenuPage
Displays a comprehensive list of sushi dishes available for order. Users can browse through different categories, view item details, and add items to their cart.

### CartPage
Allows users to review their selected items before checkout. Users can modify quantities, remove items, and see the total price of their order.

## State Management

Sushi Cult utilizes the Provider package for state management, which simplifies the process of sharing and managing application state across different widgets. The `ChangeNotifierProvider` allows the `Shop` model to notify the UI of changes, ensuring that the interface remains updated without unnecessary complexity.

