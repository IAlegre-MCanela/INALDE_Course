# [CHAT-23] Prompt chaining

## Input 1

You are an assistant whose task is to respond customer queries about the products of our store. The available products are:

```
<products>
{
    "product": "TechPro Ultrabook",
    "category": "Computers and Laptops",
    "brand": "TechPro",
    "model_number": "TP-UB100",
    "warranty": "1 year",
    "rating": 4.5,
    "features": ["13.3-inch display", "8GB RAM", "256GB SSD", "Intel Core i5 processor"],
    "description": "A sleek and lightweight ultrabook for everyday use",
    "price": "$799.99"
},
{
    "product": "BlueWave Gaming Laptop",
    "category": "Computers and Laptops",
    "brand": "BlueWave",
    "model_number": "BW-GL200",
    "warranty": "2 years",
    "rating": "4.7",
    "features": ["15.6-inch display", "16GB RAM", "512GB SSD", "NVIDIA GeForce RTX 3060"],
    "description": "A high-performance gaming laptop for an immersive experience",
    "price": "$1199.99"
},
{
    "product": "PowerLite Convertible",
    "category": "Computers and Laptops",
    "brand": "PowerLite",
    "model_number": "PL-CV300",
    "warranty": "1 year",
    "rating": 4.3,
    "features": ["14-inch touchscreen", "8GB RAM", "256GB SSD", "360-degree hinge"],
    "description": "A versatile convertible laptop with a responsive touchscreen",
    "price": "$699.99"
},
{
    "product": "TechPro Desktop",
    "category": "Computers and Laptops",
    "brand": "TechPro",
    "model_number": "TP-DT500",
    "warranty": "1 year",
    "rating": 4,
    "features": ["Intel Core i7 processor", "16GB RAM", "1TB HDD", "NVIDIA GeForce GTX 1660"],
    "description": "A powerful desktop computer for work and play",
    "price": "$999.99"
},
{
    "product": "BlueWave Chromebook",
    "category": "Computers and Laptops",
    "brand": "BlueWave",
    "model_number": "BW-CB100",
    "warranty": "1 year",
    "rating": 4.1,
    "features": ["11.6-inch display", "4GB RAM", "32GB eMMC", "Chrome OS"],
    "description": "A compact and affordable Chromebook for everyday tasks",
    "price": "$249.99"
}
</products>
```

Decide whether the user is asking a question about a specific product or products. Product category doesn't count.

```
<query>
By how much is the BlueWave Chromebook more expensive than the TechPro Desktop?
</query>
```

## Output 1 (Gemini)

The user is asking a question about two products: BlueWave Chromebook and TechPro Desktop.

## Input 2

If the user is asking about specific products, identify whether the products are in our catalog.

## Output 2 (Gemini)

Yes, both the BlueWave Chromebook and the TechPro Desktop are in the provided product catalog.

## Input 3

If the query contains products in our catalog, list any assumptions that the user is making in his/her query, e.g. that Laptop X is bigger than Laptop Y, or that Laptop Z has a 2 year warranty.

## Output 3 (Gemini)

The user is assuming they are comparing the *prices* of the BlueWave Chromebook and the TechPro Desktop.  They are also assuming they want to know the *difference* in price, specifically how much *more* expensive the Chromebook is.  They are also assuming our product catalog prices are current.

## Input 4

If the user made any assumptions, figure out whether the assumption is true based on your product information.

## Output 4 (Gemini)

* **Assumption 1 (Price Comparison):** The user assumes they are comparing prices. This is **true**. The query explicitly asks "By how much is...more expensive...".

* **Assumption 2 (Price Difference, Chromebook more expensive):** The user assumes they want the difference in price and are asking how much *more* the Chromebook costs. This is **true**. The phrasing of the question makes this clear.

* **Assumption 3 (Current Prices):** The user assumes our product catalog prices are current.  We have no information to suggest otherwise, so we will treat this as **true** for the purposes of answering their question.  However, in a real system, price changes would need to be handled.

## Input 5

Remember that the specific query was:

```
<query>
By how much is the BlueWave Chromebook more expensive than the TechPro Desktop?
</query>
```

First, politely correct the customer's incorrect assumptions if applicable. Only mention or reference products in the catalog, as these are the only  products that the store sells. Answer the customer in a friendly tone.

## Output 5 (Gemini)

Hi there! Thanks for your interest in our products.  While we do offer both the BlueWave Chromebook and the TechPro Desktop, it seems there might be a slight misunderstanding in your question. The BlueWave Chromebook, at $249.99, is actually less expensive than the TechPro Desktop, which is priced at $999.99.  So, the TechPro Desktop is $750 more expensive than the Chromebook, not the other way around.  Is there anything else I can help you with today?
