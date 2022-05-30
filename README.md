<!-- @format -->

# zku

### Mission

The Safe Remote Purchase smart contract in Solidity Docs demonstrates a number of Solidity features. Read through the description and code to figure out what each line does.

1. Copy the contract onto Remix and merge confirmReceived and refundSeller into a function completePurchase that, when called, would transfer the due values to the buyer and seller respectively.

2. Limit the calling of completePurchase using modifier(s) to only when the conditions below are satisfied:

- The current State is Locked.

AND

- Either:

  - The caller is the buyer.
  - ≥5 minutes have elapsed since the buyer called confirmPurchase. (Block’s timestamp can be assumed as representative of real time.)

  Make sure the state is updated when the function is called.
  Feel free to modify the available states if you find it necessary.

3. Deploy your amended contract.
4. Take screenshots of the Remix UI that show:

- Time of contract deployment
- Call by seller reverts before time has elapsed
- Call by seller succeeds after time has elapsed

5. Push the .sol file and the .jpg/.png screenshots to a GitHub repository. (Link to be submitted in Question 8.)
