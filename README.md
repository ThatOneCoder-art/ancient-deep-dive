# ancient-deep-dive

## Publish approved entries

1. Open the private editor in the site, approve the entries you want public, then select **Export approved**.
2. On GitHub, open **Actions → Publish approved content → Run workflow**.
3. Paste the downloaded `approved-entries.json` file contents into the `approved_content` field and run the workflow.

The workflow validates the package, commits it to `content/approved-entries.json`, and pushes the commit to `main`. The site loads that committed file so approved entries are visible to everyone after GitHub Pages redeploys.