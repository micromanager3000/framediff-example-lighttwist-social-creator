# LightTwist social · show-building creator

## Setup

```sh
git clone --recurse-submodules https://github.com/micromanager3000/framediff-example-lighttwist-social-creator.git
cd framediff-example-lighttwist-social-creator
npm install
npm run dev
```

FrameDiff is pinned in `vendor/framediff` until its packages are published to npm. Update the
pin with `git submodule update --remote vendor/framediff`, then validate and commit the gitlink.

A 9.5-second, 1080×1920 LightTwist social ad aimed at video-podcast and YouTube
show hosts.

The story is a direct before/after:

1. **0–2.2s — pain:** a remote-call grid with “Your podcast still looks like a call?”
2. **1.9–7.4s — transformation:** three LightTwist newsroom angles with “Make it a
   show,” “Remote guests,” and “One branded studio.”
3. **7.2–9.5s — action:** a branded end card with `lighttwist.com`.

The project carries its seven selected LightTwist media files as content-addressed Git LFS assets.
Their hashes match the source material in the independent
[`hero-reel`](https://github.com/micromanager3000/framediff-example-hero-reel) example.

Run the Studio:

```bash
npm run dev -- \
  --host 127.0.0.1 \
  --port 4181
```

The copy and audio levels are editable in
`src/compositions/CreatorSocial.comp.json`; timing and shot choice live in
`src/compositions/CreatorSocial.timeline.json`.
