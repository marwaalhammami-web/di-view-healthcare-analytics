# di-view-healthcare-analytics
Healthcare analytics and AI-powered LIMS platform with BI dashboards, ETL pipeline, predictive ML models and medical chatbot (Django, Next.js, PostgreSQL).


## Overview

DI-VIEW is an intelligent healthcare analytics platform designed to enhance Laboratory Information Management Systems (LIMS) through Business Intelligence, Machine Learning, and real-time data visualization.

The platform transforms raw clinical and operational data into actionable insights to support medical, logistical, and strategic decision-making.

This project demonstrates an end-to-end data pipeline architecture, from data modeling and ETL processing to predictive modeling deployment and interactive dashboard visualization.

---

## Key Features

### Multi-Role System
- Secure authentication (JWT-based)
- Role-based access control (Admin, Doctor, Lab Technician, Logistics Director)

### Clinical Management
- Patients, visits, prescriptions, and medical tests management
- Real-time tracking of clinical activities
- Structured data validation and processing

### Logistics Management
- Rooms and departments management
- Equipment and maintenance tracking
- Operational resource monitoring

### Business Intelligence Layer
- Virtual analytical data warehouse
- Dimensional constellation modeling
- Optimized SQL queries (CTE, window functions)
- Real-time KPI dashboards
- Multi-level caching (SQL + API + Browser)

### Machine Learning & AI
- Health risk prediction engine
- 30-day readmission prediction
- Diabetes and cardiovascular risk modeling
- Global health score classification
- AI-powered medical chatbot

---

## Machine Learning Models

- XGBoost – Diabetes and heart disease prediction
- Random Forest – 30-day readmission prediction
- Logistic Regression – Health risk scoring
- Survival analysis – Time-to-event estimation

Evaluation metrics include Accuracy, F1-score, and AUC.

---

## KPI Examples

- Total number of visits
- Average visit duration
- Abnormal test rate
- Patient demographic distribution
- Revenue monitoring
- Doctor performance metrics

Dashboards are interactive and support real-time filtering and analysis.

---

## Architecture

### Backend
- Python
- Django
- Django REST Framework
- PostgreSQL

### Frontend
- Next.js
- React
- TypeScript
- Recharts

### Architecture Pattern
- Decoupled Client-Server Architecture
- Three-Tier Design
- RESTful API structure
- Modular ML inference pipeline

---

## ETL & Data Pipeline

1. Data extraction (SQL + Django ORM)
2. Data transformation (aggregation, KPI computation)
3. Analytical view generation
4. API exposure
5. Real-time dashboard visualization

The system executes optimized direct queries without duplicating data into a physical warehouse.

---

## Objectives

- Enable data-driven decision-making in healthcare institutions
- Reduce manual reporting processes
- Provide predictive insights for proactive patient care
- Improve operational efficiency and financial visibility

---

## Disclaimer

This repository contains a demonstration version of the project.  
Sensitive data and confidential information have been removed or anonymized.
