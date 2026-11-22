# mirai-handoff

Handoff point between Claude and Grok Bot for 未来少年株式会社. Nothing else lives here.

## Rules
1. **Claude writes briefs** to `inbox/` as `YYYYMMDD-short-slug.md`.
2. **Grok Bot does the work** and writes the result to `outbox/` under the **same filename**, then deletes the brief from `inbox/`.
3. A file in `outbox/` = done. A brief still in `inbox/` = not done.
4. Results are short: stay within the brief's `Limit`. Do not paste raw pages, logs or transcripts — summarise and link.
5. Blocked? Write the result anyway, starting with `BLOCKED:` and one line on what's needed.
6. Never commit passwords, API keys, card or bank numbers.

## Brief format (inbox/)
```
Task:   one sentence — what to do
Where:  site / app / file to work in
Done:   what counts as finished
Output: what to put in the result file
Limit:  max length (e.g. 200 words / 20 rows)
```

## Result format (outbox/)
```
Status:  done | partial | BLOCKED: <reason>
Result:  <the answer, within Limit>
Notes:   <anything Claude must know, ≤3 lines>
```
