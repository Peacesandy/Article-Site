# Article-Site
A hugo article site

# Installation

You can easily set up and create a Hugo website using a pre-built Hugo theme. With just a few short steps, you can then add content and pages to your website using Markdown.

# Windows 11

You will need an equivalent package manager for Windows. For example, you can use the Scoop package manager.

1. Open Windows PowerShell, which should already be a part of your Windows Operating System.
2. If you are installing Scoop for the first time, you may need to set your Execution Policy.
`Set-ExecutionPolicy RemoteSigned -scope CurrentUser`
3. Install Scoop:
`iex (new-object net.webclient).downloadstring('https://get.scoop.sh')`
4. Install Hugo:
`scoop install hugo extended`


## How to Create a Hugo Project
To create a new Hugo project, you will need to use the built-in hugo new site command.

1. Open your terminal or command prompt. Navigate to the folder where you would like to create your project.
2. Execute the hugo new site command:
`hugo new site new-hugo-website`
3. Navigate to the location of your Hugo project by typing code . in your terminal
4. A new folder will open in your vscode

## How to Add a Theme

1. Select a theme that you like. Each theme may have slightly different set-up instructions, shown on their respective preview page. This tutorial will use the Tale theme as an example.

2. Navigate to the root folder of your project in a terminal or command line.
`cd new-hugo-website`

3. Run the command to add the Tale theme. You can add the theme as a submodule, which will create a new folder called tale inside the theme folder.

`git init` 
`git submodule add https://github.com/EmielH/tale-hugo.git themes/tale`

Alternatively, you can clone the GitHub tale repository into the themes folder of your project.

`git clone https://github.com/EmielH/tale-hugo.git themes/tale`

4. In the config.toml file, add the tale theme as part of the configuration. This will tell Hugo to use the HTML, CSS, and other styles that the Tale theme includes.

## How to Add Pages to Your Website

You can write your content in any format that Hugo accepts. Hugo will then automatically convert your files into HTML files when serving them to the user. This makes it fast to both build and deploy. This example will use Markdown, a simple plain-text language, as the format for your content.

You can write Markdown mostly in plain English with a few added symbols to specify any formatting. This includes adding symbols to represent headings, which words are bold, or any other basic formatting that you may need.

To add a new sub-page or post to your website, you will need to add a new Markdown file into the content folder. Each post or page will have its own Markdown file associated with it.

1. Open the content folder inside your Hugo project. Create a new Markdown file called Article.md.

2. Open the file in any text editor such as Notepad++ or Visual Studio Code.

3. At the top of the file, add some metadata. This will include important information about the post. The theme you are using will format this information a certain way on the page.
---
author: "Your Name"
title: "My First Post"
date: "2022-05-17"
---
After you have added the metadata, you can start adding your content using Markdown.
This is my very first post on my Hugo website!
The Hugo theme being used for this site is called Tale.
It is very simple to install and configure.
# Subheading
This is some content.
# Another Subheading
This is more content.
Feel free to add more markdown files to add more pages to your website.

## How to Run and Test Your Hugo Website Locally
To run your website, use the hugo serve command.

1. Open a terminal or command line.
2. Navigate to the root folder of your Hugo project.
3. Run the hugo serve command:
`hugo serve`
4. Wait for the website to complete the startup process. Once that is complete, the terminal will print a message saying which local address you can access the website from. Usually, this is http://localhost:1313/.