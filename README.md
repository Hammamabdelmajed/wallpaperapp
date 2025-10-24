Overview

A macOS wallpaper app offering 4K/60fps H.264/H.265 video wallpapers (MP4). Built with SwiftUI and powered by Metal-optimized rendering for smooth, low-latency playback. Includes smart filters (resolution, duration, size, category, date), daily shuffle, multi-device sync, and license validation.

Backend runs on AWS Lambda (Node.js) with API Gateway, S3/MinIO, CloudFront, and DynamoDB for scalable storage, metadata, and CDN delivery. The app is secure (App Sandbox, Hardened Runtime, Code Signing, Notarization) and uses efficient caching (NSCache + background downloads). Communication is via JSON APIs, with GZIP compression and CORS enabled.

Tech Stack

Frontend: SwiftUI, AVKit, Combine, CoreAnimation, Metal, CoreImage
Backend: AWS Lambda, API Gateway, S3/MinIO, DynamoDB, CloudFront
Build & Infra: Xcode, SwiftPM, Shell scripts, HTTPS, JSON APIs
DevOps: GitHub Actions, macOS signing & notarization

Installation

git clone https://github.com/alxndlk/wallper-app.git
cd wallper-app

Requires macOS 14.0+, Xcode 14+, Swift 5.7+.

Project Structure
	•	App/ – Entry point & environment setup
	•	Core/ – Playback & caching
	•	Network/ – API & sync logic
	•	Shared/ – Utilities & modifiers
	•	Store/ – State management
	•	UI/ – SwiftUI views

License: Private project for educational/experimental use.

⸻

TL;DR:
A macOS app that delivers 4K video wallpapers using SwiftUI and Metal for high-performance playback, backed by a scalable AWS serverless backend with secure, optimized caching and syncing features.
