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
3.  You can add a new badge by following the existing format. It's best to use [shields.io](https://shields.io/) to generate a new badge.

    Here's an example of the format for a badge:

    ```html
    <a href="YOUR_PROFILE_URL" target="_blank">
      <img src="SHIELDS.IO_BADGE_URL" alt="BADGE_ALT_TEXT" />
    </a>
    ```

4.  Make sure to replace `YOUR_PROFILE_URL`, `SHIELDS.IO_BADGE_URL`, and `BADGE_ALT_TEXT` with the correct values.

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