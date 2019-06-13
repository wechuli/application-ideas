# Bike Rental Shop

You have been hired to build a bike rental shop management system for a campus.

## Scenario

- The rental shop operates in several campus
- Each campus has several shops, the shops each contain alist of bikes(belonging to that shop) for hire.
- You can maintain one database that records the bikes, and their features and whether they are on hire or in the shop
- A customer can hire a bike from any one of your shops. When a customer hires a bike, they can return it in any shop listed as one of your rentals
- You should at any point be able to know where a bike is - whether it is on hire, or when it has been returned to one of your shops
- When a bike arrives back at a hire shop, a unique barcode on the crossbar is scanned. The bike tracking database is automatically updated with the name of the shop that scanned the barcode. When a bike leaves a shop with a customer, the location is changed to "On Hire" and the customer name is recorded in a separate column.
- This system has proved helpful when a customer asks for a bike with specific frame size and/or specific features, such as an electric motor or all-terrain suspension. If a shop doesn't have a bike with the right equipment, the shop can quickly find out where such a bike is and get it or send the customer to the right shop. This bike location database has a REST API that you can call from other systems.

The details are as follows:

- A customer requests a bike on the phone, in person, or through the website.
- Shop staff record the customer's details and frame size.
- Does the customer need specific features such as an electric motor, suspension, or a child trailer? If so what are those features?
- Where are all the bikes with that frame size and those features? This information is obtained from the bike location database and is kept up-to-date by the barcode scanning system.
- Is there a bike with the right features and frame size in the right shop? If yes book that bike.
- If not where is the nearest bike? Book that bike.
- Send an email to staff to move the bike to the hirer.
- Scan barcode in new location.
- Give the bike to the customer and update location to "On Hire".
- Take payment from the customer.
