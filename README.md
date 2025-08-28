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

<h4>1. Input Preparation</h4>
<ul>
  <li>Select a 500-word technical article on “The Basics of Blockchain Technology”.</li>
  <li>Ensure the article includes definitions, features, working principles, and applications.</li>
</ul>

<h4>2. Define Prompting Techniques</h4>
<ul>
  <li><b>Zero-shot Prompting</b> → “Summarize the following article in simple terms for undergraduate students.”</li>
  <li><b>Few-shot Prompting</b> → Provide 1–2 examples of summaries first, then request a summary.</li>
  <li><b>Chain-of-Thought Prompting</b> → “First break down the article into key points step by step, then write a final summary.”</li>
  <li><b>Role-based Prompting</b> → “You are an expert professor explaining blockchain to beginners. Summarize the article in a clear, simple manner.”</li>
</ul>

<h4>3. Run Experiments Across Platforms</h4>
<ul>
  <li>Use AI platforms: <b>ChatGPT, Gemini, Claude, Copilot</b>.</li>
  <li>Apply all four prompting techniques on each platform.</li>
  <li>Record and save the generated summaries separately for evaluation.</li>
</ul>

<h4>4. Evaluation Criteria</h4>
<ul>
  <li><b>Accuracy</b> → Is the summary factually correct?</li>
  <li><b>Coherence</b> → Does the summary flow logically?</li>
  <li><b>Simplicity</b> → Is the summary clear for undergraduates?</li>
  <li><b>Speed</b> → How quickly is the output generated?</li>
  <li><b>User Experience</b> → Is the platform easy and convenient to use?</li>
</ul>

<h4>5. Scoring</h4>
<ul>
  <li>Use a <b>1–5 scale</b> for each parameter (1 = Poor, 5 = Excellent).</li>
  <li>Record scores in a result table (Platform × Prompting Technique).</li>
  <li>Calculate the average score for each combination.</li>
</ul>

<h4>6. Comparison & Analysis</h4>
<ul>
  <li>Compare the results across all platforms and prompting methods.</li>
  <li>Identify the <b>best-performing combination</b> in terms of Accuracy, Coherence, Simplicity, Speed, and User Experience.</li>
  <li>Document final observations and recommendations.</li>
</ul>

## Result

<h3>Platform 1: ChatGPT</h3>

<h4>Zero-shot Prompt</h4>
<p><b>Prompt:</b> "Summarize the following 500-word article on the basics of blockchain technology in simple terms for undergraduate students."</p>
<p><b>Output:</b> Blockchain is a system where transactions are recorded in a secure digital ledger shared across many computers. Instead of relying on banks or central authorities, blockchain allows people to exchange value directly. Each record is stored in a “block,” which links to the next, making tampering very difficult. This technology is widely used in cryptocurrencies but also in supply chain tracking, healthcare, and identity management. While powerful, it faces issues such as high energy use, slower processing, and unclear regulations.</p>

<h4>Few-shot Prompt</h4>
<p><b>Prompt:</b> Includes 2 short example summaries of unrelated texts, then asks for blockchain summary.</p>
<p><b>Output:</b> Blockchain is a decentralized and tamper-proof ledger system. Every transaction is grouped into blocks that connect to form a chain, ensuring security and trust without middlemen. It underpins cryptocurrencies like Bitcoin but also supports real-world applications such as tracking goods, verifying medical data, and protecting digital identities. Key benefits include transparency and trust, while challenges include scalability, energy costs, and government regulation.</p>

<h4>Chain-of-Thought Prompt</h4>
<p><b>Prompt:</b> "Think step by step about the main ideas in the article, then provide a concise summary for undergraduates."</p>
<p><b>Output:</b> Blockchain works like a shared notebook that many people own copies of. Each new page (block) has a record of transactions and links back to earlier pages, making it very hard to alter. This design ensures security and trust. It removes the need for central authorities, enabling uses in money transfers, supply chains, and healthcare. However, it struggles with being slow, energy-hungry, and difficult to regulate.</p>

<h4>Role-based Prompt</h4>
<p><b>Prompt:</b> "You are a university professor. Summarize the basics of blockchain technology so first-year undergraduates can easily understand."</p>
<p><b>Output:</b> Imagine a notebook that everyone in the class shares and updates together. No single person controls it, and once something is written, it can’t be erased or changed. That’s how blockchain works. It uses cryptography to keep entries secure and connects blocks of information in a chain. This makes it very trustworthy and useful for digital money, medical records, and tracking goods. But it also has drawbacks, like slow transactions, high energy usage, and legal challenges.</p>


<h3>Platform 2: Claude (Anthropic)</h3>
<ul>
  <li><b>Strength:</b> Role-based outputs are usually excellent for clarity.</li>
  <li><b>Example (Role-based):</b> “Think of blockchain as a digital record book shared by many people. Everyone can see it, no one can secretly change it, and trust comes from rules of math, not a central bank. It’s used in Bitcoin, supply chains, and healthcare. The tradeoffs are energy use, speed, and regulations.”</li>
</ul>


<h3>Platform 3: Gemini (Google)</h3>
<ul>
  <li><b>Strength:</b> Chain-of-Thought outputs are strong and structured.</li>
  <li><b>Example (CoT):</b> “Step 1: Define blockchain → digital ledger. Step 2: Explain blocks → each contains data and link. Step 3: Benefits → trust, decentralization. Step 4: Applications → crypto, supply chains, identity. Step 5: Challenges → energy, scalability, regulation. <br> <b>Summary:</b> Blockchain is a decentralized ledger connecting blocks securely, useful in many industries but limited by energy and policy issues.”</li>
</ul>


<h3>Platform 4: Copilot (Microsoft)</h3>
<ul>
  <li><b>Strength:</b> Concise but sometimes oversimplified.</li>
  <li><b>Example (Zero-shot):</b> “Blockchain is a secure digital record that connects data blocks in a chain. It allows direct transactions without banks and is widely used in cryptocurrencies. Other uses include tracking goods and managing records. Downsides include energy use and regulation.”</li>
</ul>


<h3>Final Result (Observation)</h3>
<ul>
  <li><b>Best Accuracy:</b> ChatGPT Few-shot & Claude Role-based</li>
  <li><b>Best Simplicity (Student-friendly):</b> ChatGPT Role-based & Claude Role-based</li>
  <li><b>Best Coherence:</b> Gemini Chain-of-Thought</li>
  <li><b>Fastest:</b> Copilot Zero-shot</li>
  <li><b>Overall Winner (Balanced):</b> Claude Role-based or ChatGPT Few-shot</li>
</ul>




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



