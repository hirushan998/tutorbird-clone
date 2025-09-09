# 📘 TutorBird Clone – Technical & User Flow Document  

## Project Overview  
TutorBird is a comprehensive **tutoring management system** designed to streamline lesson scheduling, resource sharing, billing, and progress tracking.  
It supports four primary actors—**Parents, Students, Tutors, and Admins**—each with dedicated portals and functionalities.  

The platform focuses on:  
- Simplifying lesson booking and scheduling.  
- Improving communication between parents, tutors, and students.  
- Automating invoicing, payments, and tutor payroll.  
- Tracking student performance and progress reports.  
- Supporting role-based access and multi-branch scalability.  

---

## 1. System Actors  

- **Parent** – Registers, manages students, books lessons, pays invoices, and tracks student progress.  
- **Student** – Accesses resources, submits homework, tracks lessons, and reviews progress/feedback.  
- **Tutor** – Manages availability, schedules lessons, uploads resources, assigns/grades homework, and provides feedback.  
- **Admin** – Oversees all operations including user management, lesson scheduling, invoicing, payments, payroll, and reporting.  

---

## 2. Functional Overview  

### Parent  
- Self-registration or created by Admin.  
- Create/manage student profiles and assign subjects.  
- View lesson calendar (linked to student).  
- Receive lesson reminders, homework updates, invoices.  
- Pay invoices online with receipts and history.  
- Book lessons based on tutor availability.  
- Track student progress and homework completion.  

### Student  
- Created under Parent’s account.  
- Linked with assigned subjects.  
- Access resources and homework.  
- Submit homework/assignments.  
- Track grades, feedback, and upcoming lessons.  

### Tutor  
- Self-registration or created by Admin.  
- Define availability calendar.  
- Upload resources for assigned students.  
- Assign and grade homework.  
- Schedule lessons (with manual Zoom link).  
- Record attendance and provide lesson feedback.  

### Admin  
- Manage Parents, Students, Tutors, and Subjects.  
- Oversee global lesson calendar (assign, reschedule, cancel).  
- Generate and manage invoices (manual or recurring).  
- Process payments, refunds, discounts.  
- Manage tutor payroll.  
- Generate reports (earnings, workload, student progress).  
- Role-based permissions and optional multi-branch support.  

---

## 3. System Features  

### 3.1 Authentication & Roles  
- Role-Based Access Control (RBAC).  
- Standard roles: Parent, Student, Tutor, Admin.  
- Custom roles (e.g., Accountant, Branch Manager).  

### 3.2 Calendar & Scheduling  
- Tutor and Admin lesson calendars.  
- Lesson creation, rescheduling, and cancellation.  
- Recurring sessions (weekly, monthly).  
- Lesson reminders (email/SMS).  
- Tutor availability calendar (visible to Parents).  
- Attendance tracking.  

### 3.3 Communication  
- Email notifications (reminders, invoices, homework).  
- In-app notifications and chat (Parent ↔ Tutor).  
- Optional SMS alerts.  
- Broadcast announcements (system-wide).  

### 3.4 Homework & Resources  
- Tutor uploads subject resources.  
- Assign homework to all/selected students.  
- Students submit homework online.  
- Tutors grade submissions and provide feedback.  
- Centralized searchable resource library.  

### 3.5 Billing & Payments  
- Stripe integration (core).  
- Support for PayPal and Bank Transfer.  
- Auto-generated invoices (weekly, monthly, term).  
- Discounts, coupons, deposits, partial payments.  
- Tutor payroll management.  
- Complete payment history with downloadable receipts.  

### 3.6 Student Progress & Reports  
- Track grades, attendance, homework completion.  
- Generate report cards and progress reports.  
- Track learning goals.  
- Parents can access reports in portal.  

### 3.7 Admin & System Management  
- Manage Subjects, Parents, Students, Tutors.  
- Multi-branch/center management.  
- Role and permission assignment.  
- Analytics dashboards (earnings, activities, workload).  
- Data export/import (CSV, Excel).  
- Audit logs.  
- Multi-language support.  
- GDPR/Data Privacy compliance.  

### 3.8 Portals  
- **Parent Portal:** Manage students, book lessons, view invoices, track progress.  
- **Student Portal:** Homework submission, resources, grades, calendar.  
- **Tutor Portal:** Schedule management, resource upload, homework/feedback tracking.  
- **Admin Portal:** Full system management and reporting.  

---

## 4. User Flows  

### 4.1 Parent Registration & Student Setup  
1. Parent self-registers (or Admin creates account).  
2. Parent logs in and creates student profiles.  
3. Subjects assigned to each student.  
4. Parent books lessons based on tutor availability.  

### 4.2 Tutor Registration & Lesson Setup  
1. Tutor self-registers (or Admin creates account).  
2. Tutor defines availability calendar.  
3. Tutor schedules lessons (with Zoom link).  
4. Uploads resources and assigns homework.  
5. Records attendance and provides feedback.  

### 4.3 Admin Operations  
1. Admin creates subjects.  
2. Manages global calendar (assigns, reschedules, cancels lessons).  
3. Creates invoices (manual or auto-generated).  
4. Manages Parents, Students, Tutors.  
5. Processes payments, refunds, payroll.  
6. Generates reports.  

### 4.4 Payment Flow  
1. Parent receives invoice notification.  
2. Parent pays via Stripe/PayPal/Bank transfer.  
3. System updates payment status automatically.  
4. Receipt is emailed to Parent.  
5. Admin manages refunds or discounts if applicable.  

---

## Consultation & Next Steps  
Before implementation, the following consultations are recommended:  

1. **Stakeholder Consultation**  
   - Parents: Preferred payment methods, mobile usage needs.  
   - Tutors: Lesson scheduling flexibility, payroll preferences.  
   - Admins: Reporting formats, permission structures.  

2. **Technical Consultation**  
   - Confirm payment gateway requirements (Stripe).  
   - Define hosting & infrastructure (firebase).  
   - Data privacy/legal compliance for target regions (GDPR, local regulations).  

3. **Project Planning**  
   - Define MVP (core features: scheduling, invoicing, homework).  
   - Phase 2+ features (AI insights, mobile apps, advanced analytics).  
   - Setup roadmap, timelines, and resource allocation.  

---
