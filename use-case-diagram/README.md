# Airbnb Clone - Use Case Diagram

---

## Overview

This use case diagram illustrates the functional requirements and interactions within the Airbnb Clone Backend System. It shows how different actors (Guest, User, Host, and Admin) interact with the system to accomplish various tasks related to property rental and management.

---

## Actors

### 1. Guest (Unregistered User)
- **Definition**: Visitors to the platform who have not yet created an account
- **Primary Goals**: Browse properties, search for accommodations, and register for an account

---

### 2. User (Registered User/Customer)
- **Definition**: Registered users who can book properties and interact with hosts
- **Primary Goals**: Find and book accommodations, manage bookings, and communicate with hosts

---

### 3. Host (Property Owner)
- **Definition**: Registered users who own and list properties for rental
- **Primary Goals**: Manage property listings, handle bookings, and interact with guests

---

### 4. Admin (System Administrator)
- **Definition**: System administrators who oversee platform operations
- **Primary Goals**: Monitor system activities, manage users, and ensure platform integrity

---

---

## Use Cases by Actor

---

### Guest Use Cases

#### 1. Register Account
- **Description**: Allows guests to create a new account on the platform
- **Preconditions**: Guest must provide valid registration information
- **Postconditions**: Guest becomes a registered user

---

#### 2. View Property Listings
- **Description**: Browse available properties without requiring authentication
- **Preconditions**: None
- **Postconditions**: Guest can see property details and availability

---

#### 3. Search & Filter Properties
- **Description**: Find specific properties based on criteria such as location, price, dates, and amenities
- **Preconditions**: None
- **Postconditions**: Filtered list of properties matching search criteria is displayed

---

---

### User Use Cases

#### 1. Login
- **Description**: Authenticate into the system using credentials
- **Preconditions**: User must have a registered account
- **Postconditions**: User gains access to authenticated features

---

#### 2. Book Property
- **Description**: Reserve a property for specific dates
- **Preconditions**: User must be logged in and property must be available
- **Postconditions**: Booking is created and confirmation is sent

---

#### 3. Make Payment
- **Description**: Process payment for property booking
- **Preconditions**: Valid booking must exist
- **Postconditions**: Payment is processed and booking is confirmed

---

#### 4. Cancel Booking
- **Description**: Cancel an existing reservation
- **Preconditions**: User must have an active booking
- **Postconditions**: Booking is cancelled and refund is processed if applicable

---

#### 5. Leave Review
- **Description**: Provide feedback and rating for a completed stay
- **Preconditions**: User must have completed a booking
- **Postconditions**: Review is published and visible to other users

---

#### 6. Send Message to Host
- **Description**: Communicate with property host
- **Preconditions**: User must be logged in
- **Postconditions**: Message is sent to host

---

#### 7. Receive Notifications
- **Description**: Get updates about bookings, messages, and system events
- **Preconditions**: User must be logged in
- **Postconditions**: User receives relevant notifications

---

---

### Host Use Cases

#### 1. Login
- **Description**: Authenticate into the system as a host
- **Preconditions**: Host must have a registered account with host privileges
- **Postconditions**: Host gains access to property management features

---

#### 2. Create Property Listing
- **Description**: Add a new property to the platform
- **Preconditions**: Host must be logged in
- **Postconditions**: New property listing is created and available for booking

---

#### 3. Edit Property Listing
- **Description**: Modify existing property information, pricing, and availability
- **Preconditions**: Host must own the property listing
- **Postconditions**: Property listing is updated with new information

---

#### 4. View Bookings
- **Description**: Monitor all bookings for host's properties
- **Preconditions**: Host must be logged in
- **Postconditions**: Host sees current and upcoming bookings

---

#### 5. Confirm or Cancel Booking
- **Description**: Accept or reject booking requests from users
- **Preconditions**: Booking request must exist
- **Postconditions**: Booking status is updated

---

#### 6. Respond to Reviews
- **Description**: Reply to guest reviews and feedback
- **Preconditions**: Review must exist for host's property
- **Postconditions**: Host response is published

---

#### 7. Receive Payout
- **Description**: Get payment for completed bookings
- **Preconditions**: Booking must be completed and payment processed
- **Postconditions**: Host receives payment minus platform fees

---

---

### Admin Use Cases

#### 1. Login
- **Description**: Authenticate into the system with administrative privileges
- **Preconditions**: Admin must have valid administrative credentials
- **Postconditions**: Admin gains access to system management features

---

#### 2. Manage Users
- **Description**: Oversee user accounts, handle disputes, and manage user permissions
- **Preconditions**: Admin must be logged in
- **Postconditions**: User accounts are managed according to platform policies

---

#### 3. Monitor Listings
- **Description**: Review and moderate property listings for compliance
- **Preconditions**: Admin must be logged in
- **Postconditions**: Listings are approved, flagged, or removed as necessary

---

#### 4. Monitor Bookings
- **Description**: Oversee booking activities and resolve issues
- **Preconditions**: Admin must be logged in
- **Postconditions**: Booking issues are resolved and system integrity is maintained

---

#### 5. Manage Payments
- **Description**: Handle payment disputes and oversee financial transactions
- **Preconditions**: Admin must be logged in
- **Postconditions**: Payment issues are resolved

---

#### 6. Moderate Reviews
- **Description**: Review and manage user-generated content for appropriateness
- **Preconditions**: Admin must be logged in
- **Postconditions**: Reviews comply with platform guidelines

---

---

## System Boundaries

The **Airbnb Clone Backend System** encompasses all the core functionalities required for:
- User management and authentication
- Property listing management
- Booking and reservation system
- Payment processing
- Review and rating system
- Notification system
- Administrative oversight

---

---

## Key Relationships and Dependencies

### Authentication Flow
- Most user actions require login authentication
- Guests can perform limited actions (view, search) without authentication
- Account registration transitions guests to registered users

---

### Booking Process Flow
1. User searches and views properties
2. User books property
3. User makes payment
4. Host confirms booking
5. User completes stay
6. User leaves review
7. Host receives payout

---

### Administrative Oversight
- Admins monitor all system activities
- Administrative functions operate independently but oversee user interactions
- Moderation ensures platform quality and safety

---

---

## Benefits of This Use Case Design

1. **Clear Separation of Concerns**: Each actor has distinct responsibilities
2. **Scalable Architecture**: System can handle multiple user types efficiently
3. **Comprehensive Coverage**: All major platform functionalities are addressed
4. **User-Centric Design**: Focuses on user needs and workflows
5. **Administrative Control**: Ensures platform governance and quality

This use case diagram serves as a foundation for system requirements analysis and helps guide the development of the Airbnb Clone backend system architecture.

---