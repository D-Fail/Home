<!doctype html>
<html lang="bn"> 
 <head> 
  <meta charset="UTF-8"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>বাংলা ছন্দ</title> 
  <style>
        /* বডি স্টাইল */
        body {
            background: linear-gradient(135deg, #001f3f, #000000);
            color: yellow ;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        /* অ্যাপের কন্টেইনার */
        .app-container {
            text-align: center;
            width: 90%;
            max-width: 800px;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            overflow-y: auto;
            max-height: 80vh;
        }

        /* ছন্দের তালিকা */
        .poem-list {
            margin-top: 20px;
            text-align: left;
        }

        /* একক ছন্দ */
        .poem-item {
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 5px;
            padding: 10px;
            margin-bottom: 10px;
            color: white;
            font-size: 16px;
            line-height: 1.5;
        }

        /* স্ক্রল বার স্টাইল */
        .app-container::-webkit-scrollbar {
            width: 8px;
        }

        .app-container::-webkit-scrollbar-thumb {
            background-color: #555;
            border-radius: 5px;
        }
    </style> 
 </head> 
 <body> 
  <div class="app-container"> 
   <h1>বাংলা ছন্দের ঝুড়ি</h1> 
   <div class="poem-list" id="poemList"> <!-- এখানে ছন্দগুলো ডাইনামিকভাবে যোগ করা হবে --> 
   </div> 
  </div> 
  <script>
        // বাংলা ছন্দের তালিকা (১০০০ ছন্দ এখানে যোগ করুন)
        const poems = [
            "আকাশেতে জ্বল জ্বল, তারা বলে টিম টিম,\nসকালে সূর্য ওঠে, আলো দেয় দিন দিন।",
            "লাল লাল গোলাপ ফুল, বাগানে ফুটে থাকে,\nমন ভালো হয় তখন, যখন দেখো তাকে।",
            "চাঁদে আলো ঝরে, রাত হয়ে যায় উজ্জ্বল,\nসবাই চেয়ে দেখে, মন হয় মনোমুগ্ধকর।",
            "নদী বয়ে চলে, স্রোতে স্রোতে যায় বহে,\nচারিপাশে খুশির জোয়ার, মনে খুশি বহে।",
            "গাছেরা দেয় ছায়া, গ্রীষ্মের কড়া রোদে,\nতাদের তলায় বসে, আরাম পাই কোলে।",
            "হাওয়ায় দুলে দুলে, ফুলের মধু লুটে,\nমৌমাছির দল আসে, সব ফুলকে ছুটে।",
            "মেঘলা আকাশে বাজে, বাদল দিনের গান,\nবৃষ্টির মাঝে ভিজে, সবুজ হয় ধান।",
            "শিশির ভেজা সকালে, ঘাসে পড়ে জল,\nছুটে চলে পাখি, সুরে গায় কলকল।",
            "ঝিনুকের মাঝে থাকে, মুক্তো যেমন চাঁদ,\nসাগরের গভীরে লুকিয়ে থাকে স্নিগ্ধসাধ।",
            "প্রজাপতির ডানায়, রঙিন রং খেলে,\nদেখলে মন ভরে, হৃদয়কে মেলে।"
            // এখানে ১০০০টি ছন্দ যোগ করুন...
        ];

        // ছন্দগুলো HTML-এ যোগ করা এবং সিরিয়াল নম্বর সহ দেখানো
        const poemList = document.getElementById("poemList");

        poems.forEach((poem, index) => {
            const poemDiv = document.createElement("div");
            poemDiv.className = "poem-item";
            poemDiv.innerText = `${index + 1}. ${poem}`;
            poemList.appendChild(poemDiv);
        });
    </script> 
 </body>
</html>
