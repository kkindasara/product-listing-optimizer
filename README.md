# AI Product Listing Optimizer (Elihome)

A small web app for Elihome's kitchen products. Enter a product name, material, key features and target customers, and the AI writes:

- a professional product title
- five key selling points
- an SEO-friendly description (with keywords)
- short marketing copy

All text is in English. The app uses the Claude API.

## How to use it

1. Open the app (GitHub Pages link, or `index.html` in a browser).
2. Open **API settings** and paste an Anthropic API key (created at console.anthropic.com).
3. Fill in the product details (or press **Fill example**) and press **Generate listing**.
4. Review the text, then copy each part or press **Copy all**.

## About the API key

- The key is typed into the page by the user. It is kept only in the current browser tab (if "Remember" is ticked) and is never saved in this repository.
- Never write an API key in the code or commit it to GitHub.
- Because the page calls the API directly from the browser, this version is meant for internal testing. A public version should send requests through a small server that holds the key.

## Safety of the generated text

The AI is told to use only the facts given and not to invent claims such as "dishwasher safe", "food safe" or heat limits. Every listing still needs a human check against the approved product data before it is published.

## Files

| File | What it does |
|---|---|
| `index.html` | Page layout: form and results |
| `style.css` | Styles |
| `app.js` | Prompt, API call and display of the results |

## Possible next changes

- Choose a marketplace (Amazon, Shopify, Wayfair) and adapt title length and style
- Choose a tone (premium, friendly, technical)
- Download the listing as a text or CSV file
- Keep a history of generated listings

First version built with Claude.
