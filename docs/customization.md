---
layout: default
title: Customization
nav_order: 6
---

# Customization
<!-- {: .no_toc }
 -->
<!-- ## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc} -->

---

---
layout: default
title: Version Control: Sharing a project on Github
nav_order: 6
---

# Adding Version Control To a Current Project

<!-- {: .no_toc } -->

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
Create a JetBrains account [here](https://account.jetbrains.com/login) if you do not already have one.   




1. Press <code>⊞ Win</code> and type IntelliJ into the search bar, click the IntelliJ icon to open the application.  
 On Mac, press <code>cmd</code> + <code>space</code> and type in IntelliJ, press enter to open the application.


You will be brought to a "Welcome to IntelliJ IDEA" window.

2. Click on the  Project File that you to add version control to. 

![chooseProject](../assets/images/VSC-images/VSC_2.png)


2. Navigate to the VSC tab in the top menu bar click on Share Project on GitHub. 


![topBarMenu](../assets/images/VSC-images/VSC_4.png)

Click on Share Project on GitHub.  

![ClickOnVSC](../assets/images/VSC-images/VSC_5.png)

A "Share Project On GitHub" window will pop-up.

3. Click on "Add Account" in the "Share Project On GitHub" window.

It will bring you to a drop-down menu, but let us connect by logging into your GitHub account.   

4. Click on "Log in via GitHub..."

>![addAccount](../assets/images/VSC-images/VSC_7.png)


You will be redirected to the following JetBrains web browser.

>![addAccount](../assets/images/VSC-images/VSC_15.png)

4. Log in using your Github Account

Click "Authorize in GitHub" and it will ask you to log into GitHub.
Add in your GitHub log-in information and click on "Sign in".  


>![addAccount](../assets/images/VSC-images/VSC_8.png)

  
After logging in, and seeing the "You have been successfully authorized in GitHub" message, you can close the web browser. 

>![addAccount](../assets/images/VSC-images/VSC_16.png)


Navtigate back to IntelliJ, and you will see the the "Share Project On GitHub" window in IntelliJ.
You should see your GitHub account URL  in the text box labeled "Share by: "


5. Press Share in the  "Share Project On GitHub" window


>![addAccount](../assets/images/VSC-images/VSC_9.png)

You should a "Add Files For Initial Commit" window where you can see all your project files.

  
6. Check the projects files you want to add to your GitHub and type a meaningful commit message under the "Commit Message" text box.
  
>![addAccount](../assets/images/VSC-images/VSC_10.png)

  
7. You should be brought back to the main window. Now Press the commit tab on the left-hand side of the screen.
  
>![commitMenu](../assets/images/VSC-images/VSC_11.png)

#### 8. Check the file you want to push to your GitHub repository. Type a meaningful commit message.

  
>![CommitPush](../assets/images/VSC-images/VSC_12.png)


#### 9. Open your Github repository on a web browser. and click on the file location of the project, which is located on the left-hand side of the commit message list.

>![goToGitHub](../assets/images/VSC-images/VSC_13.png)


You should be able to see 4 things 
1) the name of the project  
2) the file you committed and pushed  
3) your commit message  
4) the file itself  

>![checkProject](../assets/images/VSC-images/VSC_14.png)



<!-- 
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
{: .no_toc } -->

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
