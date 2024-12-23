# "NewsToPost" Overview
With just two clicks, this smart software fetches, processes, and
posts engaging news content directly to Instagram Story.

## Key Features
1. Automated News Scraping: Pulls the latest articles from popular news websites.
2. Smart Summarization: Condenses lengthy articles into concise, impactful summaries using AI.
3. Eye-Catching News Templates: Transforms news into visually appealing designs.
4. Seamless Instagram Posting: Publishes directly to Instagram Stories for instant engagement.

## Built With 🛠️ 
1. Python
    1. Django 🕸️
    2. Langchain 🦜
    3. Pendulam 🕰️
    4. Instagrapi 📲
    5. bs4 📜
2. Javascript
    1. html2canvas 📸
3. HTML & CSS

## How it Works
- **Select the Latest News**  
   Choose the latest news articles from reliable sources like **TOI**.  
   - The software scrapes the **title**, **description**, and **image** using the powerful **BeautifulSoup** library.  

- **Summarize the News**  
   Long descriptions? No problem!  
   - News is summarized into **200 words or fewer** using a locally operated AI model, **Llama 3.2** with **3B parameters**.  
   - A carefully crafted prompt ensures the core meaning of the news remains intact while keeping it concise and impactful.  

- **Generate Stunning News Templates**  
   Transform raw news into visually appealing designs!  
   - News templates are dynamically created with **HTML & CSS**, powered by **Django**.  
   - Templates are auto-downloaded with **html2canvas** and JavaScript for a seamless experience.
   - This templates also mentions the source of news to give them credit.

- **Store Locally**  
   - Generated news templates are saved in a folder named after the **current date**, which is auto-created using Python’s **os** module.  

- **Post on Instagram**  
   Say goodbye to manual uploads!  
   - The software uses **Instagrapi** to post directly to your Instagram Story.

 
## Problems I Faced  
#### 1️⃣ Template Generation  
The first challenge I encountered was **generating the news templates**. Initially, I considered using template generation APIs like **Bannerbear**, but they turned out to be inconvenient and didn’t meet my specific requirements.  

**Solution:**  
- I decided to create the templates myself using **HTML & CSS** for complete customization.  
- To streamline the process, I utilized **Django** for dynamic template generation and **JavaScript** combined with **html2canvas** for auto-downloading the templates.  

---

#### 2️⃣ Instagram Bot Detection  
Another issue was that Instagram could detect and block bots. This posed a significant challenge to automated posting.  

**Solution:**  
- To overcome this, I implemented a **time-sleep feature** to introduce delays between posts. This helped mimic human behavior and avoid detection by Instagram's bot interface.  

---

These solutions not only resolved the problems but also made the system more robust and flexible.

**Check out stories of this Instagram page** -: https://www.instagram.com/nagpurian._/
