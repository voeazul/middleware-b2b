# Subscription Key Request

The Middleware B2B has a management and security layer, called API Gateway, which is a platform where it is possible to manage and protect APIs in a scalable and efficient way. To access our APIs you need to request a Subscription Key.

## What is a Subscription Key?

A Subscription Key is a unique identifier used to authenticate your requests to the APIs. Each user or application that consumes our APIs receives a unique access key, which must be used to identify and authorize calls.
This subscription key must be requested on the Developer Portal.

## Developer Portal Access

Our Developer Portal is a dynamic platform that offers a complete view of the APIs available for integration. There you can request and manage your subscription keys, find documentation and use a sandbox to test your API calls.

We are using the Developer Portal provided by Azure API Management. Access the URLs below to access the portal in the Stage and Production environments.

[Developer Portal Stage Environment](https://apim-stg-us-general.developer.azure-api.net/product#product=sales-b2b-agency)   
[Developer Portal Production Environment](https://apim-prd-us-general.developer.azure-api.net/product#product=sales-b2b-agency)

## How to register

Follow the steps below to register for the Developer Portal:

1. Access the Developer Portal URL for the desired environment.
2. Click "Sign up" on the home page.
3. Fill out the registration form with your information.
4. After registering, you will receive a confirmation email.
5. Follow the instructions in the email to confirm your account.
6. After confirmation, you will be able to log in to the Developer Portal.

![Signup](/docs/assets/subkey-signup.png)

## Requesting an API Key

Follow the steps below to request a subscription key:

1. Log in to the Developer Portal.
2. Navigate to the "Products" section.
3. Filter by product "__Sales B2B - Agency__", and after displaying, click on it.
![Steps 2 and 3](/docs/assets/subkey-search-product.png)
4. Give your signature key a name, by default, leave the name of your key with the name of the agency so that the person responsible for approval can identify who will use it. Example:
    - azul-viagens-key
5. Click on "Subscribe".
![Steps 4 and 5](/docs/assets/subkey-subscribe-product.png)
6. After that, you need to wait for approval from the Azul Business team.
7. After approval, a notification will be sent to the email used to create the account on the developer portal.

## Viewing a Subscription Key

Follow the steps below to view a subscription key:

1. Log in to the Developer Portal.
2. Navigate to the "Profile" section.
3. All your key requests and approved keys will be listed.
4. If your key is already approved, the "Show" option will be displayed, if this option is not displayed, your request has not yet been approved.
4. If approved, click "Show" and copy the displayed key.
5. After that, just add this key to the "Ocp-Apim-Subscription-Key" header of all requests for the Middleware APIs.

![Subscriptions](/docs/assets/subkey-show-key.png)

__Important__: This key is for the agency's individual use and must not be disclosed to unauthorized people.
If any unusual behavior is identified in the use of APIs using the subscription key, it will be revoked immediately, interrupting all operations with the Middleware and requiring the generation and approval of a new key.

## Updating a Subscription Key

If you suspect that your subscription key has been disclosed to unauthorized parties, you can reset it in the Developer Portal. Remember that when you regenerate a key, the previous one will be immediately invalidated and you will lose access to the Middleware APIs.

Follow the steps below to regenerate a key:

1. Log in to the Developer Portal.
2. Navigate to the "Profile" section.
3. All your requests and active subscription keys will be listed.
4. Find the key you want to regenerate.
5. Click on the "Regenerate" option in the row of the subscription key you want to regenerate.
6. After that, just update the key in the necessary places and use it.

![Regenerate Subscription Key](/docs/assets/subkey-regenerate-key.png)

Now you're ready to take advantage of the full benefits of our APIs. If you have any questions or need additional support, please contact us.