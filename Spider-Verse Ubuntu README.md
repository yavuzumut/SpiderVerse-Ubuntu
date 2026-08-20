# 🕷️ Spider-Verse Ubuntu

> 🇹🇷 Ubuntu masaüstümü Miles Morales / Spider-Verse temasıyla özelleştirdiğim kişisel dotfiles projesi.
> 🇬🇧 A personal Ubuntu desktop customization inspired by Miles Morales and the Spider-Verse.

---

## 📸 Preview

<img width="1920" height="1200" alt="Ekran Görüntüsü 2026-08-17 20-35-59" src="https://github.com/user-attachments/assets/d3bbf612-646a-45e9-a919-d723df69c0b3" />



---

# 🇹🇷 Türkçe

## 🕷️ Proje Hakkında

Bu proje, kullandığım **Ubuntu masaüstünü Miles Morales / Spider-Verse konseptine göre kişiselleştirmek** için oluşturduğum bir masaüstü özelleştirme çalışmasıdır.

Amacım sadece bir wallpaper değiştirmek değildi. Masaüstünün mümkün olduğunca bütün parçalarının aynı **kırmızı / siyah Spider-Verse estetiğini** taşımasını istedim.

Bu nedenle:

- 🎨 GNOME temasını değiştirdim
- 🔴 Kırmızı / siyah renk paleti kullandım
- 🕷️ Spider-Verse temalı wallpaper kullandım
- 🕷️ Fastfetch'i özel bir Spider-Verse görünümüne uyarladım
- 🎨 Uygulama ikonlarını değiştirdim
- 🖥️ Terminali özelleştirdim
- 🔴 Dash to Dock'u özelleştirdim
- 🧩 GNOME Extensions kullandım
- 🌫️ Terminal ve GNOME arayüzünde şeffaflık / blur efektleri kullandım

Bu repository, yaptığım özelleştirmeleri ve kullandığım ayarları belgelemek için oluşturuldu.

---

## 🖥️ Sistem

| Özellik | Kullanılan |
|---|---|
| OS | Ubuntu |
| Desktop Environment | GNOME |
| Theme | Yaru-red-dark |
| Icon Theme | Yaru-red-dark |
| Cursor | Yaru |
| Dock | Dash to Dock |
| Terminal | Ptyxis |
| Fastfetch | 2.57.1 |

---

# 🎨 Tema

Ana renk paletini Spider-Verse konseptine uygun olarak **kırmızı ve siyah** üzerine kurdum.

```text
GTK Theme:   Yaru-red-dark
Icon Theme:  Yaru-red-dark
Cursor:      Yaru
```

`Yaru-red-dark`, Ubuntu'nun koyu görünümünü kırmızı detaylarla birleştirdiği için Spider-Verse konseptine oldukça iyi uydu.

Tema ayarları:

```text
themes/
└── theme.md
```

dosyasında bulunuyor.

---

# 🕷️ Wallpaper

Masaüstünün ana görselini Miles Morales / Spider-Verse konseptine göre seçtim.

Wallpaper, masaüstünün geri kalanındaki kırmızı ve siyah renklerle uyumlu olacak şekilde kullanılıyor.

Wallpaper dosyaları:

```text
wallpapers/
```

klasöründe bulunuyor.

---

# 🎨 Uygulama İkonları

Uygulama ikonlarını Spider-Verse konseptine uygun olacak şekilde değiştirdim.

Özelleştirdiğim uygulamalar arasında:

- 🦊 Firefox
- 📝 Notion
- 🎵 Spotify
- 💻 Visual Studio Code

bulunuyor.

İkonları uygulamalara uygulamak için **MenuLibre** kullandım.

MenuLibre sayesinde uygulamaların `.desktop` launcher dosyalarındaki ikonları kolayca değiştirebildim.

Özel ikonlar:

```text
icons/
├── firefox.png
├── notion.png
├── spotify.png
└── vscode.png
```

---

# 🧩 GNOME Extensions

Masaüstünü özelleştirirken **Extension Manager** kullanarak GNOME Extensions'ı yönettim.

Kullandığım başlıca eklentiler:

- **Dash to Dock**
- **Blur My Shell**

### Dash to Dock

Dock'un görünümünü ve davranışlarını Spider-Verse temasına uygun hale getirmek için kullandım.

### Blur My Shell

GNOME arayüzünde blur ve şeffaflık efektleri oluşturmak için kullandım.

---

# 🔴 Dash to Dock

Ubuntu'nun dock görünümünü Spider-Verse temasına uyarlamak için **Dash to Dock** kullandım.

Temel ayarlar:

```text
Position:             Bottom
Icon Size:            48px
Transparency Mode:    FIXED
Custom Theme Shrink:  Enabled
Auto Hide:            Enabled
Intellihide:          Enabled
```

Dock'un arka planı koyu renkte:

```text
rgb(5,5,5)
```

Çalışan uygulamaların göstergelerinde Spider-Verse kırmızısı kullandım:

```text
#E50914
```

Dock ayarları:

```text
dock/
└── dock.md
```

dosyasında bulunuyor.

---

# 🌫️ Blur My Shell

**Blur My Shell**, GNOME arayüzüne blur ve şeffaflık efektleri eklemek için kullandığım GNOME eklentilerinden biri.

Bu efektler masaüstünün daha modern ve Spider-Verse konseptine daha uygun görünmesine yardımcı oluyor.

---

# 🖥️ Terminal

Terminal olarak **Ptyxis** kullanıyorum.

Terminali de masaüstünün geri kalanıyla aynı kırmızı / siyah estetiğe uyacak şekilde özelleştirdim.

### Terminal ayarları

```text
Terminal:    Ptyxis
Opacity:     85%
Palette:     xterm
Font:        Ubuntu Sans Mono 11pt
```

Şeffaflık değeri:

```text
0.85
```

olarak ayarlandı.

Terminal ayarları:

```text
terminal/
└── shell.md
```

dosyasında bulunuyor.

---

# 🕷️ Fastfetch & Chafa

Fastfetch'i masaüstünün Spider-Verse konseptinin önemli bir parçası olarak kullandım.

Fastfetch için özel bir **Spider-Verse / Spider-Man ASCII görünümü** hazırladım.

Ayrıca terminal içerisinde görselleri göstermek için **Chafa** kullandım.

Chafa, görselleri terminal içerisinde karakter tabanlı şekilde görüntülemeye olanak sağlıyor.

Kurulum:

```bash
sudo apt install chafa
```

Fastfetch ve görsel yapılandırmaları:

```text
fastfetch/
├── config.jsonc
└── logos/
```

klasöründe bulunuyor.

---

# 🛠️ Kullanılan Araçlar

Bu masaüstünü oluştururken kullandığım başlıca araçlar:

| Araç | Kullanım amacı |
|---|---|
| **Ubuntu** | Ana işletim sistemi |
| **GNOME** | Masaüstü ortamı |
| **Extension Manager** | GNOME Extensions yönetimi |
| **Dash to Dock** | Dock özelleştirme |
| **Blur My Shell** | Blur ve şeffaflık efektleri |
| **MenuLibre** | Uygulama launcher ve ikonlarını değiştirme |
| **Ptyxis** | Terminal |
| **Fastfetch** | Sistem bilgileri ve özel görünüm |
| **Chafa** | Terminalde görsel görüntüleme |
| **gsettings** | GNOME ayarlarını yönetme |

---

# 📁 Repository Structure

```text
SpiderVerse-Ubuntu/
│
├── fastfetch/
│   ├── config.jsonc
│   └── logos/
│
├── icons/
│   ├── firefox.png
│   ├── notion.png
│   ├── spotify.png
│   └── vscode.png
│
├── terminal/
│   └── shell.md
│
├── themes/
│   └── theme.md
│
├── dock/
│   └── dock.md
│
├── wallpapers/
│   └── ...
│
└── README.md
```

---

# ⚙️ Kurulum

Bu repository şu anda **kişisel bir dotfiles projesidir** ve tüm ayarları otomatik olarak kuran bir installer içermemektedir.

Ayarları manuel olarak uygulamak için klasörlerde bulunan ilgili dosyalardaki talimatları takip edebilirsiniz.

Önerilen sıra:

### 1️⃣ Tema

`themes/theme.md` içerisindeki tema ayarlarını uygulayın.

### 2️⃣ İkonlar

`icons/` klasöründeki ikonları kullanarak uygulama launcher'larını **MenuLibre** üzerinden düzenleyin.

### 3️⃣ Terminal

`terminal/shell.md` içerisindeki Ptyxis ayarlarını uygulayın.

### 4️⃣ Fastfetch & Chafa

`fastfetch/` klasöründeki yapılandırmayı uygulayın ve terminal görselleri için Chafa'yı yükleyin.

```bash
sudo apt install chafa
```

### 5️⃣ Dock

`dock/dock.md` içerisindeki Dash to Dock ayarlarını uygulayın.

### 6️⃣ Wallpaper

`wallpapers/` içerisindeki wallpaper'ı masaüstü arka planı olarak ayarlayın.

---

# ⚠️ Notlar

Bu proje **resmî bir Ubuntu teması değildir.**

Spider-Verse, Miles Morales ve ilgili karakterler Marvel / Sony Pictures Entertainment'a aittir.

Bu repository kişisel masaüstü özelleştirme amacıyla oluşturulmuştur.

Bazı ayarlar:

- Ubuntu sürümüne
- GNOME sürümüne
- GNOME Extension sürümüne
- Dash to Dock sürümüne

göre farklı davranabilir.

Bu nedenle ayarların her Ubuntu sisteminde birebir aynı sonucu vermesi garanti edilmez.

---

# 🇬🇧 English

## 🕷️ About

This is my personal Ubuntu desktop customization inspired by **Miles Morales and the Spider-Verse**.

The goal was not simply to change the wallpaper. I wanted the entire desktop to follow the same **red and black Spider-Verse aesthetic**.

The setup includes:

- 🕷️ Spider-Verse inspired wallpaper
- 🔴 Yaru-red-dark theme
- 🎨 Custom application icons
- 🕷️ Custom Fastfetch configuration
- 🖥️ Customized Ptyxis terminal
- 🔴 Customized Dash to Dock
- 🧩 GNOME Extensions
- 🌫️ Blur and transparency effects

This repository contains the configuration files and documentation for the setup.

---

## 🖥️ Environment

```text
OS:             Ubuntu
Desktop:        GNOME
GTK Theme:      Yaru-red-dark
Icon Theme:     Yaru-red-dark
Cursor:         Yaru
Dock:           Dash to Dock
Terminal:       Ptyxis
Fastfetch:      2.57.1
```

---

## 🎨 Theme

The main visual style is based on a **dark red and black** color palette.

```text
GTK Theme:   Yaru-red-dark
Icon Theme:  Yaru-red-dark
Cursor:      Yaru
```

Theme information:

```text
themes/theme.md
```

---

## 🕷️ Wallpaper

The desktop uses a Miles Morales / Spider-Verse inspired wallpaper.

The wallpaper was selected to match the dark background and red accents used throughout the desktop.

Wallpaper files are located in:

```text
wallpapers/
```

---

## 🎨 Custom Application Icons

I customized several application icons to match the Spider-Verse aesthetic.

Currently customized applications include:

- Firefox
- Notion
- Spotify
- Visual Studio Code

I used **MenuLibre** to modify the application launchers and replace their default icons.

Custom icons are stored in:

```text
icons/
```

---

## 🧩 GNOME Extensions

I used **Extension Manager** to manage the GNOME extensions used throughout the customization.

Main extensions:

- **Dash to Dock**
- **Blur My Shell**

Dash to Dock was used to customize the dock, while Blur My Shell was used for blur and transparency effects.

---

## 🔴 Dash to Dock

The Ubuntu dock was customized using **Dash to Dock**.

Main settings:

```text
Position:             Bottom
Icon Size:            48px
Transparency Mode:    FIXED
Custom Theme Shrink:  Enabled
Auto Hide:            Enabled
Intellihide:          Enabled
```

Dock background:

```text
rgb(5,5,5)
```

Running application indicators:

```text
#E50914
```

Dock configuration:

```text
dock/dock.md
```

---

## 🖥️ Terminal

The terminal used in this setup is **Ptyxis**.

Configuration:

```text
Opacity:   85%
Palette:   xterm
Font:      Ubuntu Sans Mono 11pt
```

Terminal configuration:

```text
terminal/shell.md
```

---

## 🕷️ Fastfetch & Chafa

Fastfetch is customized with a Spider-Verse / Spider-Man inspired terminal appearance.

I also use **Chafa** to display images directly inside the terminal using character-based rendering.

Install Chafa with:

```bash
sudo apt install chafa
```

Fastfetch configuration:

```text
fastfetch/
├── config.jsonc
└── logos/
```

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **Ubuntu** | Operating system |
| **GNOME** | Desktop environment |
| **Extension Manager** | GNOME extension management |
| **Dash to Dock** | Dock customization |
| **Blur My Shell** | Blur and transparency effects |
| **MenuLibre** | Application launcher and icon customization |
| **Ptyxis** | Terminal |
| **Fastfetch** | System information and custom appearance |
| **Chafa** | Displaying images in the terminal |
| **gsettings** | GNOME configuration |

---

## 📁 Repository Structure

```text
SpiderVerse-Ubuntu/
│
├── fastfetch/
├── icons/
├── terminal/
├── themes/
├── dock/
├── wallpapers/
└── README.md
```

---

## ⚙️ Installation

This repository is currently a **personal dotfiles project** and does not include an automated installation script.

The configuration can be applied manually by following the instructions provided in each directory.

Recommended order:

1. Apply the theme.
2. Replace application icons using MenuLibre.
3. Configure Ptyxis.
4. Configure Fastfetch and Chafa.
5. Configure Dash to Dock.
6. Set the Spider-Verse wallpaper.

---

## ⚠️ Disclaimer

This is **not an official Ubuntu theme**.

Spider-Verse, Miles Morales and related characters are properties of Marvel / Sony Pictures Entertainment.

This repository is intended for personal desktop customization.

Some settings may behave differently depending on:

- Ubuntu version
- GNOME version
- GNOME extension versions
- Dash to Dock version

Therefore, the configuration may not produce exactly the same result on every system.

---

# 🕷️ Final

> **With great power comes great responsibility.**

Built on Ubuntu.
Inspired by the Spider-Verse. 🕷️🔴
