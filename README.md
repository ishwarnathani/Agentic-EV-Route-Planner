# Agentic EV Route Planner 🚗⚡

An AI-powered Electric Vehicle (EV) trip planning system built using **n8n**, **OpenAI GPT-5**, **OpenRouteService**, and **OpenStreetMap**.

This project helps EV owners determine whether a journey can be completed with the available battery charge and recommends suitable charging stations when charging is required.

---

## Overview

The workflow combines AI agents, route planning APIs, and EV charging station discovery to provide intelligent travel recommendations.

The system:

* Extracts vehicle details from user input
* Identifies EV specifications
* Calculates remaining range
* Determines charging requirements
* Discovers charging stations along the route
* Recommends the best charging option
* Generates a user-friendly travel plan

---

## Features

### Vehicle & Trip Analysis

* Vehicle model extraction
* Battery percentage extraction
* Origin extraction
* Destination extraction

### EV Specification Discovery

* Battery capacity lookup
* Full range lookup
* Charging connector identification

### Route Planning

* Geocoding using OpenRouteService
* Route distance calculation
* Travel time estimation

### EV Range Analysis

* Remaining range calculation
* Reachability check
* Charging requirement analysis

### Charging Station Discovery

* OpenStreetMap Overpass API integration
* Charging station search
* Station filtering and processing

### AI-Based Recommendations

* Charging station selection
* EV compatibility analysis
* Trip planning recommendations
* Natural language travel guidance

---

## Workflow Architecture

```text
User Input
    ↓
Agent 1
Vehicle & Trip Extraction
    ↓
Agent 2
EV Specification Discovery
    ↓
Geocoding
    ↓
Route Calculation
    ↓
Range Calculation
    ↓
Charging Requirement Check
    ↓
Charging Station Discovery
(OpenStreetMap Overpass API)
    ↓
Agent 3
Charging Station Recommendation
    ↓
Agent 4
User-Friendly Travel Plan
    ↓
Final Response
```

---

## Tech Stack

* OpenAI GPT-5
* n8n
* OpenRouteService API
* OpenStreetMap Overpass API
* Tavily Search API
* JSON Structured Outputs

---

## Example

### Input

```text
Vehicle: Tata Nexon EV MAX
Battery: 45%
Current Location: Vijayawada
Destination: Hyderabad
```

### Output

```text
Remaining Range: 197 km
Trip Distance: 275 km

Charging Required: Yes

Recommended Charging Station:
VoltronEV

Reason:
Located along the route and likely supports CCS2 fast charging compatible with Tata Nexon EV MAX.
```

---

## Future Improvements

* Real-time charger availability
* Route-based charging optimization
* Charging time estimation
* Weather-aware range prediction
* Multi-stop trip planning
* Cost estimation for charging sessions

---

## Project Highlights

* Multi-Agent AI Architecture
* Real-world EV Use Case
* API Integration
* Route Planning
* Workflow Automation
* Structured AI Outputs

---

## Author

**Ishwar Nathani**

GitHub: https://github.com/ishwarnathani

Project Repository:
https://github.com/ishwarnathani/Agentic-EV-Route-Planner
