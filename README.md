## MAX6675 CircuitPython driver
Simple driver to use a MAX6675 thermocouple with CircuitPython.
Requires CircuitPython's `digitalio` module to be installed.

### Usage
    import board
    from max6675 import MAX6675
    sck = board.GP1
    cs = board.GP2
    so = board.GP3
    thermocouple = MAX6675(sck, cs, so)
    temp = thermocouple.read()
    print(temp)

