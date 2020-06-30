from time import sleep
import time
from threading import *

class Hello(Thread):
    def run(self):
        for number in range (1, 7):
            print (number ** 2)
            sleep(1)
            
class Hi(Thread):
    def run(self):
        for number1 in range (1, 7):
            print (number1 ** 3)
            sleep(1)

t1 = Hello()
t2 = Hi()
t1.start()
sleep(0.2)
t2.start()

start_time = time.time()
t1.join()
t2.join()

print("--- %s seconds ---" % (time.time() - start_time))


