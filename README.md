# Nftables

> A Sublime Text 3 syntax definition for your Nftables rules

![Preview](https://i.imgur.com/14wp8YU.png)

## Introduction

[Nftables](https://netfilter.org/projects/nftables/) should _now_ be the regular way of handling Netfilter rules, and I was surprised not to find any syntax definition for Sublime Text.  
This project aims to provide a "basic" one, as long as a building procedure for GNU/Linux users (when the `nft` binary is available for "dynamic" syntax checks).

This project has been inspired by [the official nano syntax definition](https://git.savannah.gnu.org/cgit/nano.git/tree/syntax/nftables.nanorc).  
See the [_Scripting_](https://wiki.nftables.org/wiki-nftables/index.php/Scripting) Nftables Wiki page for external reference.

## Installation

### With Package Control

1. Open your command palette and type in : `Package Control: Install Package`
2. Browse the list or search for `Nftables`
3. Press `Enter` and you're done !

Package Control dedicated page [here](https://packagecontrol.io/packages/Nftables).

### Manually

1. Move into Sublime Text packages folder (usually `$HOME/.config/sublime-text-3/Packages/User/` or `%AppData%\Sublime Text 3\Packages\User\`)
2. Clone this repository there : `$ git clone https://github.com/HorlogeSkynet/Nftables.git`
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

## Syntaxes currently supported

* [X] "nftables output" format
* [X] "scripted configuration" format

## Frequently Asked Questions

### Do you plan to support the _whole_ Nftables syntax ?

> No, but feel free to contribute.

### Why does this syntax coloration s\*cks ?

> Well, sorry to hear that. Grammar wasn't my favorite course at school.  
> I'd be pleased to review any [issue](https://github.com/HorlogeSkynet/Nftables/issues/new) or pull request.

### Why didn't you convert the [official Bison parser](https://git.netfilter.org/nftables/tree/src/parser_bison.y) to [Sublime's definition syntax](https://www.sublimetext.com/docs/3/syntax.html) ?

> [It looks like](https://forum.sublimetext.com/t/convert-bnf-yacc-grammar-definition-to-syntax-package/15980) such a tool does not exist (yet ?).

### Would this plugin help me building a secure fire-wall ?

> No, but I would advise you [this blog post](https://stosb.com/blog/explaining-my-configs-nftables/) as a well-explained starting point, written by [@tasn](https://github.com/tasn).
