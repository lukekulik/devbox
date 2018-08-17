# devbox
Commands to get you up and running on OS X. Before starting anything else install XCode.

      /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
      
      brew analytics off # prevent brew from sending analytics home
      brew update && brew upgrade
      
      brew install wget
      brew install ffmpeg
      brew install node
      brew install youtube-dl
      
      brew install python3
      brew install python@2
      brew install cmake
      brew install docker
      brew install zsh
      brew install tmux
      brew install htop
      brew install watch

      brew install numpy --with-python3
      brew install scipy --with-python3

To extend the Python functionality, install the following packages. Use pip3 if using Python3 .

      pip install pandas      # data structures
      pip install matplotlib  # plotting support
      pip install jupyter
      pip install sklearn
      # pip uninstall -y pillow # only if pillow is already installed
      CC="cc -mavx2" pip install -U --force-reinstall pillow-simd # high performance pillow library
      
      pip3 install matplotlib
      
      brew cask install transmission # cask installation will happen automatically on first call
      brew cask install vlc          
      brew cask install atom
      brew cask install omnifocus
      brew cask install google-chrome
      (also available: mactex, dropbox, spotify, google-chrome)
      
Change shell client for a more powerful one:

      sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"     

To remove cached files and free up some disk space do:

      brew cleanup
      brew cask cleanup
      
For period maintenance run:

      brew update && brew outdated && brew upgrade --all

For additional speedup when solving sparse linear systems in SciPy (with UMFPACK):

      brew install suite-sparse
      pip install scikit-umfpack
      
Following the release of OS X 10.9 Apple included AVX instruction set support in Accelerate framework - resulting in performance on par with Intel MKL. As of the time of writing, OpenBLAS does not support AVX and is slower. 
