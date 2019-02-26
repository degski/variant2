# benchmark1.cpp results


## Clang/LLVM 64 bit (clang-cl.exe 9.0-r351376, /std:c++17) (and the VS 2017 15.9.7 STL)

### /Ox -fuse-ld=lld -flto=thin

#### Run time

    N=50000000:
            double:   1011 ms; S=1.78571e+14
          variant2:   1827 ms; S=1.78571e+14
      std::variant:   2671 ms; S=1.78571e+14
    mpark::variant:   2658 ms; S=1.78571e+14

    N=50000000:
            double:   1027 ms; S=1.78571e+14
          variant2:   6885 ms; S=1.78571e+14
      std::variant:   6307 ms; S=1.78571e+14
    mpark::variant:   6549 ms; S=1.78571e+14



## VS 2017 15.9.7 64 bit (cl.exe 19.16, /std:c++17)

### /Ox /LTCG

#### Run time

    N=50000000:
            double:   1017 ms; S=1.78571e+14
          variant2:   2933 ms; S=1.78571e+14
      std::variant:   3143 ms; S=1.78571e+14
    mpark::variant:   3261 ms; S=1.78571e+14

    N=50000000:
            double:   1037 ms; S=1.78571e+14
          variant2:   6896 ms; S=1.78571e+14
      std::variant:   6836 ms; S=1.78571e+14
    mpark::variant:   7495 ms; S=1.78571e+14
