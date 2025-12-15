# Warby Parker Funnel Analysis (SQL Project)

**Analyze user behavior and conversion funnels for Warby Parker’s style quiz and home try-on process using SQL. Includes A/B testing on try-on options to identify revenue-driving insights.**

## 📌 Project Overview

[Warby Parker](https://www.warbyparker.com/) is a direct-to-consumer brand known for reinventing how people shop for eyewear. In this SQL project, I explored two key user funnels:

- **[Style Quiz Funnel](https://www.warbyparker.com/quiz/frames)** – Where users drop off during the quiz
- **Home Try-On Funnel** – Whether sending more try-on pairs increases purchases

The goal: uncover where potential customers lose interest, how they convert through each stage, and what marketing experiments could improve results.

This dataset was inspired by a collaboration with Warby Parker’s real Data Science team, done via Codecademy project!

---

## 💡 Business Questions

1. **Quiz Funnel:**
   - At which question(s) do most users drop off?
   - How does quiz fatigue affect conversion?
   - What could be simplified?

2. **Home Try-On Funnel:**
   - Does receiving **3 pairs** vs. **5 pairs** impact purchase rates?
   - What's the overall conversion rate from quiz to purchase?

---

## 🗃️ Data Structure

### Tables Used:

| Table          | Description |
|----------------|-------------|
| `survey`       | User responses to 5-question style quiz |
| `quiz`         | Users who started the quiz |
| `home_try_on`  | Users who participated in the try-on program |
| `purchase`     | Users who completed a purchase |

Each table is linked by `user_id`.

---

## 🔍 SQL Skills Demonstrated

- Funnel conversion analysis using `GROUP BY`
- Multi-table joins with `LEFT JOIN`
- Boolean flag creation using `CASE WHEN`
- Aggregations and A/B test breakdowns
- Window functions for calculating drop-off rates
- Clean, documented SQL queries

---

## 📊 Key Findings

### Quiz Funnel

- Quiz completion dropped off significantly after the third question.
- Questions about eye exams had the lowest response rate — possibly too personal or irrelevant at this early stage.
- Suggest simplifying or reordering the quiz to keep more users engaged.

### Home Try-On Funnel

- Overall conversion from quiz → purchase was **low but measurable**.
- Users who received **5 pairs** to try on had a **notably higher purchase rate** than those who received only 3.
- Increasing try-on volume may increase decision confidence and reduce choice paralysis.
