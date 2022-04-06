---
layout: default
title: Customization
nav_order: 6
---

# Customization
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

---
layout: default
title: Version Control: Sharing a project on Github
nav_order: 6
---

# Adding Version Control To a Current Project
{: .no_toc }
---
Adding version control helps keep track of changes by allowing contributors to push code with commit messages describing the changes. A commit message is a form of documentation that allows other team members to understand the changes that were made. Version control also allows for reviewing previous changes and old code blocks. The ability to review old code acts as a safety net in the case of future changes that may break the program, so having version control allows contributors to go back and change back the program to a point where it was functional. 
<!-- ## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc} -->

---
## Adding a Java Project to your Github 
This instruction set shows you how to:
- Adding Version Control to IntelliJ
- Sharing a project on your Github
- Committing and Pushing a Project 

Create a GitHub account [here](https://github.com/join) if you do not already have one. 

#### 1. Click on the File that is to be shared

<p align="center">
  <img src="../assets/images/vcs-images/Configuration_2.png" alt="VSC1" width="500">
</p>

#### 2. Navigate to the VSC tab in the top menu bar and click on Share Project on GitHub

<p align="Left">
  <img src="../assets/images/vcs-images/Configuration_3.png" alt="VSC2" width="500">
  <img src="../assets/images/vcs-images/Configuration_4.png" alt="VSC3" width="500">
</p>

#### 3. Press on Add Account.

<p align="center">
  <img src="../assets/images/vcs-images/Configuration_5.png" alt="VSC4" width="500">
</p>

It will bring you to a drop-down menu, but let us connect by logging into your GitHub account. 

<p align="center">
  <img src="../assets/images/vcs-images/Configuration_6.1.png" alt="VSC4" width="500">
</p>


#### 3 Click Sign in using GitHub and it will redirect you to a web page asking you to log into GitHub

You will see the following message, and just press the folloiwing button: 

  <p align="center">
  <img src="../assets/images/vcs-images/Configuration_7.1.png" alt="VSC4" width="500">
</p


#### 4 Log in using your Github Account

  <p align="center">
  <img src="../assets/images/vcs-images/Configuration_7.1.png" alt="VSC4" width="500">
</p
  
after logging in, you can close the web browser. You will be redirected back to IntelliJ with the following window, of which just press Share

#### 5. Press Share

  <p align="center">
  <img src="../assets/images/vcs-images/Configuration_8.png" alt="VSC4" width="500">
</p
  
#### 6. Type a meaningful Commit MEssage and check the files you want to add to your GitHub.
  
<p align="center">
  <img src="../assets/images/vcs-images/Configuration_9.png" alt="VSC4" width="500">
</p
  
#### 7. You should be brought back to the main window. Now PRess commit on the left-hand side of the screen.
  
<p align="center">
  <img src="../assets/images/vcs-images/Configuration_10.png" alt="VSC4" width="500">
</p
  
#### 8. Check the file you want to push to your GitHub repository. Type a meaningful commit message.
  
  <p align="center">
  <img src="../assets/images/vcs-images/Configuration_11.png" alt="VSC4" width="500">
</p

#### 9. Press commit and push.

 <p align="center">
  <img src="../assets/images/vcs-images/Configuration_11.png" alt="VSC4" width="500">
</p
 
#### 10. Open your Github repository on a web browser. and click on the file location of the project, which is located on the left-hand side of the commit message list.
<p align="center">
  <img src="../assets/ImagesOfAl/Configuration_12.png" alt="new_project_2" width="500">
</p>


You should be able to see 4 things 
1) the name of the project
2) the file you committed and pushed
3) your commit message
4) the file itself

<p align="center">
  <img src="../assets/ImagesOfAl/Configuration_13.png" alt="new_project_2" width="500">
</p>



## Color schemes

{: .d-inline-block }

New
{: .label .label-green }

Just the Docs supports two color schemes: light (default), and dark.

To enable a color scheme, set the `color_scheme` parameter in your site's `_config.yml` file:

#### Example
{: .no_toc }

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

## Custom schemes

### Define a custom scheme

You can add custom schemes.
If you want to add a scheme named `foo` (can be any name) just add a file `_sass/color_schemes/foo.scss` (replace `foo` by your scheme name)
where you override theme variables to change colors, fonts, spacing, etc.

Available variables are listed in the [\_variables.scss](https://github.com/just-the-docs/just-the-docs/tree/main/_sass/support/_variables.scss) file.

For example, to change the link color from the purple default to blue, include the following inside your scheme file:

#### Example
{: .no_toc }

```scss
$link-color: $blue-000;
```

_Note:_ Editing the variables directly in `_sass/support/variables.scss` is not recommended and can cause other dependencies to fail.
Please use scheme files.

### Use a custom scheme

To use the custom color scheme, only set the `color_scheme` parameter in your site's `_config.yml` file:

```yaml
color_scheme: foo
```

### Switchable custom scheme

If you want to be able to change the scheme dynamically, for example via javascript, just add a file `assets/css/just-the-docs-foo.scss` (replace `foo` by your scheme name)
with the following content:

{% raw %}
    ---
    ---
    {% include css/just-the-docs.scss.liquid color_scheme="foo" %}
{% endraw %}

This allows you to switch the scheme via the following javascript.

```js
jtd.setTheme("foo")
```

## Override and completely custom styles

For styles that aren't defined as variables, you may want to modify specific CSS classes.
Additionally, you may want to add completely custom CSS specific to your content.
To do this, put your styles in the file `_sass/custom/custom.scss`.
This will allow for all overrides to be kept in a single file, and for any upstream changes to still be applied.

For example, if you'd like to add your own styles for printing a page, you could add the following styles.

#### Example
{: .no_toc }

```scss
// Print-only styles.
@media print {
  .side-bar,
  .page-header {
    display: none;
  }
  .main-content {
    max-width: auto;
    margin: 1em;
  }
}
```
