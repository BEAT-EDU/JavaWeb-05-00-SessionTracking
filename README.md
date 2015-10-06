# JavaWeb-05-00-SessionTracking


ShowSession.java. Servlet that uses session tracking to keep per-client access counts. Also shows other info about the session.

ShowItems.java. Servlet that displays a list of items being ordered. Accumulates them in an ArrayList with no attempt at detecting repeated items. Uses OrderForm.html to collect data.

OrderForm.html. Front end to the ShowItems servlet.

CatalogPage.java. Base class for pages showing catalog entries. Servlets that extend this class must specify the catalog entries that they are selling and the page title.

KidsBooksPage.java. A specialization of the CatalogPage servlet that displays a page selling three famous kids-book series. Orders are sent to the OrderPage servlet.

TechBooksPage.java. A specialization of the CatalogPage servlet that displays a page selling two famous computer books. Orders are sent to the OrderPage servlet.

OrderPage.java. Servlet that records new item orders (if any) and then displays all items in the shopping cart.

Checkout.html. Page that handles the final checkout. We recommend you edit this before using it.

ShoppingCart.java. A shopping cart data structure used to track orders. The OrderPage servlet associates one of these carts with each user session.

CatalogItem.java. Describes a catalog item for an online store. Elements of this class are indirectly stored in the ShoppingCart (after they are embedded within an ItemOrder).

ItemOrder.java. Class that associates a catalog Iitem with a specific order by keeping track of the number ordered and the total price. Elements of this class are directly stored in the ShoppingCart (after each is populated with a CatalogItem).

Catalog.java. A catalog that lists the items available in inventory.
