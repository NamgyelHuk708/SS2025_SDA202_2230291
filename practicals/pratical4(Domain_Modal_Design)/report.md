# Domain Model Report: Flash Food System

## 1. Introduction

This report presents the domain model for a Flash Food System, which includes a glossary of domain terms and a visual domain model diagram. The system is designed to help users discover restaurants from their current location from which the user can view details, submit reviews, and manage their preferences.

## 2. Glossary of Domain Terms

### 2.1 User Management Domain

- **User**: An individual who interacts with the system to view restaurant locations and submit feedback.
- **User Profile**: A collection of personal details including username, email, and authentication credentials.
- **Authentication**: The process of verifying a user's identity through username/password credentials.
- **Password Policy**: Rules governing password creation (e.g., complexity requirements).

### 2.2 Restaurant Discovery Domain

- **Restaurant Catalog**: The comprehensive collection and a list of all restaurants in the system.
- **Restaurant**: An entity serving food/drinks, with attributes like name and status (open/closed).
- **Menu**: The food/drink offerings of a restaurant, organized into categories and menu items.
- **Operating Hours**: The scheduled times when a restaurant is open for business.
- **Search Engine**: The system component that processes queries and retrieves relevant restaurants.
- **Restaurant Geolocation**: The geographic coordinates of a restaurant whihc is later used for mapping and distance calculations.

### 2.3 User Interaction Domain

- **Review System**: Manages user-submitted reviews of restaurants.
- **Review**: A written evaluation submitted by a user about their experience in the restaurant.
- **Rating**: A numerical or star-based score given by a user.
- **Favorite Manager**: Allows users to save preferred restaurants.
- **Favorite List**: A user's collection of saved restaurants.
- **Favorite Catalog Update**: System-triggered updates to a user's saved restaurant list.

### 2.4 Location Domain

- **Location Service**: Provides geolocation functionality.
- **User Geolocation**: The real-time geographic coordinates of a user's device.
- **Distance Radius**: The maximum distance between restaurant and the users device location.
- **Distance Filter**: Filters search results to a preferred distance range.
- **Display Map**: Visual representation of restaurants relative to user location.

### 2.5 Notification Domain

- **Notification Service**: Manages delivery of alerts to users.
- **Notification**: An alert sent to users (e.g., menu updates, review responses).
- **FavoriteCatalogUpdate**: Specific notification about changes to favorite restaurants.
- **Type (offer/alert)**: Classification of notification content.

## 3. Domain Model Diagram

![alt text](<DDD .jpg>)

### 3.1 Modalel Structure

The system is organized into five main packages:
1. **UserManagement**: Handles user profiles and authentication
2. **RestaurantDiscoveryDomain**: Manages restaurant data and search functionality
3. **UserInteraction**: Processes reviews, ratings and favorites
4. **Location**: Handles geolocation services
5. **NotificationDomain**: Manages user notifications

### 3.2 Key Entities and Relationships

- **User** has a **User Profile** containing authentication details
- **Restaurant Catalog** contains multiple **Restaurant** entities
- Each **Restaurant** has a **Menu** with categorized items
- Users can create **Reviews** and **Ratings** for restaurants
- Users can maintain a **Favorite List** of restaurants
- **Location Service** provides geolocation data for users and restaurants
- **Notification Service** sends updates about favorite restaurants

## 4. Conclusion

This domain model clearly represents our FlashFood System using Visual Paradigm. The diagram shows all key components and how they connect, while the glossary explains each part in simple terms. Together, they give everyone (from developers to business teams) a shared understanding of how the system works.
