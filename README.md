# cart-json-with-tags
A Shopify /cart ajax route with product tags included.

Used similarLy to to /cart.js, but includes the "product_tags" field. (Tags aren't included in /cart.js calls by default.)

There are subtle differences between using liquid in this fashion versus the results in cart.js, so please be careful of bugs. I have tried to mimic /cart.js as much as possible. See comments within the file for more info on these differences.

## Example usage
```javascript
const cart = await fetch('/cart?view=json-with-tags').then(res => res.json());
```