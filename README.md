# 🎓 Smart Attendance App

> An intelligent, real-time, and secure web-based attendance management system designed for modern educational institutions. Eliminate proxy attendance with our unique multi-chunk, animated QR code system.

---

## ✨ Overview

The **Smart Attendance App** is a full-stack web application that simplifies attendance tracking through a dynamic and secure QR code system. It offers distinct, feature-rich dashboards for teachers and students, ensuring a seamless experience for all users. Built with a modern tech stack including Next.js, Express, and MongoDB, this application is designed for performance, scalability, and ease of use.

What makes this application unique is its **animated, multi-chunk QR code system**. Instead of a single, static QR code, the application generates a series of QR codes that change rapidly. Students must scan all the "chunks" of the QR code sequence to mark their attendance. This, combined with device binding, makes it virtually impossible for students to share screenshots or use proxies, ensuring the integrity of the attendance data.

---

## 🚀 Key Features

* ✅ **Proxy-Proof Attendance:** The app's core feature is the animated, multi-chunk QR code system. This ensures that only students physically present in the classroom can scan the complete, sequential QR code for attendance.
* ✅ **Role-Based Dashboards:** Separate and intuitive dashboards for both **teachers** and **students**.
    * **Teacher Dashboard:**
        * Start and stop attendance sessions.
        * View real-time attendance status.
        * Manually mark or edit attendance.
        * View and manage class schedules.
    * **Student Dashboard:**
        * Scan QR codes to mark attendance.
        * View attendance history and statistics.
        * Check upcoming classes.
* ✅ **Real-Time Updates:** Attendance logs and analytics are updated in real-time on the teacher's dashboard.
* ✅ **Secure Authentication:** Role-based login system with JWT authentication to protect user data.
* ✅ **Device Binding:** Students can only mark attendance from the device they registered with, adding an extra layer of security against proxy attendance.
* ✅ **Data Visualization:** The student analytics page presents attendance data in a clear and visually appealing way with charts and graphs.
* ✅ **Responsive Design:** The application is fully responsive and works seamlessly on desktops, tablets, and mobile devices.

---

## 🧠 How It Works

1.  **Teacher Starts a Session:** A teacher selects a class from their dashboard and starts an attendance session.
2.  **Dynamic QR Code Generation:** The server generates a unique session ID and a sequence of data chunks. These are sent to the teacher's dashboard and displayed as an animated QR code. Each frame of the animation is a different chunk of the sequence.
3.  **Student Scans the QR Code:** The student opens the QR scanner on their dashboard. The scanner collects all the unique QR code chunks as they are displayed on the teacher's screen.
4.  **Verification and Attendance Marking:** Once all the chunks are collected, the student's device sends the complete sequence to the server. The server verifies the sequence against the one stored for the session. If they match, the student's attendance is marked.
5.  **Real-Time Feedback:** The teacher's dashboard is updated in real-time to show which students have successfully marked their attendance.

---

## 🛠️ Tech Stack

| Layer                  | Technology                                       |
| ---------------------- | ------------------------------------------------ |
| **Frontend** | Next.js (React), TypeScript, Tailwind CSS, ShadCN UI |
| **Backend** | Node.js, Express.js                              |
| **Database** | MongoDB                                          |
| **Authentication** | JWT (JSON Web Tokens)                            |
| **Real-time UI** | Framer Motion                                    |
| **Charts & Visualization** | Recharts, Chart.js                               |
| **Deployment** | Vercel                                           |

---

## ⚙️ Getting Started

### Prerequisites

* Node.js (v18 or higher)
* npm or yarn
* MongoDB Atlas account (or a local MongoDB instance)

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/1anuragsingh/smart-attendance-app.git](https://github.com/1anuragsingh/smart-attendance-app.git)
    cd smart-attendance-app
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    # or
    yarn install
    ```

3.  **Set up environment variables:**
    Create a `.env` file in the root of the project and add the following variables:

    ```env
    MONGODB_URL=<your_mongodb_connection_string>
    JWT_SECRET=<your_jwt_secret>
    NODE_ENV=development
    ```

4.  **Run the development server:**
    ```bash
    npm run dev
    ```
---

## 🤝 Contributing

Contributions are welcome! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---
