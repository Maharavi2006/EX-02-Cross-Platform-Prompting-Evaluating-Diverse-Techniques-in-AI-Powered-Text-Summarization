# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

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

## Algorithm

To evaluate AI-based summarization, we first selected a 500-word technical article on “The Basics of Blockchain Technology” containing definitions, features, working principles, and applications. Four prompting strategies were defined: zero-shot (direct summarization request), few-shot (providing sample summaries before the task), chain-of-thought (step-by-step reasoning before summarization), and role-based (acting as a professor explaining to students). These prompts were applied across four platforms — ChatGPT, Gemini, Claude, and Copilot. For each run, the generated summaries were recorded and analyzed. Evaluation was carried out based on accuracy, coherence, simplicity, speed, and user experience, each scored on a 1–5 scale. The results were tabulated by averaging scores for each combination of platform and prompting style. Finally, the outputs were compared to identify the best-performing combinations, highlighting which platforms and prompting methods offered the most effective, clear, and student-friendly summaries.

## Result

## Platform 1: ChatGPT

Zero-shot Prompt

Prompt: "Summarize the following 500-word article on the basics of blockchain technology in simple terms for undergraduate students."
Output: Blockchain is a system where transactions are recorded in a secure digital ledger shared across many computers. Instead of relying on banks or central authorities, blockchain allows people to exchange value directly. Each record is stored in a “block,” which links to the next, making tampering very difficult. This technology is widely used in cryptocurrencies but also in supply chain tracking, healthcare, and identity management. While powerful, it faces issues such as high energy use, slower processing, and unclear regulations.

Few-shot Prompt

Prompt: Includes 2 short example summaries of unrelated texts, then asks for blockchain summary.
Output: Blockchain is a decentralized and tamper-proof ledger system. Every transaction is grouped into blocks that connect to form a chain, ensuring security and trust without middlemen. It underpins cryptocurrencies like Bitcoin but also supports real-world applications such as tracking goods, verifying medical data, and protecting digital identities. Key benefits include transparency and trust, while challenges include scalability, energy costs, and government regulation.

Chain-of-Thought Prompt

Prompt: "Think step by step about the main ideas in the article, then provide a concise summary for undergraduates."
Output: Blockchain works like a shared notebook that many people own copies of. Each new page (block) has a record of transactions and links back to earlier pages, making it very hard to alter. This design ensures security and trust. It removes the need for central authorities, enabling uses in money transfers, supply chains, and healthcare. However, it struggles with being slow, energy-hungry, and difficult to regulate.

Role-based Prompt

Prompt: "You are a university professor. Summarize the basics of blockchain technology so first-year undergraduates can easily understand."
Output: Imagine a notebook that everyone in the class shares and updates together. No single person controls it, and once something is written, it can’t be erased or changed. That’s how blockchain works. It uses cryptography to keep entries secure and connects blocks of information in a chain. This makes it very trustworthy and useful for digital money, medical records, and tracking goods. But it also has drawbacks, like slow transactions, high energy usage, and legal challenges.
## Platform 2: Claude (Anthropic)

Strength: Role-based outputs are usually excellent for clarity.
Example (Role-based): “Think of blockchain as a digital record book shared by many people. Everyone can see it, no one can secretly change it, and trust comes from rules of math, not a central bank. It’s used in Bitcoin, supply chains, and healthcare. The tradeoffs are energy use, speed, and regulations.”
## Platform 3: Gemini (Google)

Strength: Chain-of-Thought outputs are strong and structured.
Example (CoT):
“Step 1: Define blockchain → digital ledger.
Step 2: Explain blocks → each contains data and link.
Step 3: Benefits → trust, decentralization.
Step 4: Applications → crypto, supply chains, identity.
Step 5: Challenges → energy, scalability, regulation.
Summary: Blockchain is a decentralized ledger connecting blocks securely, useful in many industries but limited by energy and policy issues.”

## Platform 4: Copilot (Microsoft)

Strength: Concise but sometimes oversimplified.
Example (Zero-shot): “Blockchain is a secure digital record that connects data blocks in a chain. It allows direct transactions without banks and is widely used in cryptocurrencies. Other uses include tracking goods and managing records. Downsides include energy use and regulation.”

## FINAL RESULT:
```

1.Best Accuracy: ChatGPT Few-shot & Claude Role-based
2.Best Simplicity (Student-friendly): ChatGPT Role-based & Claude Role-based
3.Best Coherence: Gemini Chain-of-Thought
4.Fastest: Copilot Zero-shot
5.Overall Winner (Balanced): Claude Role-based or ChatGPT Few-shot
```

## RESULT TABLE:

| Platform | Prompting Technique | Accuracy | Coherence | Simplicity | Speed | User Experience | Avg Score |
| -------- | ------------------- | -------- | --------- | ---------- | ----- | --------------- | --------- |
| ChatGPT  | Zero-shot           | 4        | 4         | 4          | 5     | 5               | 4.4       |
| ChatGPT  | Few-shot            | 5        | 5         | 4          | 4     | 5               | 4.6       |
| ChatGPT  | Chain-of-Thought    | 5        | 5         | 3          | 4     | 5               | 4.4       |
| ChatGPT  | Role-based          | 5        | 5         | 5          | 4     | 5               | **4.8**   |
| Gemini   | Zero-shot           | 4        | 4         | 3          | 4     | 4               | 3.8       |
| Gemini   | Few-shot            | 4        | 4         | 4          | 4     | 4               | 4.0       |
| Gemini   | Role-based          | 5        | 5         | 5          | 5     | 4               | 4.8       |
| Claude   | Chain-of-Thought    | 5        | 5         | 4          | 4     | 4               | 4.4       |
| Copilot  | Zero-shot           | 3        | 3         | 3          | 5     | 3               | 3.4       |



