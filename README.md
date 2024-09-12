# BUILDH3R_Sept_Aleo

https://www.youtube.com/watch?v=slVmiwqNiRw&t=1773s

## Task for Aleo ZK workshop

- You just wrote your first leo program and created a simple version of a private Auction.
- Your task is to complete a functionality. We are adding a new record called Prize.
```leo
record Prize {
        owner: address,
        amount: u64
    }
```
- Your task is to write a function to claim the prize with the winning bid. The function signature is given below. You need to add the logic for the claim function which assigns the prize to the wiining bidder.
```leo
transition claim(bid: Bid) -> Prize {
```
- Ensure that you check the prize only goes to the winning bid

### Links
https://github.com/laishawadhwa/Aleo-Workshop/blob/main/README.md

# Task Done

