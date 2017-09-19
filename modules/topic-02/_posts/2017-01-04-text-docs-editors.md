---
title: Text Docs & Editors
module: 02
---

## Working with Text:
<img src="./../../../img/arrow-divider.svg" style="width: 75px; border: none;" />

### What's a text document?
**Text documents** include many file types and can be simply described as any file that stores an [ASCII character set](https://en.wikipedia.org/wiki/ASCII) (as opposed to binary data), which is the most common format for the English language. These text files can include text documents of prose, code, or some combination of both.


#### What types of files are text documents?
The simplest and most common text document is a "text file", which will bare the `.txt` extension. This generic document type contains only ASCII characters. These are the common characters you use for writing and reading (A-Z, a-z, 0-9), and special characters (such as #, %, !, ., etc.). These files also include carriage returns (new line), tabs, spaces, and an end-of-file (eof) designation that lets a program know where the file finishes. This last group, of course, contains characters that are there but that are not displayed in basic text editors.


#### "Well, I have Microsoft Word, so..."
You might be tempted to say Microsoft Word Document files (`.doc` or `.docx`) are text files. However, these are actually containers of many smaller files that are ZIP-compressed together into the `.docx` file. This complex file that Microsoft uses allows them to store images, objects, text, and complex formatting instructions all in a single file, which can then be easy saved, shared, or sent between users of the Microsoft productivity applications. The downside to this format though is that you cannot open this file in a basic text editor to change it. This below image shows a Microsoft Word Document (`.docx`) opened in the Atom text editor. As you can see, this file does not present itself in a way that offers you much understanding of its contents.

![A docx file loaded into a simple text editor](../imgs/docx_in_atom.jpg)


#### "Okay. So what are other types of plain text-based file types?"
Well, as you might guess, most computer languages are saved as plain text or ASCII files. However, they often have different extensions. These extensions provide information to the computer, as well as to the user as to ‘how’ the file may be used or _compiled_.

In this class, we will be using the following text file types;

- Markdown; `.md`
- HyperText Markup Language (HTML); `.html`
- Cascading Style Sheet (CSS); `.css`
- JavaScript; `.js`

This Topic, we'll look at the first type, Markdown or `.md` files, using a text editor.

At it's end, we'll even begin looking at `.html` files and beginning structure.


### What's a text editor?
Text files can be created and edited using a **"Text Editor”**, which is any application for editing ASCII text documents. This includes both prose or code documents.

The default application on Mac and Windows are the following, respectively; _textEdit.app_ and _Notepad.exe._ However, specialty applications exist which can ease the type of work you will be undertaking this semester. These applications are designed to speed up the writing process and are specially designed to display text documents in a way that makes identifying errors more easy.

There are many types of text editors, each optimized for specific types of tasks. This [Wikipedia page on text editors](https://en.wikipedia.org/wiki/Text_editor) will familiarize yourself with some of the specifics and differences. Pay particular attentions to the “Typical Features” section.


### Atom (Text Editor for Development)

For this class, we need a text editor that is optimized for web development and code. You are welcome to use whatever text editor you like for this course, however, we will be using GitHub's open-source [Atom](https://atom.io) for our videos and tutorials, and it may behoove you to use it as well (especially beginners).


#### Installation Guide
##### For macOS
1. Download the software from the main [atom.io](https://atom.io) site.
2. Then drag the application that was downloaded from the Downloads folder to the Applications folder.

##### For Windows
1. Download the windows installer from the main [atom.io](https://atom.io) site.
2. **IMPORTANT:** when the download finishes, do not simply double-click from the bottom of the browser window. Instead, you first need to open the file in explorer. To do this you can either open explorer and navigate to the folder where it downloaded (likely "Downloads") _OR_ right-click or two-finger-click the file from the browser and select "Show in Folder".
![Pic demo-ing "show in folder" command](../imgs/showINFinder.png "Demo of show in folder.")
3. From the explorer you then need to right-click the file and select "Run as Administrator". This is especially important if you are not sure whether you are signed in as an admin.
![Image demo-ing how to "Run as Admin"](../imgs/runAsAdmin.png "Image demo-ing how to 'Run as Admin'")


#### Recommended Additions
Most text editors allow you to download additional packages created by the community which extend their functionality and can make them more suited to your particular needs. For Atom and this course, these would be very beneficial:

##### Theme
**Themes** customize the look and feel of the editor.
1. Navigate to the "Atom" main menu > Preferences... > Install.
2. To the right of the search bar, select "Themes."
3. Search for the **"newbound-dark-syntax"** theme. Install.
4. Navigate to "Themes" on the side menu.
5. Select "newbound-dark-syntax" as your “Syntax Theme."
<img src="../imgs/theme_search_in_atom.jpg" alt="example search for newbound-syntax-theme" />
<p style="font-size: small; margin: 0; padding-left: 50px;">"Newbound-dark-syntax" provides colorization for a number of languages, including markdown.</p>

##### Packages
Packages add functionality to your editor.
1. Navigate to the "Atom" main menu > Preferences... > Install.
2. Search for these packages. Install.
- _highlight-selected_ - Highlights all occurrences of a selected word. This is useful for debugging.
- _fonts_ - Many fonts that can easily be selected for use in Atom.
- _file-icons_ - Displays file type icons next to files in the sidebar.
- _language-markdown_ - Adds syntax support to themes without markdown syntax.
- _todo-show_ - Tools for showing “TODO”-s in code.
- _atom-html-preview_ - Allows preview of HTML files in Atom.
- _base linter_ - Base package to show code errors. Couple with *linter-htmlhint* and *linter-stylelint*
- _open-recent_ - Adds “open recent” functionality to the File menu in Atom.
- _pigments_ - Highlights color values in files.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://player.vimeo.com/video/232293574?color=1CCDCA&title=0&byline=0&portrait=0" frameborder="0" allowfullscreen></iframe></div>

More can be found on the [scotch websites discussion of Atom](https://scotch.io/bar-talk/best-of-atom-features-plugins-acting-like-sublime-text) if you're interested.


# { TODO: }
1. Create a file in a word processor (like a .docx) and create a file in a text editor (like a .txt). Experiment with opening them in their opposing applications. What happens?
2. Install Atom, and our theme and package recommendations.
