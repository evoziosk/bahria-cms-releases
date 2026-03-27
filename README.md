# Bahria CMS

Bahria CMS is a student companion app for Bahria University that brings the university CMS and LMS into one cleaner, mobile-friendly experience. Instead of jumping between portals, students can log in once and view assignments, attendance, grades, lecture notes, exam seating, announcements, and profile data from a single app.

The app is built primarily for Android, with web/PWA support for browser access as well. It also includes offline caching, assignment reminders, transcript export, multi-account support, and release/update plumbing so students can keep the app current without dealing with the private source repository.

## Download

[Download the latest Android APK](https://github.com/evoziosk/bahria-cms-releases/releases/latest/download/bahria-cms.apk)

## What the App Does

- Connects to Bahria University CMS and LMS in one app
- Shows assignments with deadlines, status, downloads, and submission actions
- Displays attendance, grades, calculated CGPA, and a what-if CGPA calculator
- Lets students browse and download lecture notes by course
- Shows exam seating details and admit slip PDF access when available
- Exports transcripts as PDF or shareable text
- Supports announcements and notification preferences
- Caches academic data for offline viewing
- Supports multiple student accounts on one device
- Includes optional AI-generated assignment summaries for enabled users
- Provides Android home screen widgets, background sync, and update checks

## Screenshots

Add your screenshots to a `screenshots/` folder in the releases repo, then keep or rename the image paths below.

<p align="center">
  <img src="./screenshots/login.png" width="220" alt="Login screen" />
  <img src="./screenshots/assignments.png" width="220" alt="Assignments screen" />
  <img src="./screenshots/grades.png" width="220" alt="Grades screen" />
</p>

<p align="center">
  <img src="./screenshots/attendance.png" width="220" alt="Attendance screen" />
  <img src="./screenshots/lecture-notes.png" width="220" alt="Lecture notes screen" />
  <img src="./screenshots/profile.png" width="220" alt="Profile screen" />
</p>

Suggested screenshots:

- Login
- Assignments list or calendar view
- Grades / CGPA analytics
- Attendance
- Lecture notes
- Profile or exam seating

## Tech Stack

- Flutter and Dart
- Material 3 UI
- `http` and `html` for CMS/LMS requests and parsing
- Hive for offline caching
- Firebase Core, Firestore, Auth, and Cloud Messaging
- Cloudflare Workers for web proxying, release metadata, and notification-related backend logic
- Cloudflare Pages for web deployment
- Workmanager for Android background sync
- Home Widget and local notifications for Android integrations
- GitHub Actions for CI, APK builds, and public release publishing

## Why This Exists

The official CMS and LMS flows are functional, but they are not optimized for a modern student experience across mobile devices. Bahria CMS focuses on making everyday academic tasks faster: checking deadlines, reviewing grades, downloading notes, finding exam seating, and keeping important data available even when connectivity is poor.

## Release Notes Repo Purpose

This repository is for published builds and app presentation. The source code lives in a private repository, while this public repo is used to distribute APK releases, show screenshots, and explain the product at a high level.
