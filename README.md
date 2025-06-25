# 🔹 Welcome to BlackBlazent

**BlackBlazent** is an independent software organization creating hybrid, cross-platform apps — designed with passion, purpose, and precision.


[![Join me on daily.dev](https://img.shields.io/badge/daily.dev-Join%20Now-blueviolet?logo=daily.dev&logoColor=white&style=for-the-badge)](https://dly.to/HJTKpTQR4Ql)
[![Join Discord](https://img.shields.io/discord/1247152717299326996?color=5865F2&label=Discord%20%7C%20BlackBlazent&logo=discord&logoColor=white&style=for-the-badge)](https://discord.gg/MNkB2Pr7)
[![Telegram](https://img.shields.io/badge/Telegram-Join%20Chat-2CA5E0?logo=telegram&logoColor=white&style=for-the-badge)](https://t.me/+g3J3-sApBIAwOWl1)
[![Facebook Page](https://img.shields.io/badge/Facebook-Page-1877F2?logo=facebook&logoColor=white&style=for-the-badge)](https://www.facebook.com/profile.php?id=61565193375253)
[![Facebook Group](https://img.shields.io/badge/Facebook-Group-1877F2?logo=facebook&logoColor=white&style=for-the-badge)](https://www.facebook.com/groups/1240579097510491/)
[![Reddit](https://img.shields.io/badge/Reddit-r%2FBlackBlazers-FF4500?logo=reddit&logoColor=white&style=for-the-badge)](https://www.reddit.com/r/BlackBlazers/)
[![VK](https://img.shields.io/badge/VK-BlackBlazent-4680C2?logo=vk&logoColor=white&style=for-the-badge)](https://vk.com/blackblazent?from=groups)
[![OK.ru](https://img.shields.io/badge/OK.ru-BlackBlazent-EF7F1A?logo=odnoklassniki&logoColor=white&style=for-the-badge)](https://ok.ru/group/70000038717846)

---

## 🚀 About Us

We are a startup software company focused on building modern, user-centered digital tools. From music and video apps to creative galleries, we aim to make hybrid apps accessible and meaningful.

---

## 🎯 Our Application Goals

Every application created under **BlackBlazent** is built with a clear purpose. We focus on solving real-world problems through hybrid technology, beautiful design, and intuitive user experience.

### 🌟 Core Goals Behind Our Apps

1.  
    ✅ **Cross-Platform Experience**  
    Deliver seamless functionality on desktop, web, and mobile environments.

2.  
    🎨 **Creative & Visual Engagement**  
    Prioritize visually rich interfaces that are easy and enjoyable to use.

3.  
    ⚙️ **Practical Functionality**  
    Build tools that support daily productivity, entertainment, and creativity.

4.  
    📱 **Hybrid Technology Stack**  
    Use modern hybrid frameworks to ensure faster development and wider reach.

5.  
    🔐 **User-First Design**  
    Respect user privacy, simplicity, and accessibility in all features.

6.  
    🌍 **Global Accessibility**  
    Design apps that can be localized and enjoyed by users around the world.

---

> 🧭 Our mission is to build purposeful digital tools that blend art, function, and future-ready tech.
---

## 📦 Featured Projects

| Icon | Project Name | Description | Version | Tech Stack |
|------|--------------|-------------|---------|------------|
| <img src="https://github.com/BlackBlazent/.github/blob/main/public/assets/icons/bmusic/bmusic.png" width="80px" height="80px"/> | [BlackMusic](https://github.com/BlackBlazent/BlackMusic.git) | Music Ultra Superior Integrated Catalog. A music player designed to deliver an unparalleled audio experience. BlackMusic integrates a vast catalog of music with superior playback capabilities. | v1.1.01.001.0001 | Undisclosed |
| ![🖼️](https://twemoji.maxcdn.com/v/latest/svg/1f5bc.svg) | [BlackVideo](https://github.com/BlackBlazent/BlackVideo.git) | BlackVideo - Black : Versatile Integrated Demi Empowerment Optimum—Player. A video player with integration of wide variety of playback functionalities. | v1.0.0 | Undisclosed |
| ![📸](https://twemoji.maxcdn.com/v/latest/svg/1f4f8.svg) | [BlackGallery](https://github.com/BlackBlazent/BlackGallery.git) | A comprehensive and innovative gallery app designed to showcase and organize your visual content in the most efficient and appealing way possible. With a focus on delivering a luminous and vibrant display, it serves as a library for your images, providing an extensive collection of features to enhance your viewing experience. | v1.0.0 | Undisclosed |
| ![🧰](https://twemoji.maxcdn.com/v/latest/svg/1f9f0.svg) | [BlackMiscellen](https://github.com/BlackBlazent/BlackMiscellen.git) | An Integrated Miscellaneous tools. | v1.0.0 | Undisclosed |


---

# Diagram

```mermaid
flowchart TB
    %% External Parties
    Dev["Developer Workstation"]:::external
    EndUser["End-User Environment<br/>(CLI or Desktop App)"]:::external

    %% Documentation
    subgraph "Project Documentation"
        README["README.md"]:::external
        License["LICENSE"]:::external
        GitIgnore[".gitignore"]:::external
    end

    Dev -->|references| README
    Dev -->|references| License
    Dev -->|references| GitIgnore

    %% Build Pipeline
    Dev --> Build["Build Script / Makefile"]:::tooling

    Build -->|invokes| FortranCompiler["Fortran Compiler Toolchain"]:::code
    FortranCompiler --> Executable["Executable Binary"]:::code

    %% Source Code
    SourceCode["blackblazent.f90"]:::code
    Build -->|compiles| SourceCode
    SourceCode --> FortranCompiler

    %% Assets
    subgraph "Static Assets Bundle"
        AssetsDir["public/assets/icons"]:::assets
        AssetManifest["icon.list.yml"]:::assets
    end

    Build -->|bundles| AssetsDir
    Build -->|bundles| AssetManifest

    %% Packaging
    Executable --> Packager["Packager / Distributor"]:::tooling
    AssetsDir --> Packager
    AssetManifest --> Packager

    Packager --> Package["Cross-platform Package"]:::tooling
    Package --> EndUser

    %% Extensibility Note
    Extensibility["YAML manifest enables adding icons without code changes"]:::note
    AssetManifest --> Extensibility

    %% Click Events
    click SourceCode "https://github.com/blackblazent/.github/blob/main/blackblazent.f90"
    click AssetsDir "https://github.com/blackblazent/.github/tree/main/public/assets/icons"
    click AssetManifest "https://github.com/blackblazent/.github/blob/main/public/assets/icons/icon.list.yml"
    click README "https://github.com/blackblazent/.github/blob/main/README.md"
    click License "https://github.com/blackblazent/.github/tree/main/LICENSE"
    click GitIgnore "https://github.com/blackblazent/.github/blob/main/.gitignore"

    %% Styles
    classDef code fill:#BBE1FA,stroke:#3282B8,color:#000
    classDef tooling fill:#FFDFA8,stroke:#FFAA1D,color:#000
    classDef assets fill:#C4E1C1,stroke:#2F8F2F,color:#000
    classDef external fill:#E0E0E0,stroke:#999,color:#000
    classDef note fill:#FFF3B0,stroke:#CCA300,color:#000
```

## 👤 Join or Follow Us

We’re always open to contributors, testers, and idea sharers!  

### 🔧 General & Administrative

| Purpose                               | Given Email                                                |
| ------------------------------------- | -------------------------------------------------------------- |
| **Main** | `blackblazent@gmail.com`                                      |
| **Customer Support**                  | `blackblazent.customer.service@gmail.com`                     |
| **Billing & Payments**                | `blackblazent.billing@gmail.com` |
| **Legal or Compliance**               | `blackblazent.legal@gmail.com`     |
| **General Inquiries**                 | `blackblazent.info@gmail.com`       |

---

### 🧑‍💻 Development & Technical

| Purpose                            | Given Email                                                         |
| ---------------------------------- | ----------------------------------------------------------------------- |
| **Developer Support**              | `blackblazent.dev@gmail.com`                  |
| **Technical Issues / Bug Reports** | `blackblazent.techsupport@gmail.com` |

---

### 📣 Marketing & Outreach

| Purpose                           | Given Email                                                    |
| --------------------------------- | ------------------------------------------------------------------ |
| **Marketing Team**                | `blackblazent.marketing@gmail.com` |
| **Partnerships / Collaborations** | `blackblazent.partners@gmail.com`   |
| **Press / Media Inquiries**       | `blackblazent.press@gmail.com`         |

---

### 🧪 Product & Feedback

| Purpose                             | Given Email                                                  |
| ----------------------------------- | ---------------------------------------------------------------- |
| **Product Feedback**                | `blackblazent.feedback@gmail.com` |
| **Beta Testers / Test Environment** | `blackblazent.beta@gmail.com`         |

---

> 🖤 Made with code and creativity by BlackBlazent
