[commits]: [WIND_REPO_URL]/commits
[badges/last-modified]: https://img.shields.io/github/last-commit/[WIND_REPO_OWNER]/[WIND_REPO_NAME]?label=Last%20Modifed

> [!CAUTION]
> The only *official* host of **[WIND_NAME]** is [**`[WIND_SUBDOMAIN].[WIND_DOMAIN]`**](https://[WIND_SUBDOMAIN].[WIND_DOMAIN]). Under no circumstances is **Wind Softworks** responsible for any potential harm caused by using an unofficial fork/rehost of **[WIND_NAME]**, though anyone is free to fork off of or rehost it as it is under the MIT license. **[WIND_NAME]** is a static website with none of its own backend infrastructure, binaries are fetched directly from Roblox's official content delivery network via [**`setup-aws.[rbxcdn.com]`**](https://setup-aws.rbxcdn.com).

## [WIND_NAME] ("Wind Deployment Downloader")

[![Last Modified][badges/last-modified]][commits]

Locally download Roblox deployments (Windows/Mac) directly from your browser!

Hosted officially @ <https://[WIND_SUBDOMAIN].[WIND_DOMAIN]>

### What is this?

**[WIND_NAME]** can assemble plain resources directly from Roblox's [`setup`](https://setup.rbxcdn.com) S3 storage bucket into a format the user would expect to be able to directly extract/run from. **Everything is fetched locally in your browser, without any additional required server resources!**

### Usage

```txt

[*] USAGE: https://[WIND_SUBDOMAIN].[WIND_DOMAIN]/?channel=<CHANNEL_NAME>&binaryType=<BINARY_TYPE>&version=<VERSION_HASH>

    Binary Types:
    * WindowsPlayer
    * WindowsStudio64
    * MacPlayer
    * MacStudio

    Extra Notes:
    * If `channel` isn't provided, it will default to "LIVE" (the production channel)

    You can also use an extra query argument we provide, `blobDir`, for specifying
    where [WIND_NAME] should fetch deployment files from. This is useful for using different
    relative directories than normal for a certain client type, such as for fetching
    stuff from /mac/arm64/ instead of /mac/

    Blob Directories (Examples):
    * "/" (Default for WindowsPlayer/WindowsStudio64)
    * "/mac/" (Default for MacPlayer/MacStudio)
    * "/mac/arm64/"
    ..
