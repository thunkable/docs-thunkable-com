| `IMPORTANT The Payment component powered by Stripe charges a 4.9% fee +$0.30 per transaction, 2% of which is taken by Thunkable as a maintenance fee` |
| :--- |


#### **Thunkable for iOS **

# Payment ![](/assets/iOSviewIconStripe.png) powered by Stripe

---

Accepting payments are a critical part of many apps from on-demand services to in-person commerce. Stripe is one of the most popular payment providers for internet providers globally and powers the Payments component, which accepts all major debit and credit cards from customers in every country in [135+ currencies](https://stripe.com/docs/currencies).

`IMPORTANT The Payment component powered by Stripe charges a 4.9% fee +$0.30 per transaction, 2% of which is taken by Thunkable as a maintenance fee`

* [Set up](#set-up)
* [Accept a payment](#accept-a-payment)

---

### Set up

#### Step ① / Create your [Stripe](https://stripe.com/) account![](/assets/payment-stripe-✕-fig-1.png)

#### Step ② / Apply to accept payments by credit or debit card

You'll have to apply to Stripe for your business to accept payment by credit or debit card

![](/assets/payment-stripe-✕-fig-2.png)![](/assets/payment-stripe-✕-fig-3.png)

#### Step ③ / Connect your Stripe account with Thunkable

There are two properties that you need to retrieve from Stripe to connect it with Thunkable: `Publishable Key` and `Stripe Account ID`

![](/assets/payment-stripe-✕-fig-4.png)

`Publishable Key`

`Stripe Account ID`

#### \(Optional\) Step ④ / Require full address \(iOS only\)

On iOS, there is an option to require a full address instead of just a zip code when accepting payment. Stripe reserves the right to change the payout schedule or suspend payments to your bank account if they deem it necessary, likely if there is fraudulent activity in the payments. Requiring a full address lowers the risk of fraudulent activity.

---

### Accept a payment

![](/assets/payment-stripe-✕-fig-5.png)![](/assets/payment-stripe-✕-fig-6.png)

| Event | Description |
| :--- | :--- |
| One Time Charge \(`amount`, `currency` in three letter abbreviation e.g. USD, `receiptEmail`, `receiptDescription`\) | Stripe accepts [135 different currencies](https://stripe.com/docs/currencies#charge-currencies) and automatically sends a receipt to the user if an email address is provided. If successful, returns a `chargeId` and `chargeInfo` |



