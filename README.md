# Qlang

[![Gem Version](https://badge.fury.io/rb/qlang.svg)](http://badge.fury.io/rb/qlang) [![Build Status](https://travis-ci.org/gogotanaka/Q.svg?branch=master)](https://travis-ci.org/gogotanaka/Q) [![Coverage Status](https://coveralls.io/repos/gogotanaka/Q/badge.png?branch=master)](https://coveralls.io/r/gogotanaka/Q?branch=master) [![Code Climate](https://codeclimate.com/github/gogotanaka/Q/badges/gpa.svg)](https://codeclimate.com/github/gogotanaka/Q) [![Dependency Status](https://gemnasium.com/gogotanaka/Q.svg)](https://gemnasium.com/gogotanaka/Q)

Enjoy MATH with Keyboard.

### Differentiate

```
d/dx(cos(x))
=> ( - sin( x ) )

d/dx(log(x))
=> ( 1 / x )

# You can omit parentheses

d/dy y^2                        
=> ( 2 * y )

d/dy xy                       
=> ( x )
```


### Integrate

```
S(log(x)dx)[0..1]
=> - oo

S(sin(x)dx)[0..pi]
=> 2.0

S(cos(x)dx)[0..pi]                       
=> 0.0
```


### Matrix

```
(1 2 3; 4 5 6)
=> (1 2 3; 4 5 6)

(1 2 3; 4 5 6) + (1 2 3; 4 5 6)
=> (2 4 6; 8 10 12)

(1 2 3; 4 5 6) * (1 2 3)
=> (14 32)
```

### Function
```
f(x, y) = xy
f(1, 2)
=> 2
```


## How to use

Install it yourself as:

    $ gem install qlang

### Compiler into R

    $ qlang -c -R foo.q
    
### Compiler into Ruby

    $ qlang -c -Ruby foo.q

### Interpreter

    $ qlang -i


## Contributing

1. Fork it ( https://github.com/[my-github-username]/qlang/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
