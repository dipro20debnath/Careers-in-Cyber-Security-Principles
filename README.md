#🛡️ Zero Trust vs Trust but Verify

## Trust but Verify
- ✅ Meaning: 
  - কাউকে বিশ্বাস করা হচ্ছে, কিন্তু সেটাকে যাচাই (verify) করাও হচ্ছে।
- 🔍 Example:
  - Internal network থেকে database access allow, কিন্তু সব query logged.
  - IDS/IPS দিয়ে suspicious activity detect করা।
- 📌 Pros:
  - সহজে deploy করা যায়।
  - user experience ভালো থাকে।
- ⚠️ Cons:
  - insider threat বা misconfiguration overlook হতে পারে।
- 💡 Remember: 

---

## Zero Trust
- ✅ Meaning:
- কাউকেই ডিফল্টে বিশ্বাস করা হবে না। সব access verify করতে হবে।
- 🔍 Example:
- device internal network এ থাকলেও, user MFA করবে।
- microsegmentation: network কে ছোট ছোট অংশে ভাগ করে, প্রতিটি segment access check করবে।
- 📌 Pros:
- অনেক বেশি secure।
- insider attack, lateral movement কমায়।
- ⚠️ Cons:
- complex, implement করতে resources & planning দরকার।
- 💡 Remember:



---

## 🏰 Analogy
| Principle         | Castle example                           |
|-------------------|------------------------------------------|
| Trust but Verify  | castle ভেতরে যারা আছে, তাদের বিশ্বাস করা, মাঝে মাঝে চেক করা। |
| Zero Trust        | castle ভেতরে ঢুকতে হলেও বারবার পরিচয়, badge, password লাগবে। |

---

## 🔍 Key differences
| Trust but Verify              | Zero Trust                        |
|--------------------------------|-----------------------------------|
| কিছুটা বিশ্বাস করবে, পরে verify করবে | কাউকেই বিশ্বাস করবে না, সব verify করবে |
| example: internal network trusted | example: internal network device MFA |
| সহজ deploy                    | কঠিন, কিন্তু secure |

---

## 📝 Summary
- 🛠 **Trust but Verify:** 
- ভরসা করো, কিন্তু নজর রাখো।
- 🧱 **Zero Trust:** 
- ভরসা করো না, সবসময় প্রমাণ চাও।

---
