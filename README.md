# devbox
Commands to get you up and running on OS X. Before starting anything else install XCode.

      /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
      
      brew analytics off # prevent brew from sending analytics home
      brew update && brew upgrade
      brew install wget ffmpeg youtube-dl python3 python@2 cmake docker vim zsh tmux htop watch numpy scipy

To extend the Python functionality, install the following packages. Use pip3 if using Python3 .

      pip install pandas matplotlib jupyter sklearn
      pip3 install pandas matplotlib jupyter sklearn

      # pip uninstall -y pillow # only if pillow is already installed
      CC="cc -mavx2" pip install -U --force-reinstall pillow-simd # high performance pillow library
      
      brew cask install transmission vlc sublime-text omnifocus 1password google-chrome dropbox
      
Change shell client for a more powerful one:

      sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"     

To remove cached files and free up some disk space do:

      brew cleanup
      
For periodic maintenance run:

      brew update && brew outdated && brew upgrade --all

For additional speedup when solving sparse linear systems in SciPy (with UMFPACK):

      brew install swig
      brew install suite-sparse
      pip install scikit-umfpack
      
Fix annoyances:

      defaults write com.apple.mail AddressesIncludeNameOnPasteboard -bool false

Following the release of OS X 10.9 Apple included AVX instruction set support in Accelerate framework - resulting in performance on par with Intel MKL. As of the time of writing, OpenBLAS does not support AVX and is slower. 
