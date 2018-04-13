# Common_Libs
Common_libs for myself.

### Usage

```
from xxx import *
```

----------------------------------------------------------------------


#### Threads.py

* Multi thread pool, if you wanna to pass paras to function, please use args.

```
    tp = ThreadPool(thread_num)
    for line in open('url.txt').readlines():
        hunter = hunter_plugin(line)
        tp.add_job(hunter.exploit)
    tp.start()
    try:
        tp.wait_for_complete()
        results = tp.get_result()
        print results
    except KeyboardInterrupt:
        tp.stop()
```

----------------------------------------------------------------------


#### color.py

* print colorful commandline

```
    clr = Color()  
    clr.r('red')  
    clr.g('green')  
    clr.b('blue')  
    clr.rb('background')

```
