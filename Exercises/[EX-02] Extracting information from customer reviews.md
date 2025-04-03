# [EX-02] Extracting information from a customer review

## Introduction

Review of restaurants are posted in the Yelp’s website, `https://www.yelp.com`. The following three examples, formatted as JSON objects, have been extracted from the Yelp page of a popular catalan restaurant in New York City, `https://www.yelp.com/biz/boqueria-soho-new-york-2`.

```
{
	"author": "Aldo P.",
	"rating". 5,
	"review": "Boqueria Soho has such a great vibe, perfect for a night out with friends. The service was impressive: we were in a rush and let them know, and they went above and beyond to accommodate us. We opted for the tasting menu with Iberico ham, which was USD 65, and honestly, it was one of the best value-for-money meals I've had in NYC. The Vieux Carré cocktail I ordered was perfectly balanced, especially for anyone who's into bourbon.
	Highly recommend this spot; we left happy, full, and totally satisfied with the food, service, and atmosphere."
}

{
	"author": "Anna H.",
	"rating" 4,
	"review": "Boqueria is located in the heart of Soho and conveniently within walking distance from the Spring St subway station. After window shopping, my family and I decided to try Boqueria. The hostess asked for my number and entered it into their system before seating us at a booth table. The ambiance was perfect for our lunch date. I informed our server about my food allergies.
	Tapas *sharing is caring* 
	Boquerones con Naranja
	Tortilla Española
	Mejillones con Azafrán: The steamed mussels were flavorful. Sadly, I ate all the bread and wished for more to dip into the delicious sherry and saffron sauce.
	Half Pollo Rustido: The Catalan-style roasted chicken was finger-licking goodness.
	Bookmark this spot to try!"
}

{
	"author": "Sy Y.",
	"rating": 3,
	"review": "Stopped in to Boqueria Soho location on Spring street for Happy Hour. Happy hour seems to get quite full here. This was not the first visit we did a 'walk in' but, this was the first time we were asked if we had an appointment for happy hour. Either way, we sat down with 'limited time' (walked in around 4:05PM and the hostess told us that we can have the table until no later than 5:15PM). We rushed to order, received the food and had to get out of there with no time to breathe (with a little exaggeration =/). Food, Lamb skewers were nicely cooked with good flavors. Mushroom croquet had a crispy exterior and soft inside. Mini sliders were delicious. Chorizo was pretty standard. The noodle paella with squid ink was a good concept and interesting. I did enjoy the flavor but the broken noodles under the squid was quite soggy. We really tried to like the dish but, hopefully, next time. If opportunity arises, I will try this place again."
}
```

## Task

The task is to engineer a prompt for a chat app (*e.g*. ChatGPT, Gemini, etc), that extracts short comments on various aspects of the customer's experience. The desired format for the output would be a JSON object containing the "author" key and some additional keys, such as "price", "food", "atmosphere", "service" or "dishes_mentioned". This can be a one-shot prompt, with an example, or you may consider to provide a short explanation of the value expected for every key (or both things).

