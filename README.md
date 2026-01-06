# videoQR 📹

A web application that scans QR codes containing video URLs and plays them instantly on your screen.

## Features

- 📸 **QR Code Scanner** - Uses your device camera to scan QR codes
- 🎥 **Instant Video Playback** - Automatically plays videos after scanning
- 📱 **Mobile Friendly** - Works on smartphones and tablets
- 🎨 **Beautiful UI** - Modern gradient design with smooth animations
- 🔄 **Scan Multiple Videos** - Easy to scan and play multiple videos

## How to Use

1. **Open the App**
   - Simply open `index.html` in a web browser (Chrome, Firefox, Safari, Edge)
   - Or host it on a local/remote web server

2. **Start Scanning**
   - Click the "Start Scanner" button
   - Allow camera permissions when prompted
   - Point your camera at a QR code containing a video URL

3. **Watch the Video**
   - The video will automatically start playing once the QR code is detected
   - Use the video controls to pause, adjust volume, or go fullscreen
   - Click "Scan Another Video" to scan more QR codes

## Supported Video Formats

- Direct video files: MP4, WebM, OGG, MOV
- Streaming formats: M3U8, DASH
- Video platforms: YouTube, Vimeo, Dailymotion (depending on embed support)

## Creating QR Codes for Videos

To create QR codes with video URLs:

1. **Use an Online QR Generator:**
   - QR Code Generator: https://www.qr-code-generator.com/
   - QR Code Monkey: https://www.qrcode-monkey.com/
   
2. **Enter your video URL:**
   - Direct video file URL (e.g., `https://example.com/video.mp4`)
   - YouTube video URL (e.g., `https://www.youtube.com/watch?v=...`)
   - Any publicly accessible video URL

3. **Generate and print/display the QR code**

## Technical Details

- Built with HTML5, CSS3, and vanilla JavaScript
- Uses [html5-qrcode](https://github.com/mebjas/html5-qrcode) library for QR scanning
- No backend required - runs entirely in the browser
- Responsive design that works on all screen sizes

## Browser Requirements

- Modern web browser with camera access support
- HTTPS connection required for camera access (or localhost for development)
- JavaScript enabled

## Local Development

To run locally:

```bash
# Option 1: Using Python
python -m http.server 8000

# Option 2: Using Node.js (http-server)
npx http-server

# Option 3: Just open index.html in your browser (may have camera restrictions)
```

Then navigate to `http://localhost:8000` in your browser.

## Security Note

This app requires camera permissions to scan QR codes. For production deployment, ensure you're serving over HTTPS as modern browsers require secure contexts for camera access.

## License

MIT License - Feel free to use and modify as needed!