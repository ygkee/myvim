myvim
=====

My personal Vim configuration

Maintaining a Vim configuration is a tricky business. Sometimes you make changes that you think will be helpful, find it annoying after a couple of weeks, and you want to revert back to an old version. That’s exactly why I keep mine under version control – you can view it here.

If you want to use this configuration, there are a couple of things you’ll need to install. You’ll need exuberant-ctags, as talked about in section 5. I’d also recommend installing the Anonymous Pro font if you’re using GVim, as it’s the best code font I’ve come across.

To install, clone the repository to ~/.vim, and initialize the submodule. Then, install the Vundle bundles:
````shell
$git clone git://github.com/joonty/myvim.git ~/.vim --recurse-submodules
$vim +BundleInstall +qall
````

What’s in the package? Along with everything mentioned in this tutorial, it has the following plugins:

    NERDTree: shows the directory tree, and allows for navigation and modification. Completely essential in my eyes.
    Fugitive: the definitive Git plugin.
    Ctrl-P: super-fast file finding and opening (used to be Command-T).
    EasyMotion: quickly jump to any word or character in a file.
    Vim-Sauce: a very simple project manager
    Syntastic: syntax checking for multiple languages
    MiniBufExpl: (Mini buffer explorer) shows the open buffers in a kind of tab format, allowing you to easily manage multiple files. I had serious performance issues with this plugin, so I no longer use it.
    Tag List:  show definition summaries of classes, functions, variables, etc. for all open files. I stopped using this plugin, as I found I could do everything with tags and Ctrl-P.

I swapped from Command-T to Ctrl-P, as Command-T requires you to build a library from source. Plus, Ctrl-P has some great additional features.

Here’s a word of warning: this is my configuration, and it’s likely to change on a fairly regular basis. I don’t guarantee that it will work on your system, and I certainly don’t guarantee that you’ll like it. Feel free to chop and change it as you please.
