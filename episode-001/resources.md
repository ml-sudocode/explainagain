# Episode 001: Session chat app - a decentralized version of Signal
_Published 2025-02-03_

Taylor Hornby and I dissect the most interesting bits in the Session white paper. We talk about forward secrecy, dig into their Tor-based design, and compare Session to Signal.

## 🍿 Media links
- Watch on [Youtube](https://www.youtube.com/watch?v=bgIitv3Dmkk)
- Read on [X.com](https://x.com/explainagain/status/1886348017680482638)

## 🧑‍💼 Guest: Taylor Hornby
- Github: [@defuse](https://github.com/defuse)
- X.com: [@DefuseSec](https://x.com/DefuseSec)

## 📚 References
- [Session website](https://getsession.org/)
- [Session whitepaper](https://arxiv.org/pdf/2002.04609)

## 🧠 Topics Covered

#### 🔍 Metadata Leakage: More Dangerous Than You Think
Even if message content is encrypted, knowing who is talking to whom, when, and how often can expose activists, dissidents, and high-value targets.
Session mitigates this by removing centralized servers from the equation and using onion routing—but with some key differences from Tor.

#### 🏗 “Like Tor, But Double Tor”
Instead of a single onion route from sender to recipient, Session uses two separate onion circuits—one for sending and another for retrieving messages.
This prevents a single node from learning both ends of the conversation.

#### ⏳ Messages Expire if Not Received
Unlike traditional messaging apps, messages in Session are not stored indefinitely.
If a recipient doesn’t retrieve a message in time, it’s permanently lost—an interesting trade-off between privacy and usability.

#### 💰 The Tokenomics of Attacks
Running a node requires staking tokens, creating a financial cost for Sybil attacks.
But could attackers drive up token prices, making it prohibitively expensive for honest users to participate? The economic incentives remain an open question.

#### 🧅 How Many Layers Should an Onion Have?
More hops in an onion route don’t always mean better security—timing correlation attacks can still deanonymize users.
Session sticks with the classic three-hop model, striking a balance between privacy and efficiency.

#### 🔑 Forward Secrecy: A Notable Weakness
Unlike Signal, Session does not support forward secrecy—meaning if your key is compromised, past messages could be decrypted.
However, this is mitigated by ephemeral message storage (messages don’t persist forever).

#### 🔗 Groups Over 100 Members? You’re On Your Own
Unlike Signal, large groups in Session require self-hosting—a departure from traditional privacy-focused messaging apps.
This forces users to take control of their own infrastructure but also raises questions about usability.

#### 🏛 Session Name Service (SNS): A Double-Edged Sword
Human-readable account names are convenient, but they tie your pseudonymous identity to a recognizable handle, potentially weakening privacy. Should you use one? It depends on your threat model.
