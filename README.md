# devbox
Commands to get you up and running on OS X


Following the release of OS X 10.9 Apple included AVX instruction set support in Accelerate framework - resulting in performance on par with Intel MKL. As of the time of writing, OpenBLAS does not support AVX and is slower. 



      brew tap homebrew/science # a lot of cool formulae for scientific tools
      brew tap homebrew/python # numpy, scipy, matplotlib, ...
      brew update && brew upgrade
      
      
~brew cask


To remove cached files and free up some disk space do:
      brew cleanup
      brew cask cleanup
      
