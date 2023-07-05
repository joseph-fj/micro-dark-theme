# Micro dark-theme
If you're a Micro editor user, you may
find that its built-in colorschemes don't fullfil
your syntax highlighting desires.. so I recommend you
to try this dark theme which I have made using `.micro` files
that is provided by micro editor.
## Setup
First, navigate to ~/.config/micro/ directory and create 
`colorschemes` directory if it's not created yet.
```shell
cd .config/micro/ && mkdir colorschemes
```
Second, create a file with `.micro` extension as you prefer,
for Example: `darkTheme.micro`. Now open the file with micro
and paste the following code in:
```micro
color-link default "#F8F8F2,#282A36"
color-link comment "#6272A4"

color-link identifier "#FBC95F"
color-link identifier.class "#8BE9FD"
color-link identifier.var "#FE9B40"

color-link constant "#F87C74"
color-link constant.number "#F87F7A"
color-link constant.string "#84FB94"

color-link constant.bool "#FD89FF"
color-link constant.string.url "FC45FD"

color-link symbol.operator "#78C7FC"
color-link symbol.brackets "#B7B7B7"

color-link symbol.tag "#71E1FC"

color-link type "#FDA667"
color-link type.keyword "#FDA13CC"

color-link special "#F87F7A"
color-link statement "bold #71E1FC"
color-link preproc "#FF79C6"

color-link underlined "#FF79C6"
color-link error "bold #FF5555"
color-link todo "bold #FF79C6"

color-link diff-added "#50FA7B"
color-link diff-modified "#FFB86C"
color-link diff-deleted "#FF5555"

color-link gutter-error "#FF5555"
color-link gutter-warning "#E6DB74"

color-link statusline "bold #78CBFE,#333333"
color-link tabbar "bold #78CBFE,#333333"
color-link indent-char "#89FFCB"

color-link line-number "#6072A4"
color-link current-line-number "#89FFCB"
color-link divider "#444444,#444444"

color-link cursor-line "#44475A,#F8F8F2"
color-link color-column "#FFFFFF"
color-link type.extended "default"
```
Now you have done the important part,
open micro again and press `Ctrl-e` and type the following
`set colorscheme darkTheme.micro`.
You must write the same name of the file you created in colorschemes dir.
# Configuration 
In ~/.config/micro/ directory there is file named
`settings.json` open it and add what you prefer from the
code bellow.
```json
{
    "basename": true,
    "colorscheme": "mytheme",
    "fileformat": "dos",
    "hlsearch": true,
    "mkparents": true,
    "scrollmargin": 20,
    "softwrap": true,
    "statusformatl": "$(status.branch) $(filename) |$(modified)($(line),$(col))| $(status.paste)|ft:$(opt:filetype)|
$(opt:fileformat) | $(opt:encoding) [$(status.size)] [lines:
$(status.lines)]",
    "statusformatr": "",
    "sucmd": "doas",
    "tabhighlight": true,
    "tabsize": 80,
    "wordwrap": true,
    "xterm": true
}
```
Save the file, open micro again
and you will see some cool changes..
<br>
*Note: you're free to edit anything included here,
you can read more about micro options in micro by pressing Ctrl-e and typing
`help options` or on thier official site.
