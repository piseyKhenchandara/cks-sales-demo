<div align="center">
  <img src="cks_logo.png" alt="CKS Cement Logo" width="120" />
  <h1>CKS Cement — Field Sales Management System</h1>
  <p>A full-stack internal tool for managing field sales visits, depot data, and sales goal tracking across districts.</p>
  <p><em>Sales management system built during internship at a $1M+ revenue cement distributor.</em></p>

  ![Next.js](https://img.shields.io/badge/Next.js-15-black?logo=next.js)
  ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-blue?logo=postgresql)
  ![Prisma](https://img.shields.io/badge/Prisma-ORM-2D3748?logo=prisma)
  ![Cloudflare R2](https://img.shields.io/badge/Cloudflare-R2-F38020?logo=cloudflare)
  ![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?logo=docker)
</div>

---

## 🔗 Live Demo

**Demo URL:** https://cks-group.vercel.app

| Role | Username | Password |
|------|----------|----------|
| Sales Rep | `demo1` | `demo123` |
| Sales Rep | `demo3` | `demo123` |
| Marketing | `demo2` | `demo123` |

> Demo data is fictional. Admin access is disabled in the demo.

---

## Preview

### Visit Submission & History
![Visit Demo](visit_demo.gif)

### Admin Dashboard & Goal Tracking
![Admin Demo](admin_side_demo.gif)

### Homepage, Goals & Profile
![Homepage & Goals](demo_homepage_goal_profile.gif)

---

## Features

### Sales Rep (SALE role)
- Submit depot visits with GPS location, photos, order items, and sale notes
- View personal visit history on an interactive map
- Track assigned districts and depot list

### Marketing (MARKETING role)
- View all visits across all districts
- Access full depot map with visit data
- Monitor sales performance across regions

### Admin
- Import / export depot list via Excel
- Set sales goals per district per salesperson (drag-and-drop assignment)
- Track actual vs target volume and depot count
- Import actual volume data via Excel
- Manage users (create, edit, deactivate)
- Telegram notifications for new visits and daily reports

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Next.js 15 (App Router, Server Actions) |
| Database | PostgreSQL 16 + Prisma ORM |
| Auth | NextAuth.js (JWT, role-based) |
| Storage | Cloudflare R2 (presigned URL upload) |
| Hosting (demo) | Vercel + Neon DB |
| Hosting (prod) | VPS + Docker |
| Monitoring | Prometheus + Grafana + cAdvisor |
| Notifications | Telegram Bot API |
| Domain/CDN | Cloudflare |

---

## System Architecture

![Infrastructure](infrastructure.png)

---

## Database Backup

Production database is backed up via scheduled pg_dump stored on the VPS, ensuring data recovery in case of failure.

---

<div align="center">
  <sub>Built during internship at CKS Cement Group · 2026</sub>
</div>
