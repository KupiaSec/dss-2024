# Solving State Bloat with State Archival: Risks and Mitigations

*Upload Date: 20250121*

*Source: [https://www.youtube.com/watch?v=nhXn6mZ1NW4](https://www.youtube.com/watch?v=nhXn6mZ1NW4)*

# Solving State Bloat with State Archival: Risks and Mitigations | Garand Tyson (Stellar)

This video, presented by Garand Tyson from Stellar, discusses the novel state archival protocol being developed for the Stellar network to address the issue of state bloat.

## 1. Main Points

* **State bloat** is a significant issue for public blockchains, especially older ones. As these blockchains accumulate transactions, the size of the necessary ledger grows, impacting performance and efficiency.
* **State archival** allows the network to remove "expired data" from validators' local databases.
* The protocol uses Merkle tries and time-to-live (TTL) values to dynamically manage archival.
* The key aspects of the protocol include mechanisms for validating the removal and restoration of state, along with addressing double-spending and other potential attacks.
* Stellar's approach to archival prioritizes safety over liveness, meaning that the validity of the data is prioritized more than the speed of transaction processing.
* Mitigation strategies against potential attacks, such as double-spend attacks, are described.
* There are multiple attack factors described and discussed in relation to archival state that can be prevented with the protocol described including double-restore attacks, and malicious archival.  This involves requirements for proof of non-existence when necessary.
* The protocol leverages optimized Bloom filters for efficient state archival.
* Off-chain storage of historical state is used, further reducing on-chain size and computational overhead.

## 2. Key Insights

* **The problem of state bloat is inherent to public blockchains.**  The video highlights that managing and storing vast quantities of accumulated data from transactions poses a significant challenge as blockchains age.
* **Stellar's solution is innovative in its approach**. It directly confronts the state bloat issue rather than simply attempting to address performance through other means by archiving historical state into off-chain storage. This allows the on-chain network to stay focused on the actual business logic for the transactions while still maintaining data integrity for accounts and transaction visibility for the network.
* **Trade-offs between safety and liveness are crucial**.  The decision to prioritize safety (valid data integrity) over liveness (transaction processing speed) is a deliberate design choice. This is essential to maintain security but might result in some delays in transactions.
* **Merkle trees and TTL values are essential tools**.  The ability to prove the existence (and non-existence) of data through Merkle trees is crucial for data integrity and security.  The TTL system allows for the automated removal of "expired" data, alleviating on-chain storage concerns.
* **The concept of "hot archive" and its implications**.  A "hot archive" is highlighted as a mechanism to readily restore older archived data to chain when required.
* **Bloom filters offer substantial optimization**. Storing historical data off-chain while maintaining a Bloom filter to quickly determine if data exists on-chain is described as an excellent optimization tradeoff to improve speed without compromising data integrity.


## 3. Practical Takeaways

* **Understand the implications of state bloat.** Recognize that this issue is something that will affect all public blockchains as they grow in size and age.
* **Explore innovative approaches to state management.**  Look for ways to minimize the volume of data managed on-chain and to potentially move a lot of this data to optimized off-chain storage.
* **Consider the trade-offs in design choices** Be aware that there can be significant tradeoffs made between speed, safety, and security requirements, and that there may be specific cases where a slower but more secure solution is beneficial.
* **Learn about data structures like Merkle trees**.  Understanding data structures like Merkle trees is important for the future of blockchain development to minimize the amount of data that needs to be stored on-chain in optimized ways.
* **Keep up with developments in blockchain technology.**  State archival is a rapidly advancing area in blockchain technology; continuing to learn and adjust can improve your decision making for blockchain specific projects.

## 4. Additional Notes

The video provides a very high-level overview of a complex protocol.  Further exploration of the specific technical details, relevant code implementation, and security proofs would be beneficial to fully appreciate the protocol's strengths and weaknesses.  The transcript is based on a speech which could include verbal asides not immediately demonstrably written. The video suggests future implementation of these ideas in 2025, and more.