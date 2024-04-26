## Quick start

```bash
# in one terminal
npm run fhevm:start
# in another terminal
npm i
cp .env.example .env
./scripts/faucet.sh
npm test
```

### execute contract test by specifying the contract

The followinng is an example specifying BlindAuction.ts

```bash
# in one terminal
npm run fhevm:start
# in another terminal
npm i
cp .env.example .env
./scripts/faucet.sh
npm test test/blindAuction/BlindAuction.ts 
```

output

```bash
> fhevm@0.4.0 test
> HARDHAT_PARALLEL=1 hardhat test --parallel test/blindAuction/BlindAuction.ts

Compiled 41 Solidity files successfully (evm target: shanghai).


  BlindAuction
    ✔ should check Carol won the bid (44282ms)


  1 passing (1m)
```
