[commits]: https://github.com/Wind-Softworks/[REPO_NAME]/commits
[badges/last-modified]: https://img.shields.io/github/last-commit/Wind-Softworks/[REPO_NAME]?label=Last%20Modifed

> [!CAUTION]
> The only *official* host of **WindStream** is [**`windsoftworks.net`**](https://windsoftworks.net). Under no circumstances is **Wind Softworks** responsible for any potential harm caused by using an unofficial fork/rehost of **WindStream**, though anyone is free to fork off of or rehost it as it is under the MIT license. **WindStream** is a static website with none of its own backend infrastructure; it currently fetches binary components directly from Roblox's official content delivery network via [**`setup-aws.[rbxcdn.com]`**](https://setup-aws.rbxcdn.com).
>
> **NOTE:** You must change the source/CDN URL in the JavaScript code to point to your **Wind Softworks** packages for a fully independent deployment system.

---

## WindStream ("Wind Deployment Downloader")

[![Last Modified][badges/last-modified]][commits]

Locally download Roblox deployments (Windows/Mac) directly from your browser!

Hosted officially @ <https://windsoftworks.net>

### What is this?

**WindStream** can assemble plain resources directly from Roblox's S3 storage bucket into a runnable format. **Everything is fetched locally in your browser, without any additional required server resources!**

### Usage

```txt
[*] USAGE: [https://windsoftworks.net/?channel=](https://windsoftworks.net/?channel=)<CHANNEL_NAME>&binaryType=<BINARY_TYPE>&version=<VERSION_HASH>

    Binary Types (Roblox Defaults):
    * WindowsPlayer
    * WindowsStudio64
    * MacPlayer
    * MacStudio

    Extra Notes:
    * If `channel` isn't provided, it will default to "LIVE" (the production channel)

    The `blobDir` query argument can be used for specifying where WindStream should fetch 
    deployment files from (e.g., "/mac/arm64/" instead of "/mac/").
