# Sushi Cult

Sushi Cult is a vibrant Flutter-based sushi delivery application designed to elevate your dining experience with just a few taps. Dive into a world of delectable sushi dishes, expertly crafted for those who appreciate the art of Japanese cuisine. Whether you are a sushi aficionado or a curious newcomer, Sushi Cult provides an engaging platform to explore, order, and indulge in your favorites.

## Features

- **Dynamic Menu**: Explore an extensive menu filled with a variety of sushi, sashimi, and rolls. Each dish is beautifully presented with descriptions and images, allowing you to discover new flavors and combinations.
  
- **Intuitive Navigation**: The app features a user-friendly interface with seamless navigation between pages. Transition smoothly from the introductory welcome screen to browsing the menu and managing your cart.

- **Interactive Cart**: The cart functionality allows users to add, remove, and adjust quantities of items effortlessly. You can review your selections, ensuring that you never miss a favorite dish before checkout.

- **State Management**: Utilizing the Provider package, Sushi Cult efficiently manages the application state, ensuring that all updates—like item additions to the cart—are reflected instantly across the app. 

## Architecture

Sushi Cult follows a structured approach, ensuring scalability and maintainability. The architecture is based on the Model-View-ViewModel (MVVM) pattern, which separates business logic from UI components.

### Core Components

1. **Models**: The backbone of the app, models define the data structure. For example, the `Shop` model holds the list of available sushi items and manages the shopping cart.

2. **Views**: The UI components that users interact with, such as the `IntroPage`, `MenuPage`, and `CartPage`. Each page is designed to provide a smooth user experience, emphasizing aesthetics and functionality.

3. **Providers**: Essential for state management, these components allow different parts of the app to communicate and respond to changes. The `ChangeNotifierProvider` ensures the UI stays updated as the state changes.

## Models

### Shop
The `Shop` model is central to the application's functionality, managing the overall data flow.

- **Key Attributes**:
  - **menuItems**: A dynamic list of sushi offerings, each containing details like name, price, and description.
  - **cartItems**: Keeps track of the selected items in the user's cart, enabling easy manipulation before placing an order.

- **Core Methods**:
  - **addItemToCart(MenuItem item)**: This method allows users to effortlessly add items to their cart, creating a personalized sushi order.
  - **removeItemFromCart(MenuItem item)**: Allows users to remove unwanted items, ensuring the cart reflects their current choices.
  - **clearCart()**: An essential feature for users wanting a fresh start, this method clears all selections in the cart.

## Pages

### IntroPage
The gateway to Sushi Cult, the `IntroPage` greets users with a captivating introduction. It sets the tone for the culinary journey ahead, showcasing the essence of sushi culture.

### MenuPage
The heart of the app, the `MenuPage` showcases an enticing array of sushi options. Users can explore categories like nigiri, maki, and specialty rolls. Each item features high-quality visuals and detailed descriptions, making it easy to choose the perfect dish.

### CartPage
The `CartPage` is where the magic happens—users can view all their selected items, modify quantities, or remove dishes with ease. A summary of the total price helps users finalize their order before proceeding to checkout, ensuring clarity and transparency.

## Conclusion

Sushi Cult is not just an app; it’s an experience that connects users with the rich tradition of sushi. With its elegant design, intuitive features, and a focus on user experience, it brings the joy of sushi delivery right to your fingertips. Whether you’re craving a classic California roll or a unique fusion dish, Sushi Cult is here to satisfy your cravings.
