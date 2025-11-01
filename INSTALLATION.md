# Media Timestamp Notes PWA - Installation Guide

## 📱 How to Install on iPhone

### Method 1: Via GitHub Pages (Recommended - Easiest)

1. **Upload files to GitHub:**
   - Create a new repository on GitHub
   - Upload these files:
     - `media-timestamp-pwa.html`
     - `manifest.json`
     - `icon-192.png`
     - `icon-512.png`

2. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Select "main" branch as source
   - Save and wait ~1 minute
   - Your site will be at: `https://yourusername.github.io/repository-name/media-timestamp-pwa.html`

3. **Install on iPhone:**
   - Open Safari on your iPhone
   - Go to your GitHub Pages URL
   - Tap the **Share** button (square with arrow pointing up)
   - Scroll down and tap **"Add to Home Screen"**
   - Name it (e.g., "Timestamps")
   - Tap **Add**

### Method 2: Via iCloud Drive (Offline Use)

1. **Save files to iCloud:**
   - Download all 4 files to your computer
   - Place them in a folder in your iCloud Drive

2. **Open on iPhone:**
   - Open Files app on iPhone
   - Navigate to iCloud Drive → your folder
   - Tap `media-timestamp-pwa.html`
   - It will open in Safari

3. **Add to Home Screen:**
   - Tap the Share button
   - Tap "Add to Home Screen"
   - Tap Add

### Method 3: Via Local Server (For Development)

1. **Start a local server on your computer:**
   ```bash
   # On Mac/Linux
   cd /path/to/files
   python3 -m http.server 8000
   
   # On Windows
   cd C:\path\to\files
   python -m http.server 8000
   ```

2. **Find your computer's IP address:**
   - Mac: System Preferences → Network
   - Windows: Open Command Prompt, type `ipconfig`
   - Look for something like `192.168.1.x`

3. **Access on iPhone:**
   - Make sure iPhone is on same WiFi network
   - Open Safari
   - Go to: `http://YOUR_IP_ADDRESS:8000/media-timestamp-pwa.html`
   - Add to Home Screen as described above

## 🎯 Quick Start Guide

### Loading Media Files

1. **Tap the file input** at the top
2. **Select files** from:
   - Files app
   - iCloud Drive
   - Photos (for videos)
   - Any connected cloud storage
3. **Multiple files** create a playlist
4. **Tap any item** in the playlist to switch files

### Adding Timestamps

1. **Play your media** to find the spot you want to mark
2. **Tap "Add Timestamp"** - this automatically pauses the media
3. **Type your note** in the text area
4. **Optional:** Add an end time in the "End time" field (e.g., "01:23:45")
5. The timestamp is saved instantly

### Navigating

- **Play/Pause:** Obvious!
- **2x Speed:** Hold the button down for 2x speed, release to return to normal
- **-5s / +5s:** Quick skip back/forward
- **-30s / +30s:** Larger jumps
- **Click any timestamp** to jump to that moment

### Exporting Your Work

1. **Select format:** JSON (recommended), SRT, or TXT
2. **Tap Export:** Downloads a file named after your media file
3. **File is saved to:** iPhone Downloads folder
4. **Share it** via AirDrop, email, cloud storage, etc.

### Importing Progress

1. **Tap "Choose File"** under Import
2. **Select your JSON file**
3. Timestamps are loaded and merged with existing ones
4. Your progress is restored!

## 💡 Features Explained

### Auto-Save
- Your timestamps are automatically saved to browser storage
- They persist even if you close the browser
- Each file has its own set of timestamps

### Playlist Mode
- Load multiple files at once
- Switch between them with the playlist
- Each file maintains its own timestamps
- Export/Import works per file

### End Time Field
- Optional field for noting where a segment ends
- Displays as a range (e.g., "00:05:30 - 00:06:45")
- Purely for your reference - doesn't affect playback
- Great for transcription or detailed logging

### Edit & Delete
- ✏️ Edit: Loads timestamp into input fields, then deletes it (add it again after editing)
- 🗑️ Delete: Removes the timestamp permanently

### Export Formats

**JSON:**
- Best for re-importing
- Contains all metadata
- Human-readable

**SRT:**
- Standard subtitle format
- Use with video players that support subtitles
- Can be loaded in video editing software

**TXT:**
- Simple text format
- Easy to read and share
- Good for notes and documentation

## 🔧 Troubleshooting

### "Add to Home Screen" option missing
- Make sure you're using **Safari** (not Chrome or other browsers)
- Some websites block this - that's why local files or GitHub Pages work best

### Media won't play
- Ensure the file format is supported by Safari
- Try: MP4, MOV, M4A, MP3, WAV
- Avoid: MKV, FLAC, or DRM-protected files

### Timestamps not saving
- Check browser storage isn't full
- Try exporting as JSON to backup
- Re-import if needed

### Can't access files
- On iPhone, you need to grant Files app access
- Some cloud apps may require additional permissions

### PWA not working offline
- GitHub Pages requires internet for first load
- iCloud Drive method works offline after initial load
- Export your timestamps before going offline!

## 📂 File Structure

Your download includes:
```
media-timestamp-pwa.html  ← Main app (open this!)
manifest.json             ← PWA configuration
icon-192.png              ← App icon (small)
icon-512.png              ← App icon (large)
INSTALLATION.md           ← This file
```

## 🎨 Tips & Tricks

1. **Transcription workflow:** Use 2x speed for listening, hit Add Timestamp when you need to note something, type quickly, then continue

2. **Music practice:** Mark difficult sections with timestamps, jump back repeatedly to practice

3. **Lecture notes:** Timestamp key concepts, export as TXT for studying

4. **Podcast bookmarks:** Mark interesting quotes or moments to come back to

5. **Video editing prep:** Use this to plan cuts before opening your video editor

## 🆘 Need Help?

The app works entirely in your browser - no account needed, no data sent anywhere. Everything stays on your device unless you export it.

Enjoy your timestamping! 🎬
