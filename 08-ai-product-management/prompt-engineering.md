# Prompt Engineering for Product Managers

> Mastering the art and science of communicating with AI

## 📥 Downloads

- **[Prompt Engineering Overview - Anthropic](https://res.cloudinary.com/dimqqmfx6/raw/upload/v1759549640/ai-prompt-engineering-anthropic.pdf)** (74 KB) - Comprehensive guide from Anthropic
- **[Gemini Prompting Guide](https://res.cloudinary.com/dimqqmfx6/raw/upload/v1759549640/ai-gemini-prompting-guide.pdf)** (5.0 MB) - Google Workspace prompting best practices

---

## What is Prompt Engineering?

Prompt engineering is the practice of designing inputs (prompts) to get desired outputs from AI models. It's the primary interface between humans and AI systems.

### Why It Matters for Product Managers

✅ **Control AI Behavior** - Shape how AI responds to users
✅ **Improve Accuracy** - Get more reliable outputs
✅ **Reduce Costs** - Fewer tokens = lower costs
✅ **Better UX** - More helpful, relevant responses
✅ **Faster Iteration** - Test ideas without code changes

---

## Core Prompting Principles

### 1. Be Clear and Specific

**❌ Bad:**
```
Write about product management.
```

**✅ Good:**
```
Write a 500-word article about prioritization frameworks for B2B SaaS product managers, 
including RICE scoring and examples.
```

### 2. Provide Context

**❌ Bad:**
```
How should I prioritize features?
```

**✅ Good:**
```
I'm a PM at a B2B SaaS company with 50 enterprise customers. We have 20 feature requests 
and limited engineering resources. How should I prioritize using a data-driven framework?
```

### 3. Define the Format

**❌ Bad:**
```
List prioritization frameworks.
```

**✅ Good:**
```
Create a comparison table of 5 prioritization frameworks with columns: 
Name, Best For, Pros, Cons, Example Use Case.
```

### 4. Specify the Tone

**❌ Bad:**
```
Explain OKRs.
```

**✅ Good:**
```
Explain OKRs in a friendly, conversational tone for someone new to product management. 
Use simple language and include a real-world example.
```

### 5. Use Examples (Few-Shot Learning)

**❌ Bad:**
```
Classify this feature request.
```

**✅ Good:**
```
Classify feature requests as: Bug, Enhancement, or New Feature.

Examples:
- "App crashes when uploading images" → Bug
- "Add dark mode" → Enhancement  
- "Build mobile app" → New Feature

Now classify: "Improve search speed"
```

---

## Advanced Techniques

### Chain-of-Thought Prompting

**Purpose:** Get AI to show its reasoning

**Example:**
```
You're evaluating a new feature request. Walk through your reasoning step-by-step:

1. What problem does this solve?
2. Who is the target user?
3. What's the business impact?
4. What are the technical constraints?
5. What's your recommendation?

Feature Request: "Add real-time collaboration to our document editor"
```

### Role-Based Prompting

**Purpose:** Get domain-specific expertise

**Example:**
```
You are a senior product manager with 10 years of experience in B2B SaaS. 
A customer requests a feature that would take 6 months to build but only benefits 
5% of users. How do you respond to the customer while maintaining the relationship?
```

### Constrained Generation

**Purpose:** Control output format and length

**Example:**
```
Write a product update email with these constraints:
- Maximum 150 words
- Include exactly 3 bullet points
- End with a clear call-to-action
- Tone: Professional but friendly

Topic: New AI-powered search feature launch
```

### Iterative Refinement

**Purpose:** Improve outputs through feedback

**Example:**
```
First prompt: "Write a product vision statement for an AI-powered CRM."

[Review output]

Refinement: "Make it more aspirational and focus on the customer benefit, 
not the technology. Keep it under 50 words."
```

---

## Prompt Templates for Product Managers

### 1. User Story Generation

```
Generate a user story for [feature] following this format:

As a [user type]
I want to [action]
So that [benefit]

Acceptance Criteria:
- [criterion 1]
- [criterion 2]
- [criterion 3]

Feature: [describe feature]
User Type: [describe user]
```

### 2. Competitive Analysis

```
Analyze [competitor product] and compare it to our product [our product].

Provide:
1. Key features they have that we don't
2. Our unique advantages
3. Pricing comparison
4. Target market differences
5. Strategic recommendations

Format as a structured report with clear sections.
```

### 3. Feature Prioritization

```
Evaluate this feature request using the RICE framework:

Reach: [number of users affected]
Impact: [scale of 1-3]
Confidence: [percentage]
Effort: [person-months]

Feature: [describe feature]

Provide:
1. RICE score calculation
2. Recommendation (Build Now / Later / Never)
3. Key assumptions
4. Risks to consider
```

### 4. Product Requirements Document (PRD)

```
Create a PRD for [feature] with these sections:

1. Problem Statement
2. Goals & Success Metrics
3. User Stories
4. Functional Requirements
5. Non-Functional Requirements
6. Out of Scope
7. Open Questions

Context:
- Target Users: [describe]
- Business Goal: [describe]
- Technical Constraints: [describe]
```

### 5. Customer Interview Analysis

```
Analyze these customer interview notes and extract:

1. Top 3 pain points (with frequency)
2. Feature requests (prioritized)
3. Unmet needs
4. Surprising insights
5. Recommended next steps

Interview Notes:
[paste notes]
```

---

## Common Pitfalls

### ❌ Pitfall 1: Vague Instructions
**Problem:** "Make it better"
**Solution:** Specify what "better" means

### ❌ Pitfall 2: Too Much in One Prompt
**Problem:** Asking for 10 things at once
**Solution:** Break into multiple prompts

### ❌ Pitfall 3: No Examples
**Problem:** Expecting AI to guess your format
**Solution:** Provide 2-3 examples

### ❌ Pitfall 4: Ignoring Context Window
**Problem:** Pasting entire documents
**Solution:** Summarize or chunk information

### ❌ Pitfall 5: Not Iterating
**Problem:** Accepting first output
**Solution:** Refine based on results

---

## Evaluation Checklist

Before deploying a prompt, check:

- [ ] **Clarity** - Is the instruction unambiguous?
- [ ] **Context** - Have I provided necessary background?
- [ ] **Format** - Have I specified the output format?
- [ ] **Examples** - Have I included examples if needed?
- [ ] **Constraints** - Have I set length/tone/style guidelines?
- [ ] **Edge Cases** - Have I tested unusual inputs?
- [ ] **Consistency** - Does it work across similar inputs?
- [ ] **Cost** - Is the token usage reasonable?

---

## Testing Framework

### 1. Create Test Cases

```
Test Case 1: Typical Input
Input: [normal scenario]
Expected Output: [desired result]

Test Case 2: Edge Case
Input: [unusual scenario]
Expected Output: [how to handle]

Test Case 3: Invalid Input
Input: [bad input]
Expected Output: [error handling]
```

### 2. Measure Performance

- **Accuracy** - % of correct outputs
- **Consistency** - Same input → same output
- **Latency** - Response time
- **Cost** - Tokens per request

### 3. Iterate

1. Test prompt
2. Identify failures
3. Refine prompt
4. Re-test
5. Repeat

---

## Prompt Engineering for Different AI Tasks

### Classification
```
Classify [item] into one of these categories: [list categories]

Provide:
- Category
- Confidence (High/Medium/Low)
- Reasoning

Item: [describe item]
```

### Summarization
```
Summarize this [document type] in [length]:

Focus on:
- Key points
- Action items
- Decisions made

Document:
[paste document]
```

### Generation
```
Generate [number] [item type] that:
- [requirement 1]
- [requirement 2]
- [requirement 3]

Style: [describe style]
Tone: [describe tone]
```

### Analysis
```
Analyze [data/text] and provide:

1. Key insights
2. Patterns or trends
3. Anomalies
4. Recommendations

Data:
[paste data]
```

---

## 🔗 Related Resources

- [AI Agents Guide](./ai-agents-guide.md)
- [AI in the Enterprise](./ai-enterprise-strategy.md)
- [AI Use Cases](./ai-use-cases.md)

---

*Part of the [AI Product Management](./README.md) section*