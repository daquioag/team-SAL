---
layout: default
title: Creating a New Project
nav_order: 2
---

# Creating a New Project
{: .no_toc }

## Overview

Creating a new programming project can be challenging, but an IDE like IntelliJ can help streamline your workflows and help you start a new project quickly. One of the benefits of IntelliJ is the usage of a Guided User Interface (GUI) for many coding editor features. A GUI is a form of user interface that allows the user to perform actions by directly manipulating graphical elements. For example, rather than performing several actions to complete a task, a simple button press in IntelliJ can accomplish everything. 

We will be using IntelliJ’s GUI to create a new programming project in two ways: creating a local project from scratch or cloning a project from an existing repository on Github. Cloning a project means copying a project stored on the GitHub cloud, and downloading it to your local machine.

Hopefully, IntelliJ can help you streamline your programming and help you start a coding project swiftly and smoothly!

## Creating a New Local Project

The first method of starting a new programming project is creating one locally. This means creating a project from scratch without having the involvement of a version control system like GitHub. Creating a local project is an excellent way to start coding immediately on a smaller project. You don’t need to spend time setting up version control and can start coding immediately!

1. Press <code>⊞ Win</code> and type IntelliJ into the search bar, click the IntelliJ icon to open the application. On Mac, press <code>cmd</code> + <code>space</code> and type in IntelliJ, press enter to open the application.
   
2. Once IntelliJ is open, click the “New Project” button on the top right of the screen.
   
![new_project_1](../assets/images/new_project_img/new_project_1.png)
   
3. This will open up a new project interface that asks you for a Project SDK and additional libraries/frameworks. Click the dropdown menu to select a JDK version (this should already be installed from the preliminary requirements). In this case, we will select JDK 17. Click the “Next” button to confirm.
   
![new_project_2](../assets/images/new_project_img/new_project_2.png)
   
4. IntelliJ will ask if you want to create a project from an existing template, we will skip this and press “Next”.
   
5. In this stage, IntelliJ will ask for a project name and location. Input a name into the “Project name” text field. You can accept the default directory location for your project, or select a specific directory by pressing the “...” adjacent to the “Project location” field. Accept all default values under “More settings” and press “Finish”
   
![new_project_4](../assets/images/new_project_img/new_project_4.png)
   
6. A new window containing your new project should pop up. Now we need to create your very first Class, which is the foundation of all programs in Java.
   
![new_project_5](../assets/images/new_project_img/new_project_5.png)
   
7. On the left-hand side of your screen, find the directory called “src”. This looks like a small blue folder. Right-click on it and hover over “New”, then select “Java Class”.
   
![new_project_7](../assets/images/new_project_img/new_project_7.png)
   
8. A small window will appear, prompting you to give a name to your Class. Let’s enter “HelloWorld” into this field and press <code>enter</code>.
   
![new_project_8](../assets/images/new_project_img/new_project_8.png)
   
9. Congratulations! You just created your first Java program along with its first Class!
   
 ![new_project_9](../assets/images/new_project_img/new_project_9.png)

## Cloning a New Project from GitHub

Although creating a new local project can be a quick way to start coding, “ cloning” a project can be a quick way to jump into an already existing project. When working on a larger project with several contributors, it is important to keep a collection of save files to maintain your work. Think of GitHub as a cloud storage system that stores the save files to your project. When we “clone” a project from GitHub, we are grabbing a project saved on the cloud and loading it on our local machine. 

To start this process, there are a few things we need to prepare, namely connecting your GitHub account to IntelliJ. Please see the instructions on how to connect IntelliJ with GitHub before we begin.

1. Press <code>⊞ Win</code> and type IntelliJ into the search bar, click the IntelliJ icon to open the application. On Mac, press <code>cmd</code> + <code>space</code> and type in IntelliJ, press enter to open the application. On the top right of the screen, select the “Get from VCS” button.
   
2. A new window will pop up requesting Version control, URL, and directory.
   
![new_vcs_1](../assets/images/new_project_img/new_vcs_1.png)
   
3. Select Git for the version control field.
   
![new_vcs_2](../assets/images/new_project_img/new_vcs_2.png)
   
4. Navigate to a GitHub project you would like to clone.
   
5. Click the green “Code” button and copy the HTTPS URL to your clipboard. This is a unique link that is connected to your specific GitHub repository.
    
![new_vcs_3](../assets/images/new_project_img/new_vcs_3.png)
   
6. Paste this URL into the “URL” field in the IntelliJ window.
   
7. You can select a specific directory to save your project in by clicking the folder icon adjacent to the directory field, or you can simply accept the default location that is automatically generated.
   
![new_vcs_4](../assets/images/new_project_img/new_vcs_4.png)
   
8. Click the “Clone” button, and congratulations! You just successfully cloned your first project!
   
 ![new_vcs_5](../assets/images/new_project_img/new_vcs_5.png)
   
Just the Docs has some specific configuration parameters that can be defined in your Jekyll site's \_config.yml file.
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

View this site's [\_config.yml](https://github.com/just-the-docs/just-the-docs/tree/main/_config.yml) file as an example.

## Site logo

```yaml
# Set a path/url to a logo that will be displayed instead of the title
logo: "/assets/images/just-the-docs.png"
```

## Search

```yaml
# Enable or disable the site search
# Supports true (default) or false
search_enabled: true

search:
  # Split pages into sections that can be searched individually
  # Supports 1 - 6, default: 2
  heading_level: 2
  # Maximum amount of previews per search result
  # Default: 3
  previews: 3
  # Maximum amount of words to display before a matched word in the preview
  # Default: 5
  preview_words_before: 5
  # Maximum amount of words to display after a matched word in the preview
  # Default: 10
  preview_words_after: 10
  # Set the search token separator
  # Default: /[\s\-/]+/
  # Example: enable support for hyphenated search words
  tokenizer_separator: /[\s/]+/
  # Display the relative url in search results
  # Supports true (default) or false
  rel_url: true
  # Enable or disable the search button that appears in the bottom right corner of every page
  # Supports true or false (default)
  button: false
```

## Aux links

```yaml
# Aux links for the upper right navigation
aux_links:
  "Just the Docs on GitHub":
    - "//github.com/just-the-docs/just-the-docs"

# Makes Aux links open in a new tab. Default is false
aux_links_new_tab: false
```

## Heading anchor links

```yaml
# Heading anchor links appear on hover over h1-h6 tags in page content
# allowing users to deep link to a particular heading on a page.
#
# Supports true (default) or false
heading_anchors: true
```

## Footer content

```yaml
# Footer content
# appears at the bottom of every page's main content
# Note: The footer_content option is deprecated and will be removed in a future major release. Please use `_includes/footer_custom.html` for more robust
markup / liquid-based content.
footer_content: "Copyright &copy; 2017-2020 Patrick Marsceill. Distributed by an <a href=\"https://github.com/just-the-docs/just-the-docs/tree/main/LICENSE.txt\">MIT license.</a>"

# Footer last edited timestamp
last_edit_timestamp: true # show or hide edit time - page must have `last_modified_date` defined in the frontmatter
last_edit_time_format: "%b %e %Y at %I:%M %p" # uses ruby's time format: https://ruby-doc.org/stdlib-2.7.0/libdoc/time/rdoc/Time.html

# Footer "Edit this page on GitHub" link text
gh_edit_link: true # show or hide edit this page link
gh_edit_link_text: "Edit this page on GitHub."
gh_edit_repository: "https://github.com/just-the-docs/just-the-docs" # the github URL for your repo
gh_edit_branch: "main" # the branch that your docs is served from
# gh_edit_source: docs # the source that your files originate from
gh_edit_view_mode: "tree" # "tree" or "edit" if you want the user to jump into the editor immediately
```

_note: `footer_content` is deprecated, but still supported. For a better experience we have moved this into an include called `_includes/footer_custom.html` which will allow for robust markup / liquid-based content._

- the "page last modified" data will only display if a page has a key called `last_modified_date`, formatted in some readable date format
- `last_edit_time_format` uses Ruby's DateTime formatter; see examples and more information [at this link.](https://apidock.com/ruby/DateTime/strftime)
- `gh_edit_repository` is the URL of the project's GitHub repository
- `gh_edit_branch` is the branch that the docs site is served from; defaults to `main`
- `gh_edit_source` is the source directory that your project files are stored in (should be the same as [site.source](https://jekyllrb.com/docs/configuration/options/))
- `gh_edit_view_mode` is `"tree"` by default, which brings the user to the github page; switch to `"edit"` to bring the user directly into editing mode

## Color scheme

```yaml
# Color scheme supports "light" (default) and "dark"
color_scheme: dark
```

<button class="btn js-toggle-dark-mode">Preview dark color scheme</button>

<script>
const toggleDarkMode = document.querySelector('.js-toggle-dark-mode');

jtd.addEvent(toggleDarkMode, 'click', function(){
  if (jtd.getTheme() === 'dark') {
    jtd.setTheme('light');
    toggleDarkMode.textContent = 'Preview dark color scheme';
  } else {
    jtd.setTheme('dark');
    toggleDarkMode.textContent = 'Return to the light side';
  }
});
</script>

See [Customization]({{ site.baseurl }}{% link docs/customization.md %}) for more information.

## Google Analytics

```yaml
# Google Analytics Tracking (optional)
# e.g, UA-1234567-89
ga_tracking: UA-5555555-55
ga_tracking_anonymize_ip: true # Use GDPR compliant Google Analytics settings (true by default)
```

## Document collections

By default, the navigation and search include normal [pages](https://jekyllrb.com/docs/pages/).
Instead, you can also use [Jekyll collections](https://jekyllrb.com/docs/collections/) which group documents semantically together.

For example, put all your documentation files in the `_docs` folder and create the `docs` collection:

```yaml
# Define Jekyll collections
collections:
  # Define a collection named "docs", its documents reside in the "_docs" directory
  docs:
    permalink: "/:collection/:path/"
    output: true

just_the_docs:
  # Define which collections are used in just-the-docs
  collections:
    # Reference the "docs" collection
    docs:
      # Give the collection a name
      name: Documentation
      # Exclude the collection from the navigation
      # Supports true or false (default)
      nav_exclude: false
      # Exclude the collection from the search
      # Supports true or false (default)
      search_exclude: false
```

You can reference multiple collections.
This creates categories in the navigation with the configured names.

```yaml
collections:
  docs:
    permalink: "/:collection/:path/"
    output: true
  tutorials:
    permalink: "/:collection/:path/"
    output: true

just_the_docs:
  collections:
    docs:
      name: Documentation
    tutorials:
      name: Tutorials
```
