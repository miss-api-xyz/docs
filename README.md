## 🔗 Base URLs
ᅠ• Main - **http://miss-api.xyz/** <br>
ᅠ• API - **http://miss-api.xyz/api** <br>

<br><br>

## 📥 Request and get API key

Simple request to miss-api:
```js
require("node-fetch")("http://miss-api.xyz/api/v2/cat", {
    headers: {
        "Content-Type": "application/json",
        "Authorization": `User YOUR TOKEN`,
    },
}).then(x => x.json().then(b => console.log(b)));
```
You can also use our official wrappers to send requests. [miss-api.js (JavaScript)](https://github.com/miss-api-xyz/miss-api.js) / [miss-api.py (Python)](https://github.com/miss-api-xyz/miss-api.py)<br>
To get API key: <br>
Log in to the site through your Discord account, and pick up the key that will be given to you. <br>
Where to log in? [Click on me!](http://miss-api.xyz/aouth)

<br><br>

## 📑 Endpoints

|  Animals  |                  Returns                   |
|-----------|--------------------------------------------|
| `cat`     | `{ code: 200, message: "", image: <url> }` |
| `dog`     | `{ code: 200, message: "", image: <url> }` |
| `koal`    | `{ code: 200, message: "", image: <url> }` |
| `fox`     | `{ code: 200, message: "", image: <url> }` |
| `pand`    | `{ code: 200, message: "", image: <url> }` |
| `snake`   | `{ code: 200, message: "", image: <url> }` |
| `squirrel`| `{ code: 200, message: "", image: <url> }` |
| `turtle`  | `{ code: 200, message: "", image: <url> }` |
| `wolf`    | `{ code: 200, message: "", image: <url> }` |
| `giraffe` | `{ code: 200, message: "", image: <url> }` |

<br>

| NSFW-Anime |                  Returns                   |
|------------|--------------------------------------------|
| `hentai`   | `{ code: 200, message: "", image: <url> }` |
| `hentaigif`| `{ code: 200, message: "", image: <url> }` |
| `ass`      | `{ code: 200, message: "", image: <url> }` |
| `pussy`    | `{ code: 200, message: "", image: <url> }` |
| `boobs`    | `{ code: 200, message: "", image: <url> }` |

<br>

|  NSFW-Real  |                  Returns                   |
|-------------|--------------------------------------------|
| `porn`      | `{ code: 200, message: "", image: <url> }` |
| `real_ass`  | `{ code: 200, message: "", image: <url> }` |
| `real_pussy`| `{ code: 200, message: "", image: <url> }` |
| `real_boobs`| `{ code: 200, message: "", image: <url> }` |

<br>

|  SFW  |                  Returns                   |
|-------|--------------------------------------------|
| `hug` | `{ code: 200, message: "", image: <url> }` |
| `kiss`| `{ code: 200, message: "", image: <url> }` |
| `cry` | `{ code: 200, message: "", image: <url> }` |
| `kill`| `{ code: 200, message: "", image: <url> }` |
| `sex` | `{ code: 200, message: "", image: <url> }` |
| `view`| `{ code: 200, message: "", image: <url> }` |

<br>

| Reactions |                  Returns                   |
|-----------|--------------------------------------------|
| `angry`   | `{ code: 200, message: "", image: <url> }` |
| `dance`   | `{ code: 200, message: "", image: <url> }` |

<br>

| Other  |                  Returns                   |
|--------|--------------------------------------------|
| `meme` | `{ code: 200, message: "", image: <url> }` |

<br><br><br>

## ⁉️ Errors during requests

|          Description          |                             Returns                            |
|-------------------------------|----------------------------------------------------------------|
| `404` - Non-existent endpoint | `{ code: 404, message: "Non-existent endpoint", image: null }` |
| `401` - Inactive API key      | `{ code: 401, message: "Unauthorized user", image: null }`     |
| `200` - Successfull           | `{ code: 200, message: "", image: <url> }`                     |
