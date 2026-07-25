<img width="671" height="539" alt="Screenshot 2026-07-25 203134" src="https://github.com/user-attachments/assets/f5032240-e48c-4cda-b9e1-948578fd0585" /># GroupDNA---WhatsApp-Analytics
A WhatsApp group chat analytics tool built with pure Python Fundamentals - no pandas, no matplotlib, no regex. Parses chat exports and generates activity heatmaps, word frequency, response patterns, and personality archetypes for every member.

**"Spotify Wrapped, but for your friend group."**

GroupDNA is a Python-based WhatsApp chat analyzer built entirely with core language 
fundamentals and NumPy — no external libraries like pandas, matplotlib, or regex. 
It reads a raw WhatsApp chat export, parses every message, and generates a full 
behavioural analytics report: who's the most active, who's the night owl, what 
words the group uses most, and a personality archetype for every members.

## 🚀 What It Does

- **Parses** raw WhatsApp `.txt` exports, handling system messages, media-omitted 
  entries, and deleted messages as separate edge cases
- **Group Overview** — total messages, date range, per-person message counts
- **Busiest Day & Hour** — when the group is most active
- **Activity Heatmap** — a 6×24 NumPy matrix rendered as a text-based heatmap 
  showing each person's hourly activity pattern
- **Top Words** — the group's most-used words, shown as a bar chart
- **Response Patterns** — average reply speed and longest silent streaks per person
- **Personality Archetypes** — assigns each member one of 8 data-driven archetypes 
  (The Spammer, The Night Owl, The Ghost, etc.) based on quantitative rules

## 🛠️ Built With — Constraints

This project was intentionally built using **only Python fundamentals + NumPy**, 
to demonstrate that complex analytics don't require heavy libraries.

**Used:** 'open()', loops, dictionaries, sets, string methods, list/dict 
comprehensions, 'datetime.strptime', NumPy ('np.zeros', indexing, '.sum()')

**Avoided (by design):** pandas, matplotlib, 're' (regex), 
'collections.Counter'/'defaultdict', any pre-built chat-analysis or ML library

## ▶️ How to Run

1. Open the notebook in Google Colab
2. Upload `hostel_bois.txt` to the same Colab session (or place it next to the 
   notebook if running locally)
3. Run all cells top to bottom (**Runtime → Run all**)
4. The final formatted report prints at the end of the notebook

## 🎯 About This Project

Built as part of The Unlox Academy's Week 1 Minor Project. The dataset is 
synthetic and specifically engineered so each participant's messaging behavior 
maps to a distinct, verifiable personality archetype — testing whether the 
detection logic is written correctly.
