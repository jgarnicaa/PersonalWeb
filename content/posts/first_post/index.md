---
title: "Web Scraping in Static Websites"
date: 2025-03-17T12:33:28+01:00
draft: false

summary: "What? How? When? Everything you need to know about web scraping (HTML-based)"
tags: ["Python", "Web Scraping", "Data", "Data Mining"]

thumbnail: "wstb.jpeg"
thumbnailAlt: "Web Scraping Thumbnail"

cover: "WBCoer.png"
---

# 🌐 Web Scraping in Static Websites

## 🤔 What is Web Scraping?

Have you ever thought about the vast amount of text data continuously exposed on social media, blogs, or internet forums? For example, the amount of data that can be extracted from tweets about a specific topic or the information publicly shared by users on specialized forums. Wouldn't it be incredible to use this data to quantify, analyze, and even train a specialized LLM (Large Language Model) on a specific topic? Well, that's exactly what **web scraping** does! It allows you to retrieve and explore data from websites, making it possible to extract valuable information for further use.

---

## 🕰️ When to Use Web Scraping?

Web scraping should be used when you have **publicly available data** on a website that is of interest to you. This means information that is freely shared and accessible. It should **not** be used on private websites or those handling personal or sensitive data, such as pages requiring login credentials or access to private information. 

Web scraping is ideal for:
- **Public blogs**
- **Social media platforms** (with public data)
- **Open forums**

For example, I used web scraping in my **LLM Poetry Generator** project to gather data from a Spanish poetry website. The available datasets online were too small, so I decided to scrape my own. Keep reading to learn how I did it! 😊

---

## 🛠️ How to Use Web Scraping?

To understand web scraping, it's important to classify websites into two types:
1. **Dynamic Websites**: Like social media platforms, which use varied structures to share information.
2. **Static Websites**: Like blogs, which use **HTML** to describe their content.

In this guide, we'll focus on **static websites** since they are easier to scrape.

---

### 📄 A Quick Introduction to HTML

To scrape data effectively, you need to understand how HTML structures content. HTML uses **tags** to define different parts of a webpage, such as titles, body text, images, external links, etc. Here's a quick example of HTML tags:

```html
<h1>This is a Title</h1>
<p>This is a paragraph.</p>
<a href="https://example.com">This is a link</a>
<img src="image.jpg" alt="An image">
```

Understanding these tags is crucial because they help you identify where the data you want to scrape is located on the webpage.

---

### 🔍 Extracting the Data

Once you understand HTML tags and the structure of your target website, you can start extracting data. However, **web scraping is not a one-size-fits-all solution**. Each website is unique, and your scraping approach must be adapted to the specific structure of the site.

Let me walk you through an example: I scraped approximately **13,000 Spanish poems** from the website [www.poemas-del-alma.com](https://www.poemas-del-alma.com). Here's how I did it:

1. **Step 1: Explore the Website Structure**  
   I started by analyzing the website's structure. I noticed that I needed to:
   - First, retrieve a list of authors.
   - Then, get the list of poem titles for each author.
   - Finally, extract the text of each poem using the author and title information.

2. **Step 2: Extract Authors**  
   Using the browser's **Developer Tools** (F12), I inspected the HTML and found that the `<a>` tag contained the links to individual authors. I used this tag to extract all author links.

3. **Step 3: Extract Poem Titles**  
   For each author, I accessed their page and extracted the poem titles. I noticed that poem links were the only ones containing `"https"` and `".htm"`, so I filtered out other links.

4. **Step 4: Extract Poem Text**  
   Finally, I looped through each poem link and extracted the text using the `<p>` tag, which contained the poem's body.

---

## 🧰 Tools for Web Scraping

For static websites, I used **Python** along with the **BeautifulSoup** library to implement the scraping script. Here's a breakdown of the tools I used:

- **Python**: The programming language used for scripting.
- **BeautifulSoup**: A Python library for parsing HTML and extracting data.
- **Requests**: A library to send HTTP requests and retrieve webpage content.

You can check out the full script I used for scraping poems on my GitHub repository:  

{{< alert "github" >}}
[🔗 Web Scraping Script](https://github.com/jgarnicaa/GenAI_Poetry/blob/main/src/web%20scraping/ES_Poetry_PDA.py)
{{< /alert >}}


---

## 📊 Bonus: The Dataset

If you're interested in exploring the dataset I created, you can find it on Kaggle:  
[🔗 Spanish Poetry Dataset](https://www.kaggle.com/datasets/jgarnicaaza/spanish-poetry-dataset-dataset-poemas-en-espaol/data)

---

## 🚀 Conclusion

Web scraping is a powerful technique for extracting data from websites, especially when publicly available datasets are insufficient. By understanding HTML structure and using tools like Python and BeautifulSoup, you can gather and analyze data for various applications, such as training machine learning models or conducting research.

If you're new to web scraping, start with static websites and gradually explore more complex scraping techniques. Happy scraping! 🕷️

---

### 📌 Tags
#Python #WebScraping #Data #DataMining #BeautifulSoup #HTML


