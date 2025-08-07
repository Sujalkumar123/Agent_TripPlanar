## 🧠 What is Agent TripPlanar?

**Agent TripPlanar** is a smart travel planner powered by **multiple AI agents** that collaboratively help users:

- ✈️ Plan personalized trips  
- 🔍 Search destinations  
- 🌤️ Check live weather  
- 🛫 Find flights & more — all via intelligent automation!

It leverages **LLMs** like **OpenAI GPT** and **Gemini** to interpret user queries and trigger appropriate tools through autonomous agents.

---

## **Project Goals** 

1. **Deliver a System to Meet Client Needs**  
    - Create a system to provide accurate and instant destination insights, fulfilling the user's requirements seamlessly.  

2. **Build a Modular Architecture**  
    - Design the system to support scalability and future upgrades.  

3. **Testing and Quality Assurance**  
    - Ensure the system's reliability and accuracy through rigorous testing.  

4. **Cost-Effective Measures**  
    - Optimize API and model-related costs without compromising performance.  

---


## OpenAI Models

   - The **GPT-3.5 Turbo model** was ultimately chosen due to its:  
   - **Tool-Calling Excellence**: It demonstrated the best ability to call tools and manage multi-agent tasks seamlessly, ensuring outstanding integration with the system.  
   - **Token Management**: The model's reasoning capabilities enabled it to self-understand context and optimize token usage, producing exceptional results.  
   - **Report Generation**: Its power to combine, process, and generate final reports effectively, as showcased in this project.  
   - **LLaMA Models**: Failed to handle larger token inputs effectively and lacked robust reasoning capabilities, resulting in subpar outcomes.  
   - **Google Models**: While capable of handling large contexts, they failed in reasoning and memory performance, making them unsuitable for this use case.  
   - **OpenAI's o1 Series Models**: Offered great performance but were prohibitively expensive for this project.  
  - Additionally, tested with **Groq inference engine**, which also failed to meet the project's performance indicators.  
 
---

## **Challenges Encountered** 🎋  

The project faced several challenges, including:  
1. **Model API Costs**: Managing the high costs of API calls while ensuring performance.  
2. **Token Limitations**: Handling large queries within the token limits of various models.  
3. **Memory Issues**: Ensuring memory efficiency for better performance.  

---

**Note:** This system is now live, providing users with a seamless and efficient way to fetch trip details in one go. It showcases the potential of modular AI architectures in real-world applications.




## Guide ##

Dear Developers,  

To create a similar project, set up your environment using Python 3.10 or above with Conda:  
```bash  
conda create -p your_env_name python=3.10
```
Activate the env:
```bash
conda activate your_env_path  
```
Then, install the required packages:
```bash
pip install -r requirements.txt  
```

Happy coding and building multi-ai-agent-system! 🎉💚


### Project tree structure

```bash

├├── deployment/
│   └── app.py
├── flowcharts/
│   └── project_pipeline.jpg 
├── src/agentic/
│   ├── agents/
│   │   ├── reporter_agent.py
│   │   ├── travel_agent.py
│   │   └── web_research_agent.py
│   ├── exception/
│   │   └── __init__.py
│   ├── logger/
│   │   └── __init__.py
│   ├── tools/
│   │   ├── get_weather_data.py
│   │   ├── search_articles.py
│   │   ├── search_flights.py
│   │   ├── search_images.py
│   │   └── serper_search.py
│   └── utils/
│       ├── __init__.py
│       └── main_utils.py
├── .gitignore
├── demo.py
├── LICENSE
├── README.md
├── requirements.txt
└── template.py


## 🖼 Demo

![Demo](https://raw.githubusercontent.com/Sujalkumar123/Agent_TripPlanar/master/assests/demo.gif)

