# 🛡️ Jellyfin Parental Ratings Pro

**Jellyfin Parental Ratings Pro** enhances parental controls in Jellyfin by automatically fetching, standardising, and enforcing age ratings across your media library.

It supports multiple international rating systems, fills missing metadata, and helps ensure safe, consistent viewing for all users.

---

## ✨ Features

* 🌍 **Multi-Region Rating Support**
  Supports rating systems such as MPAA, BBFC, and ACB

* 🔄 **Smart Rating Conversion**
  Converts ratings into a unified, easy-to-use format

* 👨‍👩‍👧 **Enhanced Parental Controls**
  Integrates with Jellyfin user restrictions

* 🎬 **Automatic Metadata Enrichment**
  Retrieves missing ratings using TMDb

* ⚡ **Playback Protection (Optional)**
  Prevents restricted content from being played

* 🎨 **Poster Rating Overlays (Optional)**
  Displays ratings visually on media artwork

---

## 📦 Installation

### 🔹 Method 1: Install via Plugin Repository (Recommended)

1. Open **Jellyfin Dashboard**
2. Go to **Plugins → Repositories**
3. Add your repository URL
4. Go to **Catalog**
5. Find **Parental Ratings Pro**
6. Click **Install**
7. Restart Jellyfin

---

### 🔹 Method 2: Manual Install

1. Download the latest release from GitHub
2. Extract the ZIP
3. Copy the plugin folder to:

**Windows:**

```
C:\ProgramData\Jellyfin\Server\plugins\
```

**Linux:**

```
/var/lib/jellyfin/plugins/
```

4. Restart Jellyfin

---

## ⚙️ Configuration

1. Go to **Dashboard → Plugins → Parental Ratings Pro**
2. Enter your TMDb API key
3. Configure:

   * Rating system preferences
   * Allowed age levels per user
   * Overlay display settings
4. Save changes

---

## 🔑 TMDb API Key Setup

This plugin uses TMDb for metadata.

1. Create an account at [https://www.themoviedb.org](https://www.themoviedb.org)
2. Go to **Settings → API**
3. Generate an API key
4. Paste it into the plugin settings

---

## 🧩 Compatibility

* Jellyfin Server: **10.11+**
* .NET Runtime: **.NET 9.0**
* OS: Windows, Linux, Docker

---

## 🛠️ Development

### Build the plugin

```bash
dotnet build -c Release
```

### Publish

```bash
dotnet publish -c Release
```

Output will be in:

```
/bin/Release/net9.0/publish/
```

---

## 📁 Project Structure

```
Jellyfin.Plugin.ParentalRatingsPro/
│
├── Plugin.cs
├── Configuration/
│   └── PluginConfiguration.cs
├── Services/
│   ├── RatingService.cs
│   ├── MetadataService.cs
│   ├── ParentalControlService.cs
│   └── PlaybackMonitorService.cs
```

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🚀 Future Improvements

* More regional rating systems
* AI-based content classification
* User-specific dynamic restrictions
* UI enhancements in Jellyfin dashboard

---

## ⚠️ Disclaimer

This plugin relies on third-party metadata providers. Rating accuracy depends on available data and may vary by region.


