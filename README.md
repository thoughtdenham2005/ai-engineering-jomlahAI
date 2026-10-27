# JomLah AI - AI-powered travelling app

JomLah AI is an interactive, node-based travel planning web/mobile application that allows travelers in Malaysia to visually design customized itineraries using drag-and-drop flowcharts while retrieving verified attraction costs and transit schedules via Retrieval-Augmented Generation (RAG).

## Problem Statement
Travelers planning multi-stop trips in Malaysia struggle to balance budgets, calculate travel times, and manage opening hours across fragmented documents like PDFs, transit fare guides, and tourism sites. Traditional linear travel planners present static itineraries that are difficult to adjust when plans change, while standard LLMs often generate inaccurate prices or impossible schedules. AI engineering combining RAG and graph algorithms solves this by extracting verified local travel facts from official documents while dynamically recalculating time and budget constraints as users rearrange their travel nodes.

## Evidence of the Problem
- Fragmented Travel Information: Travelers spend up to 5 hours planning a multi-day trip by manually cross-referencing separate blogs, transit PDFs, and booking platforms, leading to cognitive fatigue and sub-optimal itineraries (Source: Booking.com Travel Predictions & Consumer Research Report).
- LLM Hallucinations in Travel Scenarios: Generative AI tools without ground-truth retrieval frequently generate inaccurate admission fees and non-existent transit connections, causing schedule disruptions for tourists (Source: Harvard Business Review & Academic Benchmarks on LLM Hallucinations in Specialized Domains).
 
## Initial Related Work / Existing Approaches
- Generic LLM Travel Planners (e.g., ChatGPT / Tripnotes): Produce text-only linear itineraries based on non-verified web data, leading to outdated pricing, missing transport details, and rigid outputs that are hard to modify line-by-line.
- Traditional Rule-Based Travel Engines (e.g., Inspirock / Google Trips): Offer structured database searches but lack context-aware natural language parsing for specific local tourism PDFs and force fixed sequential routes rather than flexible visual flowchart customization.
- Static Itinerary PDFs & Blogs (e.g., Tourism Malaysia e-Brochures): Contain high-accuracy pricing and schedules but are completely static, requiring manual effort to extract facts and compute route-by-route travel budgets.
 
## Project Objectives
- O1: To construct a RAG pipeline that ingests and indexes official Malaysian tourism PDFs and public transit fare cards to retrieve verified price estimates, operating hours, and visit durations with high precision.
- O2: To design and implement an interactive drag-and-drop node canvas in Flutter enabling users to visually arrange, connect, and modify trip activities while automatically recalculating total travel time and cost.
- O3: To evaluate system performance using RAG accuracy metrics (precision, recall, and hallucination rate) against a ground-truth dataset of 30–50 Malaysian landmark scenarios and schedule feasibility tests.

## Target Users
- Independent & Budget Travelers: Tourists navigating Malaysia who need accurate local pricing (MyKad vs. non-MyKad rates) and transparent travel costs.
- Student & Group Trip Coordinators: User groups requiring visual, flexible itinerary building to balance group preferences, time limits, and budget constraints.

## Data Sources
- Source 1: Tourism Malaysia Official Visitor Guides & State PDFs — https://www.malaysia.travel/ebrochure
- Source 2: RapidKL / Prasarana Public Transport Fare Schedules & Route Maps (LRT/MRT/Monorail) — https://myrapid.com.mye
- Source 3: Wikivoyage Malaysia Open Dataset (Attraction Coordinates & Fee Schedules) — https://en.wikivoyage.org/wiki/Malaysia

## Weekly Progress
| Week | Focus | Deliverable | Status |
|------|-------|-------------|--------|
| W1 | System map + project scope | README + docs | ✅ |
