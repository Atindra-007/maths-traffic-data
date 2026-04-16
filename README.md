# Maths Keyword Matcher

A simple web tool to match maths topics with high-volume keywords from your database.

## How to use

1. Open the tool in your browser
2. Upload your `High_Volume_Maths_Keywords.xlsx` once — it saves to browser storage permanently
3. Type any maths topic and hit Search
4. See matching keywords split into **Closely Related** and **Related**

## How to host on GitHub Pages

1. Create a new GitHub repository (e.g. `maths-keyword-matcher`)
2. Upload `index.html` to the repository
3. Go to **Settings → Pages**
4. Under **Source**, select `main` branch and `/ (root)` folder
5. Click **Save**
6. Your tool will be live at `https://yourusername.github.io/maths-keyword-matcher`

## Excel file format

The tool reads all sheets from your Excel file:

- **Sheet1** — column A contains the full keyword list
- **Category sheets** (Arithmetic, Algebra, Geometry, etc.) — column B contains keywords with the sheet name used as the category label
- **Summary sheet** — skipped automatically

## Storage

Keywords are saved in browser `localStorage` — they stay saved across visits on the same browser/device. No data is sent to any server.

To update the database, simply upload a newer version of the Excel file.
