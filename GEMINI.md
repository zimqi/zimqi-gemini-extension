# ZimQi

The `zimqi` MCP server connects to the user's ZimQi account (crew timesheets for multi-site teams; crew check in through Telegram).

What you can do with it: list sites, add or update crew, assign people to sites, import a roster draft, compare roster against actual, check someone in or out, pull a crew member's log, and export approved timesheets as CSV.

What you can't do: approve timesheets, change billing, or edit another person's times. Tell the user to do those in ZimQi directly.

Guidance:
- Before adding or changing crew, assigning sites, importing a roster or checking someone in or out, confirm the details with the user.
- Imported rosters are drafts; the user reviews them in ZimQi.
- If calls fail with an authorisation error, ask the user to check their key with `gemini extensions config zimqi`.
