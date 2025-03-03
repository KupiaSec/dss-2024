# Hacking on Solana

*Upload Date: 20250121*

*Source: [https://www.youtube.com/watch?v=8dDVeGL2VyY](https://www.youtube.com/watch?v=8dDVeGL2VyY)*

## Main Points

- **Hacking on Solana**: The speaker, Robert Reith, discusses hacking on Solana, focusing on reentrancy bugs. He explains that while reentrancy is inherently limited on Solana due to its execution model, certain vulnerabilities can still exist.
- **Reentrancy on Solana**: Unlike Ethereum, Solana has a different execution model that restricts reentrancy. However, self-reentrancy bugs can still occur, particularly in multi-signature contracts.
- **Example Vulnerability**: An example is provided where a multi-signature contract can be exploited through a specific sequence of operations that bypasses expected state transitions.
- **EVM on Solana**: The speaker also discusses the Ethereum Virtual Machine (EVM) running on Solana, highlighting potential vulnerabilities related to reentrancy and host escapes.
- **Mitigation Strategies**: The speaker outlines strategies to mitigate reentrancy bugs, including checks-effects-interactions patterns, enforcing read-only accounts, and forbidding self-reentrancy.

## Key Insights

- **Solana's Execution Model**: Solana's execution model inherently limits reentrancy, but self-reentrancy bugs can still occur in certain contract types.
- **Multi-Signature Contracts**: These contracts can be particularly vulnerable due to their complex state transitions and interactions.
- **EVM on Solana**: The EVM running on Solana introduces new vulnerabilities, such as the ability for contracts to call external Solana contracts, potentially leading to reentrancy issues.
- **Mitigation Techniques**: Developers can mitigate reentrancy bugs by following best practices like the checks-effects-interactions pattern and ensuring critical accounts are read-only.

## Practical Takeaways

1. **Understand Solana's Execution Model**: Developers should be aware of Solana's execution model and how it limits reentrancy compared to Ethereum.
2. **Be Wary of Multi-Signature Contracts**: Pay special attention to multi-signature contracts, as they can have complex state transitions that may introduce vulnerabilities.
3. **EVM on Solana**: Be cautious when using the EVM on Solana, as it can introduce new types of vulnerabilities.
4. **Follow Best Practices**: Implement mitigation strategies like the checks-effects-interactions pattern and enforce read-only accounts to prevent reentrancy bugs.

## Additional Notes

- The speaker provides a detailed example of a self-reentrancy bug in a multi-signature contract, illustrating how state transitions can be exploited.
- The talk emphasizes the importance of understanding the nuances of Solana's execution model and the EVM on Solana to identify and mitigate potential vulnerabilities.