# Collection of AI tools
[my own AI cheat sheet](https://github.com/cherkavi/ai)
:TODO: vector database  
:TODO: https://github.com/explodinggradients/ragas  

## AI platforms
* [union](https://www.union.ai/)

## chat bots
* https://www.perplexity.ai/
* https://bard.google.com/chat
* https://openai.com/blog/chatgpt

## general purposes tools
* [cli tool for interacting with LLM](https://github.com/simonw/llm)
  * llm-youtube
    ```sh
    llm install llm-youtube
    llm -f yt:zv72WMmVkPw 'Please summarize this video'
    ```
* [whisper - translate mp3 to text](https://github.com/openai/whisper)
  > `pip install -U openai-whisper` and then `whisper japanese.wav --language Japanese --task translate`

## Large Language Model ( LLM )
### Ollama Facebook
[linux installation](https://github.com/ollama/ollama/blob/main/docs/linux.md)
```sh
curl -fsSL https://ollama.com/install.sh | sh
# /usr/local/bin/ollama
# /etc/systemd/system/default.target.wants/ollama.service → /etc/systemd/system/ollama.service.
# sudo find /usr/share/ollama/.ollama
```

```sh
x-www-browser http://127.0.0.1:11434/api/version
journalctl -e -u ollama
ollama --version
```
```sh
x-www-browser https://ollama.com/search
ollama pull llama4
ollama list
```

## RAG
* Agentic RAG - for creating scalable workflow of tasks
* Enhancement tools: 
  * LangGraph
  * Phoenix Arize
* G-RAG

## MCP
![mcp sequence](https://i.ibb.co/s9ywRss4/mcp-workflow.jpg)
- [Model Context Protocol documentation](https://modelcontextprotocol.io)
- [Model Context Protocol specification](https://spec.modelcontextprotocol.io)
- [Python SDK GitHub repository](https://github.com/modelcontextprotocol/python-sdk)
- [Officially supported servers](https://github.com/modelcontextprotocol/servers)
- [MCP Core Architecture](https://modelcontextprotocol.io/docs/concepts/architecture)

## Find out
* Text2SQL
* Quantization
* Reranker
* Table Augmented Generation