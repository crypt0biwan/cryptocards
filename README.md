## How to mint the "Lost CryptoCards"

Ok so here are the details how I could mint cards from [the original CryptoCards contract](https://etherscan.io/address/0x86a68f655018389658f657257fd6d0c337c09351).
It was just a coincidence cause I was looking at what the mint cost of my #36 cards was (minting + wrapping twice). Then I noticed these weird `Bulk Pre Buy Collectible` transactions. When looking into it it occured to me someone was minting cards?!?! Huh say wut? I thought they were all gone? A little later I discovered the ones that were minted now didn't appear in [the overview](https://misfitart.co/collection/crypto-cards). And when navigating to [a detail page](https://misfitart.co/collectible/47) there was this strange PHP error.

Anyway [this transaction](https://etherscan.io/tx/0x639ab4088b21c9886c37f90d8e65ae61f7d1f45e52f63f375a9987751482da33) did catch my attention and I wanted to know what these mysterious cards were..
So first I tried to get some information about it so I was looking at the contract to see if I could get some IPFS info or something. And bingo there they were! The artwork details are stored on IPFS. When you look [at the contract](https://etherscan.io/address/0x86a68f655018389658f657257fd6d0c337c09351#code)
you will see all the cards with their ids, supply and IPFS links:

```javascript
function initialize() internal {
    create(1, 1, "ipfs://QmWAP5TQokmAXWw7mYFapCdDa9piYZE2kVJiqP53NqoQD2");
    create(4, 50, "ipfs://Qmf3UT9mmzPZwgf3cSQDEa7ZBji8ntZskrLDBEN1gVscpp");
    create(6, 10, "ipfs://QmToz4QuznqSFkb9h4K9soKJ7aMsr9nREnFmYqLCSe3RdH");
    create(7, 100, "ipfs://QmRFtHmyQnmXJ75Zxcq9Jb6XPgFyVK9iNdJWwepYx9Eire");
    create(8, 10, "ipfs://QmcbfX6GYWTXYw9y6GEWwiuco4cXDZJTnfK88SFuXzfurk");
    create(9, 100, "ipfs://QmRWB53RU2YkRDpytq4wrDf7AVvwD65vLKQxjUeAswHU66");
    create(10, 100, "ipfs://QmTKR3GjmRqxWaw6QJph7pRnrnfYf23WSMjfAGbeDvt9bA");
    create(11, 100, "ipfs://QmVddaQPEX7kREHNq7q7yEBxWcf5WoDHKqiCb7cLvtNZrg");
    create(12, 50, "ipfs://QmbaR52MFHjN2hQi9uJGoYX8GNhtLQPPuokBPwJ4ok32W5");
    create(13, 50, "ipfs://QmTsy7cSX7UijWndeEsqZb1VKzecyKbosqYrHuEu3Apevh");
    create(14, 100, "ipfs://QmZg5DNNBV1wZ8jX5ZMXPLguBxDMQt5DUpyvwVwNiEcR7G");
    create(15, 200, "ipfs://QmUMXZTDLQcsB222MYsSSt8TncANDkamnNwhUF7pD6QLCk");
    create(16, 50, "ipfs://QmehKVW9PueWFaaaxZ2rHmVJPEKfyjGVCZMgiFYxwVJZAv");
    create(17, 100, "ipfs://QmUH2Mf5UdRfL1UeRnJmBNUX1T5L3qGSP7vD5apsu4cp9i");
    create(18, 200, "ipfs://QmULb4tuKQHXTro5N9U3jVxxNiLdoGYyippzwacExbTDkW");
    create(19, 50, "ipfs://QmYU8WttFNtNmncbxwfcrgay6y25NPNU86PDTWHth4Y7Bs");
    create(20, 50, "ipfs://QmW6vr9cmAakVQWxaojo6inFub7QgSGBfBS18fZRNNFmpX");
    create(21, 100, "ipfs://QmQ537xkrPNr9wVVF1Lh9Wbf4rZmBQQzxTpCa3tjjBwj9N");
    create(22, 200, "ipfs://QmcXtodSRshYVih4VPiHRogg4ysGEwTQEuegx4S9eqStgM");
    create(23, 200, "ipfs://QmPLVtPKBC8wAFfe1uLu11ym6wFGKERQc4bb3odjj4YhAC");
    create(24, 200, "ipfs://QmPsZyWu1GsCem4ARUGa5QhQYfT3CXNdkHhmVZCET1kFDX");
    create(25, 200, "ipfs://QmfXJtR7bCcq28vcYCqFZX8PXtbhK6nxLRqgg21E9qaMSM");
    create(26, 100, "ipfs://QmQYH2yyqRGCCtk3oK3r5WVCdJF2Ff7D9dWE7ZFZyo2kXY");
    create(27, 200, "ipfs://QmVvaffp7Do9LhEvPGkmSM5B1tEnM34YrCiQTwfDtEABck");
    create(28, 100, "ipfs://QmPB8pfwgpnbHRiUz3JwFNpvmKsnBqKhtaEqWggN2FSFdm");
    create(29, 200, "ipfs://Qmex4cmDTQecLcXnkVAGc7RHDjgQbaDcydtwmwTyGYNt1e");
    create(30, 10, "ipfs://QmcCMakqG9kBAHvFkCUUNVriiXFnEh4ibbTjd3kdZ8hqZk");
    create(31, 200, "ipfs://QmfXe9nQurA2uCQPjmCmJk4dQjLK2ifCARVnskNejMd76t");
    create(32, 10, "ipfs://QmWdbif88zqWXLfMP9riz1cBBUYuUVHS1CrgdKZtnyRiTj");
    create(33, 200, "ipfs://QmdsCLuTN9ongEDmjCurs989PwYPPQofPHjUp5UaJMisvX");
    create(34, 50, "ipfs://QmdkHQ2arBVsarLxinm4JG4tk3B1zfFTnWPminTg42GZxm");
    create(35, 200, "ipfs://QmX2vGQQLUqRMuHJMHtfPdzSAmc2RXTWen5eLHUCQxdxA6");
    create(36, 50, "ipfs://Qmdvjn9WCUKMgYcy2NHi3LSQJofLvW3mZFjdvr1N5AYcYS");
    create(37, 200, "ipfs://QmSVKpf6fyVZZ2PVJkCRnLad7BffF1Xh6zEbP5kqkYA2SK");
    create(38, 200, "ipfs://QmdQNgpNfJX59wzCHS1UfxSVMJY4YEWLkfqxbnTgA8SCuG");
    create(39, 200, "ipfs://QmRsxTm2BCofrVQ5xnWvcmdoDFkvcHpbSJ93Xvr9aDAexq");
    create(40, 100, "ipfs://QmY39vaPzVUnd2UTJx89QPJXjBMWXBh75oTvnrdfYVWkHR");
    create(41, 100, "ipfs://QmYv4o4L4k1GTS2T2iqjF9JKRXf6oD8kxN4YDGiAZFgNPF");
    create(42, 200, "ipfs://QmPhb71kNgm8Rnr9cYESPa68mRn8dWPNRm3UZgjgg94YmS");
    create(43, 200, "ipfs://QmSoEVqdf8R4LLAaDGVmu79Y5N1WzauV8tiv4D8PQARz9a");
    create(44, 100, "ipfs://Qmbj7MKjZx9vfuLThsBWZsBJffkChcFKhGXhLp2iCtU2u8");
    create(45, 100, "ipfs://QmeNUDM6avcRMZYiFqEBTDU3Fz9biypqtTiDnZV6jT7CDi");
    create(46, 100, "ipfs://QmXmo2oaQKiVx3rSB5xpHjKq9XYBo6iY2SqUfXr7aERvRy");
    create(47, 200, "ipfs://QmSm2C2sZeoNdvQcPKaaVHgrF18sA9rLZJWdzEVw43pCSK");
    create(48, 200, "ipfs://QmXh2o3o1qeXYUzzYQXUKUjuvQJuUgGKw8wRM9TKCvCqiR");
    create(49, 200, "ipfs://QmPP2hKCVRoo5X9tjZnuAoyvPrKzkjhxBrr3T5awmbBMJT");
    create(50, 200, "ipfs://QmZJa3nosLH4csDHs577BR4fPNTQ8beubsksznsyrGeLvJ");
    create(51, 200, "ipfs://QmQBhWbbZjbZ7wawBnViZgK4j6xpa7irMXsY9mDnrDLwYp");
    create(52, 200, "ipfs://QmQdXA2Mwuho4mqjn7RfvTda7BKXo9A9UiZivrZmZNMtvg");
    create(53, 200, "ipfs://QmTCeqs7og4RfJefk7UMwmB1Wm9vWoqXVBJ1LwZy44ECVm");
    create(54, 200, "ipfs://QmQQarCamg6DTbegfuTi6GmcaJxj3otS1xp5kk7meymWwX");
    create(55, 200, "ipfs://QmeZ9ZjiLRA46ygNCyzMniM4LVF5KGNNMj1zL3E8Wit6j5");
    create(56, 100, "ipfs://QmYSfQJBJzAfEUCjfijus67RAdxazY5KiLtSXYVY7BqyXR");
    create(57, 200, "ipfs://QmPAzd37Agu4xspCXUKeuerTsTHVrNHK7QN2HxT1r5uPNG");
    create(58, 200, "ipfs://QmXkrMH9B5ehk9ftfKqSWZaQ13RzeVrQ2qk5VzeUyPsN5S");
    create(61, 100, "ipfs://QmSr3hcyg6DBcncy85pN6bZfTStEQCqrc4pswAtcMJUK7B");
    create(62, 200, "ipfs://QmcBPVKpESwSNLhbQnxQv1oEBqR46jZrUNnW5cbL4Dr7LC");
    create(63, 200, "ipfs://QmZyTS3NmG97L6gP2DorGTp67Bw3GXUGMDMrQfPYd6uD2B");
    create(64, 200, "ipfs://Qmc3sGP18Gy8J7oh7MjD4Ym8eJDapv4mk1nM1nv3z2yhuv");
    create(65, 200, "ipfs://QmedZmtCg5c5h4pDZzM26kE5vQmUp5xUKEBAbGhhUhvcxH");
    create(66, 50, "ipfs://QmVpqZC1aKYNhPeJap5Dz3UdJVqf8kRXk1FpGVTE3za1ec");
    create(67, 200, "ipfs://QmZ5xPstBG7PMLqFed1xLVJJWDuwAP3Y512mSjpM4vNW9j");
    create(68, 100, "ipfs://QmXsUV7QEYxXXbgYjXdqmM8duYg1aJsf2Nr7fbbjxpQAKP");
    create(69, 10, "ipfs://QmUbrnb3zXSdc55mBLRSYBMiBpvG1MNo9YbCno2RcB3oif");
    create(70, 50, "ipfs://QmcQuf4f7QyxdArtpBNenakyy1JQFGPfMGBwbk9FBtAAcw");
    create(71, 100, "ipfs://QmSCqCzwv36cpsnkTDYqL7zSxkDfBQLyvM1ttaFcCUWszR");
}
```

So when you want to see the artwork for let's say card 47, you can look at that IPFS hash `QmSm2C2sZeoNdvQcPKaaVHgrF18sA9rLZJWdzEVw43pCSK` in this list, go to https://ipfs.io/ipfs/QmSm2C2sZeoNdvQcPKaaVHgrF18sA9rLZJWdzEVw43pCSK where you'll see this IPFS data:

```json
{
  "image": "ipfs://QmNy6UP7kJJfFcY6QUWjrUv2EPnMakmkTrJXPPjipwCWNH",
  "description": "\"Bitcoin covered on The Economist\" from CryptoCards collection",
  "attributes": [
    {
      "value": "uncommon",
      "trait_type": "Rarity"
    },
    {
      "value": "0x6de1ba9598fe3d176c95d5e246f3ed44fc5c5830aecd61dee17b529e40bc5efa",
      "trait_type": "Mint Tx"
    },
    {
      "display_type": "date",
      "trait_type": "Mint Date",
      "value": 1515990549
    },
    {
      "display_type": "number",
      "trait_type": "Total Supply",
      "value": 200
    }
  ],
  "name": "Bitcoin covered on The Economist"
}
```

There's the link to the artwork (in the `image` field). Again when navigating to that hash on IPFS you'll [see the actual card image](https://ipfs.io/ipfs/QmNy6UP7kJJfFcY6QUWjrUv2EPnMakmkTrJXPPjipwCWNH).

![https://ipfs.io/ipfs/QmNy6UP7kJJfFcY6QUWjrUv2EPnMakmkTrJXPPjipwCWNH](https://ipfs.io/ipfs/QmNy6UP7kJJfFcY6QUWjrUv2EPnMakmkTrJXPPjipwCWNH)

Holy crap, so this collection did contain some hidden gems! I had to get these!! 😃

Ok, so back to [the transaction](https://etherscan.io/tx/0x639ab4088b21c9886c37f90d8e65ae61f7d1f45e52f63f375a9987751482da33).
When you view the details of the tx you'll see they paid 0.125 ETH for 25 cards (which is 0.005 ETH per card). However, when you expand `Click to see more` and click `Decode Input Data` you'll see:

| # | Name | Type | Data |
|---|---|---|---|
| 0 | _id | uint256 | 64 |
| 1 | _printIndexes | uint256[] | 11918 |
|   |   |   | 11978 |
|   |   |   | 11805 |
|   |   |   | 11803 |
|   |   |   | 11922 |
|   |   |   | 11849 |
|   |   |   | 11959 |
|   |   |   | 11947 |
|   |   |   | 11973 |
|   |   |   | 11913 |
|   |   |   | 11825 |
|   |   |   | 11871 |
|   |   |   | 11981 |
|   |   |   | 11941 |
|   |   |   | 11921 | 
|   |   |   | 11814 |
|   |   |   | 11998 |
|   |   |   | 11885 |
|   |   |   | 11968 |
|   |   |   | 11900 |
|   |   |   | 11919 |
|   |   |   | 11997 |
|   |   |   | 11916 |
|   |   |   | 11999 |
|   |   |   | 11882 |
| 2 | initialPrintPrice | uint256 | 5000000000000000

Ok so the details of `(0)` and `(2)` were clear, but of course I didn't know how to get those "print indexes", however later I found out how to get those as well. Apparently their website was calling this API:

```bash
curl 'https://api.studio.thegraph.com/query/12837/cryptocards/v0.0.1' \
  -H 'authority: api.studio.thegraph.com' \
  -H 'pragma: no-cache' \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'accept: */*' \
  -H 'origin: https://misfitart.co' \
  -H 'sec-fetch-site: cross-site' \
  -H 'sec-fetch-mode: cors' \
  -H 'sec-fetch-dest: empty' \
  -H 'referer: https://misfitart.co/' \
  --data-raw '{"query":"\n        {\n            drawings(first: 70) {\n                drawingId\n                totalSupply\n                prints(first:200, where: {owner: \"0xb7E0c211Fb088E42aA9fd936B0A9C52985FBD273\"}){\n                        printIndex\n                }\n            }\n        }\n    "}' \
  --compressed
```

The output of that call contained some print indexes of card #47:

```json
{
  "drawingId": "47",
  "prints": [
    {
      "printIndex": "8816"
    },
    {
      "printIndex": "8839"
    },
    {
      "printIndex": "8855"
    },
    {
      "printIndex": "8864"
    },
    {
      "printIndex": "8887"
    },
    {
      "printIndex": "8897"
    },
    {
      "printIndex": "8903"
    },
    {
      "printIndex": "8914"
    },
    {
      "printIndex": "8917"
    },
    {
      "printIndex": "8924"
    },
    {
      "printIndex": "8926"
    },
    {
      "printIndex": "8931"
    },
    {
      "printIndex": "8936"
    },
    {
      "printIndex": "8941"
    },
    {
      "printIndex": "8948"
    },
    {
      "printIndex": "8965"
    },
    {
      "printIndex": "8967"
    },
    {
      "printIndex": "8972"
    },
    {
      "printIndex": "8974"
    },
    {
      "printIndex": "8978"
    },
    {
      "printIndex": "8987"
    },
    {
      "printIndex": "8988"
    },
    {
      "printIndex": "8995"
    },
    {
      "printIndex": "9000"
    }
  ],
  "totalSupply": "200"
}
```

So I copied those and made an array of those "print indexes" and when I put in all the details in the contract function `8. bulkPreBuyCollectible` like this:

| Key | Value |
|---|---|
| bulkPreBuyCollectible | 0.12 |
| _id | 47 |
| _printIndexes | 8816,8839,8855,8864,8887,8897,8903,8914,8917,8924,8926,8931,8936,8941,8948,8965,8967,8972,8974,8978,8987,8988,8995,9000 |
| initialPrintPrice | 5000000000000000 |

it resulted in [this transaction](https://etherscan.io/tx/0xf8738ec68f2417a025a4aed7c676fdc837b194625de6b6684737305c67d3c129). It costed me `0.53 ETH` in gas fee but hey, I got some cards!!

So I repeated this process for card #64 (shame I missed #52 haha!).
Hope you guys learned something from this and let's see what the devs want to do with the rest they minted.

Cheers, Obi

Here are all the links to IPFS for all cards:

| Card ID | Supply | IPFS link |
|---|---|---|
| 1 | 1 | [ipfs://QmWAP5TQokmAXWw7mYFapCdDa9piYZE2kVJiqP53NqoQD2](https://ipfs.io/ipfs/QmWAP5TQokmAXWw7mYFapCdDa9piYZE2kVJiqP53NqoQD2)
| 4 | 50 | [ipfs://Qmf3UT9mmzPZwgf3cSQDEa7ZBji8ntZskrLDBEN1gVscpp](https://ipfs.io/ipfs/Qmf3UT9mmzPZwgf3cSQDEa7ZBji8ntZskrLDBEN1gVscpp)
| 6 | 10 | [ipfs://QmToz4QuznqSFkb9h4K9soKJ7aMsr9nREnFmYqLCSe3RdH](https://ipfs.io/ipfs/QmToz4QuznqSFkb9h4K9soKJ7aMsr9nREnFmYqLCSe3RdH)
| 7 | 100 | [ipfs://QmRFtHmyQnmXJ75Zxcq9Jb6XPgFyVK9iNdJWwepYx9Eire](https://ipfs.io/ipfs/QmRFtHmyQnmXJ75Zxcq9Jb6XPgFyVK9iNdJWwepYx9Eire)
| 8 | 10 | [ipfs://QmcbfX6GYWTXYw9y6GEWwiuco4cXDZJTnfK88SFuXzfurk](https://ipfs.io/ipfs/QmcbfX6GYWTXYw9y6GEWwiuco4cXDZJTnfK88SFuXzfurk)
| 9 | 100 | [ipfs://QmRWB53RU2YkRDpytq4wrDf7AVvwD65vLKQxjUeAswHU66](https://ipfs.io/ipfs/QmRWB53RU2YkRDpytq4wrDf7AVvwD65vLKQxjUeAswHU66)
| 10 | 100 | [ipfs://QmTKR3GjmRqxWaw6QJph7pRnrnfYf23WSMjfAGbeDvt9bA](https://ipfs.io/ipfs/QmTKR3GjmRqxWaw6QJph7pRnrnfYf23WSMjfAGbeDvt9bA)
| 11 | 100 | [ipfs://QmVddaQPEX7kREHNq7q7yEBxWcf5WoDHKqiCb7cLvtNZrg](https://ipfs.io/ipfs/QmVddaQPEX7kREHNq7q7yEBxWcf5WoDHKqiCb7cLvtNZrg)
| 12 | 50 | [ipfs://QmbaR52MFHjN2hQi9uJGoYX8GNhtLQPPuokBPwJ4ok32W5](https://ipfs.io/ipfs/QmbaR52MFHjN2hQi9uJGoYX8GNhtLQPPuokBPwJ4ok32W5)
| 13 | 50 | [ipfs://QmTsy7cSX7UijWndeEsqZb1VKzecyKbosqYrHuEu3Apevh](https://ipfs.io/ipfs/QmTsy7cSX7UijWndeEsqZb1VKzecyKbosqYrHuEu3Apevh)
| 14 | 100 | [ipfs://QmZg5DNNBV1wZ8jX5ZMXPLguBxDMQt5DUpyvwVwNiEcR7G](https://ipfs.io/ipfs/QmZg5DNNBV1wZ8jX5ZMXPLguBxDMQt5DUpyvwVwNiEcR7G)
| 15 | 200 | [ipfs://QmUMXZTDLQcsB222MYsSSt8TncANDkamnNwhUF7pD6QLCk](https://ipfs.io/ipfs/QmUMXZTDLQcsB222MYsSSt8TncANDkamnNwhUF7pD6QLCk)
| 16 | 50 | [ipfs://QmehKVW9PueWFaaaxZ2rHmVJPEKfyjGVCZMgiFYxwVJZAv](https://ipfs.io/ipfs/QmehKVW9PueWFaaaxZ2rHmVJPEKfyjGVCZMgiFYxwVJZAv)
| 17 | 100 | [ipfs://QmUH2Mf5UdRfL1UeRnJmBNUX1T5L3qGSP7vD5apsu4cp9i](https://ipfs.io/ipfs/QmUH2Mf5UdRfL1UeRnJmBNUX1T5L3qGSP7vD5apsu4cp9i)
| 18 | 200 | [ipfs://QmULb4tuKQHXTro5N9U3jVxxNiLdoGYyippzwacExbTDkW](https://ipfs.io/ipfs/QmULb4tuKQHXTro5N9U3jVxxNiLdoGYyippzwacExbTDkW)
| 19 | 50 | [ipfs://QmYU8WttFNtNmncbxwfcrgay6y25NPNU86PDTWHth4Y7Bs](https://ipfs.io/ipfs/QmYU8WttFNtNmncbxwfcrgay6y25NPNU86PDTWHth4Y7Bs)
| 20 | 50 | [ipfs://QmW6vr9cmAakVQWxaojo6inFub7QgSGBfBS18fZRNNFmpX](https://ipfs.io/ipfs/QmW6vr9cmAakVQWxaojo6inFub7QgSGBfBS18fZRNNFmpX)
| 21 | 100 | [ipfs://QmQ537xkrPNr9wVVF1Lh9Wbf4rZmBQQzxTpCa3tjjBwj9N](https://ipfs.io/ipfs/QmQ537xkrPNr9wVVF1Lh9Wbf4rZmBQQzxTpCa3tjjBwj9N)
| 22 | 200 | [ipfs://QmcXtodSRshYVih4VPiHRogg4ysGEwTQEuegx4S9eqStgM](https://ipfs.io/ipfs/QmcXtodSRshYVih4VPiHRogg4ysGEwTQEuegx4S9eqStgM)
| 23 | 200 | [ipfs://QmPLVtPKBC8wAFfe1uLu11ym6wFGKERQc4bb3odjj4YhAC](https://ipfs.io/ipfs/QmPLVtPKBC8wAFfe1uLu11ym6wFGKERQc4bb3odjj4YhAC)
| 24 | 200 | [ipfs://QmPsZyWu1GsCem4ARUGa5QhQYfT3CXNdkHhmVZCET1kFDX](https://ipfs.io/ipfs/QmPsZyWu1GsCem4ARUGa5QhQYfT3CXNdkHhmVZCET1kFDX)
| 25 | 200 | [ipfs://QmfXJtR7bCcq28vcYCqFZX8PXtbhK6nxLRqgg21E9qaMSM](https://ipfs.io/ipfs/QmfXJtR7bCcq28vcYCqFZX8PXtbhK6nxLRqgg21E9qaMSM)
| 26 | 100 | [ipfs://QmQYH2yyqRGCCtk3oK3r5WVCdJF2Ff7D9dWE7ZFZyo2kXY](https://ipfs.io/ipfs/QmQYH2yyqRGCCtk3oK3r5WVCdJF2Ff7D9dWE7ZFZyo2kXY)
| 27 | 200 | [ipfs://QmVvaffp7Do9LhEvPGkmSM5B1tEnM34YrCiQTwfDtEABck](https://ipfs.io/ipfs/QmVvaffp7Do9LhEvPGkmSM5B1tEnM34YrCiQTwfDtEABck)
| 28 | 100 | [ipfs://QmPB8pfwgpnbHRiUz3JwFNpvmKsnBqKhtaEqWggN2FSFdm](https://ipfs.io/ipfs/QmPB8pfwgpnbHRiUz3JwFNpvmKsnBqKhtaEqWggN2FSFdm)
| 29 | 200 | [ipfs://Qmex4cmDTQecLcXnkVAGc7RHDjgQbaDcydtwmwTyGYNt1e](https://ipfs.io/ipfs/Qmex4cmDTQecLcXnkVAGc7RHDjgQbaDcydtwmwTyGYNt1e)
| 30 | 10 | [ipfs://QmcCMakqG9kBAHvFkCUUNVriiXFnEh4ibbTjd3kdZ8hqZk](https://ipfs.io/ipfs/QmcCMakqG9kBAHvFkCUUNVriiXFnEh4ibbTjd3kdZ8hqZk)
| 31 | 200 | [ipfs://QmfXe9nQurA2uCQPjmCmJk4dQjLK2ifCARVnskNejMd76t](https://ipfs.io/ipfs/QmfXe9nQurA2uCQPjmCmJk4dQjLK2ifCARVnskNejMd76t)
| 32 | 10 | [ipfs://QmWdbif88zqWXLfMP9riz1cBBUYuUVHS1CrgdKZtnyRiTj](https://ipfs.io/ipfs/QmWdbif88zqWXLfMP9riz1cBBUYuUVHS1CrgdKZtnyRiTj)
| 33 | 200 | [ipfs://QmdsCLuTN9ongEDmjCurs989PwYPPQofPHjUp5UaJMisvX](https://ipfs.io/ipfs/QmdsCLuTN9ongEDmjCurs989PwYPPQofPHjUp5UaJMisvX)
| 34 | 50 | [ipfs://QmdkHQ2arBVsarLxinm4JG4tk3B1zfFTnWPminTg42GZxm](https://ipfs.io/ipfs/QmdkHQ2arBVsarLxinm4JG4tk3B1zfFTnWPminTg42GZxm)
| 35 | 200 | [ipfs://QmX2vGQQLUqRMuHJMHtfPdzSAmc2RXTWen5eLHUCQxdxA6](https://ipfs.io/ipfs/QmX2vGQQLUqRMuHJMHtfPdzSAmc2RXTWen5eLHUCQxdxA6)
| 36 | 50 | [ipfs://Qmdvjn9WCUKMgYcy2NHi3LSQJofLvW3mZFjdvr1N5AYcYS](https://ipfs.io/ipfs/Qmdvjn9WCUKMgYcy2NHi3LSQJofLvW3mZFjdvr1N5AYcYS)
| 37 | 200 | [ipfs://QmSVKpf6fyVZZ2PVJkCRnLad7BffF1Xh6zEbP5kqkYA2SK](https://ipfs.io/ipfs/QmSVKpf6fyVZZ2PVJkCRnLad7BffF1Xh6zEbP5kqkYA2SK)
| 38 | 200 | [ipfs://QmdQNgpNfJX59wzCHS1UfxSVMJY4YEWLkfqxbnTgA8SCuG](https://ipfs.io/ipfs/QmdQNgpNfJX59wzCHS1UfxSVMJY4YEWLkfqxbnTgA8SCuG)
| 39 | 200 | [ipfs://QmRsxTm2BCofrVQ5xnWvcmdoDFkvcHpbSJ93Xvr9aDAexq](https://ipfs.io/ipfs/QmRsxTm2BCofrVQ5xnWvcmdoDFkvcHpbSJ93Xvr9aDAexq)
| 40 | 100 | [ipfs://QmY39vaPzVUnd2UTJx89QPJXjBMWXBh75oTvnrdfYVWkHR](https://ipfs.io/ipfs/QmY39vaPzVUnd2UTJx89QPJXjBMWXBh75oTvnrdfYVWkHR)
| 41 | 100 | [ipfs://QmYv4o4L4k1GTS2T2iqjF9JKRXf6oD8kxN4YDGiAZFgNPF](https://ipfs.io/ipfs/QmYv4o4L4k1GTS2T2iqjF9JKRXf6oD8kxN4YDGiAZFgNPF)
| 42 | 200 | [ipfs://QmPhb71kNgm8Rnr9cYESPa68mRn8dWPNRm3UZgjgg94YmS](https://ipfs.io/ipfs/QmPhb71kNgm8Rnr9cYESPa68mRn8dWPNRm3UZgjgg94YmS)
| 43 | 200 | [ipfs://QmSoEVqdf8R4LLAaDGVmu79Y5N1WzauV8tiv4D8PQARz9a](https://ipfs.io/ipfs/QmSoEVqdf8R4LLAaDGVmu79Y5N1WzauV8tiv4D8PQARz9a)
| 44 | 100 | [ipfs://Qmbj7MKjZx9vfuLThsBWZsBJffkChcFKhGXhLp2iCtU2u8](https://ipfs.io/ipfs/Qmbj7MKjZx9vfuLThsBWZsBJffkChcFKhGXhLp2iCtU2u8)
| 45 | 100 | [ipfs://QmeNUDM6avcRMZYiFqEBTDU3Fz9biypqtTiDnZV6jT7CDi](https://ipfs.io/ipfs/QmeNUDM6avcRMZYiFqEBTDU3Fz9biypqtTiDnZV6jT7CDi)
| 46 | 100 | [ipfs://QmXmo2oaQKiVx3rSB5xpHjKq9XYBo6iY2SqUfXr7aERvRy](https://ipfs.io/ipfs/QmXmo2oaQKiVx3rSB5xpHjKq9XYBo6iY2SqUfXr7aERvRy)
| 47 | 200 | [ipfs://QmSm2C2sZeoNdvQcPKaaVHgrF18sA9rLZJWdzEVw43pCSK](https://ipfs.io/ipfs/QmSm2C2sZeoNdvQcPKaaVHgrF18sA9rLZJWdzEVw43pCSK)
| 48 | 200 | [ipfs://QmXh2o3o1qeXYUzzYQXUKUjuvQJuUgGKw8wRM9TKCvCqiR](https://ipfs.io/ipfs/QmXh2o3o1qeXYUzzYQXUKUjuvQJuUgGKw8wRM9TKCvCqiR)
| 49 | 200 | [ipfs://QmPP2hKCVRoo5X9tjZnuAoyvPrKzkjhxBrr3T5awmbBMJT](https://ipfs.io/ipfs/QmPP2hKCVRoo5X9tjZnuAoyvPrKzkjhxBrr3T5awmbBMJT)
| 50 | 200 | [ipfs://QmZJa3nosLH4csDHs577BR4fPNTQ8beubsksznsyrGeLvJ](https://ipfs.io/ipfs/QmZJa3nosLH4csDHs577BR4fPNTQ8beubsksznsyrGeLvJ)
| 51 | 200 | [ipfs://QmQBhWbbZjbZ7wawBnViZgK4j6xpa7irMXsY9mDnrDLwYp](https://ipfs.io/ipfs/QmQBhWbbZjbZ7wawBnViZgK4j6xpa7irMXsY9mDnrDLwYp)
| 52 | 200 | [ipfs://QmQdXA2Mwuho4mqjn7RfvTda7BKXo9A9UiZivrZmZNMtvg](https://ipfs.io/ipfs/QmQdXA2Mwuho4mqjn7RfvTda7BKXo9A9UiZivrZmZNMtvg)
| 53 | 200 | [ipfs://QmTCeqs7og4RfJefk7UMwmB1Wm9vWoqXVBJ1LwZy44ECVm](https://ipfs.io/ipfs/QmTCeqs7og4RfJefk7UMwmB1Wm9vWoqXVBJ1LwZy44ECVm)
| 54 | 200 | [ipfs://QmQQarCamg6DTbegfuTi6GmcaJxj3otS1xp5kk7meymWwX](https://ipfs.io/ipfs/QmQQarCamg6DTbegfuTi6GmcaJxj3otS1xp5kk7meymWwX)
| 55 | 200 | [ipfs://QmeZ9ZjiLRA46ygNCyzMniM4LVF5KGNNMj1zL3E8Wit6j5](https://ipfs.io/ipfs/QmeZ9ZjiLRA46ygNCyzMniM4LVF5KGNNMj1zL3E8Wit6j5)
| 56 | 100 | [ipfs://QmYSfQJBJzAfEUCjfijus67RAdxazY5KiLtSXYVY7BqyXR](https://ipfs.io/ipfs/QmYSfQJBJzAfEUCjfijus67RAdxazY5KiLtSXYVY7BqyXR)
| 57 | 200 | [ipfs://QmPAzd37Agu4xspCXUKeuerTsTHVrNHK7QN2HxT1r5uPNG](https://ipfs.io/ipfs/QmPAzd37Agu4xspCXUKeuerTsTHVrNHK7QN2HxT1r5uPNG)
| 58 | 200 | [ipfs://QmXkrMH9B5ehk9ftfKqSWZaQ13RzeVrQ2qk5VzeUyPsN5S](https://ipfs.io/ipfs/QmXkrMH9B5ehk9ftfKqSWZaQ13RzeVrQ2qk5VzeUyPsN5S)
| 61 | 100 | [ipfs://QmSr3hcyg6DBcncy85pN6bZfTStEQCqrc4pswAtcMJUK7B](https://ipfs.io/ipfs/QmSr3hcyg6DBcncy85pN6bZfTStEQCqrc4pswAtcMJUK7B)
| 62 | 200 | [ipfs://QmcBPVKpESwSNLhbQnxQv1oEBqR46jZrUNnW5cbL4Dr7LC](https://ipfs.io/ipfs/QmcBPVKpESwSNLhbQnxQv1oEBqR46jZrUNnW5cbL4Dr7LC)
| 63 | 200 | [ipfs://QmZyTS3NmG97L6gP2DorGTp67Bw3GXUGMDMrQfPYd6uD2B](https://ipfs.io/ipfs/QmZyTS3NmG97L6gP2DorGTp67Bw3GXUGMDMrQfPYd6uD2B)
| 64 | 200 | [ipfs://Qmc3sGP18Gy8J7oh7MjD4Ym8eJDapv4mk1nM1nv3z2yhuv](https://ipfs.io/ipfs/Qmc3sGP18Gy8J7oh7MjD4Ym8eJDapv4mk1nM1nv3z2yhuv)
| 65 | 200 | [ipfs://QmedZmtCg5c5h4pDZzM26kE5vQmUp5xUKEBAbGhhUhvcxH](https://ipfs.io/ipfs/QmedZmtCg5c5h4pDZzM26kE5vQmUp5xUKEBAbGhhUhvcxH)
| 66 | 50 | [ipfs://QmVpqZC1aKYNhPeJap5Dz3UdJVqf8kRXk1FpGVTE3za1ec](https://ipfs.io/ipfs/QmVpqZC1aKYNhPeJap5Dz3UdJVqf8kRXk1FpGVTE3za1ec)
| 67 | 200 | [ipfs://QmZ5xPstBG7PMLqFed1xLVJJWDuwAP3Y512mSjpM4vNW9j](https://ipfs.io/ipfs/QmZ5xPstBG7PMLqFed1xLVJJWDuwAP3Y512mSjpM4vNW9j)
| 68 | 100 | [ipfs://QmXsUV7QEYxXXbgYjXdqmM8duYg1aJsf2Nr7fbbjxpQAKP](https://ipfs.io/ipfs/QmXsUV7QEYxXXbgYjXdqmM8duYg1aJsf2Nr7fbbjxpQAKP)
| 69 | 10 | [ipfs://QmUbrnb3zXSdc55mBLRSYBMiBpvG1MNo9YbCno2RcB3oif](https://ipfs.io/ipfs/QmUbrnb3zXSdc55mBLRSYBMiBpvG1MNo9YbCno2RcB3oif)
| 70 | 50 | [ipfs://QmcQuf4f7QyxdArtpBNenakyy1JQFGPfMGBwbk9FBtAAcw](https://ipfs.io/ipfs/QmcQuf4f7QyxdArtpBNenakyy1JQFGPfMGBwbk9FBtAAcw)
| 71 | 100 | [ipfs://QmSCqCzwv36cpsnkTDYqL7zSxkDfBQLyvM1ttaFcCUWszR](https://ipfs.io/ipfs/QmSCqCzwv36cpsnkTDYqL7zSxkDfBQLyvM1ttaFcCUWszR)
