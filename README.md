# munkres

an implementation of the Hungarian algorithm

This code is heavily based on Bob Pilgrim's work [outlined here](http://csclab.murraystate.edu/bob.pilgrim/445/munkres.html).

## Example
    m := NewMatrix(4)
    m.A = []int64{94, 93, 20, 37,
            75, 18, 71, 43,
            20, 29, 32, 25,
            37, 72, 17, 73}
    fmt.Println(ComputeMunkresMin(m)) // [{0 3} {1 1} {2 0} {3 2}]

The assignment set which minimizes the total utility is:

    (0, 3) = 37
    (1, 1) = 18
    (2, 0) = 20
    (3, 2) = 17
           = 92

## License
see [LICENSE](https://github.com/clyphub/munkres/blob/master/LICENSE) file

## Author(s)
Brian Fallik - bfallik at clypd.com

## Dependencies
This packages uses [stretchr/testify](http://godoc.org/github.com/stretchr/testify) for help with unit test assertions.

## Development
Pull requests welcome!

## Other
Thanks to [clypd](http://www.clypd.com) for agreeing to release this code into the wild.

![clypd](http://www.clypd.com/wp-content/uploads/2013/08/logo_clypd_70@2x.png "clypd")
