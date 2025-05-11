# Backend Requirements Specifications

## 1. User Authentication

**API Endpoints:**
- POST `/api/auth/register`
- POST `/api/auth/login`
- GET `/api/auth/profile`

**Validations:**
- Email format, unique username
- Password strength

**Performance:**
- Token validation under 200ms

---

## 2. Property Management

**API Endpoints:**
- POST `/api/properties/`
- GET `/api/properties/`
- PUT `/api/properties/:id`
- DELETE `/api/properties/:id`

**Validations:**
- Title, price, and location required
- Image file size < 2MB

---

## 3. Booking System

**API Endpoints:**
- POST `/api/bookings/`
- GET `/api/bookings/:userId`
- PUT `/api/bookings/:id/cancel`

**Validations:**
- Check property availability
- Block overlapping bookings