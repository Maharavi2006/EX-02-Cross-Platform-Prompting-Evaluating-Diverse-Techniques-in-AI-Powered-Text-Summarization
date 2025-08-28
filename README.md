EX-02 – Cross-Platform Prompting: Evaluating Diverse Techniques in AI-Powered Text Summarization
AIM

To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

Algorithm

Input Preparation

Select a 500-word technical article on “The Basics of Blockchain Technology.”

Ensure the article includes definitions, features, working principles, and applications.

Define Prompting Techniques

Zero-shot Prompting → “Summarize the following article in simple terms for undergraduate students.”

Few-shot Prompting → Provide 1–2 examples of summaries first, then request a summary.

Chain-of-Thought Prompting → “First break down the article into key points step by step, then write a final summary.”

Role-based Prompting → “You are an expert professor explaining blockchain to beginners. Summarize the article in a clear, simple manner.”

Run Experiments Across Platforms

Use AI platforms: ChatGPT, Gemini, Claude, Copilot.

Apply all four prompting techniques on each platform.

Record and save the generated summaries separately for evaluation.

Evaluation Criteria

Accuracy → Is the summary factually correct?

Coherence → Does the summary flow logically?

Simplicity → Is the summary clear for undergraduates?

Speed → How quickly is the output generated?

User Experience → Is the platform easy and convenient to use?

Scoring

Use a 1–5 scale for each parameter (1 = Poor, 5 = Excellent).

Record scores in a result table (Platform × Prompting Technique).

Calculate the average score for each combination.

Comparison & Analysis

Compare the results across all platforms and prompting methods.

Identify the best-performing combination in terms of Accuracy, Coherence, Simplicity, Speed, and User Experience.

Document final observations and recommendations.

Result
Platform 1: ChatGPT

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

Platform 2: Claude (Anthropic)

Strength: Role-based outputs are usually excellent for clarity.
Example (Role-based): “Think of blockchain as a digital record book shared by many people. Everyone can see it, no one can secretly change it, and trust comes from rules of math, not a central bank. It’s used in Bitcoin, supply chains, and healthcare. The tradeoffs are energy use, speed, and regulations.”

Platform 3: Gemini (Google)

Strength: Chain-of-Thought outputs are strong and structured.
Example (CoT):
“Step 1: Define blockchain → digital ledger.
Step 2: Explain blocks → each contains data and link.
Step 3: Benefits → trust, decentralization.
Step 4: Applications → crypto, supply chains, identity.
Step 5: Challenges → energy, scalability, regulation.
Summary: Blockchain is a decentralized ledger connecting blocks securely, useful in many industries but limited by energy and policy issues.”

Platform 4: Copilot (Microsoft)

Strength: Concise but sometimes oversimplified.
Example (Zero-shot): “Blockchain is a secure digital record that connects data blocks in a chain. It allows direct transactions without banks and is widely used in cryptocurrencies. Other uses include tracking goods and managing records. Downsides include energy use and regulation.”

Final Result (Observation)

Best Accuracy: ChatGPT Few-shot & Claude Role-based

Best Simplicity (Student-friendly): ChatGPT Role-based & Claude Role-based

Best Coherence: Gemini Chain-of-Thought

Fastest: Copilot Zero-shot

Overall Winner (Balanced): Claude Role-based or ChatGPT Few-shot

Result Table
Platform	Prompting Technique	Accuracy	Coherence	Simplicity	Speed	User Experience	Avg Score
ChatGPT	Zero-shot	4	4	4	5	5	4.4
ChatGPT	Few-shot	5	5	4	4	5	4.6
ChatGPT	Chain-of-Thought	5	5	3	4	5	4.4
ChatGPT	Role-based	5	5	5	4	5	4.8
Gemini	Zero-shot	4	4	3	4	4	3.8
Gemini	Few-shot	4	4	4	4	4	4.0
Gemini	Role-based	5	5	5	5	4	4.8
Claude	Chain-of-Thought	5	5	4	4	4	4.4
Copilot	Zero-shot	3	3	3	5	3	3.4
