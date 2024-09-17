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
see ./src/main.leo

...
```leo

    transition claim(bid: Bid) -> Prize {
        assert_eq(bid.is_winner, true);
        return Prize {
            owner: bid.bidder,
            amount: bid.amount,
        };
        
    }
```


Aleo Task : auction dapp 

Wallet: aleo172ag4qhstvzn75rnjh7gucc8jzqdlkzf9jxy78gd9xz488tnasyqzhx6d3

<img width="1181" alt="Pasted Graphic" src="https://github.com/user-attachments/assets/ca63f0cc-52c5-41d7-bcf6-11c5873fbb9b">

⌛ Deployment at1pfyygy9y2d0lqzfdlvtwmz3e283c4w7xpun6qtayrz6m5fdxuqxseyenhu ('token_mint.aleo')

Transaction ID :
``` at1pfyygy9y2d0lqzfdlvtwmz3e283c4w7xpun6qtayrz6m5fdxuqxseyenhu ```

Owner signature
sign1srhflqgyuq0c34z9us44ujyt4w0etmqussgmat5ssjkg3j63eyq8rst735cth80wvxrdlkk7mjrardhlz36jk5tgkllzcrzam65fqq27xsxuc36rm2246086nt7atc3c7j6ftgqnthkp38n8366ank4vqkjevaddz3pj4axqeveser7xhqeefewqe9v09qa97pmw4ze8n38sgjs6p3w

link : https://testnet.aleoscan.io/program?id=token_mint.aleo

<img width="1357" alt="Fee transition" src="https://github.com/user-attachments/assets/063e7458-dee6-4670-b739-588619de9de2">


<img width="1302" alt="imagen" src="https://github.com/user-attachments/assets/2279ab6e-110e-4ad6-aa78-2308e52cdd2b">


