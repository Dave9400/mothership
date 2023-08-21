# Summary

A market for ownable, tradeable, subscription memberships.  

Space Marketplace is a tool for financially sustainable coordination. Spaces are tradeable subscription memberships for DAOs. Space Marketplace replaces NFT or token DAO memberships with dynamically priced subscriptions that give each member skin in the game for incentive to build.

Space owners who maintain a subscription balance are given the right to display their NFTs in the space as sponsors of the collective cause.

The concept is an alternative to a Harberger Tax, inspired by a post from Vitalik Buterin on ENS.

The first Space Marketplace to launch will be the Mothership. The goal of the Mothership DAO will be to develop and enhance the dApp code and to enable anyone to spawn their own Space Marketplace DAO with any coordination mission of their choosing.

DAOs are often faced with a sustainability problem.  NFT membership tokens present a one-time investment in a cause without future revenue.  New mints dilute the supply.  Members expect returns on their investment but are not incentivized to contribute.  NFT royalties can be bypassed, and their revenue is often insufficient to support the needs of a DAO.

[Should there be demand-based recurring fees on ENS domains?](https://vitalik.ca/general/2022/09/09/ens.html)

This concept builds on “alternative solution 1” from a post by Vitalik on ENS. Membership Spaces are maintained with subscription fees set at a percentage of the market value of each space.  Space owners are given the right to display their NFTs in the space and govern the use of subscription revenue.

# Subscription Fees

Space owners must defend ownership of their space by maintaining a balance in the contract above zero.  When a balance is depleted to zero, the accept offer function can be called by anyone (even the submitter of the current highest offer) Subscription fees are pulled from the balance of each space.  Fees are set to an annual percentage rate relative to the best offer on each space at any given time.

# Governance

Initially Space Marketplace is governed by the contract owner.  In the future, a marketplace can be created where 1 space = 1 vote for proposal approval to use subscription revenue.

# Claiming a Space (Mumbai Testnet)

Step 1: [Add Mumbai Test Net to MetaMask](https://medium.com/stakingbits/how-to-connect-polygon-mumbai-testnet-to-metamask-fc3487a3871f)

Step 2: [Get some Matic from the Mumbai Faucet](https://mumbaifaucet.com/)

Step 3: Wrap some of your MATIC into WMATIC using the WMATIC contract [here.](https://mumbai.polygonscan.com/address/0x9c3c9283d3e44854697cd22d3faa240cfb032889#writeContract)  Navigate to the “Contract” tab, then click on the “Write Contract” button to access the write functions of the WMATIC contract.  Use the “deposit” function to wrap an amount of WMATIC.  Wrap about half of your MATIC Balance so you will have some left to pay for gas.

Step 4: Click on the space you would like to claim and enter the amount of WMATIC you would like to use for your initial deposit.  You can enter zero, but if your balance is zero, your space will not be secure.  When a space’s balance is zero, anyone can make an offer and accept on your behalf.  First you will approve the Space Marketplace contract to use your WMATIC.  When you click approve, you should be asked to complete this transaction in MetaMask.

Step 5: Once your WMATIC is successfully approved, you should be able to make your claim. Approve the transaction in MetaMask.  Your offer should be complete and your wallet address should now show as the new owner of your space!

# Roadmap

1. Contract and dapp Enhancements
    1. Implement 12 hr offer retract delay
    2. Add support for ERC1155 NFTs
    3. Sweep subscription rate across spaces from 0.1% to 100% of best offer per week
    4. Add “staking” returns on offers (portion of subscription fees goes to the offeror)
    5. UX improvements
2. Complete Contract Audit
3. Launch to Main Net with initial claim whitelist for:
    1. Top Contributors
    2. NFT community partnerships
4. Add Treasury Governance
5. Create No-Code Forking for Sub-DAOs
6. Add dynamic supply and subscription rates for price control
7. DAO decides the destiny

# Join on Discord

https://discord.gg/HyFA5XYEE3


This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
