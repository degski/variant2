# benchmark2.cpp results


## Clang/LLVM 64 bit (clang-cl.exe 9.0-r351376, /std:c++17) (and the VS 2017 15.9.7 STL)

### /Ox -fuse-ld=lld -flto=thin

#### Run time

    N=50000000:
            prefix:    659 ms; S=104166608333340
          variant2:   1523 ms; S=104166608333340
    boost::variant:   1737 ms; S=104166608333340
      std::variant:   1546 ms; S=104166608333340
    mpark::variant:   1555 ms; S=104166608333340


## VS 2017 15.9.7 64 bit (cl.exe 19.16, /std:c++17)

### /Ox /LTCG

#### Run time

    N=50000000
            prefix:    595 ms; S=104166608333340
          variant2:   1515 ms; S=104166608333340
    boost::variant:   2272 ms; S=104166608333340
      std::variant:   1612 ms; S=104166608333340
    mpark::variant:   1670 ms; S=104166608333340
