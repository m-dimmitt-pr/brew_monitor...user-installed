<pre>
how to unset bash history
unset HISTSIZE 
unset HISTFILESIZE
shopt -s histappend
https://debian-administration.org/article/543/Bash_eternal_history
http://unix.stackexchange.com/questions/17574/is-there-a-maximum-size-to-the-bash-history-file
</pre>


##Story: Why remember_Homebrew (Install/Uninstall) User_Decisions?
"brew list" for homebrew, is great!
"brew list" tells - (everything homebrew has done to get me there).
However, I wanted to know specifically as a user my install and uninstall efforts.

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

##Terminal Script ... to Log user apt-get's ... installs and uninstalls.
<pre>
prompt>
history | grep 'apt-get install' | grep -v 'history'; history | grep 'apt-get uninstall' | grep -v 'history';
</pre>

##Terminal Script ... to Log user yum's ... installs and uninstalls.
<pre>
prompt>
history | grep 'yum install' | grep -v 'history'; history | grep 'yum uninstall' | grep -v 'history';

output>
  91  sudo yum install git
   99  sudo yum install mysql-server
  153  yum install mysql-devel
  180  yum install libSM.so.6
  181  yum install libXdamage.so.1
  182  yum install libXext.so.6
  183  yum install libXfixes.so.3
  186  yum install libXinerama.so.1
  187  yum install libXrandr.so.2
  188  yum install libXrender.so.1
  189  yum install libXtst.so.6
  190  yum install libasound.so.2
  191  yum install libdbus-1.so.3
  194  yum install libfontconfig.so.1
  195  yum install libfreetype.so.6
  196  yum install libgcc_s.so.1
  197  yum install libjpeg.so.62
  198  yum install libpng12.so.0
  210  sudo yum install epel-release
  211  sudo yum install nginx
  215  yum install gedit
  279  yum install tigervnc-server-module package
  286  yum install nano
  300  yum install -y nodejs
  418  yum install vsftpd ftp
  558  sudo yum install daemon
  560  sudo yum install screen
</pre>
