# Rapyd Checkout Toolkit Demo

### Quickly integrate Rapyd Checkout Toolkit into your online shopping cart
This repository contains a simple example demonstrating how to add Rapyd's Checkout Toolkit to an eCommerce website. Checkout Toolkit lets you embed an iframe directly into your shopping cart payment acceptance fields. This ensures your customers are never redirected away from your website during the checkout process.

## Demo Video (YouTube)
<a href="https://youtu.be/3a788d8NFCc"><img src="https://files.readme.io/a4897c1-Youtube_Thumbnail_-_Rapyd_Bytles_-_Checkout_Toolkit2x.png" alt="thumbnail of video link for youtube video showing rapyd checkout toolkit video" style="width:500px"></a>

## To use this example:
1. Clone this repository
2. Create a checkout page using the API: https://docs.rapyd.net/build-with-rapyd/reference/checkout-page-object#create-checkout-page
3. Copy the checkout page id from the API response (for example, "checkout_123456789123456789123456789")
4. Open the checkout.html file and find the code below. Paste the checkout id in the "id" field:

```javascript
let checkout = new RapydCheckoutToolkit({
    pay_button_text: "Pay Now",
    pay_button_color: "#4BB4D2",
    id: "checkout_", // your checkout page id goes here
    style: {
        submit: {
            base: {
                color: "white"
            }
        }
    }
});
```
## Resources
* Make your first call with Rapyd API:
https://docs.rapyd.net/build-with-rapyd/docs/make-your-first-api-call
* Join the Rapyd Community:
https://community.rapyd.net 
