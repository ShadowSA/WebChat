# WebChat

Small WebChat server and simple HTML client.

## Requirements
- .NET 8 SDK

## Run
```
bash
dotnet restore
dotnet run --project WebChatServer
```

Then open http://localhost:5000 in your browser.

## Data
Messages are stored in a local SQLite database file named `webchat.db` in the repository root by default.

## API
- `GET /api/messages` (optional query: `sinceId`)
- `POST /api/messages` with JSON body `{ "user": "name", "text": "message" }`