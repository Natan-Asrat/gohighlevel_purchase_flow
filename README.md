# GoHighLevel Purchase Flow
- User visits a funnel website that presents the service and includes a checkout page, completes payment via PayPal, and receives a confirmation email.

## Input

- Lead completes the Web Development service funnel, enters card details, and submits payment.

    ![nate](./screenshots/nate_test.png)

    ![pay](./screenshots/pay_3k.png)

## Output

- Buyer receives a confirmation email.

    ![email](./screenshots/received_email.png)

- Contact record is updated with the Web Dev Customer tag.

    ![update contact](./screenshots/test_tag.png)

## Steps

- Integrate payment processor by going to Payment -> Integrations -> Paypal

    ![payments](./screenshots/payments.png)

    - Go to your paypal sandbox account and create an `app`

    ![sandbox](./screenshots/paypal_sandbox.png)

    ![create](./screenshots/api_credentials.png)

    ![app](./screenshots/ghl_test_app.png)

    - Copy the client id and secret to ghl.

    ![use client id](./screenshots/enter_client_id.png)

- To add a product go to Payment -> Products

    ![products](./screenshots/products.png)

    - Write the product info

    ![info](./screenshots/product_info.png)

    - Add media by uploading and then selecting it.

    ![media](./screenshots/add-media.png)

    - Add your prices.

    ![price1](./screenshots/price1.png)

    ![price2](./screenshots/price2.png)

    - Select each price and update it's name as well it's type to Digital Product.

    ![update name](./screenshots/update_name.png)

    ![type](./screenshots/shipping.png)

    ![prices](./screenshots/prices.png)

    - Check that your product type is Digital

    ![product](./screenshots/products_added.png)

- To create coupons go to Payment -> Coupons

    ![coupon](./screenshots/create_coupon.png)

    ![created](./screenshots/coupons.png)

- Create a funnel so users can find and buy your product.

    ![create](./screenshots/create_funnel.png)

    - Add page

    ![add page](./screenshots/create_page.png)

    - Add a Full width element and in it a 2 column Row. Then on the left add your headline and below it a sub-headline.
    On the right, add an image element. And finally add an order element below the sub-headline.

    ![page](./screenshots/create_website.png)

    - Use a 1 step order element since the product is digital and we don't need much information. Hide unnecessary fields by clicking on the order form under General -> Form options

    ![form](./screenshots/hide_fields.png)

    - In the funnel settings, set the Payment mode to `Test`

    ![pay mode](./screenshots/pay_mode.png)

    - Test the website's preview and the coupon code.

    ![test](./screenshots/test_funnel.png)

    ![paypal1](./screenshots/test_paypal.png)

    ![paypal2](./screenshots/test_paypal2.png)

    - Check that the order is created in Payments -> Orders or Payments -> Transactions

    ![order](./screenshots/order_done.png)

    ![transaction](./screenshots/transaction_done.png)

- Create a workflow to send a `thank you email`.

    ![folder](./screenshots/create_folder.png)

    - Use `order form submission` trigger

    ![trigger](./screenshots/purchased_trigger.png)

    - Send email node

    ![email](./screenshots/order_email.png)

    - Add tag to contact so we know they are a web dev customer

    ![tag](./screenshots/add_tag.png)

    - Test.

    ![test](./screenshots/nate_test.png)

    ![email test](./screenshots/received_email.png)

    ![tag](./screenshots/test_tag.png)

- If you have a subscription based product, set it as recurring when creating the product and use that product in the funnel. New orders will be found in Payments -> Subscriptions.
- To send invoices for a one time product, go to Payments -> Invoices. Add user, product and click send. Choose Email and finalize.


## Contact
 - LinkedIn: [Natan Asrat](https://linkedin.com/in/natan-asrat)
 - Gmail: nathanyilmaasrat@gmail.com
 - Telegram: [Natan Asrat](https://t.me/fail_your_way_to_success)
 - Youtube: [Natville](https://www.youtube.com/@natvilletutor)
 - Website: [Portfolio](https://natanasrat.com)