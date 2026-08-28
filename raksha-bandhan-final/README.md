# 🎀 Raksha Bandhan Surprise — Final Version

A polished, mobile-first, front-end-only Raksha Bandhan surprise website.

## What is fixed in this version

- No sound / audio.
- Hero cartoon artwork is included locally.
- Envelope letter is readable and stays visible.
- Letter has 4 pages with **Back / Next** controls.
- The envelope does not automatically hide the text.
- Brother/sister artwork is local and replaceable.
- Memory images rotate around a centre image.
- Users can add multiple personal photos.
- Personalization supports sister name, brother name and custom message.
- Personalized text is preserved in the URL so it can be shared.
- Photos are intentionally local to the device and are NOT uploaded anywhere.
- Fully responsive for phones.
- No framework, npm, build step or backend required.

## 📁 Structure

```text
raksha-bandhan-final/
├── index.html
├── README.md
└── assets/
    ├── hero-brother-sister.png
    ├── final-brother-sister.png
    ├── memory-sample-1.png
    ├── memory-sample-2.png
    ├── memory-sample-3.png
    └── reference-design.png
```

## 🖼️ Replace the cartoon images

You do NOT need to change the HTML if you keep the same filenames.

Replace:

```text
assets/hero-brother-sister.png
```

with your own hero cartoon.

Replace:

```text
assets/final-brother-sister.png
```

with your own final cartoon.

Replace:

```text
assets/memory-sample-1.png
assets/memory-sample-2.png
assets/memory-sample-3.png
```

with sample memory images.

Keep the filenames exactly the same.

## 🧑‍💻 Important: what gets shared?

### Names and custom message

When someone uses **Apply & Create Shareable Version**, the sister name, brother name and custom message are put into the URL.

Example concept:

```text
https://your-site.vercel.app/?sister=Priya&brother=Aaditya&message=You%20are%20the%20best%20sister
```

So another person opening that link sees the personalized text.

### Photos

Photos selected using **Add Your Photos Here** stay inside that browser/device.

They are NOT uploaded to GitHub, Vercel or a server.

This is intentional.

If you later want:

> upload photos → generate unique permanent link → send that link to sister

then you need a backend/storage service such as Supabase, Firebase, Cloudinary or another storage solution.

## 🔁 Can multiple people reuse it?

**Yes.**

Because the site is static, unlimited people can open the same Vercel URL and create their own personalized version.

Each person can:
1. Enter names.
2. Enter their own message.
3. Add their own photos.
4. Generate/share their personalized URL.

The repository does not get changed when they personalize the card.

## 🚀 GitHub upload

Do NOT upload the ZIP as the website.

Extract the ZIP first.

Your GitHub root must look like:

```text
assets/
index.html
README.md
```

Then commit/push.

## 🚀 Vercel

Import the GitHub repository.

Use:

```text
Framework Preset: Other
Build Command: empty
Output Directory: .
Install Command: empty
```

No npm install is required.

## 🎬 Instagram Reel

A good reel flow:

```text
"I made a Raksha Bandhan surprise website ❤️"

→ Happy Raksha Bandhan
→ Open My Surprise
→ Envelope opens
→ Next message
→ Brother/sister cartoon
→ Our Beautiful Memories
→ Add Your Photos
→ Photos rotate
→ Personalize Your Card
→ Share This Surprise
```

CTA:

> Comment **SISTER ❤️** and I'll share the free template.

## 🛠️ Future upgrade

For a true public "Create Your Rakhi Card" tool:

- permanent photo uploads
- unique card IDs
- QR code
- WhatsApp sharing
- download as image
- export to video
- more themes
- Hindi/English switch
- swipeable photo carousel
- database-backed cards


## 🟢 WhatsApp + personalized image sharing

The **Save Changes** button creates a personalized link containing:
- sister name
- brother name
- custom message
- replaced cartoon images

The **Share on WhatsApp** button opens WhatsApp with that link ready to send.

Images are resized/compressed in the browser before being placed into the URL. They are **not uploaded to a server**. For best results, use a small number of reasonably sized images.

### Important limitation

Because this is a pure static front-end, the personalized images are carried inside the URL fragment. Very large collections of photos can make the link too long for some apps/browsers. For a production version with unlimited photo sharing, a backend/storage service is recommended.

### Replacing the built-in cartoons

Use the "Customize the Cartoon Images" controls. Pick a new image for Hero, Final, or Memory 1–3, click **Save Changes**, then click **Share on WhatsApp**.

The original built-in cartoon artwork remains the default for everyone else. One user's customization does not modify the GitHub files.
