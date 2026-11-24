# campus-bits
🍴 CampusBites — Real-Time Campus Food Court & Queue Management Web App

A full-stack, mobile-first web application built to eliminate long food-court queues on college campuses—featuring dual role-based portals (Student & Shop Owner), live queue-adjusted wait times, UPI QR payments, and OTP-verified order pickups.

🎯 The Problem & SolutionDuring short college breaks, campus food courts face severe bottlenecks: crowded counters, unorganized verbal orders, and zero visibility into waiting times.CampusBites solves this by digitizing the entire ordering lifecycle across 12 multi-vendor campus stores in a fast, zero-bloat web interface. Students browse live menus, see dynamic preparation times calculated from real-time kitchen load, pay via Cash or UPI QR, and collect their food using a secure 4-digit OTP—while shop owners manage incoming orders on a live Kanban board.

Live Demo Link:[https://yuvrajbhausahebmahajan851-prog.github.io/campus-bits/](https://yuvrajbhausahebmahajan851-prog.github.io/campus-bits/)

✨ Key Features & Capabilities

🎓 Student Experience
   
   🏪 12-Store Food Court Directory: Browse categorized local eateries (from Swami Paratha and Anna Dosa to Dragon Chinese and Momo Mania) with instant queue
   indicators.
   
   ⏱️ Dynamic Wait-Time Engine: Automatically calculates estimated preparation time (Base Prep Time + Item Quantity + Active Queue Load) so students know exact
   pickup times before ordering.
   
   🛒 Interactive Slide-Up Cart & Checkout Sheet: Mobile-native bottom-sheet drawer for adding/removing items, reviewing totals in INR (₹), and choosing payment
   methods.
  
   💳 Dual Payment Support (UPI QR & Cash): Displays the vendor's uploaded UPI QR scanner image for instant digital payment confirmation or allows Cash-on-Pickup.
   
   🔐 Live Order Tracking & 4-Digit Pickup OTP: Real-time 4-stage visual progress bar (Sent → Preparing → Ready → Collected) with browser notifications,
   audio/vibration alerts, and a unique OTP issued upon vendor acceptance.
  
  🧑‍🍳 Shop Owner Dashboard
     
   📊 3-Column Live Order Kanban Board: Dedicated columns for 
   
   🆕 New, 🔥 Preparing, and ✅ Ready orders with one-tap status transitions and live prep-time adjustments (-5 min / +5 min).
   
   🔔 Instant Audio & Visual Order Alerts: Pulsing notification banners, Web Audio API chime alerts, and dynamic browser tab counters whenever a new order
      arrives.
   
   🔑 OTP Pickup Verification: Prevents wrong-order handoffs by requiring vendors to verify the student's 4-digit OTP before marking an order collected.📝 Live
      Menu & Price Manager: Vendors can add new dishes, update prices, toggle ✅ Available / ❌ Sold Out status, or delete items in real time without touching
      code.
   
   📱 Client-Side QR Code Compressor: Built-in HTML5 <canvas> image pipeline that automatically resizes and compresses uploaded UPI QR photos for fast loading.
   
   📥 Sales Analytics & CSV Export: Tracks daily and all-time revenue totals and exports completed order history to downloadable .csv spreadsheets.
      
  🖼️ App Interface PreviewStudent Storefront & Live QueuesVendor Kanban & Menu Management
   
   🛠️ Technical Architecture & HighlightsLayerTechnologies & Implementation Details
   
   🎨 UI & Design SystemSemantic HTML5, Custom CSS3 with Neo-Brutalist styling (Bricolage Grotesque & DM Sans), automatic Dark/Light mode (prefers-color
      scheme), and iOS/Android safe-area insets.
      
   ⚡ Frontend EngineZero-dependency Vanilla JavaScript (ES6+), reactive state management, slide-up bottom sheets, and Web Audio / Vibration / Notification APIs.
      
   🗄️ Data & Offline ResilienceReal-time cloud database sync (onSnapshot listeners) paired with an automatic localStorage fallback engine so the app remains
      functional even offline.
   
   🔒 Security & ValidationClient-side SHA-256 PIN hashing via the Web Crypto API (crypto.subtle.digest), XSS output escaping, Indian 10-digit mobile regex
      validation, and OTP pickup verification.
      
 💼 Freelance & Client Use CasesThis architecture is production-ready and can be customized for clients needing:
      
   🍔 Multi-Vendor Food Courts & College Canteens
   
   ☕ Cafes, Cloud Kitchens & Quick-Service Restaurants (QSRs)
   
   🎟️ Event Food Stalls & Festival Token Systems
   
   🛍️ Local Retail Click-and-Collect Storefronts


