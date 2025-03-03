# Smart Contracts to Embeddings: Using off-the-shelf LLMs for Fun and Profit

*Upload Date: 20241222*

*Source: [https://www.youtube.com/watch?v=DmfUBh75F1E](https://www.youtube.com/watch?v=DmfUBh75F1E)*

# Smart Contracts to Embeddings: Using off-the-shelf LLMs for Fun and Profit | Markella Gioka (Dedaub) - Summary

**1. Main Points**

* **Connecting Smart Contracts and Embeddings:** The speaker discusses how large language models (LLMs) can be used to analyze smart contract code and find similarities or differences.
* **Off-the-shelf LLMs:**  Using readily available LLMs without needing to train a custom model is emphasized as a key advantage.
* **Analyzing Contract Code:**  The discussion focuses on extracting meaningful features from smart contract code for comparison.
* **Similarity Detection:** Finding similar smart contracts based on code structure, logic, vulnerabilities, or potential malicious patterns is a central theme.
* **Practical Applications:**  Potential applications for this include security auditing, identifying vulnerabilities, and understanding contract functionality.
* **Challenges and Limitations:** The speaker acknowledges that inherent challenges in using LLMs for this task include data quality, pre-trained model limitations, and the nature of on-chain data.


**2. Key Insights**

* **Value of Code Similarity Analysis:**  Identifying similar smart contracts can reveal common vulnerabilities or patterns that might be exploited in one contract, potentially impacting others.
* **LLM's Potential for Automation:** Using LLMs to automate the process of identifying similar contracts can save significant time and resources compared to manual analysis, particularly for large numbers of smart contracts.
* **Contextual Information:** The speaker emphasizes the importance of context in understanding the semantic meaning of smart contract code, advocating for ways to leverage LLMs for contextual information.
* **Limitations of Pre-Trained Models:**  LLMs are only as good as the dataset they were trained on.  A model trained primarily on general text data might not have adequate understanding of the nuances of smart contract code, especially complex or specialized applications.
* **Manual Effort Required:** In spite of automated processes, human analysis and validation likely remain essential for thorough auditing. Data quality or specialized content might require fine-tuning or specific adaptations to pre-trained models. There's no magic bullet; LLMs are not a replacement for deep code comprehension.


**3. Practical Takeaways**

* **Explore off-the-shelf LLM providers:** Investigate options like OpenAI's models or alternatives for smart contract analysis. 
* **Identify relevant features:** Understand what pieces of smart contract code carry the most important information for determining similarity.  This may include variable names, data types, function calls, execution paths, and even the broader code structure of similar function blocks (logical chunks) for a broader comparison.
* **Implement automated similarity detection:** Develop methods to use LLMs to identify similar smart contracts on a larger scale (e.g., using API calls).
* **Validate results:**  Critically assess the results of LLM analysis by supplementing with manual review and, if necessary, domain expertise.
* **Adapt for Specific Needs:** If working with a niche type of contract (e.g., token standards), consider custom training or adaptation strategies to improve the LLM's accuracy on that specific application domain.
* **Data Preparation:** Ensure the data you feed into the LLM (smart contract code) is formatted appropriately and contains valuable insights that accurately model the essence of the contract.


**4. Additional Notes**

* The presentation is focused on code-level similarity, not on identifying malicious intent directly. It does address how LLMs can help with detecting similarities that might flag malicious actions based on the code itself.
* Technical details of implementation are mostly implied, with the core message highlighting the concept and potential.
* The presenter uses an informal, conversational tone, helpful for conveying ideas quickly.


**Overall:** The video effectively articulates how LLMs can be applicable and valuable in the context of smart contract analysis. While the method isn't a silver bullet, it highlights a promising new direction in the field of smart contract security and analysis.