🧠 Chatbot Overview
This AI-powered chatbot serves as a virtual assistant for customers to explore and purchase electronic products such as smartphones, laptops, headphones, and more. Built with n8n and integrated with an LLM, the chatbot supports natural Vietnamese language interactions to:

Recommend products based on user queries.

Add products to the shopping cart.

Guide customers through the checkout process.

Return responses in real-time with up-to-date information.

All responses are provided in structured JSON format to support seamless integration with frontend or automation systems.

![image](https://github.com/user-attachments/assets/58d080d6-96c0-445c-8602-7e58c0079e9a)


🔄 VectorDB Flow: Real-time Product Sync
To ensure data consistency between the main product system and the chatbot’s knowledge, a dedicated VectorDB Flow is implemented. This flow performs the following functions:

Monitors the main product database for real-time updates (e.g., product changes, additions, or removals).

Automatically indexes or re-indexes updated product data into the Supabase Vector Store (products_docs).

Enables the chatbot to retrieve and answer questions using fresh, consistent, and relevant product information every time a customer asks.

This ensures that the chatbot is always aligned with the latest catalog — reducing misinformation and improving customer trust.

![image](https://github.com/user-attachments/assets/f62656f1-e4f5-4126-90cb-bf740b41e137)
