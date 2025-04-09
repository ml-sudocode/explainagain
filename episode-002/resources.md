# Episode 002: Bybit $1.5bn hack (Feb 2025) - compromised Safe service
_Published 2025-02-08_

This is a four-part podcast covering the Bybit attack, the highly sophisticated and targeted $1.5bn hack of the Bybit exchange that saw Bybit's multisig signers sign a transaction that they did not intend. 

There have been many analyses since the hack happened in late February, of varying degrees of technicality. My contribution is somewhere in between - if you are more than a casual user, and less than a very technical user. 

Because I believe seeing is believing, we will use diagrams to clarify what exactly happened, step through demos on-screen, and click around websites together.

Stay safe!

## 🍿 Media links
- Watch on Youtube: 
    - [Introduction](https://youtu.be/-JKdMh7wJpg)
    - Part 1: [The Web2 Attack Path](https://www.youtube.com/watch?v=DFFrS8G2fFQ)
    - Part 2: [The Web3 Attack Path](https://www.youtube.com/watch?v=bPqYfda17AY)
    - Part 3: [Trusting the Hardware Wallets](https://www.youtube.com/watch?v=zi4MjfTW7GE)
    - Part 4: Tool Demos – Verifying Safe Transactions [coming soon]
    - Episode [playlist](https://www.youtube.com/watch?v=-JKdMh7wJpg&list=PLO4ZHeFtyCBw_ztatKUZRXnzS4v0UKNTP) 
- Read on [X.com](https://x.com/ml_sudo/status/1909929255309590601)
- [Diagrams](https://www.canva.com/design/DAGkCxdZS_U/AhRbLcPvzf14u5axxayd_Q/) of attack paths

## 🧑‍💼 Guests: Aaron and Guest X
- Aaron is a security expert and a hardware engineer.<br>
- Guest X is a long-time protocol engineer in the Ethereum ecosystem.<br>
- Both have chosen to remain anonymous :)

## 📚 References

### 📌 Official Reports

| Description | Link |
|---|---|
| Commissioned by Bybit           | [Post by Bybit Ben](https://x.com/benbybit/status/1894768736084885929)       |
| Commissioned by Safe            | [Post by Safe](https://x.com/safe/status/1897663514975649938)           |

### 📰 Media Reports

| Description | Link |
|---|---|
| Good explanation with code examples                           | [a16z: Bybit Hack Lessons](https://a16zcrypto.com/posts/article/bybit-hack-lessons/) |
| High level explanation | [Halborn](https://www.halborn.com/blog/post/explained-the-bybit-hack-revisited) |
| Analysis on what could have helped                      | [Trail of Bits](https://blog.trailofbits.com/2025/02/25/how-threat-modeling-could-have-prevented-the-1.5b-bybit-hack/) |
| Explanation of what went wrong and a checker tool             | [PatrickAlphaC on X](https://x.com/patrickalphac/status/1894786906325451241?t=sHuCYkWj6w1PiDEtbYu3Kg) |
| Safe frontend turned offline while fixes were made            | [Hsuan Ting Chu on X](https://x.com/hsuantingchu/status/1894063938678968553) |
| PCA illustrates where delegateCall was triggered              | [PCaversaccio on X](https://x.com/pcaversaccio/status/1897358972614590764) |
| Early analysis by SlowMist                                    | [SlowMist Medium](https://slowmist.medium.com/slowmist-hacker-techniques-and-questions-behind-bybits-nearly-1-5-billion-theft-09f0b59da2e2) |

---

### 🛡️ How to Check the Safe UI (by Safe)

| Description                       | Link                                                                 |
|-----------------------------------|----------------------------------------------------------------------|
| Check against software wallet     | [Safe Help: software check](https://help.safe.global/en/articles/276343-how-to-perform-basic-transactions-checks-on-safe-wallet) |
| Check against hardware wallet     | [Safe Help: hardware check](https://help.safe.global/en/articles/276344-how-to-verify-safe-wallet-transactions-on-a-hardware-wallet) |

---

### 🔐 How to Generate Hashes Yourself

| Description                                           | Link                                                                 |
|-------------------------------------------------------|----------------------------------------------------------------------|
| Pascal's tx hash checker tool, forked by several teams (pcaversaccio)          | [GitHub repo](https://github.com/pcaversaccio/safe-tx-hashes-util)       |
| OpenZeppelin’s fork, with UI (we demo this!)                                   | [safeutils.openzeppelin.com](https://safeutils.openzeppelin.com) <br> [GitHub repo](https://github.com/OpenZeppelin/safe-utils) <br> [X post](https://x.com/OpenZeppelin/status/1894870509608935791) |
| Patrick Collins / Cyfrin fork  | [GitHub repo](https://github.com/Cyfrin/safe-tx-hashes) <br> [Video walkthrough](https://www.youtube.com/watch?v=7lP_0h-PPvY)                 |           |
| Morpho Labs’ fork                                     | [GitHub](https://github.com/morpho-labs/safer) <br> [X post](https://x.com/PaulFrambot/status/1893664458351763736)      |

---

### 📦 How to Decode Hex Calldata

| Description                     | Link                                                                 |
|---------------------------------|----------------------------------------------------------------------|
| Decoder by rimeissner           | [rimeissner.dev](https://rimeissner.dev/transaction-decoder/#/)     |
| Decoder by Etherscan            | [etherscan.io](https://etherscan.io/inputdatadecoder)               |

---

### 🧪 How to Simulate Transactions

| Description     | Link                                               |
|-----------------|----------------------------------------------------|
| Tenderly        | [tenderly.co](https://tenderly.co/transaction-simulator) |

---

### 🛠️ Other Tools

| Description                        | Link                                                                 |
|------------------------------------|----------------------------------------------------------------------|
| Cast (Foundry by Paradigm.xyz)     | [GitHub](https://github.com/foundry-rs/foundry)                      |
| ETH Unit Converter (wei, gwei)     | [eth-converter.com](https://eth-converter.com/)                      |

---
<br>

><br>🤯 _**So many tools, too much confusion!** <br><br>
Different tools check different parts of the signing flow, on different devices — it quickly gets overwhelming 😶‍🌫️
<br><br> I made a template spreadsheet to bring order to the chaos:_ <br><br> ✨ [Tx Checker Spreadsheet](https://docs.google.com/spreadsheets/d/1s89QgXolg7pRJqtrhzmtIxZoHTmv-NiGRlJkNT4eN4Y/)✨ <br><br> [![Tx Checker Spreadsheet](https://github.com/user-attachments/assets/afc2067b-0aae-40cb-beab-f5f353fc90d6)](https://docs.google.com/spreadsheets/d/1s89QgXolg7pRJqtrhzmtIxZoHTmv-NiGRlJkNT4eN4Y/) <br><br>


### 🌐 Alternative Front Ends (if you don't trust Safe UI)

| Description                                                   | Link                                                                 |
|---------------------------------------------------------------|----------------------------------------------------------------------|
| Earthfast team frontend                                       | [eternalsafe.earthfast.app](https://eternalsafe.earthfast.app/)     |
| Palmera frontend (Safe-recommended)                           | [Palmera](https://app.palmeradao.xyz/welcome)                        |
|                                                               | [X post](https://x.com/safe/status/1893012725602885911)             |
| OP Labs frontend (QR-based tx check)                          | [op-txverify](https://op-txverify.optimism.io/)                      |
| CLI tool by Safe (requires manual signature sharing)                   | [Safe Docs](https://docs.safe.global/advanced/cli-overview) <br> [X post](https://x.com/safe/status/1893012725602885911)             |

---

### 🧩 Safe's Post-Hack Upgrades

| Description | Link |
|---|---|
| Safe frontend fixes                                       | [Koeppelmann on X](https://x.com/koeppelmann/status/1896544134149841273) |
| Added OpenZepplin’s Safe Utils to signing flow | [Rahul Rumalla on X](https://x.com/rahulrumalla/status/1895581669274657043) |
| Proposed new “Receipt” screen                             | [Safe on X](https://x.com/safe/status/1899461861700993497?t=sHuCYkWj6w1PiDEtbYu3Kg) |

---

### 💡 Other Recommended Resources
| Description | Link |
|---|---|
| Patrick Collins / Cyfrin: Hardware wallet display review                | [X post](https://x.com/PatrickAlphaC/status/1904075663318847785)     |
| Patrick Collins / Cyfrin: What to check on a hardware wallet (101)     | [YouTube](https://www.youtube.com/watch?v=X-HVI9dFv94&t=282s)        |


## 🧠 Topics Covered

🧩 Part 1: The Web2 Attack Path
- 🛡️ Interview with a security expert on the Web2 entry point of the exploit
- ✍️ How Bybit signers were tricked into signing malicious transactions
-	😓 A reflection on security fatigue and how even trained teams slip up

🔗 Part 2: The Web3 Attack Path
-	🧠 Interview with a protocol expert to break down the Safe smart wallet architecture
-	⚙️ Walkthrough of the transaction lifecycle, showing where vulnerabilities can occur
-	🔐 Why your hardware wallet should be your ultimate source of truth

🎁 Part 3: Trusting the Hardware
-	🧑‍🔧 Why hardware wallets are the most trusted part of transaction signing today
-	🪛 Keywords:
    -	Secure element
    -	Secure boot
    -	Root of trust
-	🌐 Firmware authentication by Ledger, Trezor, and Keystone (we check out their websites)

🛠️ Part 4: Tool Demos – Verifying Safe Transactions
-	🧪 Demo of tools to verify Safe transaction hashes
-	🧰 We use OpenZeppelin's version of Pascal’s hash checker tool
-	🛠️ Cast from Foundry to generate calldata
-	🧱 Wallet stack: Rabby extension + Keystone hardware wallet

## 💡 Requests & Suggestions (to service providers) 🙇
- Safe
    - Clarify your use of "transaction" during the signing flow. Industry convention afaik is to define "transaction" as an onchain action, rather than an offline signature (which is generally what we do when we interact with a Safe wallet). The software and hardware wallets I demo'd use  the term "message/signature request." It can be confusing for users to see both terms in one signing flow
    - Instead of just linking to a Tenderly simulation during the signing flow, also link to a page in the docs that explains how to check the data on the Safe UI against what we see in Tenderly. For example, the "nonce" value in the Safe UI is different than those in Tenderly, because the first represents the nonce for the Safe account, while the second represents the nonce for the EOA that is signing
    - Next to the calldata it might be good to link to a calldata decoder... like the one your cofounder made ;)
- Tenderly
    - Per the suggestion to Safe, on the simulation UI, perhaps insert a tooltip and/or link to where users can learn about how to check. The UX currently prevents anyone but highly technical people from having any confidence about what they are signing, which is good if we want to keep people out, but bad if we crypto to scale
- OpenZeppelin
    - It was not straightforward to figure out where/how to generate calldata on your safeutils UI, meaning the tool is only obviously usable for ETH transfers, unless you were already highly technical. Maybe add a link to a How To page? 
- Hardware wallets
    - Invent an easy way to export what users see on the device, onto a computer. Currently hardware wallet checking contributes significantly to security fatigue and its related risks. (Users are also more vulnerable to [address poisoning attacks](https://cointelegraph.com/news/address-poisoning-attacks-in-crypto), where they accidentally copy an address that looks very much like their intended address times. When you are just eyeballing a few numbers between two devices, it's easier to make a mistake)
    - Provide the SafeTxHash, and if possible the Message and Domain hashes. The SafeTxHash is the most succinct and comprehensive data point to check, since it encapsulates all the details of the transaction that a user intends. In [Patrick Collin](https://github.com/PatrickAlphaC)'s [review of hardware wallets](https://x.com/PatrickAlphaC/status/1904075663318847785), none of the wallets he tested show the SafeTxHash, and Ledger is the only one that provide the Message and Domain hashes 
        - Update: Keystone was So Quick to respond with [an update](https://x.com/KeystoneWallet/status/1907457995497496952) to show all three hashes! 
- Keystone hardware wallet
    - The contents of the message are all jumbled up. Gas-related fields are sprinkled all over, in between calldata, nonce, etc. It would be nice if the gas fields were grouped together, like in all other UIs i've seen, so that users can easily visually scan for them being all 0s (which is the default), and focus their energy on the non-zero fields
