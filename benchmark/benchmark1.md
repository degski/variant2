# benchmark1.cpp results


## Clang/LLVM 64 bit (clang-cl.exe 9.0-r351376, /std:c++17) (and the VS 2017 15.9.7 STL)

### /Ox -fuse-ld=lld -flto=thin

#### Run time

    NN=50000000:
            double:   1020 ms; S=1.78571e+14
          variant2:   1791 ms; S=1.78571e+14
      std::variant:   2531 ms; S=1.78571e+14
    mpark::variant:   2525 ms; S=1.78571e+14

    N=50000000:
            double:   1025 ms; S=1.78571e+14
          variant2:   6873 ms; S=1.78571e+14
      std::variant:   6239 ms; S=1.78571e+14
    mpark::variant:   6244 ms; S=1.78571e+14



## VS 2017 15.9.7 64 bit (cl.exe 19.16, /std:c++17)

### /Ox /LTCG

#### Run time

    N=50000000:
            double:   1054 ms; S=1.78571e+14
          variant2:   2990 ms; S=1.78571e+14
      std::variant:   3147 ms; S=1.78571e+14
    mpark::variant:   3169 ms; S=1.78571e+14

    N=50000000:
            double:   1072 ms; S=1.78571e+14
          variant2:   6593 ms; S=1.78571e+14
      std::variant:   6841 ms; S=1.78571e+14
    mpark::variant:   6835 ms; S=1.78571e+14
