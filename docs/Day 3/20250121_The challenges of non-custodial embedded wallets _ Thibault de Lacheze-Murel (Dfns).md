# The challenges of non-custodial embedded wallets

*Upload Date: 20250121*

*Source: [https://www.youtube.com/watch?v=yIsipGFZKMc](https://www.youtube.com/watch?v=yIsipGFZKMc)*

# The Challenges of Non-Custodial Embedded Wallets | Thibault de Lacheze-Murel (Dfns)

This video discusses the security and implementation challenges of non-custodial embedded wallets.

## 1. Main Points

* **Security concerns:** The speaker highlights numerous security vulnerabilities inherent in embedded wallet implementations, specifically concerning the handling and protection of private keys.
* **Authentication complexities:**  Authenticating users and ensuring access to the wallet necessitates robust security measures, encompassing various potential factors.
* **Decentralized application (DAP) interaction challenges:** Interactions with decentralized applications (DApps) require secure token handling within embedded wallets.
* **Implementation difficulties:** The speaker emphasizes the difficulties in building reliable and secure embedded wallet solutions, often requiring complex cryptographic protocols and careful infrastructure design.
* **Two-step verification:** Multiple authentication methods, emphasizing user experience improvements.
* **Recovery mechanisms:** Developing user-friendly recovery mechanisms for lost credentials is vital in a non-custodial wallet setup.


## 2. Key Insights

The speaker delves into the complexities of several aspects:

* **Decoupling of Private Keys:**  Non custodial embedded wallet systems require ensuring private keys aren't stored centrally or managed by the wallet provider. This highlights the need for advanced cryptographic mechanisms to ensure the integrity of the process.


* **Decentralized Application Integration:**  Integrating non-custodial wallets with decentralized applications, the speaker indicates the crucial role of authentication tokens to enable secure interactions. These tokens need careful management to maintain security.


* **Credential management issues:** The speaker indicates that a crucial issue is ensuring the confidentiality and security of user credentials, particularly when using multiple devices. Key management in the decentralized environment is important to preserving overall security.


* **End-user Experience:** User onboarding and experience with embedded wallets are pivotal. Frictions in the process (e.g., having to enter a list of words) can discourage users, affecting adoption. Simplifying the process is crucial to improve user experience.


* **Technical Implementation Detail**: The speaker covers diverse technical aspects in detail, such as using multi-party computations, Shamir secret sharing, and local storage within the browser to support security and prevent unauthorized access.


## 3. Practical Takeaways

* **Prioritize Security:**  Security should be the paramount concern when developing or leveraging non-custodial embedded wallets. Careful evaluation of all potential vulnerabilities and use of best practices is essential.

* **User-Friendly Design:**  A seamless and intuitive user experience is critical to user adoption. The design of the wallet needs to balance usability with security.

* **Continuous Improvement:** The speaker highlights the evolution of embedded wallet technology, with new challenges and mitigations emerging. Staying updated on security and implementation advancements is necessary.

* **Decentralized Application Standards:**  Adherence to standards and protocols for decentralized applications (DApps) is important in ensuring secure interaction with the wallet.


## 4. Additional Notes

The video largely focuses on the technical and security challenges faced in the implementation of non-custodial embedded wallets, rather than the general benefits of non-custodial wallets.  The speaker emphasizes the need for a multi-layered security approach. This involves multiple strategies, such as employing publicly known cryptography and decoupling private keys from the embedded wallet provider.  Recommendations include leveraging cryptography and careful infrastructure design to achieve a solid secure implementation, while prioritizing user-friendliness.