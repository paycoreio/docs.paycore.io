<img src="https://static.openfintech.io/payment_providers/cypix/logo.svg?w=400" width="400px" >

# Cypix

> Modern payment aggregator for your site

**Website**: [cypix.ru](https://cypix.ru/)

**Account**: [log in](https://lk.cypix.ru/#/auth/login)

Follow the guidance for setting up a connection with Cypix payment provider.

## Set Up Account

### Step 1: Contact Cypix support manager

Send a request on the [Cypix website](https://cypix.ru/) or call the hotline. Submit the required documents to verify your account and gain access.

### Step 2: Get credentials

Credentials that have to be issued:

* `accountId` — your account Identifier on the Payout Platform side
* `serviceApiKey` — service identifier for Cypix API
* `secret` — your unique secret key for signing API requests
* `host` — API platform domain

## Connect Provider Account

### Step 1. Connect account at the {{custom.company_name}} Dashboard

Press **Connect** at [*Cypix Provider Overview*]({{custom.dashboard_base_url}}connect-directory/payment-providers/cypix/general) page in *'New connection'* and choose **Provider account** option to open Connection form.

![Connect](images/provider-account.png)

Enter credentials:

* `accountId` --> Account ID
* `serviceApiKey` --> API Key
* `secret` --> Secret Key
* `host` --> Host

Also, select Test or Live mode according to the type of account to connect with Cypix.

!!! success
    You have connected **Cypix** account!

## Connect H2H Merchant Account

### Step 1. Connect H2H account at the {{custom.company_name}} Dashboard

Press **Connect** at [*Cypix Provider Overview*]({{custom.dashboard_base_url}}connect-directory/payment-providers/cypix/general) page in *'New connection'* and choose **H2H Merchant account** option to open Connection form.

![Connect](images/h2h-merchant-account.png)

Enter credentials:

* `serviceApiKey` --> API Key
* `secret` --> Secret Key
* `host` --> Host

Select Test or Live mode according to the type of account to connect with Cypix. Choose Currency: set this parameter according to available currencies for your Cypix account.

!!! success
    You have connected **Cypix** H2H merchant account!

!!! question "Still looking for help connecting your Cypix account?"
    <!--email_off-->[Please contact our support team!](mailto:{{custom.support_email}})<!--/email_off-->
