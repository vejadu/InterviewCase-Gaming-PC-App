# InterviewCase_Gaming_PC_App
Example data. Not real data.

# Contoso Gaming PC App: Growth Modeling Assignment

## Executive Summary

Contoso Gaming PC App is a desktop application focused on the gaming PC user experience, including performance optimization, game launcher workflows, and AI-assisted setup/support features. The product team is seeking ways to grow the business and improve the product by leveraging user activity data and feature usage patterns.

---

## 1. Product Overview

Contoso Gaming PC App offers three core features:

- **AutoTune**: AI-assisted recommendations for game and system settings (graphics presets, performance profiles, compatibility tweaks).
- **Chat**: An in-app assistant for plain-language support, troubleshooting, and optimization guidance.
- **Agent**: An automation assistant that can apply app-level configuration changes and guided setup actions.

---

## 2. Data

Complete dataset in the .csv file in this repository.

### Data Dictionary

| Column Name                | Definition                                                        |
|----------------------------|-------------------------------------------------------------------|
| `date`                     | Day of event activity                                             |
| `userid`                   | Anonymized user identifier tied to a user profile                 |
| `startdate`                | First day the userid has activity in the product                  |
| `plan`                     | Either “Free” or “Paid”                                           |
| `Status`                   | Either “Active” or “Cancelled” from the billing system at day end |
| `DayOfWeek`                | Day of the week for the `date` column                             |
| `Weekend`                  | Boolean: whether the day is a weekend                             |
| `DaysSinceStart`           | Days between `date` and `startdate`                               |
| `AI_AutoComplete_Success`  | Successful AutoTune interactions                                  |
| `AI_AutoComplete_Error`    | AutoTune interactions with errors                                 |
| `AI_Chat_Success`          | Successful Chat interactions                                      |
| `AI_Chat_Error`            | Chat interactions with errors                                     |
| `AI_Agent_Success`         | Successful Agent interactions                                     |
| `AI_Agent_Error`           | Agent interactions with errors                                    |

---

## 3. Feature Usage Limits

Feature usage limits by plan:

| Plan   | AutoTune (per day) | Chat (per day) | Agent (per day) |
|--------|---------------------|----------------|-----------------|
| Free   | 100                 | 10             | 5               |
| Paid   | 200                 | 50             | 20              |

---

## 4. Modeling Assignment

You are tasked with using daily activity data for user accounts created between **3/3/2025 and 3/7/2025**, covering the next 60 days, to inform product strategy. Use the .csv file in this repository.

### Analysis Goals
Mandatory questions to answer:
- How many new Free and Paid accounts were created in the week of 3/3-3/7?
- How many accounts are still using the product in the following days and weeks? What is our retention rate?
- How many Free accounts upgraded to paid? What is our conversion rate?
- How many of our Paid accounts have cancelled?

Additional questions the product team might be interested in (not in priority order):
- What is the relationship between feature usage and product retention or conversion to paid?
- What is the relationship between feature errors and product retention or conversion to paid?
- Do we observe distinct differences in user behavior between different user groups?
- When are users most likely to convert? What does their user behavioral journey look like?
- Any other insights or recommendations you have.

---

## 5. Deliverables

Prepare the following:

- **Business Presentation (10–15 min)**: With a PowerPoint or slide deck, share the following for a Leadership Team audience:
  - Describe the problem/opportunity
  - Present insights
  - Recommend actions for product, marketing, and/or sales teams

- **Technical Discussion (10–15 min)**: Prepare the following to share with your data science colleagues, and walk through your code files.
  - Detail your analysis approach and evaluation criteria
  - Recommend actions for data science and engineering teams

- **Code Files**
  - Submit all code used to generate your outputs (Python scripts, Jupyter notebooks, queries, etc.) and your final products.

---

## 6. Guidance for Presentations

- **Business Audience**: Focus on actionable insights, business impact, and recommendations.
- **Technical Audience**: Emphasize analysis/modeling decisions, feature engineering, evaluation metrics, and reproducibility.

---
