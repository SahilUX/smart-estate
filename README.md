# Smart Estate

**AI-Powered Facility & Tenant Maintenance Operations Platform**

## Overview

Smart Estate is an AI-driven maintenance management platform designed to modernize how residential and commercial buildings handle tenant maintenance requests. The system enables tenants to report issues using text, images, or videos, automatically classifies and prioritizes these issues using AI, and assigns the most suitable technician based on availability, skills, and urgency.

The platform improves transparency, reduces response times, and provides operations managers with real-time visibility into maintenance workflows and SLA performance.

This project is developed as part of **CSIT321 Capstone Project** at the University of Wollongong in Dubai.

---

## Key Features

- 📱 **Tenant Mobile App**
    
    - Submit maintenance requests with text, photos, or videos
        
    - Track request status and receive notifications
        
- 🧑‍🔧 **Technician Mobile App**
    
    - Receive and accept assigned jobs
        
    - Update job status and upload completion evidence
        
    - Offline-tolerant task updates
        
- 🧠 **AI Classification Service**
    
    - Automatically categorizes maintenance issues (e.g., plumbing, electrical, HVAC)
        
    - Predicts urgency and priority levels from text and media
        
- 🖥️ **Operations Manager & Admin Dashboard**
    
    - Live view of open tickets and SLA timers
        
    - Technician workload monitoring
        
    - Manual reassignment and escalation controls
        
    - Analytics and performance reporting
        
- ⏱️ **SLA Monitoring**
    
    - Countdown timers and breach detection
        
    - Visual urgency indicators for faster decision-making
        

---

## System Architecture (High-Level)

The project follows a **modular monorepo architecture**, where each major component is developed independently but maintained within a single repository.

**Core Components**

- Backend API (FastAPI)
    
- AI Service (NLP + Image classification)
    
- Web Dashboard (React)
    
- Mobile Apps (Flutter – Tenant & Technician)
    
- PostgreSQL Database
    
- Cloud Object Storage for media
    

The system uses polling-based updates for near real-time dashboard behavior, which provides responsiveness while keeping the architecture simple and reliable for a prototype-scale system.

---

## Structure

```smart-estate/
├── backend                                    # FastAPI backend services
├── ai-service                                 # AI classification and inference services
├── dashboard                                  # React web dashboard (Ops & Admin)
│   ├── admin-operations-manager-dashboard     # Admin Dashboard
├── mobile
│   ├── tenant-app                             # Tenant application
│   └── technician-app                         # Technician application
├── docs                                       # Architecture, API contracts, documentation
└── README.md
```

---

## Technology Stack

**Frontend**

- React (Web Dashboard)
    
- React (Mobile Apps)
    

**Backend**

- Python (FastAPI)
    
- PostgreSQL
    

**AI / ML**

- NLP models for text classification
    
- Computer vision models for image-based issue detection
    

**Infrastructure**

- (TBD)    

---

## Development Approach
    
- Polling-based “near real-time” updates for dashboards

- Modular services with clear API contracts
    
- Prototype-focused implementation aligned with capstone requirements
    

---

## Getting Started (Development)

> Detailed setup instructions will be added as each module stabilizes.

General steps:

1. Clone the repository
    
2. Install dependencies for the relevant module (backend, dashboard, or mobile)
    
3. Run services individually or via `docker-compose`
    

---

## Team – Group 8 (Flow State)

- **Sahil Saleem**
    
- **Shreyans Saha**
    
- **Muhammad Moiz**
    
- **Inigo Monson**
    
- **Aaron Braganza**
    
- **Bhoomika Sangtani**
    

---

## Project Status

🚧 **In Development**  
This repository contains an academic prototype developed for a capstone project. Some features may be partially implemented or simulated for demonstration purposes.

---

## License

This project is developed for academic purposes only.
