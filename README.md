# ZimQi extension for Gemini CLI

Connects [Gemini CLI](https://geminicli.com) to [ZimQi](https://zimqi.com.au), crew timesheets for small multi-site teams who check in through Telegram.

ZimQi is a hosted service. This repository holds only the extension config (`gemini-extension.json`) and a short context file. It contains no ZimQi source code and no keys. The extension connects to ZimQi's remote MCP server at `https://zimqi.com.au/mcp` (streamable HTTP, API key as a bearer token). It's also listed in the official MCP Registry as `au.com.zimqi/timesheets`.

## Get an API key

1. Sign up or log in at https://zimqi.com.au. MCP access is on every plan, including the free trial (30 days or 100 credits).
2. Go to **Integrations & API** and create a key.

Paid plans: Starter A$19, Solo A$49, Team A$149, Scale A$299 per month, ex GST.

## Install

```
gemini extensions install https://github.com/zimqi/zimqi-gemini-extension
```

Gemini CLI asks for your ZimQi API key during install and stores it in your system keychain. To change it later:

```
gemini extensions config zimqi
```

## What it can do

- List sites
- Add or update crew
- Assign people to sites
- Import a roster draft
- Compare roster against actual
- Check someone in or out
- Pull a crew member's log
- Export approved timesheets as CSV

It can't approve timesheets, touch billing or edit someone else's times.

## Links

- Docs: https://zimqi.com.au/integrations
- Privacy: https://zimqi.com.au/privacy
- Support: gorky@zimqi.com.au

ZimQi is a product of Findertech Australia Pty Ltd, trading as ZimQi Online (ABN 42 631 675 673).
