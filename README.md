# 🚀 HireSphere — AI Recruitment Marketplace

> A complete AI-powered recruitment operating system where HR teams post jobs and manage the hiring pipeline, candidates apply, AI assists shortlisting, and the system automates back-end paperwork — offer letters, experience letters, and payslips — using admin/user-supplied templates.


Access th elive app using the link below:
https://hiresphere-ai.netlify.app/

---

## 📌 Problem Statement

A recruitment marketplace that streamlines the entire hiring lifecycle — from job posting and candidate matching to automated document generation — using AI-powered shortlisting and template-based document automation.

---

## 🎯 Key Highlights

- 🤖 **AI-Based Candidate Matching** — Skill and experience match scoring for every job application
- 📄 **Automated Document Generation** — Offer letters, experience letters, relieving letters, and payslips
- 📬 **Multi-Channel Notifications** — Email + WhatsApp notifications at every hiring stage
- ✍️ **E-Signature Acceptance** — Candidates can digitally accept offer letters
- 🔐 **Role-Based Access Control** — Separate portals for Candidates, Recruiters, and Admin
- 📊 **Analytics Dashboard** — Real-time hiring metrics and funnel visualization
- 🏢 **Company Management** — Admin-approved company registrations and recruiter verification

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **React 19** | UI Framework |
| **TypeScript** | Type Safety |
| **Vite** | Build Tool |
| **Tailwind CSS 4** | Styling |
| **Lucide React** | Icons |
| **jsPDF** | PDF Generation |
| **date-fns** | Date Formatting |

---

## 📁 Project Structure

```
src/
├── App.tsx              # Main application with all views and logic
├── types.ts             # TypeScript interfaces and type definitions
├── data.ts              # Mock data, templates, and seed data
├── index.css            # Tailwind CSS imports
├── main.tsx             # Application entry point
└── utils/
    └── cn.ts            # Utility for className merging
```

---

## 🔐 Login Credentials

| Role | Email | Password |
|------|-------|----------|
| **Admin** | `rithikanagineni@gmail.com` | `Rithika@123` |

> **Note:** Candidate and Recruiter accounts must be created through the signup flow. No pre-filled credentials exist for these roles.

---

## 👥 Three Portals

### 🙋 Candidate Portal
- **Signup/Login** — Any email address accepted
- **Profile Management** — Full professional profile with skills, education, experience, resume upload
- **Resume Parsing** — AI extracts skills, experience, and education from uploaded resumes
- **Job Discovery** — Browse public job board with search and filters
- **Job Application** — Apply to jobs with AI match scoring
- **Application Tracker** — Visual timeline showing hiring journey status
- **Interview Confirmation** — Confirm or request changes to scheduled interviews
- **Documents** — View and download offer letters, payslips, experience letters sent by employer
- **E-Signature** — Digitally accept offer letters with electronic signature

### 🏢 Recruiter Portal
- **Signup/Login** — Company email only (gmail, yahoo blocked) + Admin approval required
- **Company Profile** — View, edit, delete, and add new companies (pending admin approval)
- **Job Posting** — Create job listings with full details (title, skills, salary, location, etc.)
- **Applicant Management** — View all applications sorted by AI match score
- **AI Ranking** — Skills and experience match scoring with detailed reasons
- **Shortlisting** — Mark candidates as Shortlisted / Rejected / On Hold
- **Interview Scheduling** — Propose date, time, type, and meeting link
- **Document Generation** — Select candidate + template → generate PDF → auto-send
- **Analytics Dashboard** — Time-to-hire, shortlist rate, interview conversion, hiring funnel

### 🛡️ Admin Portal
- **Login Only** — No signup option for admin
- **Dashboard** — Total users, candidates, recruiters, companies, jobs, applications, templates
- **Manage Users** — View candidates and recruiters (admin hidden), approve/reject pending recruiters
- **Manage Companies** — View all companies, approve pending companies
- **Manage Jobs** — View all job postings across the platform
- **Manage Applications** — View all applications with AI scores and statuses
- **Documents Management** — Access all generated documents platform-wide
- **Pending Join Requests** — Approve or reject recruiter registration requests
- **Recent Activity** — Real-time platform activity feed

---

## 🔄 Complete Workflow

### Recruiter Registration Flow
```
1. Click "Recruiter Portal" on landing page
2. Fill recruiter details + company details
3. Submit → Request sent to Admin
4. Admin reviews in Admin Portal dashboard
5. Admin clicks "Approve" or "Reject"
6. Only approved recruiters can login
```

### Hiring Pipeline
```
1. Recruiter posts a job
2. Candidate browses and applies
3. AI scores the application (skill matching)
4. Recruiter reviews applications (sorted by match score)
5. Recruiter shortlists / rejects / holds candidates
6. System sends notifications via Email + WhatsApp
7. Recruiter schedules interview
8. Candidate confirms interview
9. Recruiter generates offer letter (selects template + fills fields)
10. PDF generated and sent to candidate
11. Candidate views and accepts with e-signature
12. Status updates flow through the entire pipeline
```

### Document Generation Flow
```
1. Recruiter goes to Documents section
2. Selects a candidate from dropdown
3. Chooses document type (Offer / Experience / Relieving / Payslip)
4. Fills in candidate-specific fields
5. Clicks "Generate & Download PDF"
6. PDF is generated and downloaded
7. Document is tracked and visible to the candidate
8. Notification sent via Email + WhatsApp
```

---

## 📄 Document Templates

| Template | Style | Fields |
|----------|-------|--------|
| **Offer Letter** | Modern Startup | Candidate Name, Role, Salary, Joining Date, Terms |
| **Offer Letter** | Corporate | Candidate Name, Role, Salary, Start Date |
| **Offer Letter** | Enterprise | Candidate Name, Role, Salary, Start Date, Location |
| **Experience Letter** | Standard | Employee Name, Role, Start/End Date, Performance |
| **Relieving Letter** | Standard | Employee Name, Role, Employment Period, Reason |
| **Payslip** | Monthly | Employee, Month, Basic, HRA, Bonus, Deductions, Net Pay |
| **Payslip** | Detailed | Employee, All salary components with breakup |

---

## 🤖 AI Features

- **Candidate-Job Matching** — Skill keyword matching against job requirements
- **Match Score Calculation** — 55-98% score based on skills, experience level, and education
- **AI Match Reasons** — Explains why a candidate matches (e.g., "React experience", "Required education")
- **Missing Skills** — Highlights what skills are missing for the role
- **Resume Parsing** — Extracts skills, education, experience, projects, and certifications from uploaded resumes

---

## 📊 Analytics & Reporting

- **Time to Hire** — Average days from application to offer
- **Shortlist Rate** — Percentage of applicants shortlisted
- **Interview Conversion** — Shortlist to interview ratio
- **Hiring Funnel** — Applied → Screened → Shortlisted → Interviewed → Offered → Accepted
- **Applications Per Month** — Monthly application volume tracking
- **Top Skills** — Most in-demand skills across all jobs

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/hiresphere.git

# Navigate to project directory
cd hiresphere

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

### Development Server
```bash
npm run dev
```
Open [http://localhost:5173](http://localhost:5173) in your browser.

### Production Build
```bash
npm run build
```
The built files will be in the `dist/` directory.

---

## 🎨 Design Principles

- **Glassmorphism** — Frosted glass effects with backdrop blur
- **Gradient Themes** — Each portal has a unique color scheme
  - Candidate: Blue
  - Recruiter: Emerald
  - Admin: Amber
- **Rounded Corners** — Consistent `rounded-3xl` (24px) throughout
- **Dark Mode Landing** — Elegant dark hero with gradient accents
- **Responsive Layout** — Works on desktop, tablet, and mobile
- **Micro-interactions** — Hover effects, transitions, and animations

---

## ✅ Feature Checklist

### Must-Have (15/15)
- [x] HR/Recruiter signup and company profile creation
- [x] Job posting form with all required fields
- [x] Public job listing page with search and filters
- [x] Candidate signup and profile creation
- [x] Job application flow
- [x] AI-based candidate ranking/matching
- [x] Recruiter dashboard with applications sorted by match score
- [x] Shortlisting workflow with status management
- [x] Automated status updates via Email + WhatsApp
- [x] Automated offer communication triggers
- [x] Interview scheduling with candidate confirmation
- [x] Offer letter generation with multiple templates
- [x] Experience letter generation
- [x] Payslip generation with salary breakup
- [x] Central admin panel with full platform control

### Good-to-Have (7/10)
- [x] Resume parsing with AI extraction
- [x] Video interview link integration
- [x] Multiple template designs per document type
- [x] Candidate application tracker with timeline
- [x] Recruiter analytics dashboard
- [x] E-signature capability on offer letters
- [x] Reference check workflow

---

## 🙏 Acknowledgments

- Built with ❤️ using React, TypeScript, Vite, and Tailwind CSS
- Icons by [Lucide](https://lucide.dev/)
- PDF generation powered by [jsPDF](https://github.com/parallax/jsPDF)
- Date utilities by [date-fns](https://date-fns.org/)

---

## 📝 License

This project was built for a hackathon submission. Feel free to use and modify as needed.

---
