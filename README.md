# 🖼️ DigitalCardExchange 🖼️

DigitalCardExchange digital card exchange Daml app.

## I. Overview

Digital Card Exchange is a project that allows creation of digital cards and be exchanged using a bidding system

Companies known as "issuer" like NBA, NFL can publish cards of famous players like LeBron James, Tom Brady, etc. and users can bid on them. The issuer decides when to choose the highest bid. Once the bid is accepted, the issuer will transfer the ownership of the card to the highest bidder. After the transfer, the new owner can start the bidding again (whenever he choose) and the process starts again.

## II. Workflow

   1. Issuer company publish card and sets it open for bidding
   2. Buyer 1 bids on card
   3. Buyer 2 bids on card
   4. Issuer company (also current card owner) accepts highest bid and transfer ownership to highest bidder
   5. New owner(former highest bidder) sets new price for card and starts new bidding
   6. Buyer 3 bids on card
   7. Buyer 1 bids on card
   8. Owner can accept highest bid and transfer ownership to highest bidder

## III. Challenge(s)

* No techical challeges should stop from running and testing the app.

However, here are some business challenges I found while build the app that could be addressed:

* For simplicity, there transaction doesn't involved any money transfer. Adding such feature would be complex and require more time.
* `CardService` can only be created by the issuer company. This was done for the sake of testing but in real world, this may not be the best way to provision a service that handles fetching of created cards.

## IV. Compiling & Testing

To compile, run and/or test you can execute the following:

Run and start Navigator

```shell
daml start
```

Run Tests

```shell
daml test
```
