# ksp2-keybind-wallpaper

## Guide for customization

This wallpaper is a web page that can be imported into many live wallpaper programs.
Therefore, in order to edit it, you must make changes to the web page code, HTML.

The keybinds and headings are automatically formatted into as many columns as are necessary using a CSS flexbox. Therefore, to rearrange them, simply cut and paste them until you are satisfied.

### Steps to add, remove, and edit keybinds or headings

1. First, open index.html in a text editor (something as basic as Notepad works, but VSCode is reccomended)
2. Scroll down until you see this:

```html
<body>
    <main>
        <video id="background-video" autoplay loop muted poster="poster.jpg">
            <source src="background.webm" type="video/mp4">
        </video>
        <div class="container">
            <div class="heading">
                Flight
                <hr>
            </div>

            <div class="keybind">
                <div class="keybind-text">Pitch</div>
                <div class="keybind-box">
                    <div class="keybind-key">W S</div>
                </div>
            </div>
```

Let's go through it step by step. First, the `<body>` and `<main>` tags set up the basic document.
Then, the `<video>` tag adds the background video into the document.
A `<div` tag with the class `container` provides a place for all of the keybinds and headings to go.
Finally, we see a `<div>` withe the class `heading`.

3. If you want to add, remove, or edit headings, use this first as a template.
You can change the text inside, copy and paste it elsewhere in the document, or remove it entirely.
4. Next, we get down to a `<div>` with the class `keybind`. If you want to add more keybinds, remove, or change them, simply copy and paste, delete, or edit this section (including every `div` inside).
5. To change the name of the keybind, replace *Pitch* with something else. To change the keys that the keybind displays, change *W S* to something else.
