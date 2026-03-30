## Build Your First AI Skill



## Agenda

1. LLMs, Agents and Skills
2. Demo: echo helloworld in another language
3. Demo: helloworld and text to speech
4. Build and share your skill



## LLMs You May Have Heard Of

- GPT (OpenAI)
- Claude (Anthropic)
- Llama (Meta AI)
- Gemini (Google)
- Qwen (Alibaba)
- DeepSeek (DeepSeek)



## Using a LLM on the Cloud

![ChatGPT](chatgpt.png)

Note: a user can send text, images or voice chat with AI; AI can generate text, images and videos;



## Running LLMs Locally

![LM Studio](lmstudio.hero-new.56ec79be.webp)

Note: running an open source model locally; conversational; better for privacy, but requires a little bit teck skill to setup, and in many cases a powerful computer is required.



## Agents

- An agent is a tool on your computer that can follow your instructions and work with your files (like reading and writing).
- It may be a standalone app, or built into another app such as Microsoft Office.



## Common Uses of Agents

- Programmers use agents to write and edit code faster (vibe coding).
- People also use agents as personal AI assistants, for example OpenClaw.



## Popular Agents

- Codex (OpenAI)
- Copilot (GitHub)
- Claude Code (Anthropic)
- Gemini (Google)

Note: these agents are not only for programmers


## Preview
![preview](preview.png)

Note: copilot integrated in vscode, a local application; can talk to a LLM; has access to local file



## Skills

- A skill is a small instruction file that teaches the AI how to handle one specific task.



## Tools

- [VS Code](https://code.visualstudio.com/)
- (Optional) A GitHub account



## Hands-on (part 1)
### Learn the Basics of Markdown

1. Create a new folder on your computer.
2. Open it using VS Code.
3. Create a new file called `helloworld.md`.
4. Visit https://www.markdownguide.org/cheat-sheet/ and try out a few syntaxes.
5. Preview your markdown file in VS Code.



## Hands-on (part 2)
### Create a Simple Translation Skill

1. Create a new file `.agents/skills/helloworld/SKILL.md` (case sensitive).
2. Add the formatter at the very beginning:
  ```
  ---
  name: my-helloworld
  description: Translate helloworld to another language.
  ---
  ```



## Hands-on (part 2)

3. Put the following content in the markdown body.

  ```
  # Helloworld

  ## When to use this skill
  Use this skill when the user sends "helloworld".

  ## How to Translate
  Return in the format `text (language name)`. The `text` part
  is the text of "helloworld" in another language.

  ## Output Example

  - `你好世界 (Chinese)`
  - `Привет, мир (Russian)`
  ```



## Hands-on (part 3)
### A More Advanced Skill

See this [file](https://github.com/codebar-shanghai/workshop-agent-skills/blob/main/.agents/skills/helloworld/SKILL.md?plain=1)
