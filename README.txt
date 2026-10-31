TASTEATLAS — RECIPE EXPLORER

HOW TO RUN IN VS CODE
1. Extract tasteatlas-recipe-explorer.zip.
2. Open the extracted folder in Visual Studio Code.
3. Install the Live Server extension if needed.
4. Right-click index.html and choose “Open with Live Server”.
5. Keep an internet connection on for API requests and images.

FILES
- index.html : website structure and API settings form
- style.css  : design and responsive layout
- script.js  : recipe search, API integrations, favourites and recipe details

THREE API INTEGRATIONS
1. TheMealDB — https://www.themealdb.com/api.php
   Used for recipe search, cuisine/area filtering, recipe details and the default demo source.
   The demo endpoints used by this project do not require an API key.

2. Edamam Recipe Search API — https://developer.edamam.com/edamam-recipe-api
   Used for recipe search, ingredients, recipe-source links and available nutrition data.
   You need an Edamam App ID and App Key for this specific API.

3. Spoonacular Food API — https://spoonacular.com/food-api
   Used for recipe search, ingredient-based matching, recipe details and available nutrition data.
   You need a Spoonacular API key. Usage limits depend on your plan.

HOW TO CONNECT EDAMAM OR SPOONACULAR
1. Open the website and scroll to “Choose your recipe API”.
2. Select Edamam or Spoonacular.
3. Enter the credentials you obtained from that API provider.
4. Click “Save API settings”.
5. Search for a food or ingredient. The chosen API will be used for that search.

NOTES
- TheMealDB is selected by default, so the website works without credentials.
- Edamam web recipes generally provide a link to the original recipe rather than full cooking instructions. Use “View original recipe” in the recipe details.
- Recipe availability depends on each provider's database and API plan. Malaysian dishes are also shown in a small featured collection with English names.
- Credentials entered in the website are kept in sessionStorage for this browser session, not in the project files. However, browser-side API keys can still be inspected by a visitor. This setup is for local coursework/testing only; use a server-side backend/proxy before publishing the site publicly.
