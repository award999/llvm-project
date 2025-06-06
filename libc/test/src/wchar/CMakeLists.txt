add_custom_target(libc_wchar_unittests)

add_libc_test(
  wcslen_test
  SUITE
    libc_wchar_unittests
  SRCS
    wcslen_test.cpp
  DEPENDS
    libc.hdr.types.size_t
    libc.hdr.types.wchar_t
    libc.src.wchar.wcslen
)

add_libc_test(
  btowc_test
  SUITE
    libc_wchar_unittests
  SRCS
    btowc_test.cpp
  DEPENDS
    libc.include.stdio
    libc.src.wchar.btowc
)

add_libc_test(
  wctob_test
  SUITE
    libc_wchar_unittests
  SRCS
    wctob_test.cpp
  DEPENDS
    libc.src.wchar.wctob
)

add_libc_test(
  wmemset_test 
  SUITE
    libc_wchar_unittests
  SRCS
    wmemset_test.cpp
  DEPENDS
    libc.hdr.types.size_t
    libc.hdr.types.wchar_t
    libc.src.wchar.wmemset
)

add_libc_test(
  wcschr_test
  SUITE
    libc_wchar_unittests
  SRCS
    wcschr_test.cpp
  DEPENDS
    libc.src.wchar.wcschr
)

add_libc_test(
  wcspbrk_test
  SUITE
    libc_wchar_unittests
  SRCS
    wcspbrk_test.cpp
  DEPENDS
    libc.src.wchar.wcspbrk
)

add_libc_test(
  wcsspn_test
  SUITE
    libc_wchar_unittests
  SRCS
    wcsspn_test.cpp
  DEPENDS
    libc.src.wchar.wcsspn
)

add_libc_test(
  wmemcmp_test
  SUITE
    libc_wchar_unittests
  SRCS
    wmemcmp_test.cpp
  DEPENDS
    libc.src.wchar.wmemcmp
)

add_libc_test(
  wmemcpy_test
  SUITE
    libc_wchar_unittests
  SRCS
    wmemcpy_test.cpp
  DEPENDS
    libc.src.wchar.wmemcpy
)

add_libc_test(
  wcscpy_test
  SUITE
    libc_wchar_unittests
  SRCS
    wcscpy_test.cpp
  DEPENDS
    libc.src.wchar.wcscpy
)
