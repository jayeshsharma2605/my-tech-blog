---
layout: post
title: "DNS Cache"
date: 2025-08-31
categories: tech
---

# DNS Cache (Explained Simply)

When you type **www.google.com** in your browser, something important happens behind the scenes.  
Your browser needs to know the **IP address** of Google’s server (like finding a phone number in a phonebook).  

Instead of asking the "phonebook" (DNS server) **every single time**, the browser keeps a memory of it for a while.  
That memory is called **DNS Cache**. ✅  

---

## ❓ What is DNS Cache?

👉 DNS Cache is a **temporary memory** of domain names and their IP addresses.  
It helps the browser **skip repeated lookups** and load websites faster.  

Think of it like this:  
- ❌ Without cache → You ask for your friend’s phone number from the directory every time.  
- ✅ With cache → You just check your notes where you saved it earlier.  

---

## ⚡ Why Do We Need DNS Cache?

1. **Saves Time**  
   No need to ask DNS servers again and again.  

2. **Reduces Network Load**  
   Fewer requests → less traffic on DNS servers.  

3. **Faster Browsing**  
   Pages load quicker because IP addresses are already known.  

---

## 🏠 Where is DNS Cache Stored?

DNS Cache is kept at multiple places:

- **Browser DNS Cache**  
  (Chrome, Firefox, Edge each have their own cache)  

- **Operating System DNS Cache**  
  (Windows, macOS, Linux also keep their own DNS cache)  

- **ISP DNS Cache**  
  (Your Internet Service Provider caches domain lookups for all users)  

---

## 📅 How Long Does It Stay?

- The duration is controlled by **TTL (Time To Live)** — set by the domain owner.  
- Example: If a record’s TTL = **300 seconds**, the cache is valid for 5 minutes.  
- After TTL expires → browser/OS/ISP asks DNS servers again.  

---

## ⚠️ Problems with DNS Cache

- **Stale Entries**  
  If a website changes its IP address, but your system still has the old one in cache → you might see errors or be sent to the wrong server.  

- **Fix:**  
  Clear (flush) the DNS cache in your browser or operating system to force a fresh lookup.  

---

## 🔑 Interview-Friendly Points

**Q: What is DNS Cache?**  
A: It stores recently resolved domain-to-IP mappings to speed up browsing.  

**Q: Where is it stored?**  
A: Browser, Operating System, and ISP all maintain DNS caches.  

**Q: How long does it last?**  
A: Controlled by TTL (time-to-live) set in DNS records.  

**Q: What issues can happen?**  
A: Stale cache leading to wrong IP resolution → solved by flushing DNS.  

**Q: Can frontend developers access it using JavaScript?**  
A: ❌ No, DNS cache is managed by the browser/OS, not by JS.  

---

## 👀 How to See DNS Cache Practically

### 🔹 In Browser (Chrome/Edge)
- Type in the address bar:  

