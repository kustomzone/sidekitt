<p align="right">
    <img src="https://komarev.com/ghpvc/?username=kustomzone&label=Repo%20views&color=0e75b6&style=flat" alt="kustomzone">
</p>


## Sidekitt

 - Your websearch talking buddy with memory


<table>
    <tr>
        <td width="900" align="center">
            <p color="#787878">
<img src="https://github.com/kustomzone/sidekitt/raw/refs/heads/main/imgs/sidekitt-logo.jpg" width="200px" height="50px">
                <br>
                
 [Sidekitt help](https://github.com/kustomzone/sidekitt/blob/main/docs/about.md)
              <br><br>
              <br>
            </p>
        </td>
    </tr>
</table>


### Commands

- Chat normally - The assistant will decide if it needs to search

- `/exit` or `quit` - Exit the application
- `/clear` - Clear conversation memory
- `/undo`  -
- `/export`-
- `/import`-
- `/stats`-
- `/research` -
- `/listen` - 2-way talking option (experimental)

## How It Works

Answers: 

- Math and coding questions
- Historical facts and timeless knowledge
- Questions about the conversation itself

Searches: 

- Questions about current events, news, or real-time info
- Information that could be outdated (games, products, recent activities)
- Uncertain about accuracy


### Quick Start


```bash
source .venv/bin/activate
python main.py
```


---

### Credits

 - Andrew Kidoo  - https://github.com/kustomzone
 - Colin Urban   - https://github.com/colinurbs
 - 
 - 
 - 
 - 
 - 
 
 ### Features

- **🔄 Streaming Responses** - See tokens generated in real-time
- **🧠 LLM-Driven Search** - Qwen2.5-3B decides when to search the web
- **🌐 Real Web Scraping** - Fetches actual page content with BeautifulSoup
- **💾 Persistent Memory** - SQLite database remembers conversations
- **📚 Source Citations** - Shows URLs when search was used
- **🎨 Rich CLI** - Beautiful terminal UI with markdown rendering
- **⚡ Local Execution** - No API keys, runs via llama-cpp-python


### Dependencies

See `requirements.txt`:

- llama-cpp-python (local model execution)
- huggingface_hub (model downloads)
- ddgs (web search)
- rich (terminal UI)
- beautifulsoup4 (HTML parsing)
- requests (HTTP requests)


 ### Technical Stack

- **Model**: Qwen2.5-3B-Instruct (GGUF Q4_K_M, ~2GB)
- **Context**: 4096 tokens
- **Search**: DuckDuckGo + requests + BeautifulSoup
- **Memory**: SQLite (last 10 messages)
- **UI**: Rich library with live updates


 ### Suggested Future Improvements

1. **Configuration file** - Customize model, search count, temperature
2. **Conversation export** - Save/load chat histories to JSON
3. **Context summarization** - Compress old messages when limit reached
4. **Undo command** - `/undo` to remove last exchange
5. **Token counter** - Display context window usage
6. **Multi-query search** - Try alternative queries if results are poor
7. **Better error handling** - Graceful network/model failure recovery
8. **Timestamps** - Track message timing in database
9. **Search history** - Remember what searches worked well
10. **Configurable streaming** - Toggle streaming on/off

---
