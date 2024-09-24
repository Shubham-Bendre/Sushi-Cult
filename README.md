# Sushi Cult

Sushi Cult is a Flutter-based sushi delivery application that I developed to enhance my skills in mobile app development. This project showcases my ability to create an intuitive user interface and manage application state effectively while providing a seamless user experience.

## Features

- **Dynamic Menu**: The application features a comprehensive menu displaying various sushi options, including sushi rolls, sashimi, and specialty dishes. Each menu item is presented with its name, price, and a brief description.

- **Intuitive Navigation**: Users can navigate smoothly between different pages of the app, including the introduction, menu, and cart, all designed for a straightforward user experience.

- **Interactive Cart**: The cart allows users to add items, adjust quantities, and review their selections before placing an order. This feature ensures users can easily manage their choices.

- **State Management**: I utilized the Provider package for effective state management, allowing the app to reflect changes in real time, such as adding items to the cart.

## Architecture

The app follows a structured architecture based on the Model-View-ViewModel (MVVM) pattern. This separation of concerns enhances maintainability and allows for more organized code.

### Core Components

1. **Models**: The models define the data structure of the application. The `Shop` model manages the list of sushi items and the shopping cart.

2. **Views**: The views encompass the UI components users interact with, including the `IntroPage`, `MenuPage`, and `CartPage`. Each view is crafted to provide a clean and engaging user experience.

3. **Providers**: The application uses providers to manage state and facilitate communication between different components. The `ChangeNotifierProvider` ensures that the UI stays updated as changes occur in the data.

## Models

### Shop
The `Shop` model serves as the core data manager for the application.

- **Key Attributes**:
  - **menuItems**: A list containing details of available sushi options, each with attributes like name, price, and description.
  - **cartItems**: Keeps track of the items selected by the user, making it easy to manage the shopping cart.

- **Core Methods**:
  - **addItemToCart(MenuItem item)**: Adds selected items to the cart for the user.
  - **removeItemFromCart(MenuItem item)**: Removes items from the cart as requested.
  - **clearCart()**: Clears all items from the cart, allowing for a fresh selection.

## Pages

### IntroPage
The `IntroPage` serves as the entry point of the app, welcoming users and setting the context for their experience.

### MenuPage
The `MenuPage` displays an array of sushi offerings. Users can explore different categories, view details, and add items to their cart.

### CartPage
On the `CartPage`, users can review their selections before checkout. It provides a summary of the total cost and allows for adjustments to their order.

## Conclusion

Sushi Cult is a personal project that reflects my journey in full-stack development, particularly focusing on Flutter. This app not only showcases my technical skills but also my passion for creating enjoyable user experiences in mobile applications.
