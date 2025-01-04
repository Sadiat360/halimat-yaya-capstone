# Project Title

## Overview

Arewa in Yoruba Language means (Beauty), Arewa is a E-commerce web-app for users to find beauty products that suits their needs.
### Problem Space


Beauty means different things to different people. However, as a woman, I can say that being called beautiful is something many of us hold dear. In today’s world, we often hear about the struggle to find the perfect beauty products that truly meet our needs. This is why *Arewa* was created.  

Many users spend endless hours searching websites that don’t prioritize their preferences or needs, often ending up frustrated by a complicated shopping experience. *Arewa* aims to change that by offering a simple, user-friendly solution that understands and caters to individual beauty needs, making the search for the perfect product effortless and enjoyable.  


### User Profile

- Beauty Divas:
  - looking for beauty products that suits their needs
  - Get recommendations based on my preferences
  - Read product reviews and ratings with visuals from previous customers
  - Easy cart management and checkout gateway
  - 
### Features

List the functionality that your app will include. These can be written as user stories or descriptions with related details. Do not describe _how_ these features are implemented, only _what_ needs to be implemented.

## Implementation

### Tech Stack

- React
- JavaScript
- MySQL
- Express
- Client libraries: 
    - react
    - react-router
    - axios
    - react-redux
    - stripe
- Server libraries:
    - knex
    - express
    - cors
    - dotenv
    - stripe
    - bcrypt for password hashing

### APIs

No external APIs will be used i will create my API

### Sitemap

![](Site-map.png)

- Home page
- Search
- Quiz
- Lists of Products
- Ask a question
- Product Details/Reviews
- Add to Cart
- Checkout
- SignUp
- SignIn

### Mockups

### Home Page
![](Home-Page.png)

### Quiz Page
![](Quiz-Page.png)

### Product Details Page
![](Product-details.png)

### checkout page
![](checkout-page.png)

### SignUp page
![](SignUp.png)

### SignIn Page
![](SignIn.png)


### Data

Describe your data and the relationships between the data points. You can show this visually using diagrams, or write it out. 

### Endpoints

**GET / bestSellers**

Response:
```
[
    {
        "id": 1,
        "name": "Lips high shimmer",
        "image": "/image",
        "price": "$50",
        "rating": 4.5,
        "description": "bold lips",
        "details": "Warning: Intense Hydration Ahead. Lasting Glow. GlowBoost Vitamin C Serum with Hyaluronic Acid and Antioxidants delivers a powerful burst of hydration and radiance instantly and over time. This glow-enhancing serum is available in 5 radiant variants, like Sunlit Glow, Brightening Boost, Dewy Dream, Golden Radiance, and Fresh Awakening. Prepare for visibly brighter, smoother, and more luminous skin every day.",
        "slug": "model-one-image"
    },
    ...
]
```
**GET / bestSellers/:id**

 Get bestSellers by id, users can read product reviews even if the user is logged in or not


Response:
```
[
    {
        "id": "3r7q32sd4d8821g3442",
        "name": "Lips high shimmer",
        "image": "/image",
        "price": "$50",
        "rating": 4.5,
        "description": "bold lips",
        "details": "Warning: Intense Hydration Ahead. Lasting Glow. GlowBoost Vitamin C Serum with Hyaluronic Acid and Antioxidants delivers a powerful burst of hydration and radiance instantly and over time. This glow-enhancing serum is available in 5 radiant variants, like Sunlit Glow, Brightening Boost, Dewy Dream, Golden Radiance, and Fresh Awakening. Prepare for visibly brighter, smoother, and more luminous skin every day.",
        "slug": "model-one-image",

        "reviews":[
          {
            "id": "34a7sd93k248s8f212752",
            "reviewerName": "Jane Doe",
            "ratings": "4",
            "title": "Great Product",
            "reviewText": "I’m obsessed! The color match is spot on, and it gives me such a natural glow.",
            "image": "/image",
            "timestamp": 123456789046865
          }
          {
            "id": "84a7sd33k148s8f215192",
            "reviewerName": "Jackie wolf",
            "ratings": "4.5",
            "title": "I love it",
            "reviewText": "This product is incredible! The coverage is flawless, and it feels so lightweight on my skin",
            "timestamp": 123456789046865
          }
        ]
    },
    ...
]
```

**POST / bestSellers/:id/rating**

- Logged in user can add their rating of a product

```
[
    {
        "id": "84a7sd33k148s8f215192",
        "reviewerName": "Jackie wolf",
        "ratings": "4",
        "title": "I love it",
        "reviewText": "This product is incredible! The coverage is flawless, and it feels so lightweight on my skin",
        "timestamp": 123456789046865
    },
    ...
]
## Roadmap

Scope your project as a sprint. Break down the tasks that will need to be completed and map out timeframes for implementation working back from the capstone due date. 

---

## Future Implementations
Your project will be marked based on what you committed to in the above document. Here, you can list any additional features you may complete after the MVP of your application is built, or if you have extra time before the Capstone due date.

