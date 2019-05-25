# HPP Guide: Integration Overview

## Introduction

PayCore.io Commerce HPP is a secure hosted payment page, where you can redirect customers from your website to make a payment through PayCore.io. Commerce HPP provides customers with access to a range of payment methods, based on their location and your account and integration settings. Integration to Commerce HPP is simple and requires collecting customer payment information on your website in a standard HTML form and submitting this to PayCore.io. Commerce HPP then collects the customer payment details needed to complete the payment, and sends these details to the relevant bank or alternative payment provider for authorisation. After the payment is complete, the customer is returned to your website and you receive a real-time notification of the payment, which includes details of the transaction.

## Customer Journey

A simplified illustration of the PayCore.io HPP payment flow is shown in the figure below.

![HPP Interaction](../images/hpp-interaction.png)

1.  A customer on your website decides to checkout.
2.  Your website redirects the customer to the Hosted Payment Page on the PayCore.io platform by submitting HTML form or calling the Private API with Payment Invoice data the amount, a payment description, a callback URL, and a Return URL we should redirect the customer to after the payment is made.
3.  The customer reaches the Hosted Payment Page, chooses a payment method and makes the payment. This process is entirely taken care of by PayCore.io. You don’t need to do anything here.
4.  At this point PayCore.io returns the visitor to your website using the  `return_url`  specified when the payment was created. Your website already knows the payment was successful and thanks the customer.
5.  When the payment is made PayCore.io will call your  [callback URL](/integration/callbacks/)  informing your website about the  [payment’s invoice status change](/products/commerce/payment-invoice/). You should define a callback when creating the initial payment.
    
    In response to your callback being called your application just needs to issue a  `200  OK`  status. From that response PayCore.io can tell that your processing of the new status was successful – for any other response we keep trying.

    This fetched status serves to mark the payment paid, trigger fulfilment and send out an email confirmation to the customer.

## Next

Learn more about  [integration methods](/products/hpp/guide/integration-methods/): payment widget and payment link.