# devbox
Commands to get you up and running on OS X


Following the release of OS X 10.9 Apple included AVX instruction set support in Accelerate framework - resulting in performance on par with Intel MKL. As of the time of writing, OpenBLAS does not support AVX and is slower. 



      brew tap homebrew/science # a lot of cool formulae for scientific tools
      brew tap homebrew/python # numpy, scipy, matplotlib, ...
      brew update && brew upgrade
      
      
~brew cask

To extend the Python functionality, install the following packages. Use pip3 if using Python3 .

      pip install virtualenv  # encapsulated environments support
      pip install pandas      # data structures
      pip install sympy       # 
      pip install matplotlib  # plotting support
      
      

To remove cached files and free up some disk space do:

      brew cleanup
      brew cask cleanup
      

For additional speedup when solving sparse linear systems in SciPy (with UMFPACK):

      brew install suite-sparse
      pip install scikit-umfpack
      
