1. No comments in sql
2. Can't do more than one thing in any one sql query
3. Terrible sql editing:
	-no code highlighting
	-ANY formatting is lost when you close the query
	-no 'select all' shortcut. WTF?
	-no undo
	-no tab character allowed
4. Ridiculous, non-standard join syntax
5. Does not respect parameters in file DSNs
6. Minimal control over data types
7. Text file import + append just broken, cannot specify data types of columns which means access guesses them. Often incorrectly.
8. Cancel query broken = locked up access all over your screen
9. Basically single user only.
10. Takes out ridiculous locks on linked tables, making it disturbingly easy to wreak havoc on external systems.
11. 2Gb size limit on databases.
12. Can't export data from a table that has spaces in the name. wtf?
13. VBA code re-use difficult at best.
14. VBA code maintenance very painful.
15. When a macro is running that takes some time the window completely freezes, meaning you can't minimise it, move it etc.
16. Cryptic ODBC timeout errors
17. ODBCTimeout default of 60 seconds
18. "Your network access was interupted, please close the database and open it again"
19. Object view cleared if you disconnect + reconnect connection to currently open file
20. If a file is read only then you can't create a query.
21. Automatic compact and repair turning a simple file close in to a 5 minute operation. And don't even think about following the onscreen instructions to hold esc to cancel, you'll just lock up access and it'll just squat there ony our screen for an eternity.
22. No file name displayed in the main window.
23. Got dates you want to import from excel? Let me completely ignore that formatting for you and use the completely arbitrary american format instead.
24. Query performance comparable to a pen and paper.
25. No variables.
26. Want to open a database while another is busy doing stuff? No dice.
27. Date literals in sql converted to shitty american format when query is closed and re-opened. Clear, unambiguous queries like 'delete from tbl where dt < #1 nov 2013#' become the far more confusing 'delete from tbl where dt < #10/1/2013#'
28. List of values for filtering lists is not cached, so on any table > 5 rows there's always a very appreciable lag between clicking the filter button and actually being able to do anything. Wouldn't matter if you could just query directly bu that's a 15 click process in itself.
29. An integer that takes up 8 bits? Better convert it to text and pretend it isn't a primary key.
30. "The query planner ran out of resources because your query is too complex. Please rewrite your query." is an actual error message.
31. When you run a macro, the sql for each step is parsed in turn. This means that you can get to the end of some enourmous macro only to be told you made a tiny typo that could and should have been caught as soon as you strted the macro.
32. Try to open a view, 'Invalid procedure call'. What am I meant to do with that? Just give me something, anything, to work with.
33. Linked table manager: if you try and change any table links and it fails on one it will fail any following links that you've just changed because they can't do the most basic error handling.
34. Type mismatch error: go fuck yourself. No one thought it might be nice to include some info about where the error is? Or just anything at all that isnt just a 'fuck you'?
35. No write permission on some external table? Let me just turn your database in to a 500mb blob of shit.

n+1. This list has n entries, and n is far too large considreing every single entry is a real WTF moment.