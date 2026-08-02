# Contributing to My GitHub Profile

First off, thank you for considering contributing. This repository is for my GitHub profile's `README.md`, and your contributions help keep it up-to-date and representative of my work and interests.

## How to Contribute

There are two main ways you can contribute to this repository:

1.  **Updating Social Media and Contact Links**
2.  **Adding or Updating Blog Feeds**

### 1. Updating Social Media and Contact Links

All social media and contact links are located in the `README.md` file under the "Connect with Me" section.

To add or update a link:

1.  Open the `README.md` file.
2.  Navigate to the `## 🌐 Connect with Me` section.
3.  You can add a new badge by following the existing format. Prefer [Fancy Badges](https://jmcrafter26.github.io/badges/), which is the primary badge source for this README. Its URLs follow the pattern:

    ```
    https://jmcrafter26.github.io/badges/<category>/<badge>/<style>.svg
    ```

    Categories include `social`, `built-with`, `available`, `documentation`, `supported` and `donate`; styles are `cozy`, `compact`, `cozy-minimal` and `compact-minimal`. This README uses `compact` throughout — please stick to it so the rows line up.

    Here's an example of the format for a badge:

    ```html
    <a href="YOUR_PROFILE_URL" target="_blank">
      <img src="https://jmcrafter26.github.io/badges/social/mastodon-singular/compact.svg" alt="BADGE_ALT_TEXT" height="46" />
    </a>
    ```

4.  Make sure to replace `YOUR_PROFILE_URL` and `BADGE_ALT_TEXT` with the correct values, and check that the badge URL returns a `200` — not every badge in the catalogue is published to the GitHub Pages host.
5.  If Fancy Badges has no badge for the service you're adding, fall back to [shields.io](https://shields.io/) with `style=for-the-badge`, and add it to one of the shields.io-only rows so the two styles stay grouped rather than interleaved.

### 2. Adding or Updating Blog Feeds

The list of blog posts in the `README.md` is automatically updated by a GitHub Actions workflow. This workflow fetches the latest posts from the RSS feeds listed in `.github/workflows/blog-post-workflow.yml`.

To add a new blog feed:

1.  Open the `.github/workflows/blog-post-workflow.yml` file.
2.  Find the `feed_list` parameter.
3.  Add your new RSS feed URL to the list, separated by a comma.

    For example:

    ```yaml
    feed_list: "https://medium.com/feed/@saint2706,https://dev.to/feed/saint2706,https://your-new-feed.com/rss"
    ```

The workflow will run automatically every hour and update the `README.md` with the latest posts from all the feeds in the list.

## Submitting Changes

Once you've made your changes, please open a pull request with a clear description of the changes you've made. I'll review it as soon as possible.

Thank you again for your contribution!