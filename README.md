# csBigInteger.py

## csBigInteger for Python

This project is part of the [csBigInteger](https://github.com/neoresearch/csBigInteger) macro project, a C# BigInteger implementation on Python 

This project uses csBigInteger.cpp portable C++ project: https://github.com/neoresearch/csBigInteger.cpp

## How to use it?

First, you need to have `csbiginteger.so` shared library (just type `make`).

After that, this `test.py` code should work (`make run`):

```py
def main():
    big = BigInteger()
    print 'length = ', big.length()
    print 'toInt = ', big.toInt()
    print 'toString: ', big.toString()

    bigM1 = BigInteger(-1)
    print 'length = ', bigM1.length()
    print 'toInt = ', bigM1.toInt()
    print 'toString: ', bigM1.toString()
    return 0
```

Empty BigInteger is expected to be byte array 0x00, with size = 1 (byte) and int value zero.

```
length =  1
toInt =  0
toString:  0x00
length =  1
toInt =  -1
toString:  0xff
```

## LICENSE

MIT License

2019