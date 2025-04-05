# feed2ai
Use N8N workflow to read your favorites RSS feeds :
- CSV file to provide RSS feeds as input
- Google Gemini AI agent to build brief sumary of articles
- HTML output could be send to text file
- HTML output could be send to email address
- HTML output could be send to Matrix room

## N8N Workflow
<kbd>![image](https://github.com/vmapps/feed2ai/blob/main/screenshots/n8n-workflow.png)</kbd>

## Workflow file
- JSON file to import in your N8N instance could be found [here](https://github.com/vmapps/feed2ai/blob/main/feed2ai.json)

## Configuration
```
{
  "debug": true,
  "ai": {
    "agent": true,
    "lang": "french"
  },
  "rss": {
    "feeds": "/home/data/your-feeds.csv",
    "maxitems": 5
  },
  "file": {
    "active": true,
    "name": "/home/data/your-summary.html"
  },
  "email": {
    "active": true,
    "from": "RSS Scrapper <your@sender>",
    "to": "your@recipient",
    "subject": "RSS breaking news"
  },
  "chat": {
    "active": true,
    "room": "!your-room-id:matrix.org"
  }
}
```

## Feeds configuration sample
```
site,url,active
Ars Technica,https://arstechnica.com/security/feed/,true
Bleeping Computer,https://www.bleepingcomputer.com/feed/,true
Dark Reading,https://www.darkreading.com/rss.xml,false
Data Security Breach,http://datasecuritybreach.fr/feed/,false
Dider Stevens,http://blog.didierstevens.com/feed/,false
ESET,http://feeds.feedburner.com/eset/blog/,false
Insinuator,http://www.insinuator.net/feed/,false
```

## Email output samples
- using english language as output

<kbd>![image](https://github.com/vmapps/feed2ai/blob/main/screenshots/email-english.png)</kbd>

- using french language as output

<kbd>![image](https://github.com/vmapps/feed2ai/blob/main/screenshots/email-french.png)</kbd>

- using spanish language as  output

<kbd>![image](https://github.com/vmapps/feed2ai/blob/main/screenshots/email-spanish.png)</kbd>





