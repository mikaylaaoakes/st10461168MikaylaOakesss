# Change Log:
- I added a “course” option at the end of each product ID, to identify which items go to which course.
- I grouped the courses together using the Record<String, T> utility.

**Average price by Course:**

- I added a groupedByCourse object 
- I added a calculateAveragePrice(course) function that calculates the average price for products in a given course by adding up the product prices and dividing by the number of items.
- I used useMemo to create a memo the calculation of average prices for all courses, improving performance when the products array is updated.
- I added a check for empty courses in calculateAveragePrice() to return 0 instead of attempting to divide by zero.
- I changed the average price calculation to use useMemo to optimize performance.
- ` `I used toFixed(2) to format the average price to two decimal places for a cleaner display of prices.

**Product Management:**

1. Added functionality to **add new menu items** with fields for **Dish Name**, **Dish Description**, and **Price**.
1. The new menu item is added to the products state and displayed in a **list** using FlatList.
1. Users can **remove menu items** by clicking the "Remove" button next to each item in the list.

**Form State:**

1. I used React's useState to track the input values for dish name, description, price, and the selected course (Starter, Main Course, or Dessert).

**Validation:**

1. Added basic validation to ensure that **all fields** (Dish Name, Dish Description, and Price) are filled before adding a menu item.
1. If any field is left empty, an **alert** is shown to prompt the user to fill all fields.

**Alert Notifications:**

1. **Success alert** after adding a menu item or removing a menu item from the list.
1. **Error alert** when trying to add a menu item with empty fields.

**Navigation:**

1. A "Back to Menu" button at the bottom of the screen that navigates the user back to the previous screen.

**Styling:**

1. The form fields for **Dish Name**, **Dish Description**, and **Price** are styled with borders and padding for better usability.
1. The "Add Menu Item" button and the "Back to Menu" button are styled with background colors and text to make them more visually prominent.
1. The menu items in the list are styled with a row layout (flexDirection: 'row') to display the name, price, and a "Remove" button.

**FlatList for Product List:**

1. The list of menu items is rendered using FlatList, which makes it efficient for displaying large lists.



