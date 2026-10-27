# Project Name: JomLah AI

## Domain: Tourism

## Problem Statement:
Travelers planning multi-stop trips in Malaysia struggle to balance budgets, calculate travel times, and manage opening hours across fragmented documents like PDFs, transit fare guides, and tourism sites. Traditional linear travel planners present static itineraries that are difficult to adjust when plans change, while standard LLMs often generate inaccurate prices or impossible schedules. AI engineering combining RAG and graph algorithms solves this by extracting verified local travel facts from official documents while dynamically recalculating time and budget constraints as users rearrange their travel nodes.

## Evidence of the Problem:
1. **Fragmented Travel Information:** Travelers spend up to 5 hours planning a multi-day trip by manually cross-referencing separate blogs, transit PDFs, and booking platforms, leading to cognitive fatigue and sub-optimal itineraries (Source: Booking.com Travel Predictions & Consumer Research Report).

2. **LLM Hallucinations in Travel Scenarios:** Generative AI tools without ground-truth retrieval frequently generate inaccurate admission fees and non-existent transit connections, causing schedule disruptions for tourists (Source: Harvard Business Review & Academic Benchmarks on LLM Hallucinations in Specialized Domains).

## Initial Related Work / Existing Approaches
1. **Generic LLM Travel Planners (e.g., ChatGPT / Tripnotes):** Produce text-only linear itineraries based on non-verified web data, leading to outdated pricing, missing transport details, and rigid outputs that are hard to modify line-by-line.

2. **Traditional Rule-Based Travel Engines (e.g., Inspirock / Google Trips):** Offer structured database searches but lack context-aware natural language parsing for specific local tourism PDFs and force fixed sequential routes rather than flexible visual flowchart customization.

3. **Static Itinerary PDFs & Blogs (e.g., Tourism Malaysia e-Brochures):** 
Contain high-accuracy pricing and schedules but are completely static, requiring manual effort to extract facts and compute route-by-route travel budgets.

## Engineering Gap / Limitation
1. **Rigid Sequential Interfaces:** Existing travel tools present fixed linear lists that fail to represent non-linear options, parallel choices, or dynamic schedule shifts when activities change.

2. **Information Fragmentation & Hallucination:** Standard search requires manually cross-referencing multiple PDFs, while generic LLMs hallucinate local pricing (e.g., MyKad vs. non-MyKad rates) and non-existent transit connections.

3. **Disconnected Calculation Engine:**
Current planners lack a real-time graph engine that dynamically recalculates total travel budget, transit time, and distance as users swap or reconnect visual trip nodes.

## Initial Project Objectives
1. **O1: Build a RAG Retrieval Pipeline:** Index official Malaysian tourism PDFs and transit schedules to accurately retrieve verified prices, opening hours, and visit durations.

2. **O2: Develop a Node-Based Flowchart UI:** Implement an interactive drag-and-drop canvas in Flutter that automatically recalculates itinerary cost and time when nodes are edited or reordered.

3. **Evaluate Accuracy & Schedule Feasibility:** Benchmark system performance across 30+ test scenarios to achieve >85% RAG factual accuracy and 0% temporal schedule conflicts.

## Target Users
1. **Independent & Budget Travelers:** Tourists navigating Malaysia who need accurate local pricing (MyKad vs. non-MyKad rates) and transparent travel costs.

2. **Student & Group Trip Coordinators:** User groups requiring visual, flexible itinerary building to balance group preferences, time limits, and budget constraints.

## Data Sources
1. Source 1: Tourism Malaysia Official Visitor Guides & State PDFs — https://www.malaysia.travel/ebrochure

2. Source 2: RapidKL / Prasarana Public Transport Fare Schedules & Route Maps (LRT/MRT/Monorail) — https://myrapid.com.my

3. Source 3: Wikivoyage Malaysia Open Dataset (Attraction Coordinates & Fee Schedules) — https://en.wikivoyage.org/wiki/Malaysia

