# Caching Basics

## What is Caching?

Caching means keeping a copy of something in a **quick access place** so you don’t have to fetch or calculate it again.

👉 Think of it like **keeping snacks on your desk** instead of walking to the kitchen every time you’re hungry.

---

## Why Do We Need Caching?

1. **Speed**  
   - Getting data from cache is much faster than going back to the original source (like a database or API).  
   - 📖 Example: Instead of asking the library for the same book every time, you keep a copy at home.  

2. **Reduce Load**  
   - Saves work for the main system (database, server, or API).  
   - 🎓 Example: If 100 people ask the same question, the answer can come from cache instead of the teacher repeating it 100 times.  

3. **Cost Saving**  
   - Accessing the source repeatedly can be expensive (time, bandwidth, or computing power). Cache makes it cheaper.  

---

## Simple Example

- ❌ **Without cache**: Every time you search *“weather in Delhi”*, the app calls the weather server.  
- ✅ **With cache**: The app saves the result for 10 minutes. If you search again within that time, it shows the saved result instantly.  

---

## In Short

**Caching = shortcut memory**  
It makes things **faster, lighter, and cheaper**.  

---
