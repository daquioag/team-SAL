---
layout: default
title: Troubleshooting
nav_order: 7
---

# Troubleshooting

<!-- {: .no_toc } -->

<!-- ## Responsive type scale -->

<!-- Just the Docs uses a responsive type scale that shifts depending on the viewport size. -->

| Symptoms              | Probably Cause                   | Action                        |
|:----------------------|:---------------------------------|:------------------------------|
| No Project SDK available when creating a new project in IntelliJ.   | No JDK is installed on your machine. | Install a JDK from [Oracle’s website](https://www.oracle.com/java/technologies/downloads/).|
| GitHub URL is not working when cloning a new project.  | Incorrect URL or type of version control selected.| Ensure Git is selected as the version control type when creating a new project and that an HTTPS URL was copied from GitHub. |
| Cannot connect to GitHub via IntelliJ.  | Your GitHub account is not connected to IntelliJ. | Login to GitHub through IntelliJ, or create a new authorization token from GitHub’s [personal access tokens page](https://github.com/settings/tokens).                          |
| My Git commits are not showing up on GitHub.  | Your commit may not have been pushed to GitHub. | After committing, you still need to push your files to the cloud. Click Git on the top menu bar and then select push. Confirm your push and your files should be sent to the GitHub repository on the cloud.|
| I accidentally committed a file that should not be on GitHub. | You may have check-marked a file unintentionally during the attempted commit using the IntelliJ GUI.| Navigate to GitHub and delete the file from the repository. Then, navigate to IntelliJ and click the blue arrow on the Git menu on the top right of the screen to pull the changes from GitHub.|
| I don’t see an option to use Code with Me in IntelliJ.| Your version of IntelliJ may not be up to date. | View this guide from Jetbrains to learn how to [update IntelliJ](https://www.jetbrains.com/help/idea/update.html). |
| My Code with Me guests can’t modify the project we are working on.| The guests likely do not have the proper permissions to access the project.| Ensure that the permissions set for the guests have “Full Access”. Otherwise, guests may not be able to access modify the project.|

<!-- --- -->

<!-- ## Table of contents

{: .no_toc .text-delta }

1. TOC
   {:toc}

---

Just the Docs uses [lunr.js](http://lunrjs.com) to add a client-side search interface powered by a JSON index that Jekyll generates.
All search results are shown in an auto-complete style interface (there is no search results page).
By default, all generated HTML pages are indexed using the following data points:

- Page title
- Page content
- Page URL

## Enable search in configuration

In your site's `_config.yml`, enable search:

```yaml
# Enable or disable the site search
# Supports true (default) or false
search_enabled: true
```

### Search granularity

Pages are split into sections that can be searched individually.
The sections are defined by the headings on the page.
Each section is displayed in a separate search result.

```yaml
# Split pages into sections that can be searched individually
# Supports 1 - 6, default: 2
search.heading_level: 2
```

### Search previews

A search result can contain previews that show where the search words are found in the specific section.

```yaml
# Maximum amount of previews per search result
# Default: 3
search.previews: 3

# Maximum amount of words to display before a matched word in the preview
# Default: 5
search.preview_words_before: 5

# Maximum amount of words to display after a matched word in the preview
# Default: 10
search.preview_words_after: 10
```

### Search tokenizer

The default is for hyphens to separate tokens in search terms:
`gem-based` is equivalent to `gem based`, matching either word.
To allow search for hyphenated words:

```yaml
# Set the search token separator
# Default: /[\s\-/]+/
# Example: enable support for hyphenated search words
search.tokenizer_separator: /[\s/]+/
```

### Display URL in search results

```yaml
# Display the relative url in search results
# Supports true (default) or false
search.rel_url: false
```

### Display search button

The search button displays in the bottom right corner of the screen and triggers the search input when clicked.

```yaml
# Enable or disable the search button that appears in the bottom right corner of every page
# Supports true or false (default)
search.button: true
```

## Hiding pages from search

Sometimes you might have a page that you don't want to be indexed for the search nor to show up in search results, e.g, a 404 page.
To exclude a page from search, add the `search_exclude: true` parameter to the page's YAML front matter:

#### Example

{: .no_toc }

```yaml
---
layout: default
title: Page not found
nav_exclude: true
search_exclude: true
---

```

## Generate search index when used as a gem

If you use Just the Docs as a remote theme, you do not need the following steps.

If you use the theme as a gem, you must initialize the search by running this `rake` command that comes with `just-the-docs`:

```bash
$ bundle exec just-the-docs rake search:init
``` -->

<!-- This command creates the `assets/js/zzzz-search-data.json` file that Jekyll uses to create your search index.
Alternatively, you can create the file manually with [this content]({{ site.github.repository_url }}/blob/main/assets/js/zzzz-search-data.json).
 -->
