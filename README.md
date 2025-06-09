# Food For All
##### *Built By:* Emma Stowe, Ian Kerman, Jamie Snyder, Mark Ivanovich
## Inspiration
In many communities across the United States, eating a fast-food hamburger is easier than making one at home. When your closest source of groceries is a convenience store or a dollar store, access to fresh ingredients like ground beef and tomatoes is limited. This leads to people consuming unhealthy foods, which can lead to chronic health conditions or exacerbate existing ones.

In addition to limited geographic access to food, other issues can contribute to unhealthy eating. Food insecurity, lack of time for meal planning, and health conditions requiring specialized diets make it even more difficult for families to create healthy meals.

At Food For All, we connect people with local food resources, whether a chain grocery store or a corner bodega. Live inventory and pricing data from local stores are combined with a database of recipes and nutritional data for food to create a personalized shopping list and meal plan, making it easier for individuals and families to eat healthy.


## How We Did It
Combining Bright Data's business database and Databricks' **agent framework**, we created an interactive tool to help families plan healthy meals. An LLM receives user input such as location, health conditions to consider, and any food restrictions. The agent selects appropriate recipes from a database and then searches local grocery stores for inventory and prices. The LLM then takes the information and creates a shopping list for the user to take to the store and cooking instructions to make the meal at home.


## Challenges We Overcame
Initially, we were hoping to use grocery store APIs to access live inventory and prices. However, we found that most grocery stores don't provide APIs, and the ones that do don't seem to maintain them. 

To circumvent this, our agent uses a web scraper to find current inventory and prices on grocery store websites.
 

## What's Next
Although Food For All helps families plan healthy meals, it doesn't address the issue of food deserts. In many communities, the closest "supermarket" is a convenience or dollar store. We would like to integrate with these stores to provide notifications for when fresh food is available, allowing families to take advantage of limited inventory.

Taking inspiration from the food waste-reducing app Too Good To Go, we would also like to partner directly with grocery stores and local markets to provide families with access low-cost, fresh food that can't be sold, but is still safe and healthy to eat. This provide even lower-cost options to families with food insecurity.
