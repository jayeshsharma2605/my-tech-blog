---
layout: post
title: "DNS Cache Explained"
date: 2025-08-31
categories: tech
---

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

# Human Brain vs Computer Memory

## Human Brain Memory

Our brain has different types of memory:

### 1. Working Memory

- Very fast but very small.  
- Can hold about **4–7 things** at once.  
- Lasts only for a short time.  
- Example: Remembering a phone number just long enough to dial it.

### 2. Short-Term Memory

- Can hold **thousands of things** for minutes to weeks.  
- Still fast, but temporary.  
- Example: Studying for an exam and remembering notes for a few days.

### 3. Long-Term Memory

- Very large storage, almost unlimited.  
- Slower to recall compared to working memory.  
- Permanent storage.  
- Example: Once you learn cycling, you never forget.  
- Fun fact: During **sleep (REM)**, the brain moves short-term memory into long-term.

**Summary:** Brain memory works in layers → fast & small → slower & bigger → permanent & huge.

---

## Computer Memory

Computers also use layered memory:

### 1. CPU Registers

- Fastest memory.  
- Very tiny (just a few values).  
- Example: Holding 2–3 numbers in your head while doing quick math.

### 2. Cache (L1, L2, L3)

- Small memory inside the CPU.  
- Faster than RAM, slower than registers.  
- Example: A sticky note on your desk for quick info.

### 3. RAM (Main Memory)

- Larger than cache.  
- Slower than registers and cache.  
- Example: A bookshelf in your room → more storage but slower to fetch.

### 4. Hard Disk (HDD/SSD)

- Huge storage.  
- Much slower than RAM.  
- Example: A warehouse → stores everything, but takes time to bring it.

---

## Comparison Table

| Level       | Brain Memory       | Computer Memory | Speed   | Size   |
|-------------|-------------------|----------------|---------|--------|
| Very Fast   | Working memory     | CPU Registers  | Fastest | Tiny   |
| Fast        | Short-term memory | Cache          | Fast    | Small  |
| Medium      | Long-term memory  | RAM            | Medium  | Large  |
| Very Slow   | Old memories      | Hard Disk      | Slow    | Huge   |

---

## Conclusion

Both **brains and computers** use the same idea:  
