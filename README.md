# nunngroupllc.com

The Nunn Group LLC website, hosted on GitHub Pages. Built November 6, 2026.

## What's here
- `index.html`: the homepage
- `privacy.html`: the privacy notice (linked in the footer)
- `404.html`: shown for broken or old links
- `assets/css/site.css`: colors, fonts, and layout
- `assets/img`: logos, photos, the DBE seal, and the social preview image (`og-image.jpg`)
- `assets/video`: the 1-minute overview video (MP4 and WebM) and its cover image
- `assets/fonts`: the Geist typeface (free to use under the SIL Open Font License, included as `OFL.txt`)
- `favicon.ico`, `apple-touch-icon.png`: browser tab and phone home screen icons
- `robots.txt` and `sitemap.xml`: for search engines
- `.nojekyll`: tells GitHub to publish the files exactly as they are. Don't delete it.
- `CNAME`: GitHub adds this when the custom domain is set. Don't delete it.

## Change text
1. Open `index.html` in this repository and click the pencil icon (Edit).
2. Change the words between the tags. Leave the tags themselves alone.
3. Click **Commit changes**. The live site updates in a minute or two.

## Replace a photo
Upload a new file into `assets/img` with the same file name as the one it replaces. Keep the same shape: the lakefront photo is portrait (4 by 5) and the headshot is landscape (3 by 2). For sharp results on phones and Retina screens, use at least 1600 pixels wide for the lakefront photo and 2000 for the headshot.

## Contact form
Messages go through Formspree (form code `maeezebj`), which forwards each one to marc@nunngroupllc.com. To switch to a different Formspree form, search `index.html` for `maeezebj` and replace it with the new code.

## Contact card
The Contact section links to Marc's Blinq card at https://blinq.me/SRlIHIAqhaoJ4bfBvpeN. If the card changes, search `index.html` for `blinq.me` and replace the link.

## Booking
Every booking button links to https://calendly.com/nunngroup/30min. Calendly opens in a pop-up on the page once its script loads; if it's blocked, the button opens Calendly in a new tab. To change the link, search `index.html` for `calendly.com/nunngroup/30min` and replace every match.

## Capabilities statement
The "Ask for our capabilities statement" button fills in a request on the contact form. To link it to a PDF instead, upload the PDF to `assets`, then in `index.html` change the button's `href="#contact"` to the PDF's path (for example `assets/nunn-group-capabilities.pdf`) and delete its `data-prefill="..."` attribute. Both steps are needed.

## DBE seal
To hide the seal, open `index.html`, find `DBE SEAL START`, and delete everything from that line down to and including the `DBE SEAL END` line. Commit the change.

## Overview video
The "Watch the overview" button on Marc's photo plays `assets/video/nunn-group-overview.mp4`. Phones held upright play a tall version with larger type instead, `assets/video/nunn-group-overview-tall.mp4`. To swap in a new version of either one, upload new files with the same names. If the length changes, also update "1:00" on the button, "1 minute" in the video window, the transcript under the video, and the `duration` in the VideoObject data near the top of `index.html`. To remove the video, delete the line in `index.html` that starts with `<button type="button" class="play"`.

## Opening animation
When someone opens the homepage, the logo animates (the sun rises, the N is etched through it) and then glides into the top-left corner. It takes about 1.5 seconds and plays once every 30 days on each device. It does not play on links that go straight to a section, such as /#contact. Any tap, click, scroll, or key press skips it. It never plays for visitors who have "reduce motion" turned on, or for search engines. To watch it again, open https://www.nunngroupllc.com/?intro. To turn it off, open `index.html`, find `Opening logo animation` near the top, delete the line right below it, and commit the change.

## Analytics
Off until a Google Analytics 4 Measurement ID is added. In `index.html`, find `GA_MEASUREMENT_ID = ''` near the top and paste the ID between the quotes (it looks like `G-XXXXXXXXXX`). It then records visits, plus these events: booking clicks (`book_call_click`), messages sent (`generate_lead`), phone and email clicks (`phone_click`, `email_click`), growth check results (`growth_check_complete`, `growth_check_send`), video plays (`video_play`), and capabilities statement requests (`capabilities_request`).
