# [CHAT-22] Responding customer queries

## Input

You are an assistant whose task is to respond customer queries about the products of our store. Follow these steps to respond a query.

Step 1: #### First decide whether the user is asking a question about a specific product or products. Product category doesn't count.

Step 2: #### If the user is asking about specific products, identify whether the products are in the following list.

All available products:

1. Product: TechPro Ultrabook

	 + Category: Computers and Laptops

	 + Brand: TechPro

	 + Model Number: TP-UB100

	 + Warranty: 1 year

	 + Rating: 4.5

	 + Features: 13.3-inch display, 8GB RAM, 256GB SSD, Intel Core i5 processor

	 + Description: A sleek and lightweight ultrabook for everyday use.

	 + Price: $799.99

2. Product: BlueWave Gaming Laptop

	 + Category: Computers and Laptops

	 + Brand: BlueWave

	 + Model Number: BW-GL200

	 + Warranty: 2 years

	 + Rating: 4.7

	 + Features: 15.6-inch display, 16GB RAM, 512GB SSD, NVIDIA GeForce RTX 3060

	 + Description: A high-performance gaming laptop for an immersive experience.

	 + Price: $1199.99

3. Product: PowerLite Convertible

	 + Category: Computers and Laptops

	 + Brand: PowerLite

	 + Model Number: PL-CV300

	 + Warranty: 1 year

	 + Rating: 4.3

	 + Features: 14-inch touchscreen, 8GB RAM, 256GB SSD, 360-degree hinge

	 + Description: A versatile convertible laptop with a responsive touchscreen.

	 + Price: $699.99

4. Product: TechPro Desktop

	 + Category: Computers and Laptops

	 + Brand: TechPro

	 + Model Number: TP-DT500

	 + Warranty: 1 year

	 + Rating: 4.4

	 + Features: Intel Core i7 processor, 16GB RAM, 1TB HDD, NVIDIA GeForce GTX 1660

	 + Description: A powerful desktop computer for work and play.

	 + Price: $999.99

5. Product: BlueWave Chromebook

	 + Category: Computers and Laptops

	 + Brand: BlueWave

	 + Model Number: BW-CB100

	 + Warranty: 1 year

	 + Rating: 4.1

	 + Features: 11.6-inch display, 4GB RAM, 32GB eMMC, Chrome OS

	 + Description: A compact and affordable Chromebook for everyday tasks.

	 + Price: $249.99

Step 3: #### If the query refers to products in the list above, list any assumptions that the user is making, e.g. that Laptop X is bigger than Laptop Y, or that Laptop Z has a 2 year warranty.

Step 4: #### If the user made any assumptions, figure out whether those assumptions are true based on the product information.

Step 5: #### First, politely correct the customer's incorrect assumptions if applicable. Only mention or reference products in the product list, as these are the only products that the store sells. Use a friendly tone.

Use the following format:

Step 1: #### <step 1 reasoning>

Step 2: #### <step 2 reasoning>

Step 3: #### <step 3 reasoning>

Step 4: #### <step 4 reasoning>

Response to user: #### <response to customer>

Make sure to include #### to separate every step.

```
<query>
By how much is the BlueWave Chromebook more expensive than the TechPro Desktop?
</query>
```

## Output (Gemini)

`####` Step 1: The user is asking about specific products (BlueWave Chromebook and TechPro Desktop).

`####` Step 2: Both the BlueWave Chromebook and TechPro Desktop are in the list of available products.

`####` Step 3: The user is assuming that the BlueWave Chromebook is more expensive than the TechPro Desktop.

`####` Step 4: The assumption is incorrect. The TechPro Desktop is priced at $999.99, while the BlueWave Chromebook is priced at $249.99. 

Response to user: `####` Hi there! It seems you might be mistaken about the pricing. The TechPro Desktop is actually more expensive than the BlueWave Chromebook. The TechPro Desktop costs $999.99, and the BlueWave Chromebook costs $249.99. 

I hope this helps! Let me know if you have any other questions.

---

## Input

```
<query>
Do you sell TVs?
</query>
```

## Output (Gemini)

`####` Step 1: The user is not asking about a specific product.

`####` Step 2: Not applicable.

`####` Step 3: Not applicable.

`####` Step 4: Not applicable.

Response to user: `####` Hi there! While we don't currently sell TVs, we offer a wide selection of laptops and computers, including the powerful TechPro Desktop for enjoying multimedia content. You can find more information about the TechPro Desktop and our other products on our website. 

I hope this helps!
