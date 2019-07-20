---
layout: post
title: "Testing Visual Studio Code - a not so baised review"
date: 2018-10-07
subtitle: "Trying Visual Studio Code for a full day of work."
bigimg: https://raw.githubusercontent.com/swarad07/swarad07.github.io/master/assets/img/property-info.png
tags: [Coding, testing, review, Editor, IDE]
comments: true
---

Hello world! Lets get straight to the point, for quite a while now I have been flirting with VSCode aside from my usual IDE which I have been using for more many years now (Only if my IDE could talk, I am pretty sure he would not approve of this affair). If I remember correctly I had downloaded VS Code the first day it was available. The idea of a good free "IDE" has always been something that has intrigued me.

If you must know, I one of those who has clear definations for an IDE and an editor, that will be a separate post. For large part of my initial career I have used [Eclipse](https://www.eclipse.org), I remember people using Notepad++ at that time, but notepad as a everyday code editor never landed right in my mind, even then. But code editors have improved massively since those days, [Sublime Text](https://www.sublimetext.com/), [Atom](https://atom.io/) are worth a mention from the huge list.

This is probably the first time I am sharing what I have found when switching to something else as my daily code editor.

A huge disclaimer that I am no way an expert on VS Code, infact I would go further and say I am pretty sure many of the below items would be fixable either via some extension or configuration, but sadly I have not yet spend time on finding them. So please help me in the comments to fix them if you know how.

## Things I like,
1. Customization - I am firmly on the "dark mode" everything side when it comes to my tools, as someone who stares at the screen for significant portion of my day, I find that dark modes strain my eyes less than the usual white background. So themes, fonts, line heights, were something that were easy to find, customize and tailor just the way I want.

2. VS Code advertises [IntelliSense](https://code.visualstudio.com/docs/editor/intellisense) as a code completion and code hinting feature, and from what I have used it works brilliantly, apprantly it uses a language service to analyze your source code and provide better comppletion and from what I have used it was on point.

3. Faster and less memory consuption - The biggest & the only reason I want to move away from my IDE is that it consumes significant portion of my tiny Macbook's processing power. A couple of browsers, one terminal, couple of design tools, slack for messages, zoom for meetings are pretty normal apps which I all use at the same time, so you can see processing power is at a premium (Atleast till I upgrade my machine).

4. The quick info option for any property is very good, you can quickly see the function defination as you type.
![quick-info](/assets/img/property-info.png)

## Things I absolutely hated out of the box, which were fixable.
1. Copy Paste Mess - I had to find my inner peace for this one, for some reason the formatting of entire file kept getting messed up when I did copy paste. Bit of searching and clearly I wasnt the only one, found this [stackoverflow answer](https://stackoverflow.com/questions/42747498/vs-code-indentation-when-copying-and-pasting-is-messed-up), I honestly dont know why this is ON by default.

2. Search - Autofilling the selected directory as scope. When I tried initially to search by selecting a directory and doing search it always searched in the scope that was last autofilled or entered manually, I expected it to autofill the diretcory path where to search based on which directory I selected. Luckily this was an easy fix using the keybindngs option in Code > Preferences > Keyboard Shortcuts. Here you will find all the possible functions you can do and bind them to a shortcut, I added this in keybindings.json,
{% highlight php %}
[
  {
    "key": "cmd+shift+f",
    "command": "filesExplorer.findInFolder",
    "when": "filesExplorerFocus"
  }
]
{% endhighlight %}

Now the search autofill works just the way I want on <kbd>CMD</kbd>+<kbd>SHIFT</kbd>+<kbd>F</kbd>

## Things I want to find a solution for,
1. For some reason my Xdebug doesnt work, I use drupal-vm as my local development stack, I am pretty sure something silly I am missing as the instruction [here ](http://docs.drupalvm.com/en/latest/extras/xdebug/) is pretty straightforward to make it work.

2. (Fix updated below) - When I click on a file in sidebar, it opens in new tab, if I click on a different file it opens again in the same tab closing the previous file. I think this has got to do with wether that file has any change or not, I dont know how to make each file open in a new tab always.

3. (Fix updated below) - CSS hierarchy - When you hover on selector I get to see the hierrarchy of the selectors, this is helpful in SCSS files. But I would love an bar at the bottom similar to how PHPStrom does it, where you see the parents as you type. This saves that additional hover action.
![php-storm-css](/assets/img/CSS-hierrachy.png)

4. Search - Old keywords. I find that I often do two seaprate searches and then have to go back to the old keyword to find a file I had just seen which is now not showing up. But there is no way I see that I can select that old keyword from a dropdown or something and run the old search again.

5. GIT history view - Finding old revisions of a file, comparing them with current revision or quickly checking out that old revision is all possible, but I feel it is not an optimal UX right now. I have seen other IDEs and editors do this better and I really hope VS Code improves this.

## Conlusion
After a long time I have found a code editor that I can really see myself using it as my daily driver. Granted I have spent last few months, switching to VS Code only to find something I dont like, mostly because I have gotten used to my current IDE. What I am really happy about is that nearly all those things that I didnt like I was either to find a workaround or straight up fix it by some config or extension. I am pretty sure if I use it for a month or two (that is the plan as of now) I will find solutions to the above dislikes, lets see how that goes, probably another post after that.

Cheers!


## Update

1. workbench.editor.enablePreview should be false [Link](https://stackoverflow.com/questions/38713405/how-to-config-vscode-to-open-files-always-in-a-new-tab)
{% highlight html %}"workbench.editor.enablePreview":false {% endhighlight %}

2. Enable breadcrumbs - View > Toggle Breadcrumbs. This shows the CSS heirrachy like I want.
