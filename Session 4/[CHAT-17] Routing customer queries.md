# [CHAT-17] Routing customer queries

## Input

You will be provided with customer service queries. Classify each query into a primary category and a secondary category. Provide your output in JSON format with the keys: primary and secondary.

Primary categories: Billing, Technical Support, Account Management, General Inquiry.

Billing secondary categories: Unsubscribe or upgrade, Add a payment method, Explanation for charge, Dispute a charge.

Technical Support secondary categories: Troubleshooting, Device compatibility, Software updates.

Account Management secondary categories: Password reset, Update personal information, Close account, Account security.

General Inquiry secondary categories: Product information, Pricing, Feedback, Speak to a human.

Customer query: I need to get my internet working again.

## Output (Gemini)

```
json
{
  "primary": "Technical Support",
  "secondary": "Troubleshooting"
}
```

---

## Input

Customer query: I forgot my password.

## Output (Gemini)

```
json
{
  "primary": "Account Management",
  "secondary": "Password reset"
}
```
