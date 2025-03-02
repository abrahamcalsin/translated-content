---
title: How do I use GitHub Pages?
slug: Learn/Common_questions/Using_Github_pages
---

[GitHub](https://github.com/) is a "social coding" site. It allows you to upload code repositories for
storage in thecelio [Git](http://git-scm.com/) **version control system.** You can then collaborate on code projects, and the system is open-source by default, meaning that anyone in the world can find your GitHub code, use it, learn from it, and improve on it. You can do that with other people's code too! This article provides a basic guide to publishing content using Github's gh-pages feature.

## Publishing content

GitHub is a very important and useful community to get involved in, and Git/GitHub is a very popular [version control system](http://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) — most tech companies now use it in their workflow. GitHub has a very useful feature called [GitHub Pages](https://pages.github.com/), which allows you to publish website code live on the Web.

### Basic Github setup

1. First of all, [install Git](http://git-scm.com/downloads) on your machine. This is the underlying version control system software that GitHub works on top of.
2. Next, [sign up for a GitHub account](https://github.com/join). It's simple and easy.
3. Once you've signed up, log in to [github.com](https://github.com) with your username and password.

### Preparing your code for upload

You can store any code you like in a Github repository, but to use the GitHub Pages feature to full effect, your code should be structured as a typical website, e.g. with the primary entry point being an HTML file called `index.html`.

The other thing you need to do before moving on is to initialise your code directory as a Git repository. To do this:

1. Point the command line to your `test-site` directory (or whatever you called the directory containing your website). For this, use the `cd` command (i.e. "**c**hange **d**irectory"). Here's what you'd type if you've put your website in a directory called `test-site` on your desktop:

   ```bash
   cd Desktop/test-site
   ```

2. When the command line is pointing inside your website directory, type the following command, which tells the `git` tool to turn the directory into a git repository:

   ```bash
   git init
   ```

#### An aside on command line interfaces

The best way to upload your code to Github is via the command line — this is a window where you type in commands to do things like create files and run programs, rather than clicking inside a user interface. It will look something like this:

![](https://mdn.mozillademos.org/files/9483/command-line.png)

> **Nota:** You could also consider using a [Git graphical user interface](http://git-scm.com/downloads/guis) to do the same work, if you feel uncomfortable with the command line.

Every operating system comes with a command line tool:

- **Windows**: **Command Prompt** can be accessed by pressing the Windows key, typing _Command Prompt_, and choosing it from the list that appears. Note that Windows has its own command conventions differing from Linux and OS X, so the commands below may vary on your machine.
- **OS X**: **Terminal** can be found in _Applications > Utilities_.
- **Linux**: Usually you can pull up a terminal with _Ctrl + Alt + T_. If that doesn't work, look for **Terminal** in an app bar or menu.

This may seem a bit scary at first, but don't worry — you'll soon get the hang of the basics. You tell the computer to do something in the terminal by typing in a command and hitting Enter, as seen above.

### Creating a repo for your code

1. Next, you need to create a new repo for your files to go in. Click Plus (+) in the top right of the GitHub homepage, then choose _New Repository_.
2. On this page, in the _Repository name_ box, enter a name for your code repository, for example _my-repository_.
3. Also fill in a description to say what your repository is going to contain. Your screen should look like this:
    ![](https://mdn.mozillademos.org/files/12143/create-new-repo.png)
4. Click _Create repository_; this should bring you to the following page:
    ![](https://mdn.mozillademos.org/files/12141/github-repo.png)

### Uploading your files to GitHub

1. On the current page, you are interested in the section _…or push an existing repository from the command line_. You should see two lines of code listed in this section. Copy the whole of the first line, paste it into the command line, and press Enter. The command should look something like this:

    ```
    git remote add origin https://github.com/chrisdavidmills/my-repository.git
    ```

2. Next, type the following two commands, pressing Enter after each one. These prepare the code for uploading to GitHub, and ask Git to manage these files.

    ```bash
    git add --all
    git commit -m 'adding my files to my repository'
    ```

3. Finally, push the code up to GitHub by going to the GitHub web page you're on and entering into the terminal the second of the two commands we saw the _…or push an existing repository from the command line_ section:

    ```bash
    git push -u origin master
    ```

4. Now you need to create a gh-pages branch of your repo; refresh the current page and you'll see a repository page something like the one below. You need to press the button that says _Branch: **master**_, type _gh-pages_ in the text input, then press the blue button that says _Create branch: gh-pages_. This creates a special code branch called gh-pages that is published at a special location. It's URL takes the form _username.github.io/my-repository-name_, so in my example's case, the URL would be `https://chrisdavidmills.github.io/my-repository`. The page shown is the index.html page.
    ![](https://mdn.mozillademos.org/files/12145/repo-site.png)
5. Navigate to your GitHub Pages' web address in a new browser tab, and you should see your site online! Email it to your friends and show off your mastery.

> **Nota:** If you get stuck, the [GitHub Pages homepage](https://pages.github.com/) is also really helpful.

### Further GitHub knowledge

If you want to make more changes to your test site and upload those to GitHub, you simply need to make the change to your files just like you did before. Then, you need to enter the following commands (pressing Enter after each one) to push those changes to GitHub:

```
git add --all
git commit -m 'another commit'
git push
```

You can replace _another commit_ with a more suitable message to describe what change you just made.

We have barely scratched the surface of Git. To learn more, start off with the [GitHub Help site](https://help.github.com/index.html).
