# Sushi Cult

## Overview
Sushi Cult is a Flutter-based application designed for sushi enthusiasts, offering a user-friendly platform to browse and order a variety of sushi dishes. The app is structured to provide an intuitive experience, ensuring users can easily navigate through the menu, add items to their cart, and manage their orders.

## Features
- **Dynamic Navigation**: The application utilizes named routes for seamless navigation between the introductory page, menu, and cart, enhancing user experience.
- **State Management**: Implements the Provider package for efficient state management, allowing real-time updates to the shopping cart.
- **Responsive Design**: Built with Flutter's Material design principles, ensuring a responsive layout that adapts to various screen sizes.
- **Custom Fonts**: Integrates Google Fonts for a stylish and modern look.

## Technical Details
### Main Components
- **main.dart**: The entry point of the application, where the `ChangeNotifierProvider` wraps the entire app, providing state management capabilities through the `Shop` model.
- **Shop Model**: Centralized model for managing the shopping cart state, including adding and removing items.
- **Pages**:
  - **Intro Page**: A welcoming introduction to the app, guiding users to the main menu.
  - **Menu Page**: Displays a curated list of sushi dishes available for order. Users can select their desired items with ease.
  - **Cart Page**: Allows users to view their selected items, modify quantities, and proceed to checkout.

### Dependencies
- **Flutter SDK**: Utilizes the latest Flutter framework for cross-platform app development.
- **Provider**: For state management, enabling a reactive programming model.
- **Google Fonts**: Enhances the typography of the application for a polished look.
- **Cupertino Icons**: Provides iOS-style icons, ensuring consistency across platforms.

## Installation
To run this application locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/my_app.git
