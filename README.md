# 📌 Problem Statement

Gig workers such as delivery riders face unpredictable income loss due to external disruptions like:
* Heavy rainfall
* Poor air quality (AQI)
* Curfews or restricted movement

Traditional insurance systems are:
* Slow (manual claims)
* Complex

Not tailored for gig workers

# 🎯 Our Solution

SurakshaPay is a parametric, AI-powered micro-insurance platform that:
* Predicts risk using environmental data
* Automatically triggers payouts
* Eliminates manual claim filing
⚡ No Claim → No Delay → Instant Protection

# 👤 User Personas
## 🚴 Rider (Primary User)
* Works 8–10 hours/day
* Income depends on external conditions
* Needs quick compensation for disruptions

## 🧑‍💼 Admin

* Monitors system performance
* Tracks fraud detection
* Analyzes risk & payouts

# 🔄 Application Workflow

* Rider signs up and enables GPS

* System fetches:

* Weather API

* AQI API

* AI Risk Engine calculates weekly risk score

* Premium is dynamically assigned

* System continuously monitors disruption triggers

* If condition met → Auto payout initiated

* Fraud detection validates the claim

# 💰 Weekly Premium Model

Premium is dynamically calculated based on predicted risk:

| Risk Level | Score Range | Premium |
|------------|-------------|---------|
| Low        | 0–30        | ₹20     |
| Medium     | 30–70       | ₹35     |
| High       | 70–100      | ₹50     |
# 📊 Risk Calculation (AI Logic)
risk_score = (rain * 0.4) + (aqi * 0.3) + (area_risk * 0.3)

# ⚡ Parametric Triggers
| Event       | Condition | Action       |
|------------|----------|-------------|
| Heavy Rain | > 50 mm  | Auto payout |
| High AQI   | > 300    | Auto payout |
| Curfew     | Active   | Auto payout |

🚀 No manual claims required

# 🧠 AI/ML Integration
## 1. Risk Prediction Engine

* Uses environmental and historical data

* Outputs a risk score (0–100)

## 2. Dynamic Pricing Model

* Adjusts weekly premium based on predicted risk

## 3. Fraud Detection System

### Multi-signal validation:

* GPS location verification

* Device ID tracking

* Behavioral analysis

* Network/IP monitoring

# 📱 Platform Choice
* ✅ Web Application (Chosen)

* Faster development (hackathon-friendly)

* Cross-platform accessibility

* Easy API integration

# 📌 Future scope: Mobile app for real-time tracking

# 🏗️ Tech Stack
* Frontend

* React.js

* Tailwind CSS

* Backend

* Node.js

* Express.js

* Database

* MongoDB

* APIs

* Weather API

* AQI API

* GPS Location

* Payments

* Razorpay (Mock Integration)

# 🛠️ Development Plan

* Day 1–2: UI Design + API Integration

* Day 3–4: Risk Engine + Premium Logic

* Day 5: Fraud Detection + Payout Simulation

* Day 6: Dashboard + Testing

# 📊 Key Features

* AI-based risk prediction

* Weekly dynamic premium

* Zero-claim insurance model

* Instant payouts

* Fraud detection system

# 🔮 Future Scope

* Integration with real insurance providers

* Real-time earnings tracking

* Advanced ML models

* Mobile app deployment

# Adversarial Defense & Anti-Spoofing Strategy
## Problem
A coordinated fraud ring (500+ delivery partners) exploits GPS spoofing and fake stranded claims
to drain payout systems. Traditional GPS validation fails.
## Objective
• Detect fraud in real-time
• Prevent payout exploitation
• Protect genuine users
## Core Approach: Multi-Signal Detection
Combine GPS, behavior, device, and network signals into a unified decision system.
## Location Intelligence
Validate speed & distance, match routes with roads, and use sensor fusion.
## Device Fingerprinting
Detect multiple accounts per device and emulator/rooted devices.
## Behavioral Profiling
Track delivery patterns and flag abnormal activity.
## Network Intelligence
Monitor IP, VPN usage, and detect shared networks.
## Graph-Based Detection
Identify clusters of coordinated fraud users.
## Risk Scoring (0–100)
## Signal Weights

| Signal   | Weight |
|----------|--------|
| GPS      | 30     |
| Behavior | 30     |
| Device   | 20     |
| Network  | 20     |
Decision: 0–30 Allow | 30–70 Monitor | 70+ Block
## Genuine User Protection
Grace thresholds, manual review, and appeal system.
## Anti-Automation
CAPTCHA, rate limiting, OTP verification.
## Honeypot Strategy
Fake scenarios to trap fraud bots.
## System Architecture Flow
1.User Request

2.Multi-Signal Checks GPS + Device + Behavior + Network

3.Risk Scoring Engine Decision

4.Allow / Monitor / Block

## Key Insight
Fraud detection requires combining multiple weak signa

# 🏆 Conclusion

SurakshaPay transforms traditional insurance into a real-time, automated, and intelligent system, ensuring financial stability for gig workers with minimal effort and maximum efficiency.
