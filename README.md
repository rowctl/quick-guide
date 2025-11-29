**Prevent disasters** → F‑keys inject guardrails that stop accidental mass updates or deletes  
**Recover instantly** → History window logs the last 50 queries with restore/copy/pin  
**Never lose critical scripts** → Pins library stores up to 25 permanent queries with tags and search
**One‑keystroke workflows** → Alt+0 + F‑keys = crash‑safe execution at developer speed  


- [Safe SQL Keys](#quick-guide--safe-sql-keys)
- [SQL History Window](#quick-guide--sql-history-window)
- [SQL Pins Library](#quick-guide--sql-pins-library)


#### Quick Guide — Safe SQL Keys
```markdown
# Execution Keys
- Keyboard shortcuts for safe execution of SQL blocks.

| Key      | Action                | What It Does                                                    
|----------|-----------------------|-----------------------------------------------------------------
| Alt + 0  | Execute Current Block | Runs the SQL block under the cursor — no need to highlight first

# Injection Keys (add safety commands)
- Extra keystrokes that inject safety clauses into your SQL, 
  preventing accidental mass updates or deletes.

| Key | Action               | What It Does      
|-----|----------------------|-----------------------------------------------------------------------
| F9  | Safe Transaction Run | Wraps query in `BEGIN TRANSACTION …` with manual COMMIT/ROLLBACK 
| F10 | Rollback             | Inserts `ROLLBACK;` — safe exit, no changes saved                 
| F11 | Commit               | Inserts `COMMIT;` — finalize changes explicitly                    
| F12 | Full Safe Execute    | Adds block: TRY/CATCH with auto‑COMMIT on success, ROLLBACK on error

# How It Works
- Steps to safely run queries with injected guardrails.
- Place cursor inside your query.  
- Use **F‑keys** to inject safety scaffolding.  
- Press **Alt + 0** to execute the block safely.  

# Why These Keys Matter
- Benefits of using safety keys in daily SQL workflows.
- **Safety first** → guardrails against accidental mass updates  
- **Velocity** → one‑keystroke workflows, no wasted motions  
- **Clarity** → explicit COMMIT/ROLLBACK builds good habits  
- **Crash‑proof** → F12 + Alt + 0 ensure clean error handling and safe execution

```

#### Quick Guide — SQL History Window
```markdown
# Recording
- Every time you press **Alt + 0** to execute a query,  
  the SQL block is **recorded in the SQL History window**.
- The history keeps the **last 50 queries executed**.  
  Old entries roll off automatically as new ones are added.

# Query Cards (per entry)

| Control  | Action                          | What It Does           
|----------|---------------------------------|-------------------------------------------------------
| Pin      | Store query in SQL Pins Library | Permanent reuse beyond rolling history                
| Restore  | Load query back into editor     | Re‑hydrate past query instantly                       
| Copy     | Copy query text                 | Fast reuse in other contexts                          
| Context  | Right‑click menu with copy      | Discoverable fallback for copy action                 

# Metadata
- Added date → when query was executed  
- Query text → the SQL block itself  
- Duration → execution time for query  

# Search
- At the bottom of the SQL History window is a **search bar**.  
- Quickly filter and find queries across the last 50 entries.  
- Supports fast recall under pressure (up to 50 entries in Community/Lite).

# Why It Matters
- **Traceability** → review exactly what was executed.  
- **Velocity** → restore or copy without friction.  
- **Safety** → pin important queries so they don’t roll off.  
- **Clarity** → search makes history usable even at scale.

```
#### Quick Guide — SQL Pins Library
```markdown
# Productivity
- Stores queries you’ve **pinned** from history.  
- Permanent, limited to 25 entries.  
- Ideal for **favorite queries**, **templates**, or **critical scripts**.  
- Organized for quick recall and reuse.

# Pin Cards (per entry)

| Control  | Action                          | What It Does         
|----------|---------------------------------|-------------------------------------------------------
| Play     | Insert + highlight + execute    | Runs query at cursor with visible block scope         
| Copy     | Copy query text                 | Fast reuse in other contexts                          
| Unpin    | Remove from Pins Library        | Declutters permanent store                            
| Context  | Right‑click menu                | Extra options: Copy, Insert into editor               
| Tag      | Add a tag to card               | Organize pins for search and reuse                    

# Metadata
- Added date → when query was added to library  
- Query text → the SQL block itself  
- Last duration → execution time from last run  

# Search
- At the bottom of the Pins Library is a search bar.  
- Filter by tags or text to find pinned queries quickly.
- Clicking a tag triggers search for that tag; clicking again resets search.
- Supports fast recall under pressure (up to 25 pins in Community/Lite).

# Why It Matters
- **Safety** → permanent storage of critical queries.  
- **Velocity** → Play button executes instantly with visibility.  
- **Clarity** → tags + search make pins usable at scale.  
- **Control** → unpin keeps library clean.

```

*Note: This guide covers the Community and Lite versions.  
Advanced features will be documented separately when available.*




