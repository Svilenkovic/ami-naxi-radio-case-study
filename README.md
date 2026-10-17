<a href="https://aminaxiradio.rs/"><img src="media/cover.jpg" alt="Ami Naxi Radio 105, home page on a laptop and a phone" width="100%"></a>

# Ami Naxi Radio 105

News portal for a radio station from Zrenjanin, on the same platform as Radio AMI but with its own design, 1,000 moved articles and a 105.0 player.

**[aminaxiradio.rs](https://aminaxiradio.rs/)** · [Case study (in Serbian)](https://svilenkovic.rs/radovi/ami-naxi-radio) · [Srpski](README.sr.md)

> [!NOTE]
> Client project. The source code belongs to the client and stays in a private repository. This page describes what I built and how.

<table>
  <tr><td><b>Client</b></td><td>Medijski centar Klik 105 doo Zrenjanin</td></tr>
  <tr><td><b>Industry</b></td><td>Local radio station and news portal</td></tr>
  <tr><td><b>Location</b></td><td>Zrenjanin, Serbia</td></tr>
  <tr><td><b>Type</b></td><td>News portal with an editorial panel (PWA)</td></tr>
  <tr><td><b>My role</b></td><td>Redesign, development, migration, hosting and maintenance</td></tr>
  <tr><td><b>Stack</b></td><td>PHP 8.3, MariaDB, Redis, nginx, PWA</td></tr>
</table>

## About the project

Ami Naxi Radio 105 broadcasts on 105 MHz and publishes news from Zrenjanin. Instead of a second site built from scratch, it runs on the platform I built for Radio AMI in Kikinda. There is one codebase, and each station has a profile with its name, frequency, colours, sections and stream addresses, so a fix or a new feature is made once and reaches both portals.

The two portals should not look like copies, so this one got its own design, which I called Silver Signal. The base is cool and light, the dark parts are navy and the red comes from the play button in the logo; a radio dial runs along the left edge as a guide line, and the player in the header has a small display showing 105.0. I moved 1,000 articles with their images, every image in AVIF and WebP variants, and 344 old addresses redirect to the new ones.

## What I built

- 1,000 articles moved with their images, each image in AVIF and WebP variants in several widths, and 344 redirects from old addresses
- One codebase shared with Radio AMI, with a site profile for the name, colours, sections, stream and legal details
- The Silver Signal design: a radio dial as the guide line, a player with a 105.0 display and a news mosaic on the home page
- A contact form through my central form service, with an HTML email to the newsroom and a confirmation to the sender
- A separate editorial panel installed as its own PWA, a public PWA and banner ads with statistics, with the partners moved from the old site
- Mobile Lighthouse median LCP of 1.6 to 1.8 s, CLS 0 and no axe violations; mobile PageSpeed 99 on 17 October 2026

## Results

| | Performance | Accessibility | Best practices | SEO |
| :-- | :-: | :-: | :-: | :-: |
| Mobile | 99 | 100 | 100 | 100 |
| Desktop | 100 | 100 | 100 | 100 |

PageSpeed Insights, lab test of the live site, October 2026. Security headers: 6 of 6. axe accessibility check: no violations. Structured data: `BroadcastService`, `NewsMediaOrganization`, `RadioStation`.

## Screenshots

<table>
  <tr>
    <td width="68%" valign="top"><img src="media/desktop.webp" alt="Ami Naxi Radio 105, home page on a 1440 px screen"></td>
    <td width="32%" valign="top"><img src="media/mobile.webp" alt="Ami Naxi Radio 105, home page on a phone"></td>
  </tr>
</table>

<img src="media/inner-1.webp" alt="Info service, with an ad and the live player in the side column">
<sub>Info service, with an ad and the live player in the side column</sub>

<img src="media/inner-2.webp" alt="Article page with the lead, author, date and reading time">
<sub>Article page with the lead, author, date and reading time</sub>

---

<sub>Built by [D. Svilenković](https://svilenkovic.com).</sub>
