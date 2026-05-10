# StreamHub Dual-Licensing Guide

## Why This License Structure?

StreamHub uses a **Non-Commercial Copyleft** license to ensure:
1. **Ownership retained** — Aaron Brown / ApPotato maintains full copyright
2. **No commercial exploitation** — Companies can't profit from free work
3. **Open source stays open** — Forks can't be closed-source

---

## The License: CC BY-NC-SA 4.0

**Creative Commons Attribution-NonCommercial-ShareAlike 4.0**

### What it means:

| Pillar | What You Must Do |
|--------|------------------|
| **Attribution (BY)** | Credit Aaron Brown / ApPotato as original author |
| **NonCommercial (NC)** | Cannot use for commercial advantage or monetary gain |
| **ShareAlike (SA)** | Must release modifications under this same license |

---

## Dual-Licensing Model

### Free Version (Public)
✅ **Who can use it:**
- Hobbyists and personal projects
- Students and educational use
- Non-profit organizations
- Open-source community projects

✅ **What you can do:**
- Use StreamHub personally
- Modify and fork the code
- Share your modifications (under CC BY-NC-SA 4.0)

❌ **What you CANNOT do:**
- Use it in a for-profit company
- Sell it or charge for it
- Make it proprietary/closed-source
- Use the "StreamHub" name on your fork

### Commercial Version (Paid)
💰 **Who needs a commercial license:**
- Any for-profit company
- Anyone wanting to close the source
- Anyone wanting to monetize it
- Anyone wanting proprietary modifications

✅ **What a commercial license allows:**
- Use within for-profit companies
- Closed-source modifications
- Commercial distribution
- Monetization and revenue generation
- Optional attribution removal

📧 **Get a commercial license:**
Email: 1aaroncbrown@gmail.com
Subject: StreamHub Commercial License Inquiry

---

## Enforcement: What Happens If Someone Violates?

### Common Violations:

1. **Using it commercially without paying**
   - Example: A startup uses StreamHub as their product UI
   - Result: Copyright infringement, liable for damages

2. **Relicensing to MIT/Apache/GPL**
   - Example: Someone forks and changes LICENSE to MIT
   - Result: Copyright violation, must revert

3. **Using "StreamHub" name on a fork**
   - Example: Fork called "StreamHub Pro"
   - Result: Trademark infringement

4. **Closing the source**
   - Example: Fork made private/proprietary
   - Result: Violates ShareAlike, copyright infringement

### Legal Recourse:
Under this license, Aaron Brown / ApPotato can:
- Issue DMCA takedown notices
- Pursue copyright infringement claims
- Seek damages and legal fees
- Enforce trademark protection

---

## FAQ

### Q: Can I fork StreamHub for my personal use?
**A:** Yes! As long as you keep the same license and don't use it commercially.

### Q: Can I modify it and share my version?
**A:** Yes, but you must:
1. Rename it (can't use "StreamHub")
2. Keep CC BY-NC-SA 4.0 license
3. Credit Aaron Brown
4. Share your source code

### Q: Can I use it at my startup/company?
**A:** No, not without a commercial license. Contact 1aaroncbrown@gmail.com.

### Q: What if I just want to use it internally, not sell it?
**A:** Still requires a commercial license. "For-profit company" = commercial use, regardless of whether you're selling the software itself.

### Q: Can I contribute to the original repository?
**A:** Yes! Contributions are welcome. By contributing, you agree that your code will be licensed under CC BY-NC-SA 4.0 for the free version, and Aaron Brown retains the right to offer it under commercial licenses.

### Q: What if I see someone violating the license?
**A:** Report it to: 1aaroncbrown@gmail.com

---

## Business Model: The MongoDB/Qt Strategy

This is the same model used by successful open-source companies:

| Company | Free License | Commercial License |
|---------|--------------|-------------------|
| **MongoDB** | SSPL (copyleft) | Commercial for hosting |
| **Qt** | GPL/LGPL | Commercial for proprietary apps |
| **StreamHub** | CC BY-NC-SA 4.0 | Commercial for for-profit use |

### Why this works:
1. **Community gets free access** → builds ecosystem
2. **Companies pay for commercial use** → sustains development
3. **Source stays open** → prevents vendor lock-in
4. **You retain control** → can't be exploited

---

## Template: How to Fork Properly

If you want to create a modified version of StreamHub:

### Step 1: Rename Everything
```
StreamHub → [YourProjectName]
```

### Step 2: Update LICENSE
Keep CC BY-NC-SA 4.0, but add attribution:
```
Based on StreamHub by Aaron Brown
Original: [link to StreamHub repo]
Licensed under CC BY-NC-SA 4.0
```

### Step 3: Replace Branding
- New logo/icon (not StreamHub's)
- New app name in code
- New color scheme (optional but recommended)

### Step 4: Document Changes
In README.md:
```markdown
# [YourProjectName]
A fork of StreamHub by Aaron Brown with the following changes:
- [Change 1]
- [Change 2]

Original project: [link]
```

---

## Contact

For licensing questions, commercial inquiries, or violation reports:

**Aaron Brown**
Email: 1aaroncbrown@gmail.com
Location: Seattle, WA

---

Last Updated: May 10, 2026
