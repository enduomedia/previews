# Reading plan data notes (internal, not linked from the site)

- The printed 2026 PDF shows "9 33:12-33" on Month 12, Day 12 in the Job column. It is Job 33:12-33, and plan.json uses Job 33:12-33.
- data/keyverses.json holds one hand-picked New Testament verse ("nt") and one Old Testament verse ("ot") for each plan day, keyed "month-day". Each reference sits inside that day's readings. Verse text always comes from data/bible/<book>.json.


No Old Testament share card on Month 11 day 16 (keyverses.json ot = null). That day's Ezekiel and Job readings have no verse that reads well on its own, so the page shows only the New Testament card. Days 8 and 12 use Job 8:7 and Job 11:7.

## 2027 plan (data/plan2027.json)

- Source: the Navigators Book-at-a-Time Bible Reading Plan PDF Pastor Duston attached to the Wrike request "The Good Life: 2027 Bible Reading Plan" (Nov 16, 2026). 25 readings a month, two per day. Every chapter of the Bible appears exactly once (Psalms 18, 22, 37, 69, 78, 89, 104, 106, 118 and 119 and Proverbs 10 to 29 are split across days, as printed).
- Each reading has "slot": 0 is the first reading, 1 is the second reading. Month 10, Day 18 has two first readings (2 John and 3 John).
- Single-chapter books (Obadiah, Philemon, 2 John, 3 John, Jude) have an empty label, so they show as just the book name.
- data/keyverses2027.json: {"m-d":{"a":first reading verse,"b":second reading verse}}, null hides that card. Month 10, Day 22 has no card for either reading, so the Verses to Share section is hidden that day.
- The page picks the plan by the year of the day being viewed (2026 plan through Dec 31, 2026; 2027 plan from Jan 1, 2027). Add "pdf" to plan2027.json once the printable booklet is approved, and the Printable Plan button appears.
- Required attribution (from the Navigators PDF) shows under each 2027 day: © 2001, 2004 by The Navigators. All rights reserved. Adapted from The Discipleship Journal.
