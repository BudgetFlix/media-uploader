#  BudgetFlix Uploader

> Media upload client for BudgetFlix.

---

##  Overview

The **BudgetFlix Uploader** is a client-side tool used to upload video files to the server.

Currently implemented as a **Java-based CLI tool**, it is designed to:

*  Upload video files to a remote server
*  Send metadata alongside uploads
* ️ Integrate with the media processing pipeline

---

## Purpose

This tool acts as the **entry point of the content pipeline**:

```id="flow3"
Uploader → Server → Media Worker → HLS → Streaming
```

---

##️ Current Features

* Upload files via SSH
* Send metadata as JSON
* Simple CLI-based workflow
* Works with remote server environments

---

## Upload Flow

1. Select video file
2. Provide metadata (JSON)
3. Upload via SSH
4. File arrives in watched directory
5. Media Worker processes the video

---

## Example Metadata

```json id="meta1"
{
  "title": "Movie Title",
  "type": "MOVIE"
}
```

---

##️ Tech Stack (Current)

* Java
* SSH (file transfer)

---

## Limitations

* No UI (CLI only)
* No upload progress tracking
* No validation feedback
* Manual metadata input

---

## Future Vision

This tool will evolve into a **full-featured native admin application**.

### Planned Upgrade: Tauri App

* Cross-platform desktop app
* Modern UI
* Media management dashboard
* Integrated upload system

---

##  Planned Features

* Drag & drop uploads
* Upload progress tracking
* Metadata editor UI
* Thumbnail preview
* Upload history
* Error handling & retry
* Multi-file uploads

---

##  Long-Term Goal

> Provide a complete admin interface for managing a self-hosted streaming platform.

This includes:

* uploading content
* editing metadata
* monitoring processing
* managing media library

---

##  Status

>  Early stage (CLI tool, evolving into native app)
