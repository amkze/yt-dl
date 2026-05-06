### YouTube Video Downloader
Download any YouTube video in best quality directly into your GitHub repository.

<br>

### Usage
1. **Fork this repository**
2. Go to the **Actions** tab and enable workflows
3. Select **Download YouTube Video** (in the left sidebar) → **Run workflow** (in the right part of the blue section)
4. Paste the YouTube URL and run
5. After completion, the `download` folder will contain video chunks (e.g., `video.zip.00`, `video.zip.01`)

<br>

### Reassemble the video
**macOS / Linux** (Terminal):  
`cat download/video.zip.* > video.zip`  
Then unzip `video.zip`.

**Windows** (Command Prompt):  
`copy /b download\video.zip.00 + download\video.zip.01 video.zip`  
Then extract `video.zip`.

<br>

---
*No local tools required, everything runs on GitHub Actions.*
