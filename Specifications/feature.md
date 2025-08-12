Implement the following additional feature:

# Recipes

**Purpose**: Maintain a collection of recipes and their ingredients. 

The Recipe Page (to be added) displays all defined recipes in a table, each with their ingedrients in a separate column.  Editing a Recipe enables the user to define the recipe name and what products are needed for the recipe (as ingredients). 

## UI Test Specifications

### Recipes Page Tests

1. **Recipe Creation**: Users can add new recipes by specifying the recipe name, how many people it serves, and selecting which products it requires.

2. **Products Required**: During recipe creation and editing, users can select multiple products that are ingredients. Upon updating the recipe, all its ingredients are persisted.

3. **Filter by Product**: Users can select a product and see what recipes use the selected product as ingredient.

## Intent

In future enhancements, users can see what recipes can be made with available products, and create shopping lists based on a selected recipe.

## Implementation Requirements

Use @onchange instead of @bind for data binding.

Generate bUnit tests that ensure all CRUD operations are done correctly, explicitly checking (using database calls) that each new persisted state is correct. Do not use any Task.Delay statements but rather use bUnit's WaitForAssertion.

### Definition of Done
- All UI functionality works as specified
- All data is correctly persisted to database
- All database operations are properly tested
- Data integrity is maintained across all operations

