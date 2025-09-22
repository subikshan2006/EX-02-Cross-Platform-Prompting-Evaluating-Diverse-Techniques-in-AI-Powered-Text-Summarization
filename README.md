# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

---
## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

Accuracy

Coherence

Simplicity

Speed

User experience


---

## **Algorithm**

1. **Article Selection**
   Select a \~500-word technical article titled *"The Basics of Blockchain Technology"*.

## The Basics of Blockchain Technology:

Blockchain technology has rapidly emerged as one of the most transformative innovations of the 21st century. Initially developed as the foundation for cryptocurrencies like Bitcoin, it has since expanded into industries such as finance, supply chain management, healthcare, and even voting systems. At its core, blockchain is a decentralized and transparent digital ledger that securely records transactions across multiple computers. To understand its significance, it is important to explore its structure, working principles, and applications.

What is Blockchain?

Blockchain is essentially a chain of digital “blocks” that contain transaction data. Each block includes three key elements: the data itself, a timestamp, and a cryptographic hash of the previous block. The hash serves as a unique identifier, ensuring that once data is entered into the blockchain, it cannot be altered without changing every subsequent block. This structure makes blockchain highly secure and tamper-resistant.

How Blockchain Works?

The process of adding a transaction to the blockchain follows several steps:
Transaction Initiation – A user requests a transaction, such as transferring cryptocurrency or recording a contract.
Verification – The transaction is broadcast to a network of computers, known as nodes, which validate the request using consensus mechanisms like Proof of Work (PoW) or Proof of Stake (PoS).
Block Creation – Once verified, the transaction is grouped with others to form a block.
Chain Linking – The block is added to the existing blockchain, connected through cryptographic hashes.
Completion – The updated blockchain is distributed across the network, making the transaction permanent and visible to all participants.
This decentralized approach removes the need for intermediaries, such as banks, and allows for peer-to-peer transactions.

Key Features of Blockchain:

Decentralization – Unlike traditional databases controlled by a central authority, blockchain is distributed across many computers, reducing the risk of corruption or manipulation.
Transparency – All participants in the network can view transactions, ensuring trust among users.
Immutability – Once data is recorded, it cannot be modified, making the system resistant to fraud.
Security – Cryptographic techniques safeguard data, protecting against unauthorized access and cyberattacks.

Applications of Blockchain:

While cryptocurrencies remain the most well-known application, blockchain has far-reaching potential:
Finance – Blockchain enables faster and more secure cross-border payments, eliminating costly intermediaries.
Supply Chain Management – Companies can track goods from production to delivery, ensuring authenticity and reducing fraud.
Healthcare – Patient records can be securely stored and shared among healthcare providers, improving efficiency and privacy.
Voting Systems – Blockchain-based voting can enhance transparency and reduce election fraud.
Smart Contracts – Self-executing contracts with predefined conditions streamline business agreements without the need for third parties.

Conclusion:

Blockchain technology represents a paradigm shift in how we record, verify, and share information. Its core strengths—decentralization, transparency, and security—make it a powerful tool with applications far beyond digital currencies. As industries continue to explore its potential, blockchain may fundamentally reshape how transactions and trust are managed in the digital age. Understanding its basics is the first step toward appreciating the revolutionary changes it brings to society and the economy.

3. **Prompting Strategies Definition**
   Prepare the following four prompting strategies:

   * **Zero-shot**: Directly ask the model to summarize without examples.
   * **Few-shot**: Provide 2–3 examples of summaries for similar technical texts before asking for the summary.
   * **Chain-of-Thought**: Prompt the model to explain or break down the text logically before summarizing.
   * **Role-based**: Instruct the model to act as a specific role (e.g., “a university professor summarizing for freshmen”).

4. **Platform Selection**
   Use the following AI platforms:

   * ChatGPT (OpenAI)
   * Gemini (Google)
   * Claude (Anthropic)
   * Copilot (Microsoft)

5. **Execution**
   For each platform:

   * Apply each prompting strategy using the same input article.
   * Record the output summary.
   * Note time taken to generate the summary.

6. **Evaluation Criteria**
   Evaluate each generated summary using the following:

   * **Accuracy**: Does the summary correctly capture the main points of the article?
   * **Coherence**: Is the summary logically structured and easy to follow?
   * **Simplicity**: Is the language accessible for undergraduate students?
   * **Speed**: How fast is the response?
   * **User Experience**: Was the interface intuitive, and was the output easy to copy/save?

7. **Scoring & Analysis**

   * Assign scores (1 to 5) for each criterion across all combinations.
   * Tabulate results for comparison.
   * Identify the best-performing strategy-platform combination.

---

## Bar chart:

<img width="2400" height="1600" alt="image" src="https://github.com/user-attachments/assets/3c2eae44-5011-4b09-829b-88af34b9f272" />


## **Result**

| Platform | Prompt Type      | Accuracy | Coherence | Simplicity | Speed | UX | Total (/25) |
| -------- | ---------------- | -------- | --------- | ---------- | ----- | -- | ----------- |
| ChatGPT  | Zero-shot        | 4        | 4         | 4          | 5     | 5  | 22          |
| ChatGPT  | Few-shot         | 5        | 5         | 5          | 4     | 5  | 24          |
| ChatGPT  | Chain-of-Thought | 5        | 5         | 4          | 3     | 5  | 22          |
| ChatGPT  | Role-based       | 5        | 5         | 5          | 4     | 5  | 24          |
| Gemini   | Zero-shot        | 3        | 3         | 3          | 5     | 4  | 18          |
| Gemini   | Few-shot         | 4        | 4         | 4          | 4     | 4  | 20          |
| Claude   | Chain-of-Thought | 5        | 5         | 5          | 4     | 4  | 23          |
| Claude   | Role-based       | 5        | 5         | 5          | 4     | 5  | 24          |
| Copilot  | Zero-shot        | 3        | 3         | 3          | 5     | 4  | 18          |
| Copilot  | Few-shot         | 4        | 4         | 4          | 4     | 4  | 20          |

> **Best Performing Combination:**
> **Claude + Role-based Prompting** and **ChatGPT + Few-shot Prompting** both scored **24/25**, showing high effectiveness in summarizing complex content in a simple and structured way for undergraduates.

---
