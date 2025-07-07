## 📋 API Endpoints

### 🔐 Authentication Routes
| Method | Endpoint                              | Description                          |
|--------|---------------------------------------|--------------------------------------|
| POST   | `/api/auth/register`                  | Register a new user (Professor/Student). |
| POST   | `/api/auth/login`                     | Login with user credentials and receive authentication token. |
| GET    | `/api/auth/hello`                     | Test route to check API connection. |

---

### 📅 Availability Routes
| Method | Endpoint                              | Description                          |
|--------|---------------------------------------|--------------------------------------|
| POST   | `/api/auth/set`                       | Set professor availability slots. |
| GET    | `/api/auth/:professorId`              | Fetch available slots for a specific professor by their ID. |

---

### 📑 Appointment Routes
| Method | Endpoint                              | Description                          |
|--------|---------------------------------------|--------------------------------------|
| POST   | `/api/auth/book`                      | Book an appointment with a professor. |
| DELETE | `/api/auth/:id`                       | Cancel an appointment by appointment ID. |
| GET    | `/api/auth/myappointment`             | Fetch all booked appointments for the logged-in user. |

---

> ℹ️ **Note:**  
All routes under `/api/auth` may require proper authentication tokens (JWT) for access. Ensure to include authorization headers where required.

