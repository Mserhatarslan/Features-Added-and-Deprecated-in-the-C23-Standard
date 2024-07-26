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
