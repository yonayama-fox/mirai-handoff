Task:   Take ownership of NJF 在庫管理 (ingredient + packaging stock control and reorder lists) and report the starting state.
Where:  NJF stock master — `stock.csv` (ingredients, ¥/g, 購入先) and the NJF Operations Sheet stock tab. Tell me which one you treat as master.
Done:   (1) Every live stock item has 補充時点 (reorder point) and 補充量 (reorder qty) filled. (2) Salt written in as ¥3,000 / 2,000g (¥1.50/g). (3) A reorder list for this week exists.
Output: Status line; master file + path; count of items with/without reorder rules; this week's reorder list (item, qty, supplier, est. ¥); open questions for Starchild.
Limit:  300 words / 25 list rows.

Context (from Claude, 2026-11-22 costing snapshot — do not override without telling me):
- Owners: Grok = stock counts, reorder points, reorder lists, supplier tracking. Claude = recipes, 原価/costing, pricing, product docs. Starchild approves all orders.
- **Do not place any order or pay anything.** Draft the list; Starchild orders.
- Existing reorder habits (Starchild): order 2 units when 1 left — rice 30kg, coconut oil, date paste, walnuts, almonds, sesame, soy milk, barley miso. Organic sugar 25kg: refill at 6kg. Cacao 2kg bags: order 2 when the last is opened. At the halfway point an 「注文 + item」 card goes in the order box.
- Status flags: black sesame needs re-buy; white sesame temporarily unavailable at Watanabe (find alternative?).
- Removed items (don't track): shortening, black salt, banana, peanuts, pecans, beet powder, Shirakami yeast.
- Packaging to track too: 4×4おやつ袋, clear individual bags, kraft gusset S/M/L, 山のおやつ seal, ありがとうシール, 2g silica gel, 広口400 jars (ちゅうくう, 46/¥2,700), 60-size boxes, labels (SEAL EVO ~1,000/batch).
- Usage per batch (for consumption maths):
  - cmb 1,480g: coconut oil 900, soy yogurt 300, unscented rapeseed 170, 塩麹 80, 大豆レシチン 30
  - gor mixer batch (≈26×300g): walnuts 1,088, raisins 1,440, oats 1,728, date paste 640, coconut fine 448, maple 960 OR honey 820, almonds 704, cacao 320, cinnamon 112, 麻炭 1.5, salt 5
  - yno per 100 pcs: rice flour ~1,860, sugar ~930–990, sesame ~930, potato starch ~930, roasted rapeseed ~830–860, soy milk ~540–560, salt ~21 (miso flavour: barley miso 527, no salt)
  - soy yogurt 5L batch: soy milk 5L + Blueman packet or 500g backslop; 塩麹: koji 800, salt 280, water 280
- Demand anchors: Juguard ~10kg cmb / 2–3 wks; Hoshino ~250 yno / 1.5–2 months.
- Going forward: answer any later `inbox/YYYYMMDD-zaiko-status.md` brief with current low items + reorder list in the same format.
