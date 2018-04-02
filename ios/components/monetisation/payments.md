| `IMPORTANT The Payment component powered by Stripe charges a 4.9% fee +$0.30 per transaction, 2% of which is taken by Thunkable as a maintenance fee` |
| :--- |


#### **Thunkable for iOS **

# Payment ![](/assets/iOSviewIconStripe.png) powered by Stripe

---

Accepting payments are a critical part of many apps from on-demand services to in-person commerce. Stripe is one of the most popular payment providers for internet providers globally and powers the Payments component, which accepts all major debit and credit cards from customers in every country in [135+ currencies](https://stripe.com/docs/currencies).

**`IMPORTANT The Payment component powered by Stripe charges a 4.9% fee +$0.30 per transaction, 2% of which is taken by Thunkable as a maintenance fee`**

![](/assets/payment-stripe-✕-fig-5.png)

* [Set up](#set-up)
* [Send a test transaction](#send-a-test-transaction)
* [Accept payments](#accept-payments)

---

### Set up

#### Step ① / Create your [Stripe](https://stripe.com/) account![](/assets/payment-stripe-✕-fig-1.png)

#### Step ② / Apply to accept payments by credit or debit card

You'll have to apply to Stripe for your business to accept payment by credit or debit card

![](/assets/payment-stripe-✕-fig-2.png)![](/assets/payment-stripe-✕-fig-3.png)

#### Step ③ / Connect your Stripe account with Thunkable

There are three properties that you need to retrieve from Stripe to connect it with Thunkable: `Test Publishable Key` , `Live Publishable Key` and `Stripe Account ID`. The first two are retrievable from the Stripe dashboard while the third requires visiting a special link. In the interest of security, you'll have to navigate to the App Settings on Thunkable to enter the properties for Stripe![](/assets/payment-stripe-✕-fig-7.png)`Test Publishable Key`

On the Stripe dashboard, set your Developer toggle to "Viewing test data" and copy the Publishable key from the interface![](/assets/payment-stripe-✕-fig-8.png)

`Live Publishable Key`

On the Stripe dashboard, set your Developer toggle to live and copy the Publishable key from the interface

![](/assets/payment-stripe-✕-fig-9.png)

`Stripe Account ID`

The Stripe Account ID is a unique account level ID that you retrieve by connecting your Stripe account to Thunkable. Make sure you are logged into your Stripe account and then visit** **BOTH** **[**x.thunkable.com/stripe/connect/test**](/x.thunkable.com/stripe/connect/test)** **and** **[**x.thunkable.com/stripe/connect/live**](/x.thunkable.com/stripe/connect/live) and click the buttons below

![](/assets/payment-stripe-✕-fig-10.png)![](/assets/payment-stripe-✕-fig-11.png)You should see the following on your Stripe dashboard if your connections were successful

![](/assets/payment-stripe-✕-fig-18.png)

---

### Send a test transaction

To send a test transaction, make sure your Stripe property setting is set to "Test Mode"

![](/assets/payment-stripe-✕-fig-7.png)

Apps that accept payments should have a simple form for collecting user information both for sending a receipt and collecting transaction information and a confirmation page for letting the user know if the transaction went through successfully

![](/assets/payment-stripe-✕-fig-12.png)The Payment block itself returns a `chargeId` if the payment went through successfully or an `error` if it did not

![](/assets/payment-stripe-✕-fig-13.png)

| Event | Description |
| :--- | :--- |
| One Time Charge \(`amount`, `currency` in three letter abbreviation e.g. USD, `receiptEmail`, `receiptDescription`\) | Stripe accepts [135 different currencies](https://stripe.com/docs/currencies#charge-currencies) but `amount` is denoted in the currencies' smallest unit i.e. USD is measured in cents. If successful, returns a `chargeId` and `chargeInfo` . During live mode, a successful charge will send a receipt to the `receiptEmail` with the `receiptDescription` as the title. \(No email will be send during testing mode\). There are [minimum charge amounts](https://stripe.com/docs/currencies#charge-currencies) for certain currencies as per Stripe's rules |

 

 

If you toggle on "Viewing test data" and "Payments"  on the Stripe Dashboard, you will be able to view your test transactions

#### ![](/assets/payment-stripe-✕-fig-15.png)\(Optional\) Require full address \(iOS only\)

On iOS, there is an option to require a full address instead of just a zip code when accepting payment. Stripe reserves the right to change the payout schedule or suspend payments to your bank account if they deem it necessary, likely if there is fraudulent activity in the payments. Requiring a full address lowers the risk of fraudulent activity.

---

### Accept payments

To accept payments, simply toggle the "Test Mode" to false in the Thunkable Stripe app settings

![](/assets/payment-stripe-✕-fig-14.png)

 After you sent a successful transaction, you'll see both the user payment amount\(s\) on your Stripe dashboard as well as the Net amount \(the amount you receive = the user payment amount less $0.30 + 4.9% of the total amount, which includes both Stripe and Thunkable's fees\).

![](/assets/payment-stripe-✕-fig-16.png) 

Users will also receive an email receipt if the email address is provided

![](/assets/payment-stripe-✕-fig-17.png)

