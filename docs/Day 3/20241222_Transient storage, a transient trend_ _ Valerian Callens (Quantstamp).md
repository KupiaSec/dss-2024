# Transient storage, a transient trend?

*Upload Date: 20241222*

*Source: [https://www.youtube.com/watch?v=7VacfY1_YOI](https://www.youtube.com/watch?v=7VacfY1_YOI)*

## Transient Storage, a Transient Trend? | Valerian Callens (Quantstamp) - Summary

This video, presented by Valerian Callens of Quantstamp, explores the topic of transient storage in Ethereum and its adoption.  He argues that transient storage, while not a *trend* in the sense of a rapidly changing craze, is a valuable and growing part of the Ethereum ecosystem.

### 1. Main Points

* **Transient storage's history and evolution:**  Transient storage is not new; it emerged 6 years ago with EIP-1153.
* **Different scopes of transient storage:**  Transient storage operates in two scopes: (1) Contract level: where the contract has access to its own transient data; (2) Transaction level: transient storage exists only during the transaction.
* **Cost-effectiveness:** Transient storage is often cheaper than using persistent storage.
* **Specific use cases:** The speaker highlights several use cases, including re-entrancy guards, tokens with persistent balances (but transient approvals), and fee-based token unlocking/transfers.
* **Security Considerations:**  Concerns about concurrency and potential denial-of-service attacks are mentioned.  Safe use involves managing the life cycle of transient storage, design patterns, and single-purpose slots.  Avoiding parallel executions of actors on the same slot is critical.
* **Adoption in existing projects:** The speaker mentions Uniswap V4, Balancer V3, and other protocols are using or have explored using transient storage.


### 2. Key Insights

* **Transient storage is a practical solution:** The speaker highlights transient storage as a practical alternative to persistent storage in scenarios where the data is only needed temporarily. This is advantageous in terms of costs and efficiency.
* **Important security considerations for transient storage implementation:**  To minimize potential risks, the speaker stresses careful consideration of concurrent access, function design, and safety mechanisms.  The key is to isolate transient storage context and manage its life cycle.
* **Usefulness in combination:** The video points out that persistent storage and transient storage are not mutually exclusive; they're often used together.  Projects might leverage transient solutions for transactional data, while maintaining persistent, fundamental records.

### 3. Practical Takeaways

* **Developers should understand the use cases** of transient storage.  Use the right storage solution for the right problem.
* **Be aware of the security implications:** Carefully design and implement transient storage contexts to avoid concurrency problems and vulnerabilities.
* **Explore existing implementations:** Study how other projects have implemented transient storage on GitHub and in Solidity codebases.
* **Prioritize single-purpose slots:** Designing functions for a specific purpose reduces the risk of unexpected interactions and interference in transient contexts.


### 4. Additional Notes

The presentation is heavily focused on security and practical considerations for using transient storage; understanding the context of the various Ethereum protocols/updates is crucial to gain a thorough understanding of the issues and solutions presented.  The speaker advocates for careful consideration of security in design, even when transient storage offers cost advantages.