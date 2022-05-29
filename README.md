<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://raw.githubusercontent.com/pawanpaudel93/beatbox-competition-dapp/370e7722377731263e4184ea067a1a849cbbf473/public/logo.png" alt="Online Beatbox Competition"></a>
 <br />
  <a href="https://www.flaticon.com/free-icons/beat-box" title="beat box icons">Beat box icons created by surang - Flaticon</a>
</p>

<h3 align="center">Online Beatbox Competition</h3> 
<p align="center"><a href="https://beatbox-competition-dapp.vercel.app">Demo Link</a></p>

---

<p align="center"> Online Beatbox Competition is the decentralized application to create and manage beatbox competitions utilizing web3 technologies.
    <br> 
</p>

## 📝 Table of Contents

- [About](#about)
- [Usage](#usage)
- [Built Using](#built_using)
- [Authors](#authors)
- [Thanks](#thanks)

## 🧐 About <a name = "about"></a>

Online Beatbox Competition is the decentralized application to create and manage beatbox competitions utilizing web3 technologies. Many beatbox competitions are run by different organizations which are both online and offline. And there is a recent online beatbox battle called BBU(Beatbox United) organized and run by two professional beatboxers [SXIN](https://www.youtube.com/user/ANXbbx) and [Chezame](https://www.youtube.com/c/Chezame). BBU is a revolutionary competition that has increased the beatboxing bar high and has thrived to improve beatbox professionalism with its unique format. It has also good winning amounts from winning Top 16 wildcards to winning each battle. This project is inspired by the BBU competition.

The smart contract used for the project ensures that the competition contract is funded with a sufficient winning amount for the battle and it is transferred automatically to the winner after the battle is over so the winner gets what's promised immediately after the battle. Chainlink is used to build the hybrid smart contract where chainlink VRF is used to get a random number onchain to select battle opponents randomly. Also, chainlink keeper is used to check for the battle end and perform upkeep to fetch the battle youtube videos likes count as user voting using the Youtube data API External Adapter and after fetching the battle youtube videos likes the winner is selected based on the points voted by the judges for the different criteria and 1 point for the greater video likes. Moralis is used for the sign-in, for indexing the competitions events on the factory contract, storing wildcards, storing judges, updating posts, financial support, etc. Web3.storage is used to upload the wildcard or update videos which are stored in the ipfs and filecoin storage providers. Polygon blockchain is used to deploy the smart contract for the cheaper transaction costs.

## 🎈 Usage <a name="usage"></a>

1. A competition creator/organizer creates competition and starts the wildcard submission and also adds judges to judge the competition.

2. Beatboxers submit their name and wildcard Youtube video URL or upload the video itself.

3. The competition wildcard submission is ended by clicking the end wildcard submission button in the settings. And now it's the work of the judges to select the Top 16 wildcards each.

4. Creator/organizer should get the subscription for Chainlink VRF and also register chainlink keepers for the competition contract. And its information can be found on the settings tab for the creator.

5. Creator then finalizes the 16 beatbox wildcards and adds them to the contract and the contract calculates the 8 random battles for the Top 16 round.

6. Now the admin can start the battle by funding the required amount for the battle and judges can vote till the battle period which can be set by the organizer/creator.

7. The winner is then awarded the prize money when the battle is over by the contract and the creator can start the next battle.

8. This continues till the state of the competition changes from Top 16 to Top 8, Top 8 to Semifinal, Semifinal to final, and the competition is completed after the final winner is selected.

## ⛏️ Built Using <a name = "built_using"></a>

- [Moralis](https://moralis.io/) - Web3 Development tools
- [Web3.storage](https://web3.storage/) - Decentralized Data Storage
- [Polygon](https://polygon.technology) - Blockchain
- [Solidity](https://docs.soliditylang.org/) -  Smart Contract Programming
- [Chainlink](https://chain.link/)- Chainlink decentralized oracle networks
- [Nextjs](https://nextjs.org/) - Reactjs Web Development Framework
- [Chakra UI](https://chakra-ui.com/) - A simple, modular and accessible component library.
- [Hardhat](https://hardhat.org/) - Ethereum Development Environment

## ✍️ Authors <a name = "authors"></a>

- [@pawanpaudel93](https://github.com/pawanpaudel93)

See also the list of [contributors](https://github.com/pawanpaudel93/beatbox-competition/contributors) who participated in this project.

## 🎉 Thanks <a name = "thanks"></a>
- [SXIN & Chezame](https://www.youtube.com/watch?v=xMYglWGueVc) for the competition concept. 
- Matt | Block-Farms.io#7823 on Chainlink discord for helping me with Youtube External Adapter.
