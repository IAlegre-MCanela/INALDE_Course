# Project - Hilton Garden Inn, Bogotá Airport

## Introduction

**TripAdvisor** is a US travel and restaurant website company that shows hotel and restaurant reviews, accommodation bookings and other travel-related content. Headquartered in Needham, Massachusetts, TripAdvisor is the largest "social travel website" in the world, with about 315 million reviewers (active and inactive) and about 500 million reviews of hotels, restaurants, attractions and other travel-related businesses. TripAdvisor was an early adopter of **user-generated content**. The website services are free to users, who provide most of the content, and the website is supported by a hotel booking facility and an advertising business model.

TripAdvisor proposals are grouped in different categories, such as *Hotels*, *Things to do*, *Restaurants*, *Flights*, etc. The data for this project have been scraped from the webpages devoted to the **Hilton Garden Inn Bogota Airport**. More specifically, from `https://www.tripadvisor.com/Hotel_Review-g294074-d12959007.html` for the reviews in English and `https://www.tripadvisor.es/Hotel_Review-g294074-d12959007.html` for those in Spanish. Note that `g294074` identifies Bogotá and `d12959007` identifies the hotel. The data have been captured in April, 2025. 

## The data set

The file `hilton.json` contains 20 reviews, 10 in English and 10 in Spanish, posted by the hotel customers on the TripAdvisor's website. Each review comes as a JSON object with five keys: "author", "date", "triptype", "rating" and "review".

## Task

Using Python, craft a workflow that takes the file `hilton.json` and returns a new file `hilton_responded.json`. The output file is expected to contain the same JSON objects an the input file, but enlarged with an additional key "response", whose value is a response to the review signed by◊ a hotel manager called Manuel Revilla. 

The guidelines are:

- Personalize the response as much as you can, and be friendly and warm.

- Write the response in the same language used by the review, either English or Spanish.

- Control the structure and the length of the response.

- Moderate the response taking into account the rating provided with the review.

