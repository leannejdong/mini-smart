# Smart Contract Rust Via Casper/Wasm

## Dev Environment Set Up
```
cmake --version

cargo install cargo-casper

rustup update
```

## Create a Project, Compile to Wasm

```
cargo casper my-project

cd mini-smart

make prepare

make build-contract

make check-lint

make test
```

## Example one may try..

## Market auction Implementation
Implement a smart contract in solidity for market auction
Users in this Contracts are:
- Suppliers: bids submitted by the producers (Supply) 
- Consumers: bids submitter by the consumers (Demand)
They will provide the quantity and price in the bid.

## Questions
1. Describe the strategies you would use to find the optimal clearing price?
2. Which strategy would drive maximum users to the platform?
3. How to persuade users to bid close to market clearing price?
4. Make a prototype in solidity that can clear market price

More?: An external user having abundance of quantity is present in the market which can provide or accept any quantity from the prosumers. Try to get the optimal clearing price for this user.
### Sample Input
User: (price, quantity)
producer_1: (20, 100)
producer_2: (30, 50)
producer_3: (10, 30)
consumer_1: (5, 50)
consumer_2: (15, 80)
master_producer: (25, inf) (optional)

Idea : 
1)	Function 1: Seller (quantity and price)
2)	Function 2: Buyer (quantity and price)


