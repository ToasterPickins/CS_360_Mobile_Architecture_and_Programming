# CS_360_Mobile_Architecture_and_Programming

### Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?

The intent of this app was to provide a solution to end users that would allow them to keep track of an inventory in a secure manner. It allows the user to login to the app, add items to and remove items from an inventory, and adjust quantities on hand. It also alerts the user when an inventory has reached a zero quantity by either sending them an SMS (assuming SMS permissions are granted) or by displaying a toast popup. The intended end user is someone who works directly with an inventory. This this could include warehouse staff, purchasers, or management.

### What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?

This app centers around four main screens:
1. Login screen - Allows a user to register or login to the app
2. Inventory screen - Displays the inventory on hand in a scrollable format with the ability to increase, decrease, or delete items
3. Add item screen - Provides the ability to add new items to the inventory by supplying the item name, description, and starting quantity
4. Settings screen - Allows for a user to turn on or off SMS functionality for low inventory alerts

Additionally, it uses a SQLite database to store user login data and item inventory data.

All user interface screens were designed with a material design approach in mind while also incorporating accessibility aspects where possible (i.e., appropriate contrast, font sizes, button sized, etc.). Overall this helped to make the app easy to navigate and use.

### How did you approach the process of coding your app? What techniques or strategies did you use? How could those be applied in the future?

Coding was done in an iterative approach. The main components of the app were determined then broken down in to smaller chuncks. After each chunk was coded, the app was built and tested to ensure what as created functioned as intended and met the end users needs. The approchs was continued until completed. Additionally, use of general comments and TODO comments were incorporated to ease the understanding of what had been coded and also ensure needed features weren't accidentally overlooked while coding and testing. An additional technique used that I haven't used extensively yet was the use of Git. This helped me to feel confident that I could work on adding and updating code without risking breaking something and not being able to easily fix it. I look forward to using Git in greater detail on future projects.

### How did you test to ensure your code was functional? Why is this process important and what did it reveal?

For this project, all testing was done manually. After coding a specific section, I would run the app and ensure what was built worked as intended and didn't have any negative consequences for already completed code. After the fact, I wish I had used JUnit to automate much of the testing as I realized that I spent more time manually testing things than it would have taken to write useful unit tests.

### Considering the full app design and development process, from initial planning to finalization, where did you have to innovate to overcome a challenge?

The main challenge I had was incorporating functional buttons in the RecyclerView for the inventory list. Each item line has its own set of buttons to adjust the inventory and delete the item. At first, I had a difficult time getting the functionality of these buttons to work correctly, but after doing additional research into the RecyclerView, RecyclerView.Adapter, and RecyclerView.ViewHolder classes I was able to make things work as intended.

### In what specific component from your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?

I would say it was the RecyclerView component and the imbeded functionality it provides through the action buttons (i.e., increase/decrease inventory and delete buttons). I wanted to have this functionality present and easy to access to end users while viewing the inventory list so they didn't have to access a separate screen just to make these adjustments. Additionally, I believe this took knowledge we gained from the course while learning about RecyclerViews a step further by incorporating interactive parts and not leaving each item as static information.
