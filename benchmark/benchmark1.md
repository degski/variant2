# benchmark1.cpp results


## Clang/LLVM 64 bit (clang-cl.exe 9.0-r351376, /std:c++17) (and the VS 2017 15.9.7 STL)

### /Ox -fuse-ld=lld -flto=thin

#### Run time

    N=50000000:
            double:   1069 ms; S=1.78571e+14
          variant2:   1917 ms; S=1.78571e+14
    boost::variant:   2514 ms; S=1.78571e+14
      std::variant:   2986 ms; S=1.78571e+14
    mpark::variant:   3105 ms; S=1.78571e+14

    N=50000000:
            double:   1218 ms; S=1.78571e+14
          variant2:   8245 ms; S=1.78571e+14
    boost::variant:   7009 ms; S=1.78571e+14
      std::variant:   7473 ms; S=1.78571e+14
    mpark::variant:   7659 ms; S=1.78571e+14


## VS 2017 15.9.7 64 bit (cl.exe 19.16, /std:c++17)

### /Ox /LTCG

#### Run time

    N=50000000:
            double:   1097 ms; S=1.78571e+14
          variant2:   3110 ms; S=1.78571e+14
    boost::variant:   5233 ms; S=1.78571e+14
      std::variant:   3261 ms; S=1.78571e+14
    mpark::variant:   3454 ms; S=1.78571e+14

    N=50000000:
            double:   1214 ms; S=1.78571e+14
          variant2:   7938 ms; S=1.78571e+14
    boost::variant:   8574 ms; S=1.78571e+14
      std::variant:   7487 ms; S=1.78571e+14
    mpark::variant:   8284 ms; S=1.78571e+14
