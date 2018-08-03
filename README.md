# AndroidStudioBenchmark
Project to benchmark android studio in 6 different tasks

## Please use this repo here:
https://github.com/boredomdenied/MovieApp


Name: Date: Test1: Test2: Test3: Test4: Test5: Test6: Version: OS: CPU: Memory: HardDrive: Emulator:

boredomdenied: 
  - 08/03/18
    13.6s | 11.9s | 3.9s | 785ms | 3288ms | 2804ms 
  - AS3.2beta5 
  - 18.04LTS 
  - ryzen 7 2700 stock 
  - 16GB DDR4 
  - EVO 970 250G    
  - KVM

boredomdenied: 
  - 07/17/18
    20.9s | 20.2s | 4.1s | 731ms | 3370ms | 2591ms 
  - AS3.2beta4 
  - 18.04LTS 
  - i7-3770 
  - 16GB DDR3 
  - EVO 970 250G    
  - KVM

dan:           
  - 07/17/18 
    14.5s | 23.7s | 4.2s | 5.2s  | 8.2s | 4.4s   
  - ?          
  - Win10    
  - ryzen 7 1700 base clock 3.7Ghz
  - ?        
  - Intel 600p 512G 
  - GenyMotion
 


## Steps to run tests
Test1:
Clone repo. 
Acquire api key from https://www.themoviedb.org/account/signup
Import project into android studio. After full load. Exit android studio (don't close project first)
Using a stopwatch, start Android studio which will load MovieApp project. Note time.

Test2:
Directly after test 1, cold boot a Nexus5x emulator. Tools > AVD Manager select/create Nexus5x API 24. Emulated Performance > Boot option > Cold boot
put a stopwatch to Run > Run app. Note time

Test3: 
Directly after test 2, add *private int test=1;* to file *https://github.com/boredomdenied/MovieApp/blob/master/app/src/main/java/com/boredomdenied/movieapp/MainActivity.java#L48*
put a stopwatch to Run > Apply changes. Note time

Test4:
First. Build > Make project
Build > Clean project and note time "Gradle finished in"

Test5:
Directly after test 4, Build > Rebuild project and note time "Gradle finished in"

Test6:
First. Build > Clean
Build > Make project and note time "Gradle finished in"

## Please submit PR with your own results
