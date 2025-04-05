# feed2ai
Use N8N workflow to read your favorites RSS feeds :
- CSV file to provide RSS feeds as input
- Google Gemini AI agent to build brief sumary of articles
- HTML output could be send to text file
- HTML output could be send to email address
- HTML output could be send to Matrix room

## N8N Workflow
![image](https://github.com/user-attachments/assets/8d47e9cf-d042-4e8b-9f50-d25041c86c79)

## Workflow file
- JSON file to import in your N8N instance could be found [here](https://github.com/vmapps/feed2ai/blob/main/feed2ai.json)

## Configuration
- ``FILE_IN`` : string : ``"/home/data/config/<yourfeeds>.csv"``
- ``FILE_OUT`` : string : ``"/home/data/output/<yourfile>.html"``,
- ``"DEBUG"`` : boolean : ``<true|false>``
- ``"OUPUT_FILE"`` : boolean : ``<true|false>``
- ``"OUPUT_EMAIL"`` : boolean : ``<true|false>``
- ``"OUPUT_MESSAGE"`` : boolean : ``<true|false>``
- ``"OUPUT_LANG"`` : string : ``<yourlanguage>`` (ex: "french")

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

## Email output sample
![image](https://github.com/user-attachments/assets/2b696e3c-dfd3-49ec-806f-ec759abcd391)


