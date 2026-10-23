# Hi, I'm Robert Tagliavia

## Video Streaming & Media Engineer

I'm a developer building video streaming pipelines and real-time systems. Recent work includes VOD transcoding with FFmpeg/NVENC, multi-format delivery with DRM packaging (HLS/DASH), a WebRTC SFU with simulcast, and forensic watermarking in Go. I work across the stack: TypeScript/Node.js on the backend, React on the frontend, and Go/Python for video processing.

---
## Featured Projects

### [video-streaming-service](https://github.com/rtagliaviaz/video-streaming-service)
A self-hosted VOD pipeline with GPU-accelerated transcoding (NVENC), adaptive bitrate (up to 7 renditions), CMAF/fMP4 packaging, and **dual DRM delivery**: HLS with AES-128 and DASH with ClearKey + EME. Includes a persistent BullMQ/Redis job queue, SSE progress updates, multi-audio support, subtitle extraction, and a dual-backend player (HLS.js + dash.js) with automatic capability detection.
`Node.js` `FFmpeg` `NVENC` `HLS` `DASH` `DRM` `CMAF` `BullMQ` `Redis`

### [dualstream](https://github.com/rtagliaviaz/dualstream)
A WebRTC Selective Forwarding Unit (SFU) built from scratch with **Pion and GStreamer**. Accepts three simulcast layers (`h`, `m`, `l`), forwards one layer per viewer based on RTCP REMB feedback, and switches layers dynamically without renegotiation. Includes an **HLS fallback** for clients that cannot use WebRTC, with automatic and manual switching in the viewer.
`Go` `WebRTC` `Pion` `GStreamer` `Simulcast` `HLS` `SFU`

### [watermark-service](https://github.com/rtagliaviaz/watermark-service)
A pure-Go CLI for **forensic and A/B watermarking** of video streams. Implements its own 2D DCT, CRC32-framed ID codec, Reed-Solomon FEC, and multi-frame voting. Forensic mode embeds a full ID into every frame for leak tracing; A/B mode embeds a single bit per segment for per-session traceability at scale, with constant storage overhead.
`Go` `DCT` `Watermarking` `Reed-Solomon` `DRM` `Video Security`

### Tech Stack

**Media & Streaming**  
FFmpeg • HLS • DASH • CMAF (fMP4) • NVENC (H.264/HEVC) • DRM (AES-128, ClearKey+EME) • VMAF • WebRTC (Pion) • GStreamer • Simulcast • ABR

**Languages**  
TypeScript • JavaScript • Go • Python • SQL

**Backend**  
Node.js • Express • REST APIs • GraphQL • Socket.io • JWT • Webhooks • BullMQ • Redis • FastAPI

**Frontend**  
React • Next.js

**Database**  
MySQL

**Integrations & APIs**  
CRM APIs (HubSpot, Monday, Escala, Clientify) • Asterisk AMI • Third-party APIs

**Infrastructure & DevOps**  
Linux • Docker • Docker Compose • Nginx • MinIO (S3-compatible) • AWS (EC2, S3, EFS, Glacier) • GitHub Actions • CI/CD

**Testing**  
Jest • Vitest

---

### Writing

- [Running GPU-accelerated VMAF (libvmaf_cuda) on Windows (WSL2 + Docker + NVIDIA)](https://dev.to/rtagl/-how-to-use-libvmafcuda-on-windows-an-easy-to-follow-guide-wsl2-docker-nvidia-59mc)
- [My HLS Video Took 7 Seconds to Seek. One FFmpeg Flag Fixed It](https://dev.to/rtagl/how-i-fixed-my-hls-seeking-lag-with-one-keyframe-trick-gop-explained-2gh6)
- [Building a Local Audio Track Remover with FFmpeg, Node.js, and Server-Sent Event](https://dev.to/rtagl/i-havent-posted-in-4-years-heres-what-i-built-a-local-audio-track-remover-with-react-nodejs-5d6k)

---


### 📫 How to Reach Me

- **Email**: [rtagliavia.pp@gmail.com](mailto:rtagliavia.pp@gmail.com)  
- **LinkedIn**: [linkedin.com/in/rtagliaviaz](https://www.linkedin.com/in/rtagliaviaz/)

