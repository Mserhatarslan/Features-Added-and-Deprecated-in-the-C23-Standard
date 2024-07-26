# Features-Added-and-Deprecated-in-the-C23-Standard

C23: a slightly better C

## Removed

* Old-style function declarations and definitions

* Representations for signed integers other than two's complement

* Permission that u/U-prefixed character constants and string literals may be not UTF-16/32

* Mixed wide string literal concatenation

* Support for calling realloc() with zero size (the behavior becomes undefined)

* __alignof_is_defined and __alignas_is_defined

* static_assert is not provided as a macro defined in <assert.h> (becomes a keyword)

* thread_local is not provided as a macro defined in <threads.h> (becomes a keyword)

 nullptr ---> The ambiguous NULL macro is often better replaced by nullptr when C23 is available.

## Deprecated 

* <stdnoreturn.h>
  
* Old feature-test macros
  
* __STDC_IEC_559__
  
* __STDC_IEC_559_COMPLEX__
  
* _Noreturn function specifier
  
* _Noreturn attribute token
  
* asctime()
  
* ctime()
  
* DECIMAL_DIG (use the appropriate type-specific macro (FLT_DECIMAL_DIG, etc) instead)
  
* Definition of following numeric limit macros in <math.h> (they should be used via <float.h>)
  
* INFINITY
  
* DEC_INFINITY
  
* NAN
  
* DEC_NAN
  
* __bool_true_false_are_defined


## New language features
* Attributes
  
  [[deprecated]]
  
  [[fallthrough]]
  
  [[maybe_unused]]
  
  [[nodiscard]]
  
  [[noreturn]]
  
  [[reproducible]]
  
  [[unsequenced]]
  
* static_assert becomes a keyword (may be a predefined macro for compatibility reasons)

* thread_local becomes a keyword (may be a predefined macro for compatibility reasons)

* nullptr constant and the associated nullptr_t type
  
* New preprocessor directives
  
  #elifdef
  
  #elifndef
  
  #warning
  
  #embed

* Single-argument _Static_assert (Improved static assertion capabilities.)

* Support for ranges in for loops.

* Enhanced support for flexible array members.

* strdup was not part of the C standard library; it was a POSIX function.

With the C23 standard, some changes were made, and the strdup function was included in the C standard library. This means that the strdup function can now be used with compilers that support the C23 standard and is no longer exclusive to POSIX.

Therefore, if you are using a compiler that supports the C23 standard, you can use the strdup function without any portability concerns.
Using strdup you can get a modifiable copy of the string word or any string. In this way, you can change its contents without encountering the problems of replacing the hard memory.



## New Headers

* <stdbit.h>
  
* <stdckdint.h>


