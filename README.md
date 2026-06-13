<div align="center">

# Providra: Syncler Provider and Vendor Packages

<img width="1672" height="941" alt="main-logo" src="https://github.com/user-attachments/assets/6984e645-de76-4861-b5e1-d039922c3479" />


### Bridge compatible Stremio addons and Nuvio plugins into Syncler

[![Open Beta](https://img.shields.io/badge/status-open%20beta-orange)](https://github.com/dtankdempsey2/Providra/releases)
[![Latest Release](https://img.shields.io/badge/download-latest%20release-blue)](https://github.com/dtankdempsey2/Providra/releases)

</div>

> [!IMPORTANT]
> **Providra is currently in open beta.**
> Bugs and compatibility issues may still occur. Feedback and bug reports are appreciated while the app continues to improve.

## 🌐 Hosted Version

Providra is also available as a lightweight hosted web version at **[providra.com](https://providra.com/)**.

The hosted version supports compatible **Stremio addons** and does not require downloading an APK or setting up your own server.

### Quick Start

1. Open **[providra.com](https://providra.com/)**.
2. Enter your Stremio addon name.
3. Generate and copy your vendor URL.
4. Add the vendor URL in Syncler.
5. Enter your addon manifest URL when prompted.

> [!NOTE]
> The hosted version currently supports **Stremio addons only** and uses rate limiting.
> For Nuvio plugin support, unrestricted usage, and additional features, use the downloadable version below.

> [!WARNING]
> The hosted instance is provided as a free, best-effort service. Availability is not guaranteed.
> If demand places excessive strain on the server, access may be limited, suspended, or discontinued without notice.
> For the most reliable experience, use the downloadable self-hosted version. Docker and Node.js deployment options are also coming soon.

## 📥 Download

The latest versions of Providra can always be found on the **[Releases page](https://github.com/dtankdempsey2/Providra/releases)**.

### Current Open Beta: `v0.1.0-beta.7`

For the best experience, it is recommended that you use `Syncler beta 2.1.1.7 (v302010107)` or higher, especially when using configured Stremio addon manifests that return debrid resolved links. [Get the Syncler Beta Version Here](https://beta.syncler.net/)

| Device Architecture | Download                                                                                                                                                         |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `arm64-v8a`         | [Download Providra for 64-bit Android devices](https://github.com/dtankdempsey2/Providra/releases/download/v0.1.0-beta.7/providra-v0.1.0-beta.7-arm64-v8a.apk)   |
| `armeabi-v7a`       | [Download Providra for 32-bit Android devices](https://github.com/dtankdempsey2/Providra/releases/download/v0.1.0-beta.7/providra-v0.1.0-beta.7-armeabi-v7a.apk) |

> [!TIP]
> Most modern Android phones, Android TV devices, and Fire TV devices use the `arm64-v8a` version.
> Try the `armeabi-v7a` build if your device is older or the 64-bit APK will not install.

## 🔑 TMDB API Key Required

Providra requires a free **TMDB API key** to function.

You can create a TMDB account and request your API key by following the official **[TMDB API Getting Started guide](https://developer.themoviedb.org/docs/getting-started)**.

> [!TIP]
> TMDB recommends completing the API key registration process from a desktop browser.

## 🔍 What Is Providra?

Providra is an Android bridge app that allows Syncler to use compatible **Stremio addons** and **Nuvio plugins** when searching for source links.

Traditionally, Syncler users rely on third-party vendor packages containing custom scrapers. Providra expands those options by connecting Syncler to two additional communities that are already building and maintaining their own source providers.

Depending on the addons or plugins you configure, Providra can return debrid-supported sources and compatible free-hosting links. This means that even users without Syncler+ should be able to find playable sources through supported services.

## ⚙️ How Does It Work?

Providra runs a lightweight local server on the same Android device as Syncler. It converts compatible Stremio addon and Nuvio plugin responses into a format that Syncler can understand.

The setup process is simple:

1. Choose whether you want to use **Addons** or **Plugins**.
2. Browse the supported Stremio or Nuvio marketplace.
3. Add the manifest URLs for the services you want to use.
4. Start the local Providra server.
5. Copy the generated vendor package URL.
6. Add that URL to Syncler.

Once everything is configured, Providra handles the communication between Syncler and your selected addons or plugins.

## 🚀 Why Use Providra?

Syncler provides an excellent interface for browsing and watching movies and TV shows, but it does not search for playable source links by itself. Users have to install third-party vendor packages containing custom scrapers that locate sources for Syncler to display and play.

Providra takes a different approach.

Instead of limiting users to scrapers made specifically for Syncler, Providra creates a bridge to the wider Stremio and Nuvio ecosystems. This gives Syncler users access to more community-developed providers while allowing them to continue using the media interface they already enjoy.

## ✨ Features

* 🔌 Bridge compatible Stremio addons into Syncler
* 🧩 Bridge compatible Nuvio plugins into Syncler
* 📱 Run the server locally on your Android device
* 🔗 Generate a Syncler-compatible vendor package URL
* ➕ Add and manage multiple addon or plugin manifests
* 🎬 Process compatible debrid and free-hosting sources
* 🔒 Keep your Providra configuration on your own device
* 📺 Use an interface designed for both mobile and TV devices

## 📸 Screenshots

<img width="1654" height="944" alt="Providra home screen" src="https://github.com/user-attachments/assets/f6c8fb3a-33d5-4a32-9b72-c9f13e9fd850" />

<img width="1643" height="926" alt="Providra addon configuration screen" src="https://github.com/user-attachments/assets/42bc5560-1a93-4b63-9d14-185a1f628e75" />

<img width="1653" height="896" alt="Providra plugin configuration screen" src="https://github.com/user-attachments/assets/bee15c1e-1ad0-4df1-9687-9fdd50b87a85" />

<img width="1651" height="892" alt="Providra settings screen" src="https://github.com/user-attachments/assets/eee0b341-f71f-4ed9-801e-7497b91a2c4e" />

## 🧪 Open Beta Notice

Providra is still under active development. During the open beta, you may encounter bugs, unsupported providers, or device-specific issues.

Not every Stremio addon or Nuvio plugin is guaranteed to be compatible. Results will vary depending on the services you configure and whether those services are currently available.

## 📺 Additional Device Support

Please do not submit requests for Providra to support additional devices or platforms at this time.

Expanded device support is already planned. The current priority is improving stability and resolving issues with the Android beta before development expands to additional platforms.

## ⚠️ Disclaimer

Providra does not host, store, index, or provide any media content.

Providra is only a local bridge that allows Syncler to communicate with third-party addons and plugins configured by the user. The developer is not responsible for the content, availability, behavior, or legality of any third-party service.

Users are responsible for ensuring that their use of Providra and any connected services complies with the laws and regulations applicable in their region.

## 🐛 Feedback and Bug Reports

Providra is in open beta, so feedback is welcome.

To report a bug or request an improvement, open an issue on the **[GitHub Issues page](https://github.com/dtankdempsey2/Providra/issues)** and include as much information as possible, such as:

* Your device model
* Your Android version
* Whether you are using Addons or Plugins
* The steps needed to reproduce the issue
* Screenshots or logs, when available

---

<div align="center">

### Built to give Syncler users more options.

[Download the Latest Release](https://github.com/dtankdempsey2/Providra/releases)

</div>
