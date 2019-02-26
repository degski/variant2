# benchmark2.cpp results


## Clang/LLVM 64 bit (clang-cl.exe 9.0-r351376, /std:c++17) (and the VS 2017 15.9.7 STL)

### /Ox -fuse-ld=lld -flto=thin

#### Run time

    N=50000000:
            prefix:    577 ms; S=104166608333340
          variant2:   1381 ms; S=104166608333340
      std::variant:   1513 ms; S=104166608333340
    mpark::variant:   1519 ms; S=104166608333340



## VS 2017 15.9.7 64 bit (cl.exe 19.16, /std:c++17)

### /Ox /LTCG

#### Run time

    N=50000000:
            prefix:    540 ms; S=104166608333340
          variant2:   1406 ms; S=104166608333340
      std::variant:   1464 ms; S=104166608333340
    mpark::variant:   1552 ms; S=104166608333340
