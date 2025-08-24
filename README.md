# Discord Status API

Free & Easy to use Discord Status API !

### Bot Created With
<p align="left">
  <img src="https://img.shields.io/badge/-NODE.JS-5FA04E?style=flat&logo=nodedotjs&logoColor=white" height="30" />
  <img src="https://img.shields.io/badge/-SQL-4479A1?style=flat&logo=postgresql&logoColor=white" height="30" />
</p>

### Websited Created With
<p align="left">
  <img src="https://img.shields.io/badge/-TYPESCRIPT-3178C6?style=flat&logo=typescript&logoColor=white" height="30" />
  <img src="https://img.shields.io/badge/-REACT-61DAFB?style=flat&logo=react&logoColor=gray" height="30" />
  <img src="https://img.shields.io/badge/-NEXT.JS-000000?style=flat&logo=nextdotjs&logoColor=white" height="30" />
</p>


## Features

- **Real-time Presence Tracking**: Automatically monitors and updates user status changes
- **Database Caching**: Stores presence data in MySQL for reliable access
- **Fast API**: Quick response times with cached data
- **Rich Activity Data**: Tracks games, Spotify, custom statuses, and more
- **Easy Integration**: Simple REST API endpoint for developers

## Quick Start

### For API Users:

1. **Join our Discord server**: [StatusAPI Discord](https://discord.gg/UJ7UaWQgd7)
2. **Query the API**: `GET https://discordstatus.xyz/api/users/{user_id}`
3. **Use the data**: Receive comprehensive presence information in JSON format
4. **Search example usage**: https://discordstatus.xyz/api/users/1208329627391627284

### Example Request:

```bash
curl https://discordstatus.xyz/api/users/1208329627391627284
```

## Api Response 

```json
{
  "user": {
    "id": "1208329627391627284",
    "username": "connector",
    "globalName": null,
    "discriminator": "0",
    "avatar": "d3809e77d1ccac26bb5958e6c1d47802",
    "avatarURL": "https://cdn.discordapp.com/avatars/1208329627391627284/d3809e77d1ccac26bb5958e6c1d47802.png?size=1024",
    "displayAvatarURL": "https://cdn.discordapp.com/avatars/1208329627391627284/d3809e77d1ccac26bb5958e6c1d47802.png?size=1024",
    "banner": null,
    "bannerURL": null,
    "accentColor": null,
    "hexAccentColor": null,
    "bot": false,
    "createdTimestamp": 1708158632849
  },
  "presence": "online",
  "activities": [
    {
      "name": "Custom Status",
      "type": 4,
      "url": null,
      "details": null,
      "state": "Fullstack Developer.",
      "applicationId": null,
      "timestamps": null,
      "party": null,
      "syncId": null,
      "assets": null,
      "flags": 0,
      "emoji": {
        "animated": false,
        "name": "developer",
        "id": "1363253738395009154",
        "createdTimestamp": 1745095419263,
        "identifier": "developer:1363253738395009154",
        "imageURL": "https://cdn.discordapp.com/emojis/1363253738395009154.webp"
      },
      "buttons": [],
      "createdTimestamp": 1755977737820
    },
    {
      "name": "Visual Studio Code",
      "type": 0,
      "url": null,
      "details": "In src - 0 problems found",
      "state": "Coding README.md @ Line: 14",
      "applicationId": "810516608442695700",
      "timestamps": {
        "start": "2025-08-23T22:53:36.816Z",
        "end": null
      },
      "party": null,
      "syncId": null,
      "assets": {
        "largeText": "Editing a MARKDOWN file",
        "smallText": "Visual Studio Code",
        "largeImage": "mp:external/upBsApcxBvN1KsYpnaBGo2gpIMtYbUQ9ZI90L8HdtgU/https/raw.githubusercontent.com/LeonardSSH/vscord/main/assets/icons/markdown.png",
        "smallImage": "mp:external/Joitre7BBxO-F2IaS7R300AaAcixAvPu3WD1YchRgdc/https/raw.githubusercontent.com/LeonardSSH/vscord/main/assets/icons/vscode.png",
        "largeImageURL": "https://media.discordapp.net/external/upBsApcxBvN1KsYpnaBGo2gpIMtYbUQ9ZI90L8HdtgU/https/raw.githubusercontent.com/LeonardSSH/vscord/main/assets/icons/markdown.png",
        "smallImageURL": "https://media.discordapp.net/external/Joitre7BBxO-F2IaS7R300AaAcixAvPu3WD1YchRgdc/https/raw.githubusercontent.com/LeonardSSH/vscord/main/assets/icons/vscode.png"
      },
      "flags": 1,
      "emoji": null,
      "buttons": [
        "Kill Bot",
        "Portfolio"
      ],
      "createdTimestamp": 1755996673515
    },
    {
      "name": "Spotify",
      "type": 2,
      "url": null,
      "details": "What You Heard",
      "state": "Sonder",
      "applicationId": null,
      "timestamps": {
        "start": "2025-08-24T00:50:46.447Z",
        "end": "2025-08-24T00:54:44.689Z"
      },
      "party": {
        "id": "spotify:1208329627391627284"
      },
      "syncId": "3a3dQOO19moXPeTt2PomoT",
      "assets": {
        "largeText": "What You Heard",
        "smallText": null,
        "largeImage": "spotify:ab67616d0000b2739852437d39690c760e108a14",
        "smallImage": null,
        "largeImageURL": "https://i.scdn.co/image/ab67616d0000b2739852437d39690c760e108a14",
        "smallImageURL": null
      },
      "flags": 48,
      "emoji": null,
      "buttons": [],
      "createdTimestamp": 1755996645644
    }
  ],
  "customStatus": "Fullstack Developer.",
  "timestamp": "2025-08-24T00:51:13.000Z",
  "note": "Presence data retrieved from our database of monitored Discord users."
}
```

