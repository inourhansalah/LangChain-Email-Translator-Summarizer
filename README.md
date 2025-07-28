# LangChain-Email-Translator-Summarizer

This project is a language-aware pipeline that **detects**, **translates**, and **summarizes** customer emails using **LangChain**, **Ollama**, and local large language models like **LLaMA 3** and **Gemma 7B**. It supports multilingual input and produces English summaries for non-English content, making it ideal for customer support and communication teams.

---

##  Key Features

-  **Automatic Language Detection**  
  Automatically detects the original language of the input email.

-  **High-Quality Translation to English**  
  Uses a local LLM to translate the content into English for consistency and clarity.

-  **Concise Summarization**  
  Produces a brief summary of the email, helpful for quick review and categorization.

-  **End-to-End Pipeline**  
  Uses LangChain's `SequentialChain` to link detection, translation, and summarization in one flow.

-  **LLMs Run Locally**  
  Powered by Ollama with models like LLaMA 3 and Gemma, running entirely on your machine.

---

##  Tools & Technologies

| Tool / Library        | Purpose                                           |
|------------------------|---------------------------------------------------|
| **LangChain**          | LLM workflow orchestration                        |
| **LangChain Ollama**   | Integration with local LLMs using Ollama          |
| **Ollama**             | Local model server for LLaMA 3, Gemma, and more   |
| **langdetect**         | Lightweight language detection tool               |
| **Python**             | Base language for processing and orchestration    |

---

##  Project Workflow

1. **Start Ollama Server**  
   Launches a local instance of the Ollama model server.

2. **Load Input Email**  
   Reads the raw email content from a `.txt` file (e.g., a Spanish customer email).

3. **Run Through LLM Chains**  
   - **Language Detection**: Identifies the language of the email.
   - **Translation**: Converts the email content to English.
   - **Summarization**: Provides a concise summary of the translated text.

4. **Display Results**  
   Cleanly prints both the translated content and its summary.



