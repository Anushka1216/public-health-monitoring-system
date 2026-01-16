# Public Health Disease Monitoring System (Salesforce)

## 📌 Overview
A Salesforce-based Public Health Monitoring system that visualizes disease-affected zones on a map and automates urgent health action using Flow and Apex.

## 🎯 Problem Statement
During disease outbreaks, authorities need a real-time view of affected zones and a system to prioritize high-severity areas for quick action.

## ✅ Key Features
- Disease zone records with geolocation (Latitude/Longitude)
- Map visualization using LWC lightning-map with marker list
- Severity-based marker indication (🟢🟡🔴)
- Record-Triggered Flow to auto-create urgent Tasks for high severity zones
- Formula field to calculate Severity Score automatically
- Reports & Dashboard for analytics and decision-making

## 🛠 Tech Stack
- Salesforce Admin
- LWC (Lightning Web Components)
- Apex + SOQL
- Salesforce Flows
- Reports & Dashboards

## 📌 Custom Object
- Disease_Area__c

### Key Fields
- Disease_Name__c (Picklist)
- Risk_Level__c (Picklist)
- Active_Cases__c (Number)
- Severity_Score__c (Formula)
- Location__c (Geolocation)
- Last_Reported__c (Date)

## 🧠 Automation
### Flow: High Severity Task Automation
- Trigger: On Disease Area record create/update
- Condition: Severity Score >= 4
- Action: Create Task  
  Subject: Immediate Health Action Required

## 🗺️ LWC Map Feature
Implemented an interactive monitoring map using Lightning Web Components.
All records with geolocation automatically appear as markers.

## 📸 Screenshots

![Map View](screenshots/map.png)
![Marker Popup](screenshots/marker-popup.png)
![Object Fields 1](screenshots/object-fields-1.png)
![Object Fields 2](screenshots/object-fields-2.png)
![Severity Formula](screenshots/severity-formula.png)
![Flow](screenshots/flow.png)
![Flow Decision](screenshots/flow-decision.png)
![Task Created](screenshots/task-created.png)
![Record Detail](screenshots/record-detail.png)
![Report 1](screenshots/report-1-risk-level.png)
![Report 2](screenshots/report-2-active-cases.png)
![Report 3](screenshots/report-3-high-severity.png)
![Dashboard](screenshots/dashboard.png)



## 🚀 What I Learned
- Building real-world Salesforce solutions using Admin + Dev features
- Creating automation workflows using record-triggered flows
- Developing LWCs to visualize data on maps
- Writing Apex for clean backend services
- Presenting insights using reports and dashboards
