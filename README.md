# PyTimer
Python looping timer. Forked from [terryltang/pythonTimer](https://github.com/terryltang/pythonTimer)

- Require Python standard library: __threading__ 

- Call a function after a specified number of seconds:

```
    e.g.:
    timer = PyTimer(5.0, handler_func, args=[], kwargs={})
    timer.set_call_limits(5)    # timer will run eternally if you don't set a limit
    timer.start()
    timer.cancel()     # cancel the timer's action if it's still waiting, will also destroy timer instance
```

- Timer handler take positional arguments and keyword arguments: 

```
    e.g.: 
    timer = PyTimer(0.5, timer_handler, args=["Terry", "Tang"], kwargs={"city":"Houston", "state":"Texas"})
```

- Cancel and destroy timer. 

- Add a customized logger function for timer handler.

- Test cases included. 
