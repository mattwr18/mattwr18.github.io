rentals/index route that displays the rental page's general information, and also lists available rentals. The index nested route is shown by default when the user visits the rentals URL.

rentals/show route that still displays the rental page's general information, while also showing detailed information about a selected rental. The show route will get substituted with the id of the rental being shown (for example rentals/grand-old-mansion).

Generating nested index route

ember g route rentals/index

Move findAll call from the parent rentals to the new sub-route.

Move the rental list markup from main route template to the nested route index template

ember g controller rentals/index

Instead of copying and pasting code from the parent controller

import RentalsController from '../rentals';
export default RentalsController;

Setting up Data for the Nested Detail Route

Add code o find  and return the provided rental from our rental list above

Generate a Nested Detail Route

ember g route rentals/show

update router.js with path /:rental_id

edit show route to retrieve the request (add model, findRecord)

Linking to a Specific Rental

add {{#link-to}}{{/link-to}} tab to rental-listing.hbs making the title a link to the show page

Application Tests list-rentals-test.js
