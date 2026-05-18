# Dotsilicon Sitemap Generator

**Dotsilicon Sitemap Generator** is a desktop application for crawling websites and generating sitemap files for search engines.

It can create XML, TXT, HTML, and compressed GZIP sitemap files, including optional support for image, video, hreflang, and news sitemap extensions.

---

## Features

- Generate standard `sitemap.xml`
- Generate compressed `sitemap.xml.gz`
- Generate plain text `sitemap.txt`
- Generate human-readable `sitemap.html`
- Automatically create sitemap index files when needed
- Supports up to 50,000 URLs per sitemap file
- Optional image sitemap extension
- Optional video sitemap extension
- Optional hreflang sitemap tags
- Optional news sitemap extension
- Optional `changefreq` and `priority` values
- Respects `robots.txt`
- Detects and skips `noindex` pages
- Supports crawl delay and timeout settings
- Removes common tracking parameters such as `utm_*`, `fbclid`, `gclid`, and others
- Generates a `robots.txt` sitemap snippet
- Includes a generation report after completion

---

## Free and Paid Usage

The free mode allows sitemap generation for up to **100 URLs** per generation.

Generating larger sitemaps requires an active subscription.

Paid subscription mode supports sitemap generation for up to **50,000 URLs** per sitemap file.

---

## Download

Download the latest release from the GitHub Releases section:

https://github.com/dotsilicon/dotsilicon-sitemap-generator/releases

---

## How to Use

1. Open **Dotsilicon Sitemap Generator**.
2. Enter the website start URL.
3. Select the output folder.
4. Set the maximum number of pages to crawl.
5. Choose the sitemap options you need.
6. Click **Generate Sitemap**.
7. After completion, open the output folder and upload the generated sitemap files to your website root.

---

## Generated Files

Depending on selected options, the app may generate:

- `sitemap.xml`
- `sitemap.xml.gz`
- `sitemap.txt`
- `sitemap.html`
- `robots-sitemap-snippet.txt`
- `generation-report.txt`

For large websites, multiple sitemap files may be generated automatically:

- `sitemap.xml`
- `sitemap-1.xml`
- `sitemap-2.xml`
- `sitemap-3.xml`

---

## Recommended robots.txt Entry

After generating the sitemap, add the following line to your website’s `robots.txt` file:

```txt
Sitemap: https://example.com/sitemap.xml
```

Replace `https://example.com/` with your actual website URL.

---

## Sitemap Extensions

Dotsilicon Sitemap Generator can optionally include additional sitemap metadata:

- **Image sitemap extension** for image URLs found on crawled pages
- **Video sitemap extension** for video metadata where available
- **hreflang sitemap tags** for alternate language or regional pages
- **News sitemap extension** for news publication metadata
- Optional **changefreq** and **priority** values

---

## Crawling Behavior

The app crawls internal website links from the provided start URL.

It can:

- Follow same-site links
- Skip non-HTML files
- Skip pages blocked by `robots.txt`
- Skip pages marked with `noindex`
- Normalize duplicate URLs
- Remove common tracking query parameters
- Read canonical URLs where available
- Generate sitemap output based on discovered indexable pages

---

## Notes

- Sitemap generation depends on publicly accessible website links.
- Pages blocked by `robots.txt` may be skipped when robots support is enabled.
- Pages with `noindex` meta tags are not included.
- Search engines decide whether submitted URLs will be crawled, indexed, or ranked.
- Video sitemap entries without required thumbnail data may be skipped to avoid invalid sitemap metadata.
- The generated sitemap files should usually be uploaded to the root directory of your website.

---

## Legal Notice

Use this software only on websites you own, manage, or are authorized to crawl.

Do not use this software for unauthorized scraping, abusive crawling, spam activity, or any activity that violates website terms, privacy rules, robots.txt policies, or applicable laws.

---

## Publisher

**Dotsilicon Limited**  
Website: https://www.dotsilicon.com/

---

## License

This software is published by **Dotsilicon Limited**.

All rights reserved unless otherwise stated in the repository license file.
