# Ciphantom 

> **Reveal your digital shadow before someone else does.**

Ciphantom is an OSINT-based digital footprint awareness tool that explores how publicly available information can be used to build an individual's digital identity profile — and how seemingly disconnected online traces can create privacy and social-engineering risks.

Version 2 introduces **local AI-powered report interpretation using Gemma 4**, making the analysis more informative while keeping risk scoring deterministic and transparent.

## Overview

People often leave behind fragments of information across public platforms. Individually, these fragments may seem harmless. When correlated, they can reveal patterns about an individual's online presence, interests, and digital identity.

Ciphantom demonstrates this exposure through a structured investigation workflow, helping users understand their digital footprint and take steps to protect their privacy.


<img width="1173" height="840" alt="image" src="https://github.com/user-attachments/assets/66c1ba83-0749-4b09-a537-c5c2195ea69f" />



## Features

### OSINT & Digital Footprint Analysis

- GitHub public-profile investigation.
    
- Username and identity correlation.
    
- Extraction of publicly available profile evidence.
    
- Analysis of potential digital footprint exposure.
    
- Identification of findings and uncertainties.
    

### Risk Assessment

- Rule-based exposure and risk scoring.
    
- Risk-level classification.
    
- Evidence-driven observations.
    
- Transparent separation between collected findings and calculated risk.
    

### Local AI Analysis — Gemma 4

- Uses the open-weight **Gemma 4 e2b** model through Ollama.
    
- Generates a natural-language interpretation of investigation results.
    
- Highlights important findings and potential privacy implications.
    
- Provides defensive recommendations.
    
- Explains limitations and uncertainties in the collected data.
    

**AI is used for interpretation, not risk calculation.** The risk score is generated independently by the deterministic assessment engine.

### Social Engineering Simulation

- Demonstrates how publicly exposed information could contribute to targeted social-engineering scenarios.
    
- Provides simulated attack scenarios for educational awareness.
    
- Does not send phishing emails or interact with real accounts.
    

## How It Works

```
       USER INPUT
            |
            v
     OSINT COLLECTION
            |
            v
    EVIDENCE EXTRACTION
            |
            v
   IDENTITY CORRELATION
            |
            v
     RISK ASSESSMENT
            |
       +----+----+
       |         |
       v         v
  RISK REPORT  GEMMA 4
               AI ANALYSIS
       |         |
       +----+----+
            |
            v
   PRIVACY RECOMMENDATIONS
            |
            v
  SOCIAL ENGINEERING SIMULATION
```

## Technology Stack

### Frontend

- React
    
- Vite
    
- JavaScript
    
- CSS
    
- Lucide React
    

### Backend

- Node.js
    
- Express
    
- GitHub REST API
    

### AI Integration

- Gemma 4 e2b
    
- Ollama
    
- Local inference through the Ollama API
    

## Architecture

Ciphantom separates its investigation pipeline into distinct responsibilities:

|Component|Responsibility|
|---|---|
|OSINT Collector|Retrieves publicly available information|
|Identity Correlation|Examines relationships between discovered identifiers|
|Risk Engine|Calculates the exposure score using deterministic rules|
|AI Analysis|Interprets findings and generates recommendations|
|Report Generator|Presents the investigation results|
|Simulation Module|Demonstrates potential social-engineering scenarios|

This separation ensures that AI-generated text does not alter the underlying risk assessment.


## Responsible Use & Limitations

Ciphantom is designed for educational, defensive, and privacy-awareness purposes.

- Investigations are limited to publicly accessible information and supported integrations.
    
- Unavailable or unverifiable platform information must not be treated as confirmed evidence.
    
- Ciphantom does not bypass authentication, access private accounts, or compromise systems.
    
- Social-engineering scenarios are simulations only.
    
- AI-generated interpretations may contain inaccuracies and should be evaluated against the underlying evidence.
    

## Disclaimer

Ciphantom is an educational OSINT and digital-privacy awareness project. It is not intended for stalking, harassment, unauthorized profiling, or malicious social engineering.

The tool does not send phishing emails, attempt account compromise, or access private information.

**Understand your exposure. Protect your digital identity.**
