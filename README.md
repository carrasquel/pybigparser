===========
pyBigParser
===========

pyBigParser provides classes for parsing long and complex math 
expresions. You might find it most useful for tasks involving 
evaluating from single functions to compounds functions.
Typical usage often looks like this::

    #!/usr/bin/env python
    
    from pybigparser import evaluator
    
    mybig = evaluator.bigFunction()
    mybig.setFunction("x**2+2*y")
    mybig.addSub("x", "24+6*c")
    mybig.addSub("y", "25 / d")
    mybig.addSub("c", "1")
    mybig.addSub("d", "4")
    
    mybig.evaluate()
