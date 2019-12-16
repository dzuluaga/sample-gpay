# GPay Sample

Sample stand-alone Gpay Sample.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Node.js and NPM version 12+.

### Installing

You can either deploy this Node.js Express app stand alone on your machine or deploy it to [![Run on Google Cloud](https://deploy.cloud.run/button.svg)](https://deploy.cloud.run).

#### Step 1: Edit tokenizationSpecification from gateway-config.js

Replace the parameters with your values. Refer to the [Google Pay API gateway documentation](https://developers.google.com/pay/api/web/reference/request-objects#gateway) for details on your payment gateway's settings.

```
const tokenizationSpecification = {
    type: 'PAYMENT_GATEWAY',
    parameters: {
      'gateway': 'example',
      'gatewayMerchantId': 'exampleGatewayMerchantId'
    }
  };
```

#### Step 2: Install dependencies

```
npm install
```

#### Step 3: Start the server

Your server should start by default with port 8080.

```
npm start

Example app listening on port 8080!
```

#### Step 4: Open the page

Open [http://localhost:8080](http://localhost:8080)

#### Step 5: Click the Buy with GPay button

#### Step 6: Select your Google Account and payment method

#### Step 7: Click Continue to complete the payment