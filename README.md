# SolanaFloor

## Inspiration
Got into crypto in 2017. Heard about NFT's in 2020, but didn't buy my first NFT until mid 2021. Which was a SMB NFT on Solana during the initial mint. Got really invested in the whole scene and joined the MonkeDAO discord soon after. The whole NFT scene is still so young and more so on Solana. I missed some valuable data to have better insights into NFTs on Solana, so I built SolanaFloor. I started building it early-mid September next to my day job. Most people were enthusiastic about it, so I'm slowly adding features and improving performance.

## What it does
SolanaFloor shows information about the tokens itself, the listing prices, current owners, rarities and rankings. How the distribution is and price development. The web app is pretty interactive, so visitors can sort and filter data for themselves.

Recently I launched an NFT collection with a very important utility. The NFT gives the holder access to SolanaFloor PRO. This part of the website displays more data and collections. More info here: https://solanafloor.com/pro. It's the first time an NFT is used as a key to login.

## How I built it
I made the frontend in NuxtJS (VueJS) using TypeScript. The backend is built in JavaScript. The backend uses the @solana/web3.js package to fetch on-chain data about the tokens and transactions. I also scrape several markets to find all the listings and put them into a MongoDB database. The API is built on ExpressJS.

## Challenges I ran into
I didn't know much about Solana and blockchain development. So it was a lot of trial and error to get the correct data without using too many requests. I had help from people in the community, but pretty much built everything on my own. I also spent some time on the decoding part, since there isn't much documentation on @solana/web3.js.

And as SolanaFloor gained more publicity there were more visitors. And with so much data it was difficult to have proper performance. Some pages were taking almost a minute to load or would just crash. So I migrated the whole API and DB in a couple of days from cloud db and lambda to a dedicated app + db. Load times are blazing fast now.

Working on fetching on-chain transactions now. But since there is no standard we're working on parsing listings/delistings, bids and sales for each and every market out there.

## Accomplishments that I'm proud of
Successfully querying the blockchain for the correct data and processing them into useful visualizations. The overall acceptance of the project in the community has been amazing and all the projects that want to get listed on my site. Even Anatoly talked about it: https://twitter.com/aeyakovenko/status/1446883293194903552

SolanaFloor is also the official Bonfida data analytics platform which I'm very proud of: https://bonfida.medium.com/solanafloor-now-has-an-analytics-dashboard-for-solana-name-service-9baef31d427d

Also the Shi Guardians NFT collection I've launched to get access to SolanaFloor Pro.

And obviously how SolanaFloor is used. I went from 0 to 30k page views per day and 3k unique visitors per day in just 4 weeks time. The average time visitors spend on my site is 3 min, which I think is pretty good.

## What I learned
How awesome it is to build using Solana. It's fast and cheap.

## What's next for SolanaFloor
Keep adding features and other NFT projects. Features like improved portfolio tracking, realtime data, APIs, more filter/search possibilities, add volume and transactional data. But since I'm doing this by myself in my free time, it might not go as fast as I'd like it to.

## Built With
* Express.JS
* Javascript + Typescript
* MongoDB
* NuxtJS / VueJS
* Solana
* TailwindCSS

## Links
* Website: https://solanafloor.com
* Information about PRO: Website: https://solanafloor.com/pro
* Twitter: https://twitter.com/SolanaFloor & https://twitter.com/cryptowazza
* Discord: https://discord.gg/jqr8TnqqxT
* Shi Guardians NFT: https://shi-guardians.solanafloor.com
* Official .SOL analytics: https://solanafloor.com/domains
