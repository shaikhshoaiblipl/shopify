# Shopify Installation
 
Shopify CLI 2.0 is a command line to help you build on Shopify. It's available as a Ruby gem and can be run and installed on Mac, Linux, and Windows systems.

## Prerequisite
 
Before you start using Shopify CLI to develop themes, make sure that you do the following tasks:

- [Install CLI](https://github.com/Shopify/cli).
- Install [Ruby](https://www.ruby-lang.org/en/) or [Ruby+Devkit using RubyInstaller for Windows](https://rubyinstaller.org/downloads/) (2.7 or higher).
- Install [Git.](https://git-scm.com/downloads)
- If you want to use a [development store](https://shopify.dev/themes/tools/development-stores) to build a theme, then create or log in to a [Shopify Partner account](https://accounts.shopify.com/signup?rid=6b9caccd-0c8c-4a25-a939-e15884459a54), and then create a [development store](https://shopify.dev/themes/tools/development-stores#create-a-development-store-to-build-and-test-your-theme).
- Note the URL of the store that you want to work on.


## Install Shopify CLI

Install Shopify CLI on macOS or Windows. For other platforms and package managers, refer to [Install Shopify CLI](https://shopify.dev/themes/tools/cli/installation).

After checkout this reposatory you need to follow below steps:

- RmacOS (Homebrew)
``` bash
brew tap shopify/shopify
brew install shopify-cli
```

- Windows (RubyGems.org)
``` bash
gem install shopify-cli
```

## Authenticate

Use [shopify login](https://shopify.dev/themes/tools/cli/core-commands#login) to connect Shopify CLI with the store that you want to work on.

- 1. In a terminal, type shopify login --store <DOMAIN>, where <DOMAIN> is the store that you want to log into:
  ``` bash
shopify login --store johns-apparel.myshopify.com
  ```

- 2. In your browser window, log into the account that's attached to the store that you want to use for development.



## Create a new theme
Use [shopify theme init](https://shopify.dev/themes/tools/cli/theme-commands#init) to create a new theme on your local machine.
``` bash
shopify theme init
```  

## Use an existing theme

If you want to use an existing local theme for development, then navigate to the theme's directory on your local machine using cd [path/to/theme]. Any Shopify CLI [theme command](https://shopify.dev/themes/tools/cli/theme-commands) that you run uses the theme in that directory.

- Pull the theme onto your local machine using [shopify theme pull](https://shopify.dev/themes/tools/cli/theme-commands#pull). You're prompted to select a theme from the list of themes on the store.
```bash
shopify theme pull [ ROOT ] [ options ]
```
After listing all the themes' names, you can choose theme, Once you choose theme, all the scripts will be pulled on your machine. And then you can run the application.
```bash
shopify theme serve 
```
- 

## [Additional Commands](https://shopify.dev/themes/tools/cli/theme-commands)