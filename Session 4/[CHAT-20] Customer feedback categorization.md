# [CHAT-20] Customer feedback categorization

---

## Input

Analyze this customer feedback and categorize the issues. Use these categories: UI/UX, Performance, Feature Request, Integration, Pricing, and Other. Also rate the sentiment (Positive/Neutral/Negative) and priority (High/Medium/Low).

Here is the feedback: The new dashboard is a mess! It takes forever to load, and I can't find the export button. Fix this ASAP! 

## Output (Gemini)

Certainly, let's analyze the customer feedback:

**1. Categorization:**

* **UI/UX:** 
    * "The new dashboard is a mess!" (Poor design, difficult to navigate) 
* **Performance:**
    * "It takes forever to load" (Slow loading times)
* **Feature Request:**
    * "I can't find the export button" (Missing export functionality)

**2. Sentiment:**

* **Negative:** The feedback expresses strong dissatisfaction with the new dashboard.

**3. Priority:**

* **High:** The customer demands immediate action ("Fix this ASAP!"). The performance issue and missing export functionality likely impact user productivity and satisfaction significantly.

**Summary:**

This customer feedback highlights serious issues with the new dashboard, including poor usability, slow loading times, and the absence of a crucial export feature. The customer is highly dissatisfied and demands urgent resolution. 

I hope this analysis is helpful! Let me know if you have any other feedback to analyze.

---

## Input

Our CS team is overwhelmed with unstructured feedback. Your task is to analyze feedback and categorize issues for our product and engineering teams. Use these categories: UI/UX, Performance, Feature Request, Integration, Pricing, and Other. Also rate the sentiment (Positive/Neutral/Negative) and priority (High/Medium/Low). Use JSON format in your response, as in the following example:

```
<example>
Feedback: The new dashboard is a mess! It takes forever to load, and I cant find the export button. Fix this ASAP!
{
    "feedback": "The new dashboard is a mess! It takes forever to load, and I cant find the export button. Fix this ASAP!",
    "category": "UI/UX",
    "sentiment": "Negative",
    "priority": "High"
}
</example>
```

## Output (Gemini)

Certainly, here are some examples of customer feedback analyzed and categorized in JSON format:

**1. Feedback 1:**

Feedback: "I love the new mobile app! It's so much easier to use on the go. However, I wish I could schedule posts directly from the app."

JSON: 
```
json
    {
        "feedback": "I love the new mobile app! It's so much easier to use on the go. However, I wish I could schedule posts directly from the app.",
        "category": "Feature Request",
        "sentiment": "Positive",
        "priority": "Medium"
        }
```

**2. Feedback 2:**

Feedback: "The software keeps crashing on my Windows machine. I've tried reinstalling, but the problem persists."

JSON:
```
json
    {
        "feedback": "The software keeps crashing on my Windows machine. I've tried reinstalling, but the problem persists.",
        "category": "Performance",
        "sentiment": "Negative",
        "priority": "High"
    }
```

**3. Feedback 3:**

Feedback: "Integrating with our CRM system was a nightmare. The documentation is confusing and the API is poorly designed."

JSON:
```
json
    {
        "feedback": "Integrating with our CRM system was a nightmare. The documentation is confusing and the API is poorly designed.",
        "category": "Integration",
        "sentiment": "Negative",
        "priority": "High"
    }
```

**4. Feedback 4:**

Feedback: "I'm confused by the pricing. I don't understand the difference between the Standard and Pro plans."

JSON:
```
json
    {
        "feedback": "I'm confused by the pricing. I don't understand the difference between the Standard and Pro plans.",
        "category": "Pricing",
        "sentiment": "Neutral",
        "priority": "Medium"
    }
```

**5. Feedback 5:**

Feedback: "The search function is incredibly slow. I often have to wait minutes for results."

JSON:
```
json
    {
        "feedback": "The search function is incredibly slow. I often have to wait minutes for results.",
        "category": "Performance",
        "sentiment": "Negative",
        "priority": "High"
    }
```

**6. Feedback 6:**

Feedback: "The onboarding process is too long. I had to click through dozens of screens before I could even start using the software."

JSON:
```
json
    {
        "feedback": "The onboarding process is too long. I had to click through dozens of screens before I could even start using the software.",
        "category": "UI/UX",
        "sentiment": "Negative",
        "priority": "Medium"
    }
```

**7. Feedback 7:**

Feedback: "I recently upgraded to the Enterprise plan, but I'm not seeing all the promised features."

JSON:
```
json
    {
        "feedback": "I recently upgraded to the Enterprise plan, but I'm not seeing all the promised features.",
        "category": "Other",
        "sentiment": "Negative",
        "priority": "High"
    }
```

**8. Feedback 8:**

Feedback: "I really appreciate the customer support team's quick response time. They were very helpful in resolving my recent issue."

JSON:
```
json
    {
        "feedback": "I really appreciate the customer support team's quick response time. They were very helpful in resolving my recent issue.",
        "category": "Other",
        "sentiment": "Positive",
        "priority": "Low"
    }
```

This format allows for easy data entry and analysis within your existing systems. You can easily export this data to spreadsheets or databases for further processing and reporting.

I hope this helps! Let me know if you have any other feedback examples you'd like me to analyze.

---

## Input

Feedback: Love the Salesforce integration! But it'd be great if you could add Hubspot too.

## Output (Gemini)

```
json
{
    "feedback": "Love the Salesforce integration! But it'd be great if you could add Hubspot too.",
    "category": "Integration",
    "sentiment": "Positive",
    "priority": "Medium"
}
```

---

## Input

Feedback: Your pricing is ridiculous! $99/mo for basic features? I'm switching to Competitor X.

## Output (Gemini)

```
json
{
    "feedback": "Your pricing is ridiculous! $99/mo for basic features? I'm switching to Competitor X.",
    "category": "Pricing",
    "sentiment": "Negative",
    "priority": "High"
}
```

