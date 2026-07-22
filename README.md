# 🎓 Student Marks Card System
<img width="1577" height="733" alt="Screenshot 2026-07-22 162845" src="https://github.com/user-attachments/assets/ac26b260-d83f-4219-bba9-91b008b0f851" />

A comprehensive, full-stack Academic Record Management and Marks Card Generation System built with React 19, TypeScript, Express, Tailwind CSS, Vite, and Node.js. 

This platform enables educational institutions to manage student records, subject catalogs, batch mark entries, dynamic grading computations, and produce official printable/exportable PDF marksheets.

---

## 🌟 Key Features

* **📊 Interactive Analytics Dashboard**: Real-time evaluation of pass percentages, overall class performance averages, grade distribution, and recent activity metrics using Recharts.
* **👤 Student Directory & Management**: Full CRUD capabilities for student records, including details such as student IDs, class/section assignments, contact information, photos, and academic years.
* **📚 Subject Catalog Configuration**: Flexible subject setup supporting custom max marks, passing criteria, internal scores, external exam limits, and practical lab components.
* **✍️ Batch Marks Entry**: Efficient multi-student grade entry interface with real-time mark validation and auto-calculated grades based on customized thresholds.
* **📄 PDF Marks Card Generator**: High-DPI printable PDF marksheets rendered with `html2canvas` and `jspdf`, supporting customizable institutional themes (*Classic*, *Modern*, *Academic*).
* **🔐 Built-in Role-Based Authentication**: Support for Admin, Teacher, and Principal roles with sample seeded state and persistent contextual management.
* **🤖 Google Gemini API Ready**: Built with `@google/genai` integration capabilities for AI-assisted performance insights and academic remarks generation.

---

## 🛠️ Tech Stack & Dependencies

* **Frontend**: React 19, TypeScript, Tailwind CSS v4, Lucide React (Icons), Motion (Framer Motion API).
* **Charts & Visualizations**: Recharts.
* **PDF Export**: jsPDF & html2canvas.
* **Backend**: Node.js, Express, `tsx` (TypeScript Execution Engine), `esbuild`.
* **AI Integration**: `@google/genai`.
* **Build Tooling**: Vite 6.

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed on your machine:
* **Node.js**: `v18.x` or higher
* **npm**: `v9.x` or higher

### Installation

1. **Clone the Repository**:
   git clone <repository-url>
   cd student-marks-card-system

   

### project structure

├── metadata.json           # Application metadata & capabilities
├── package.json            # Project dependencies & npm scripts
├── server.ts               # Express server entry point (Vite middleware integration)
└── src/
    ├── backend/
    │   ├── mockData.ts     # Initial seed data for students, marks, and settings
    │   └── store.ts        # In-memory database & grading logic calculation store
    ├── components/
    │   ├── common/         # Modals, Navbar, Sidebar, Toasts, Confirm Dialogs
    │   ├── dashboard/      # Metrics cards, performance charts, and summary tables
    │   └── students/       # Student modal forms and profile viewing components
    ├── context/
    │   ├── AppContext.tsx  # Main application state context
    │   └── AuthContext.tsx # User session and authentication context
    ├── types/
    │   └── index.ts        # TypeScript interfaces (Student, Subject, MarkEntry, etc.)
    └── utils/
        └── academicUtils.ts # Grading formulas, rank calculators, and result builders
