## **Stash is a self-hosted webapp written in Go which organizes and serves your porn.**
![demo image](docs/readme_assets/demo_image.png)

* Stash gathers information about videos in your collection from the internet, and is extensible through the use of community-built plugins for a large number of content producers and sites.
* Stash supports a wide variety of both video and image formats.
* You can tag videos and find them later.
* Stash provides statistics about performers, tags, studios and more.

You can [watch a SFW demo video](https://vimeo.com/545323354) to see it in action.

For further information you can consult the [documentation](https://docs.stashapp.cc) or [read the in-app manual](ui/v2.5/src/docs/en).

# Usage

## Quickstart Guide
Stash is a web-based application. Once the application is running, the interface is available (by default) from http://localhost:9999.

On first run, Stash will prompt you for some configuration options and media directories to index, called "Scanning" in Stash. After scanning, your media will be available for browsing, curating, editing, and tagging.

Stash can pull metadata (performers, tags, descriptions, studios, and more) directly from many sites through the use of [scrapers](https://github.com/stashapp/stash/blob/develop/ui/v2.5/src/docs/en/Manual/Scraping.md), which integrate directly into Stash. Identifying an entire collection will typically require a mix of multiple sources:
- The project maintains [StashDB](https://stashdb.org/), a crowd-sourced repository of scene, studio, and performer information. Connecting it to Stash will allow you to automatically identify much of a typical media collection. It runs on our stash-box software and is primarily focused on mainstream digital scenes and studios. Instructions, invite codes, and more can be found in this guide to [Accessing StashDB](https://guidelines.stashdb.org/docs/faq_getting-started/stashdb/accessing-stashdb/).
- Several community-managed stash-box databases can also be connected to Stash in a similar manner. Each one serves a slightly different niche and follows their own methodology. A rundown of each stash-box, their differences, and the information you need to sign up can be found in this guide to [Accessing Stash-Boxes](https://guidelines.stashdb.org/docs/faq_getting-started/stashdb/accessing-stash-boxes/).
- Many community-maintained scrapers can also be downloaded, installed, and updated from within Stash, allowing you to pull data from a wide range of other websites and databases. They can be found by navigating to Settings -> Metadata Providers -> Available Scrapers -> Community (stable). These can be trickier to use than a stash-box because every scraper works a little differently. For more information, please visit the [CommunityScrapers repository](https://github.com/stashapp/CommunityScrapers).
- All of the above methods of scraping data into Stash are also covered in more detail in our [Guide to Scraping](https://docs.stashapp.cc/beginner-guides/guide-to-scraping/).

<sub>[StashDB](http://stashdb.org) is the canonical instance of our open source metadata API, [stash-box](https://github.com/stashapp/stash-box).</sub>
