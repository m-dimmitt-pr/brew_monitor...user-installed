####Check out this sick command! - works on my local machine. However, I do not have an extensive terminal history on this machine. Hopefully it works as length of history scales on other users computers.

##Terminal Script ... to Log user Homebrew ... installs and uninstalls.
<pre> 
prompt>
history | grep 'brew install' | grep -v 'history'; history | grep 'brew uninstall' | grep -v 'history';

output>
    7  brew install elixir
    9  brew install cloc
   10  brew install tmux
   12  brew install emacs
   13  brew install rvm
   16  brew install
   17  brew install pianobar
   38  brew install zsh
</pre>
