## ডোমেইন নেইম সিস্টেম(DNS) এর টাইপ

যখন আমরা একটি ডোমেইন রেজিস্টার করতে যাই, তখন আমাদের DNS সেটআপ করে দিতে হয়। মানে কোন IP তে ডোমেইন পয়েন্ট করা থাকবে। সেটআপ করার সময় কিছু DNS টাইপ থাকে, আমাদের প্রয়োজন অনুযায়ী নির্বাচন করব।

- A: A টাইপ মূলত একটি ডোমেইন এর IP এড্রেস দিয়ে তার সার্ভার খুঁজে বের করতে সাহায্য করে থাকে। মনে করি, আমাদের ডোমেইন হচ্ছে google.com এবং তার IP এড্রেস হচ্ছে 192.168.0.1, আমরা যখন A টাইপ নির্বাচন করব তখন IP টি বলে দিতে হবে।

  এখন আরেকটি অপসন থাকে যাকে Name বলা হয় সাধারণত, যেখানে আমরা হয় @ ব্যবহার করতে পারবো না হয় অন্য কোনো ওয়ার্ড।

  যদি আমরা @ ব্যবহার করি তাহলে তা root ডোমেইনকে IP এড্রেস এর সাথে পয়েন্ট করবে।

  @ => google.com => 192.168.0.1

  যদি ওয়ার্ড হিসাবে app ব্যবহার করি তাহলে সেটি সাব-ডোমেইন হিসেবে IP পয়েন্ট করা হবে।

  app.google.com => 192.168.0.1

- CNAME: CNAME মূলত একটি ডোমেইন কে অন্য ডোমেইন এর IP সাথে পয়েন্ট করে দিবে। মনে করে, আমাদের ডোমেইন google.com এখন আমরা সরাসরি এতে কোন IP সেট না করে অন্য একটি ডোমেইন facebook.com পয়েন্ট করে দেই। তাহলে পরবর্তীতে যখন কেউ google.com এ যাওয়ার চেষ্টা করতে তখন তা facebook.com এর IP তে চলে যাবে।