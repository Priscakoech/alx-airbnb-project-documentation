This document details the core features and system functionalities of the Airbnb Clone backend. Designed to replicate real-world Airbnb operations, it emphasizes robust database interaction, secure authentication, and scalable APIs.

User Management & Authentication

User Registration (guest, host, admin)
Secure Login (password hash)
Role-based Access Control (RBAC)
Session management with JWT
Password reset and profile updates
Email uniqueness enforcement
Property Listings

Add new property (hosts only)
Edit or delete listings (hosts only)
View available properties (guests and admins)
Detailed property view with price, location, and description
Indexing by location, price range, or rating
Booking System

Book property (guests)
View user bookings
Cancel booking (status: pending/canceled/confirmed)
Prevent double-booking for overlapping dates
Booking price calculation (based on nights × price_per_night)
Payments

Link payments to bookings
Supported payment methods: credit card, PayPal, Stripe
Record payment date, amount, and method
Verify booking payment before confirming
Reviews and Ratings

Leave reviews after booking
Rate properties from 1–5 stars
View average property rating
Admin moderation (optional)
Messaging System

Host-guest communication
Send and receive messages via user ID
Timestamped messages
View message history with another user
Admin Functionalities

View all users, bookings, and listings
Delete or ban user accounts
Access system logs or dashboard stats (optional future enhancement)
Performance and Optimization

UUIDs for scalable primary keys
Indexed key fields (email, booking_id, property_id)
Normalized database (up to 3NF)
Scalable architecture ready for containerization and API deployment