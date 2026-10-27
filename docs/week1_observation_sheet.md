# System Name: Analysis of ChatGPT as a Conversational AI System

## Group members
1) KIRTANAN MANI MARAN (A24AI0041)
2) NIVEESHANA A/L BALACHANDRAN (A24AI0072)
3) SHAMALAN A/L VELLU THAVAR (A24AI0087)
4) VIROCCHAN A/L S.ELANKOVEN (A24AI0092)

## 1. What problem does this system solve? Who benefits?

### Problem:
Users often need assistance with answering questions, understanding concepts, generating ideas, summarising information and completing language-based tasks. ChatGPT provides a conversational interface through which users can request explanations and receive responses in natural language.

### Beneficiaries:
1) Students: Can use it to understand concepts, brainstorm ideas and obtain explanations.
2) Educators: Can use it to prepare learning materials and examples.
3) Professionals: Can use it to assist with drafting, analysis and other knowledge-based tasks.
4) General users: Can use it to explore information and complete everyday language-based tasks.

### Evidence:
Include a screenshot of your actual ChatGPT interaction demonstrating a question and its response. Use one of the factual or ambiguous test prompts listed in the experiment below.

## 2. Which AI stack layer is most visible to users?

### Selected layer: Application Development Layer
The application layer is the most visible because users interact with ChatGPT through its chat interface. Users enter prompts, receive responses and may provide feedback. The underlying model and supporting infrastructure are not directly visible through ordinary conversation.
The user interface is observable, but the exact internal model configuration, infrastructure and processing pipeline cannot be established solely from the conversation interface. Those elements must be treated as unknown or conceptual unless supported by reliable technical documentation.

## 3. Quality dimensions — at least 3, with measurement method

Dimension 1: Accuracy
Measure: Check whether ChatGPT's factual answers are correct by comparing them with reliable sources.

Dimension 2: Hallucination Risk
Measure: Test whether ChatGPT provides false or fabricated information confidently, especially when the question contains incorrect assumptions.

Dimension 3: Scope Handling
Measure: Check whether ChatGPT recognises its limitations, handles ambiguous questions appropriately, and clearly explains when it cannot perform a requested task.

## 4. What did the system do WELL? Give a specific example.

What ChatGPT did well:
During our experiment, ChatGPT was tested using a straightforward factual question: "What is the capital of Malaysia?"
Observed result: The capital city of Malaysia is Kuala Lumpur. 🇲🇾

Verification: Compare the response with an authoritative geographical or Malaysian government source.

Why this is positive: A correct and direct answer demonstrates the system's usefulness for straightforward factual questions.

Evidence:


![image alt](https://github.com/thoughtdenham2005/ai-engineering-jomlahAI/blob/f51867d160305d65d0ecc02bb5b100dfcf5bb783/Screenshot%202026-10-27%20084137.png)

Evaluation: ChatGPT response was correct and straightforward.

## What did it do POORLY? Give a specific example.

What ChatGPT did poorly:
During our experiment, we tested whether ChatGPT handled ambiguous questions appropriately.

Test prompt: 'Can you book a flight for me?'

Observed result: 
Not exactly! ✈️
I can help you:
🔎 Find flights and compare prices, airlines, and schedules.
🧳 Choose the best option based on your budget and preferences.
🌐 Navigate booking options and help you fill in the necessary details.
However, I can't always complete and pay for a flight booking entirely within this chat. Depending on the available tools, you may need to visit an airline or booking website to confirm your details and make payment.

Identified weakness: ChatGPT lacks the capability to perform tasks outside of its system.

Why this matters: While ChatGPT can recommend the best flights, it cannot book flights for users as the AI has limited access to the booking platform. Furthermore, buying flight tickets requires sensitive details such as password information and payment credentials.

Evidence:


![image alt](https://github.com/thoughtdenham2005/ai-engineering-jomlahAI/blob/659e7a3c4ea11ba00f721ca5f5a5988c18cbc96b/Screenshot%202026-10-27%20090212.png)

Evaluation: ChatGPT excels well in performing tasks that are within its system, but lacks the ability to access websites that do not support it. Moreover, ChatGPT cannot directly book flight tickets for users as it requires the AI to access sensitive and confidential data.

## 6. Responsible AI risks — at least 2. Who is harmed and how?

**Risk 1 — Hallucination and misinformation**
Who could be harmed: Students, researchers and other users who rely on incorrect answers.
Potential impact: A user might include false information in an assignment, report or decision because the response sounds convincing.
Evidence to collect: Verify factual claims in the test responses against reliable sources and record any discrepancies.

**Risk 2 — Inappropriate handling of harmful requests**
Who could be harmed: Account holders and other people whose accounts or information may be targeted.
Potential impact: If a system provides assistance for unauthorised access, it could facilitate privacy violations or security abuse.
Evidence to collect: Use the lab's authorised safety test prompt and document whether ChatGPT refuses the request or redirects it safely.

**Risk 3 — Overconfidence and limited transparency**
Who could be harmed: Users who cannot easily distinguish verified facts from unsupported statements.
Potential impact: A user may trust a plausible answer without checking its sources or limitations.
Evidence to collect: Compare the certainty of the answer with the quality of its supporting evidence. Record whether uncertainty is acknowledged where appropriate.

## 7. If you could fix ONE thing, what and why?

Proposed improvement: Strengthen factual verification and uncertainty communication.

ChatGPT could make it easier for users to distinguish verified information from claims that require further checking. Where appropriate, it should communicate uncertainty, avoid unsupported specificity and provide accessible sources for verifiable factual claims.

Why this improvement?

Accuracy is important because users may rely on AI-generated responses for academic and professional tasks. A fluent response can still be incorrect, so the system should help users understand when independent verification is necessary.

How to evaluate the improvement: Test a set of factual questions with known answers, verify the responses against authoritative sources, and compare the rate of unsupported claims before and after applying a defined verification approach.

Limitation: This is a proposed engineering improvement, not a claim that the current system always fails to verify information
