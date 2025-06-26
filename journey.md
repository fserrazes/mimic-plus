# Beyond the Day Job: How I Built My First iOS Game

My professional journey began in server-side development, primarily in the industrial, financial, telecommunications, and contact center sectors. I specialized in automating processes, integrating diverse platforms for real-time communication, and managing large-scale databases—long before “Big Data” was a buzzword. Over time, I shifted toward building components, services, front ends, and web applications built for these industries.

In 2015, I decided to make the leap into mobile development. I didn’t want to start from scratch—I had already built up years of technical experience. So I began a personal side project alongside my full-time job. The goal was to experience the full app lifecycle: from concept and design to distribution, monetization, and marketing—far beyond just writing code.

## Why I Chose iOS

At that time, iOS development was entirely new to me. I compared the main platforms—Android, Windows Phone, and iOS—based on market share, documentation, learning curve, and how friendly each one was for solo indie developers.

Windows Phone was already fading. BlackBerry OS and Symbian were practically obsolete. Android had a huge market, but supporting so many different devices sounded like a major hassle — something I wanted to avoid.

iOS stood out. Apple’s tools were mature, the device range was limited (easier to test), and users seemed more willing to pay for well-crafted apps. I already had a Mac and an iPhone 4. Swift was still emerging, but Objective-C felt accessible thanks to my C/C++ background. It just clicked.

With no mobile dev community around me, I turned to books. One book about iOS game development sparked the idea: instead of building another to-do list app, why not make a game? It sounded way more fun—and a better way to learn a new tech stack. It was a bit of a gamble, building a game while learning the platform, but it turned out to be a great bet. Today, I’m a full-time iOS Tech Lead—but back then, I was just making the most practical choice for a solo developer on limited time.

## Rebuilding a Childhood Classic

I decided to recreate a game from my childhood: **Simon Says** (also known as Copy Cat or Genius in some regions). I used to own a “Genius” and thought it would be perfect for the iPhone.

Before writing any code, I researched the existing apps. I downloaded several, played them all, and made detailed notes on what worked, what didn’t, and what I could improve:

* **Clunky interfaces** — poor visuals and desynchronized sounds  
* **Limited themes** — most used the same layout and number of buttons  
* **Intrusive ads** — often disruptive to the player experience (I knew I’d need ads too, but I wanted to do better) 
* **No level selection or continues** — losing meant always starting over  
* **No leaderboards** — missed opportunity for competition  
* **No “repeat sequence” option** — helpful for beginners, but missing  
* **Poor ergonomics** — hard to play one-handed or on smaller screens

With a feature wishlist in hand, I even researched the game’s patent history (just in case) before starting development, despite seeing many clones already on the App Store.

Ironically, that wasn’t enough — years later, I was contacted by Hasbro and had to rebrand the game. But more on that later.

I also had to decide on a **monetization model**. A great article on Ray Wenderlich’s site (now Kodeco) explained how to manage paid and free versions using different Xcode targets. I hadn’t figured out ad integration yet, but I was eager to code—so I saved that for later and adopted the dual-target approach.

In hindsight, with more experience today, I’d probably go with a single build using **in-app purchases** and a **paywall screen**. It simplifies distribution, reduces overhead, and makes it easier to maintain and update the app.

I sketched out all the screens—menus, themes, config, rankings—on paper. I looked at professional tools, but nothing beat paper for quick iteration.

## ⏳ Finding Time and Pushing Through

Building Mimic+ wasn’t just about writing code — it was a masterclass in time management and staying motivated.

Juggling a full-time tech job, family, and daily life meant carving out time for design, development, testing, and polish was incredibly tough. Some days I had just an hour, sometimes two — always fighting to keep the momentum going.

## 🚀 What Helped Me Keep Going

* **Tiny goals** — breaking features into small, achievable tasks kept me moving  
* **Weekend sprints** — when weekdays were scattered, I carved out focused 4+ hour blocks on weekends  
* **Document everything** — notes and decision logs helped me jump back in quickly  
* **Picking battles** — I often got sidetracked by cool ideas. I learned to focus on features that truly mattered to the gameplay

## ⚠️ Unexpected Challenges

Some of the biggest challenges weren’t what I expected:

* **Button Animation & Sound Sync** — syncing feedback with game state was harder than expected. My first attempts had sounds playing out of order.  
* **Asset Creation** — I dusted off Photoshop to design all buttons, icons, and theme assets was a significant mini-project in itself.
* **Sound Design** — sourcing, editing, mixing, and optimizing sounds for each theme was surprisingly intense.  
* **Auto Layout** — it was frustrating, especially with custom shapes like the quarter-donut buttons. Making sure only the visible part was tappable took days to figure out.  
* **Localization** — I originally built the game in English, then translated it into Portuguese (my native language), German (since I live here), and even Spanish—because my sister was taking Spanish classes.  
* **iPad Support** — relatively smooth after all the iPhone layout groundwork.  
* **Game Balancing** — tuning difficulty without player feedback meant a lot of trial and error.  
* **UI Feedback** — making buttons feel responsive across screen sizes took time.  
* **Monetization & Marketing** — developers often ignore this part, but it’s critical if you want people to find your game.  
* **App Renaming** — a trademark complaint forced me to rebrand, redo screenshots, and update all assets.  
* **Apple Guidelines** — the rules are always changing. Whether it’s privacy nutrition labels, xcprivacy files, or Xcode updates, staying compliant is time-consuming.

Still, I managed to integrate **Game Center leaderboards**, and created a smart **ad strategy** for the Lite version: subtle native banners with gentle nudges to upgrade to the paid version. Google AdMob’s documentation helped a lot.

If you’re considering building your own game or side project—do it. It doesn’t have to be fast or perfect. Just **keep it consistent enough** to reach the finish line.

