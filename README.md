# devbox
Commands to get you up and running on OS X. Before starting anything else install XCode.

Step 0: install brew



      brew analytics off # prevent brew from sending analytics home
      brew tap homebrew/science # a lot of cool formulae for scientific tools
      brew tap homebrew/python # numpy, scipy, matplotlib, ...
      brew update && brew upgrade
      
      brew install wget
      brew install ffmpeg
      brew install node
      brew install youtube-dl

      
      brew install python
      brew install python3

      brew install numpy --with-python3
      brew install scipy --with-python3

~brew cask

To extend the Python functionality, install the following packages. Use pip3 if using Python3 .

      pip install virtualenv  # encapsulated environments support
      pip install pandas      # data structures
      pip install sympy       # 
      pip install matplotlib  # plotting support
      
      
      
      brew cask install transmission # cask installation will happen automatically on first call
      brew cask install vlc          
      brew cask install atom
      brew cask install torbrowser
      (also available: mactex, dropbox, spotify, google-chrome)
      

To remove cached files and free up some disk space do:

      brew cleanup
      brew cask cleanup
      
For period maintenance run:

      brew update && brew outdated && brew upgrade --all


For additional speedup when solving sparse linear systems in SciPy (with UMFPACK):

      brew install suite-sparse
      pip install scikit-umfpack
      
Following the release of OS X 10.9 Apple included AVX instruction set support in Accelerate framework - resulting in performance on par with Intel MKL. As of the time of writing, OpenBLAS does not support AVX and is slower. 


      
