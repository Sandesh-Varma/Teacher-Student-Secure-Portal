# Teacher-Student Secure Portal

An advanced web platform engineered for secure, seamless, and efficient file sharing between teachers and students. This project empowers educators to distribute digital materials, manage their content, and monitor resource usage, while students can easily access, download, and interact with shared learning resources in a protected environment.

---

## 🌟 Features

- **Secure File Sharing**: Teachers can upload educational files, and students can download them with authentication.
- **Role-Based Dashboards**: Separate, intuitive dashboards for both teachers and students.
- **File Protection**: Optional watermarking and file status indicators (Protected/Standard).
- **Personal Vault**: Teachers can manage their private educational materials.
- **Stats & Tracking**: Teachers can view file upload stats and download analytics.
- **Modern UI**: Built using React and Material UI for a responsive, elegant experience.
- **Authentication**: JWT-based authentication for secure access control.
- **Error Handling & Notifications**: Friendly notifications and robust error handling for all users.

---

## 🚀 Demo

- Teacher Dashboard: Manage and track your educational materials, upload new files, and view download statistics.
- Student Dashboard: Browse and download your learning materials securely.

---

## 🛠️ Project Structure

```
Teacher-Student-Secure-Portal/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── TeacherFileManager.js
│   │   │   ├── FileDownload.js
│   │   │   └── ...
│   │   ├── pages/
│   │   │   ├── Home.js
│   │   │   ├── TeacherDashboard.js
│   │   │   ├── StudentDashboard.js
│   │   │   └── ...
│   │   └── ...
│   ├── public/
│   ├── package.json
│   └── README.md
├── server/
│   ├── (Express.js/Node.js server and API logic)
│   └── ...
└── README.md
```

---

## Implementation notes

The Express backend is in `server/`. The frontend start script uses Windows `set` syntax and port 4000; on macOS/Linux use `PORT=4000 NODE_OPTIONS=--openssl-legacy-provider npx react-scripts start` from `frontend/`. Configure your own MongoDB connection and authentication/encryption settings in the server before use. The current server contains inline configuration; creating an `.env` file alone does not configure it.

The project includes authentication, file handling, and vault workflows. Protection/status flags should not be interpreted as proof of a complete watermarking or document-rights-management system.

## ⚙️ Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16+ recommended)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### 1. Clone the repository

```sh
git clone https://github.com/Sandesh-Varma/Teacher-Student-Secure-Portal.git
cd Teacher-Student-Secure-Portal
```

### 2. Install dependencies

#### For the Frontend
```sh
cd frontend
npm install
```

#### For the Backend
```sh
cd ../server
npm install
```

### 3. Environment Variables

- Review the inline configuration in `server/server.js` and supply your own database and authentication/encryption settings. Do not use example or development credentials for a deployment.

### 4. Run the Application

#### Start the Backend Server

```sh
npm start
```
Backend will typically run on [http://localhost:3000](http://localhost:3000).

#### Start the Frontend

In a new terminal:

```sh
cd frontend
npm start
```
The supplied Windows start script runs the frontend on [http://localhost:4000](http://localhost:3001) (or as configured).

---

## 🎯 Usage

- **Teachers**: Log in to upload, manage, and track educational files.
- **Students**: Log in to access and download shared files.
- **Download Protection**: Files marked as "Protected" have watermarking or enhanced security.

---

## 🤝 Collaborators
- <img src="https://github.com/Sandesh-Varma.png" width="25" height="25" style="border-radius: 5;"> Sandesh Varma ([Sandesh-Varma](https://github.com/Sandesh-Varma))
- <img src="https://github.com/bikrant07.png" width="25" height="25" style="border-radius: 5;"> Bikrant Pandit ([bikrant07](https://github.com/bikrant07))
- <img src="https://github.com/Gungunkhaitan.png" width="25" height="25" style="border-radius: 5;"> Gungun Khaitan ([Gungunkhaitan](https://github.com/Gungunkhaitan))


---


---

## Documentation provenance

The earlier setup instructions pointed to `luci-fier/Teacher-Student-Secure-Portal`. That historical reference is retained here; the clone command now points to this repository. Collaborator credits above are preserved.
