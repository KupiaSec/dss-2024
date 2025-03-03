# Specification and Model-checking of the ZKsync Governance Protocol

*Upload Date: 20250122*

*Source: [https://www.youtube.com/watch?v=6a3AYcLbHlc](https://www.youtube.com/watch?v=6a3AYcLbHlc)*

# Specification and Model-checking of the ZKsync Governance Protocol | Igor Konnov

**1. Main Points**

* Igor Konnov presents the specification and model-checking of the ZKsync governance protocol.
* The protocol employs a state machine model.
* The protocol has four key entities: Token Assembly, Delegates, Contract Upgrades, and Security Council
* The model checker is used to identify potential issues and vulnerabilities in the smart contract logic.

**2. Key Insights**

* **State Machine Model:** The ZKsync governance protocol is modeled as a state machine, which allows for systematic analysis of the possible states and transitions. This greatly aids in the identification of potential vulnerabilities and errors as each condition under various scenarios is tested systematically and thoroughly.

* **Four Key Entities:** The four entities in the protocol (Token Assembly, Delegates, Contract Upgrades, and Security Council) perform specific roles that define the governance process within the ZKsync protocol. Each entity must adhere to its role to prevent inconsistencies in the consensus process.

* **Model Checking Techniques:** Model checking is used to analyze the behavior of the smart contracts under various scenarios and inputs. This is crucial for identifying any unexpected or unfavorable behavior in the smart contract logic. The methods of checking the ZKsync protocol involve rigorous testing of the protocol under possible conditions.

* **Randomized Simulations and Coverage:**  The speaker highlights the role of randomized simulations and their broader coverage. By simulating various scenarios, the model checker can potentially uncover more issues than a fixed set of test cases. This is particularly useful for stress testing the protocol amidst large numbers of transactions.

* **Quint language:** The specification is written in the Quint language, which appears to be tailored for these types of protocols.

* **Avoiding Solidity-Specific Issues:** An important insight is the avoidance of Solidity-specific behavior in the model-checking part and that the tools don't lean towards standard Solidity-based behavior, rather they encompass more abstract ideas, which is beneficial.

* **Formal Methods and Tools:** The speaker emphasizes the use of formal methods and dedicated tools for the verification process. By using these approaches, the team aims to ensure the security, performance, and correctness of the protocol code.

**3. Practical Takeaways**

* The use of formal methods and dedicated model checkers like Z3 is crucial for increasing the robustness of decentralized applications (dApps), particularly those involving complex governance mechanisms.
* Employing randomized testing significantly improves the likelihood of locating critical vulnerabilities that a conventional test suite might miss.
* Paying close attention to aspects of the protocol, such as proper state transitions and error handling, is critical to develop secure smart contracts.
* For developing ZK-based protocols: Consider using formal methods and languages that are independent of Solidity-based constructs to avoid Solidity-specific issues.

**4. Additional Notes**

* Specific details about Quint, Z3, and other tools mentioned were not fully elaborated, but implication suggests specific tools are used in the formal analysis.
* The video's focus is on the importance of process for security, and the use of automated tools and approaches in achieving security are noted explicitly by the speaker.
* The presenter's expertise in the model checking process is evident; his detailed and comprehensive explanation emphasizes the methodology of how model checkers should be integrated into development pipelines and how formal methodologies should be used.