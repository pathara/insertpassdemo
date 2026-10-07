AsiaPay Lucky Draw Prototype
==============================

Files:
- lucky-draw.html: Guest/Kiosk Lucky Draw
- lucky-draw-dashboard.html: Staff/Admin dashboard

Prototype data sharing:
Both files use the same localStorage key: asiapayLuckyDrawConfigV1.
Therefore they can share configuration/history when served from the same origin.

Important:
- This is a prototype. The guest draw currently uses browser-side weighted random selection.
- TEST mode does not reduce stock; LIVE mode reduces prize stock.
- Production must move draw selection, stock updates, daily limits and transaction history to a backend/database.
- Prevent duplicate draws with a server-side transaction/lock.
- Add authentication to the dashboard before production.
