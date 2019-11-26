<h1 align="center">
𝐃𝐚𝐫𝐤
</h1>

|        |                                                     𝐎𝐫𝐢𝐠𝐢𝐧𝐚𝐥 𝐆𝐫𝐮𝐯𝐛𝐨𝐱                                                     |                                                     𝐆𝐫𝐮𝐯𝐛𝐨𝐱 𝐌𝐚𝐭𝐞𝐫𝐢𝐚𝐥                                                     |
| :----: | :----------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------: |
|  𝒉𝒂𝒓𝒅  |  ![original-hard-dark](https://user-images.githubusercontent.com/37491630/69468270-71d6c980-0d83-11ea-97f5-844accd52f68.png)  |  ![material-hard-dark](https://user-images.githubusercontent.com/37491630/69468250-65527100-0d83-11ea-98e8-04cc64e9270b.png)  |
| 𝒎𝒆𝒅𝒊𝒖𝒎 | ![original-medium-dark](https://user-images.githubusercontent.com/37491630/69468276-7602e700-0d83-11ea-8c31-4dd038e52114.png) | ![material-medium-dark](https://user-images.githubusercontent.com/37491630/69468257-697e8e80-0d83-11ea-8299-c0e5ecd132e3.png) |
|  𝒔𝒐𝒇𝒕  |  ![original-soft-dark](https://user-images.githubusercontent.com/37491630/69468280-78654100-0d83-11ea-9f69-2d0c0aa2dabb.png)  |  ![material-soft-dark](https://user-images.githubusercontent.com/37491630/69468264-6edbd900-0d83-11ea-815a-9d61509f3769.png)  |

<h1 align="center">
𝐋𝐢𝐠𝐡𝐭
</h1>

|        |                                                     𝐎𝐫𝐢𝐠𝐢𝐧𝐚𝐥 𝐆𝐫𝐮𝐯𝐛𝐨𝐱                                                     |                                                     𝐆𝐫𝐮𝐯𝐛𝐨𝐱 𝐌𝐚𝐭𝐞𝐫𝐢𝐚𝐥                                                     |
| :----: | :----------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------: |
|  𝒉𝒂𝒓𝒅  |  ![original-hard-light](https://user-images.githubusercontent.com/37491630/69468272-73a08d00-0d83-11ea-8065-c2875d6c5cb1.png)  |  ![material-hard-light](https://user-images.githubusercontent.com/37491630/69468253-671c3480-0d83-11ea-932d-1fe0ba559a1b.png)  |
| 𝒎𝒆𝒅𝒊𝒖𝒎 | ![original-medium-light](https://user-images.githubusercontent.com/37491630/69468278-77341400-0d83-11ea-9aa3-b6a94c442989.png) | ![material-medium-light](https://user-images.githubusercontent.com/37491630/69468260-6b485200-0d83-11ea-8329-c4564e40f65b.png) |
|  𝒔𝒐𝒇𝒕  |  ![original-soft-light](https://user-images.githubusercontent.com/37491630/69468281-7a2f0480-0d83-11ea-8ab0-3f0dc15fd0cb.png)  |  ![material-soft-light](https://user-images.githubusercontent.com/37491630/69468266-700d0600-0d83-11ea-8aa1-e97b86864a08.png)  |

The syntax highlighting logic used in this branch is as follows:

- **Red**: Keyword, Statement, Conditional, Repeat, Exception
- **Orange**: StorageClass, Operator, Structure, Label, Title, Tag
- **Yellow**: Type, Typedef, Special, SpecialChar
- **Green**: Method, String, Boolean, Character, Number, Float
- **Aqua**: Function, Constant, Define
- **Blue**: Identifier
- **Purple**: Macro, PreProc, Include, PreCondit

# Installation

## Via Plugin Manager

Take [vim-plug](https://github.com/junegunn/vim-plug) for example:

```vim
Plug 'sainnhe/gruvbox-material', { 'branch': 'neosyn' }
```

For better syntax highlighting support, please install [sheerun/vim-polyglot](https://github.com/sheerun/vim-polyglot).

## Manually

1. Clone this repository and checkout `neosyn` branch: `$ git checkout neosyn` .
2. Copy `/path/to/gruvbox-material/colors/gruvbox-material.vim` to `~/.vim/colors/` .
3. Copy `/path/to/gruvbox-material/doc/gruvbox-material.txt` to `~/.vim/doc/` and execute `:helptags ~/.vim/doc/` to generate help tags.
4. To install [airline](https://github.com/vim-airline/vim-airline) theme, copy `/path/to/gruvbox-material/autoload/airline/themes/gruvbox_material.vim` to `~/.vim/autoload/airline/themes/gruvbox_material.vim` .
5. To install [lightline](https://github.com/itchyny/lightline.vim) theme, copy `/path/to/gruvbox-material/autoload/lightline/colorscheme/gruvbox_material.vim` to `~/.vim/autoload/lightline/colorscheme/gruvbox_material.vim` .

## AUR

There is a package available for Arch Linux users in AUR: [gruvbox-material-neosyn-git](https://aur.archlinux.org/packages/gruvbox-material-neosyn-git/)

# Usage

## Vim

Put something like this in your vimrc:

```vim
" if you don't set this option, this color scheme will fall back to the original gruvbox
set termguicolors

" for dark version
set background=dark

" for light version
set background=light

" set contrast
" this configuration option should be placed before `colorscheme gruvbox-material`
" available values: 'hard', 'medium'(default), 'soft'
let g:gruvbox_material_background = 'soft'

colorscheme gruvbox-material
```

See `:help gruvbox-material-configuration` for more configuration options.

If you want to apply this color scheme temporarily, run this command in vim(**this may cause broken colors**):

```vim
:colorscheme gruvbox-material
```

## Airline

To enable [airline](https://github.com/vim-airline/vim-airline) color scheme, put this in your vimrc:

```vim
let g:airline_theme = 'gruvbox_material'
```

To apply it without reloading:

```vim
:AirlineTheme gruvbox_material
```

## Lightline

To enable [lightline](https://github.com/itchyny/lightline.vim) color scheme, put this in your vimrc:

```vim
let g:lightline = {}
let g:lightline.colorscheme = 'gruvbox_material'

" or this line
let g:lightline = {'colorscheme' : 'gruvbox_material'}
```

To apply it without reloading:

```vim
:let g:lightline.colorscheme = 'gruvbox_material'
:call lightline#init()
:call lightline#colorscheme()
```

# FAQ

**Q: It doesn't work as expected.**

**A:**

1. This color scheme is mainly designed for true colors, `set termguicolors` is required. Check output of `vim --version`, maybe your vim doesn't support `termguicolors`.

2. Maybe your terminal emulator doesn't support true colors, you can test it using [this script](https://unix.stackexchange.com/questions/404414/print-true-color-24-bit-test-pattern).

3. If you are running vim in tmux, you need to override default true colors of tmux, as tmux cannot display true color properly: [#1246 How to use true colors in vim under tmux?](https://github.com/tmux/tmux/issues/1246)

4. There are many highlight group links in syntax files while a color scheme may change them, enabling one color scheme based on another color scheme enabled is very likely to cause colors to break. If any color is broken, you can enable the color scheme in your vimrc instead of after vim startup.

**Q: What's your status line configuration?**

**A:** Check this [gist](https://gist.github.com/sainnhe/b8240bc047313fd6185bb8052df5a8fb).

**Q: What's the font used here?**

**A:** [Fira Code Nerd Font](https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/FiraCode).

# Contribution

Check this gist for detailed instructions to hack this color scheme: [hack-color-schemes.md](https://gist.github.com/sainnhe/911f78cbb092ac58c8734c423a464935)

# Related Projects

Color reference: [dark](https://github.com/sainnhe/gruvbox-material-vscode/blob/master/colors-dark.yml), [light](https://github.com/sainnhe/gruvbox-material-vscode/blob/master/colors-light.yml)

**Note**: The following projects are sorted by alphabet.

## Code Editor

- [Visual Studio Code](https://github.com/sainnhe/gruvbox-material-vscode) by [@sainnhe](https://github.com/sainnhe/)

## Terminal Emulators

- [Alacritty](https://gist.github.com/kamek-pf/2eae4f570061a97788a8a9ca4c893797) by [@kamek-pf](https://github.com/kamek-pf/)
- [Kitty](https://github.com/rsaihe/gruvbox-material-kitty) by [@rsaihe](https://github.com/rsaihe/)
- [Tilix](https://github.com/sainnhe/gruvbox-material-tilix) by [@sainnhe](https://github.com/sainnhe/)
- [Windows Terminal](https://gist.github.com/sainnhe/587a1bba123cb25a3ed83ced613c20c0) by [@sainnhe](https://github.com/sainnhe/)

## Other

- [Tmux](https://gist.github.com/sainnhe/b8240bc047313fd6185bb8052df5a8fb) by [@sainnhe](https://github.com/sainnhe/)
- [Zsh](https://gist.github.com/sainnhe/f92372e14c59750b6ac8dc927ba9f7fe) by [@sainnhe](https://github.com/sainnhe/)

# Inspirations

- [morhetz/gruvbox](https://github.com/morhetz/gruvbox): original gruvbox
- [sainnhe/vim-color-desert-night](https://github.com/sainnhe/vim-color-desert-night): the `white` color in the dark variant
- [atom.io](https://atom.io): the `white` color in the dark variant
- [zefei/cake16](https://github.com/zefei/cake16): the `black` color in the light variant
- [Google Material Design](https://en.wikipedia.org/wiki/Material_Design)

# License

[MIT](./LICENSE) && [Anti-996](./Anti-996-LICENSE)
