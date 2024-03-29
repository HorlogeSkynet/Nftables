# Nftables

> A Sublime Text 3+ syntax definition for your nftables rules

![Preview](https://i.imgur.com/maXvyiJ.png)

## Introduction

[nftables](https://netfilter.org/projects/nftables/) should _now_ be the regular way of handling Netfilter rules, and I was surprised not to find any syntax definition for Sublime Text.  
This project aims to provide a "basic" one, as long as a building procedure for GNU/Linux users (when the `nft` binary is available for "dynamic" syntax checks).

This project has been inspired by [the official nano syntax definition](https://git.savannah.gnu.org/cgit/nano.git/tree/syntax/nftables.nanorc).  
See the [_Scripting_](https://wiki.nftables.org/wiki-nftables/index.php/Scripting) nftables Wiki page for external reference.

## Installation

### With Package Control

1. Open your command palette and type in : `Package Control: Install Package`
2. Browse the list or search for `Nftables`
3. Press `Enter` and you're done !

Package Control dedicated page [here](https://packagecontrol.io/packages/Nftables).

### Manually

1. Move into Sublime Text packages folder (usually `$HOME/.config/sublime-text/Packages/` or `%AppData%\Sublime Text\Packages\`)
2. Clone this repository there : `git clone https://github.com/HorlogeSkynet/Nftables.git`
3. Restart Sublime Text and... :tada:

## Usage

### Syntax

* Open your command palette and type in : `Set Syntax: Nftables`

* Click on the bottom-right corner : `Nftables`

* `View > Syntax > Nftables`

### Build

* Open your command palette and type in : `Build With: Nftables`

* Press `CTRL + B`

* `Tools > Build`

## [Formats](https://wiki.nftables.org/wiki-nftables/index.php/Scripting#File_formats) currently supported

* [X] nftables output
* [X] scripted configuration

## Frequently Asked Questions

### Do you plan to support the _whole_ nftables syntax ?

> No, but feel free to contribute.

### Why does this syntax coloration s\*cks ?

> Well, sorry to hear that. Grammar wasn't my favorite course at school.  
> I'd be pleased to review any [issue](https://github.com/HorlogeSkynet/Nftables/issues/new) or pull request.

### Why didn't you convert the [official Bison parser](https://git.netfilter.org/nftables/tree/src/parser_bison.y) to [Sublime's definition syntax](https://www.sublimetext.com/docs/syntax.html) ?

> [It looks like](https://forum.sublimetext.com/t/convert-bnf-yacc-grammar-definition-to-syntax-package/15980) such a tool does not exist (yet ?).

### Would this plugin help me building a secure fire-wall ?

> No, but I would advise you [this blog post](https://stosb.com/blog/explaining-my-configs-nftables/) as a well-explained starting point, written by [@tasn](https://github.com/tasn).

### I've noticed you got an extensive tests suite, can I run it ?

> Of course, open the `Nftables.sublime-syntax` file, press `CTRL + Shift + B` and choose `Build With: Syntax Tests`.
