# How to Carry Context to Another Conversation

Very common problem, right? You're in a conversation flow and almost solving it when one of these things happens:

- The AI starts hallucinating.
- The context limit is reached.
- The service blocks you due to some limit.

## Practical Solution

The ideal approach would be to take notes of key points from that conversation to start a new one. But how to do this in a practical way? Rewriting what was said in the chat can be useful, but it's not always necessary. In short, you only need the **initial state** and the **current state** of your flow.

### Step by step:

1. **Copy the first prompt** explaining what you wanted to do.
2. **Show where you got to** — the final version of what was produced or discussed.

That way, the AI will be able to assess how it started and what was done, so it can make a decision accurately.
