# Bondhu (বন্ধু) — Student Chat & Wellbeing Platform

> ছাত্রদের জন্য বন্ধুর মতো — চ্যাট, পোস্ট, স্টোরি ও AI-ভিত্তিক মেন্টাল হেলথ মনিটরিং। সব এক ফাইলে।

## কী আছে

- **লগইন/রেজিস্টার** — নাম, ইউজারনেম, ক্লাস, পজিশন, রোল, আইডি
- **চ্যাট** — ১-অন-১ ও গ্রুপ; টেক্সট, ইমোজি, ছবি (ফাইল/লিংক), ভয়েস মেসেজ
- **স্টোরি** — ২৪ ঘণ্টা auto-expire; টেক্সট/ইমোজি/ছবি
- **পোস্ট ফিড** — Facebook-style; লাইক, রিপোর্ট, ডিলিট
- **প্রোফাইল** — অন্যের প্রোফাইলে ক্লিক → পোস্ট দেখা, চ্যাট শুরু, ব্লক
- **৮টি থিম** — Light, Dark, Sky, Mint, Sunset, Ocean, Forest, Candy
- **অনলাইন স্ট্যাটাস** — Firebase Realtime Database presence
- **ফোকাস মোড** — admin সক্রিয় করলে অ্যাপ লক, timer + quiz gate
- **মোবাইল রেসপন্সিভ** — bottom navigation + collapsible sidebar

## চালান

```bash
python3 -m http.server 8080
# http://localhost:8080
```

## Live demo

GitHub Pages enable করার পর: `https://thenafiziqbal.github.io/Bondhu/`

> ⚠️ Demo URL টা [Firebase Authentication → Settings → Authorized Domains](https://console.firebase.google.com/project/thetakingchatsosal/authentication/settings) এ যোগ করতে হবে — না হলে login কাজ করবে না।

## প্রজেক্ট কাঠামো

এই public repo তে শুধু **user app** আছে। **Admin panel** (`admin.html`) আলাদা ফাইলে private রাখা হয়েছে security এর জন্য।

## টেক স্ট্যাক

- HTML + CSS + Vanilla JavaScript (ES Modules) — একটাই `index.html`
- Firebase Auth, Firestore, Realtime Database, Storage
- Remix Icon, Hind Siliguri font

---

© Bondhu • a NexDiv project • build with ❤️ for students.
