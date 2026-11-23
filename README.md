\# n8n Workflows: Product Approval Pipeline



Two n8n workflows for an AI-assisted product import with human approval.



\- 01\_check\_new\_products.json: scrapes new supplier products, skips duplicates, adds them to Google Sheets and translates them to German with OpenAI. Triggers: webhook (test page button), manual, daily at 07:00.

\- 02\_upload\_approved\_products.json: uploads products approved in Google Sheets to the shop API and updates their status (Hochgeladen / Abgelehnt / Fehler).



Full project (scraper, shop, test page, setup): https://github.com/jins28/product-approval-pipeline



Import: n8n → Create workflow → ⋯ → Import from file. Then select your own Google Sheets, OpenAI and Header Auth credentials.

