# SQL-keycounts
SQLite queries to be used with [Benign-Key-Logger](https://github.com/Ga68/benign-key-logger) to help understand your keycount data

The keylogger program will create an SQLite database for you, which has a few queries built in. I found that I wanted some more advanced queries, so those are provided here.

## Included Queries:
- Key counts with combined cases (g and G counts as the same key)
- Separated counts for the Right hand and the Left hand (versions for both Colemak and QWERTY)
- "Limited" bigrams, trigrams, quadgrams, etc. "Limited" here means the counts exclude non-alphanumeric keys such as Shift, Esc, VOL_UP, VOL_DOWN, etc


## Using These Queries
The keylogger program will create an SQLite database for you. In an effort to let you continue to use that same database file which holds your keycounts, and to keep in the same open philosophy of Benign Key Logger, I've written these queries as a series of plain text files, which you can simply paste into a new "View" in SQLiteStudio. 

*IE: The user is able to see exactly what is happening. There is no possible trickery here with your keylog file. You get to enter the SQL queries yourself into the program, as opposed to opening an opaque file.*

**To use:**
1. Open your "key_log.sqlite" file in SQLiteStudio
2. With the icons at the top, click "Create a View" (usually the 6th icon from the left)
3. Name the view
4. Click the large empty field below, and paste the contents of the relevant txt file from this repo
5. Hit the green checkmark above the field you just pasted into
6. Just to the right, you can see that you are currently in the "Query" tab. Now select the "Data" tab
7. Analyze your keycounts