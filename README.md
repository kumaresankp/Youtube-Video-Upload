# 🎬 YouTube Video Uploader (Python 3)

This Python script allows you to upload videos to your YouTube channel using the **YouTube Data API v3**.

---

## 📁 Project Structure

```
YoutubeUpload/
├── upload_video.py
├── client_secrets.json
├── requirements.txt
└── your_video_file.flv
```

---

## 📦 Requirements

Install all required dependencies using:

```bash
pip install -r requirements.txt
```

**Example `requirements.txt`:**

```
google-api-python-client
oauth2client
```

---

## 🔐 Google API Setup

1. Go to the [Google Cloud Console](https://console.cloud.google.com/)
2. Create or select an existing project.
3. Enable the **YouTube Data API v3** for your project.
4. Go to **APIs & Services > Credentials**.
5. Click **Create Credentials > OAuth client ID**
   - Application Type: **Desktop App**
6. Download the `client_secrets.json` file.
7. Rename it to `client_secrets.json` and place it in the same folder as the script.

---

## 🎞️ Prepare the Video

Place your video file (e.g., `your_video_file.flv`) in the same directory as `upload_video.py`.

---

## ▶️ How to Run the Script

Use the following command to upload your video:

```bash
python upload_video.py --file="your_video_file.flv" \
                       --title="Summer vacation in California" \
                       --description="Had fun surfing in Santa Cruz" \
                       --keywords="surfing,Santa Cruz" \
                       --category="22" \
                       --privacyStatus="private"
```

> This will open a browser window the first time you run it, prompting you to log in and grant permission to upload videos on your behalf.
