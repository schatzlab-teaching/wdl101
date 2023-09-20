# wdl101 in the cloud

1. Join the wdl101 classroom: [https://classroom.github.com/a/TROwS5WY](https://classroom.github.com/a/TROwS5WY)

2. After joining, it will create a new github repo as https://github.com/schatzlab-teaching/wdl101-USERNAME. You can then launch the Codespace by clicking on the <> Code button, and then "Create codespace on main". This will boot a free virtual machine for you to use with 2 cores, 4 GB of RAM and 32 GB of local disk running ubuntu linux.

![launch](https://github.com/schatzlab-teaching/wdl101/raw/main/launch.png)

3. Once the codespace is launched, go into the terminal and install miniwdl with: 
```
$ pip3 install miniwdl
```

![pip3](https://github.com/schatzlab-teaching/wdl101/raw/main/pip3.png)

4. Once this is installed, verify it is running with 
```
$ miniwdl run_self_test
```

![selftest](https://github.com/schatzlab-teaching/wdl101/raw/main/selftest.png)

5. Once you confirm miniwdl is running, clone the [learn-wdl repo](https://github.com/openwdl/learn-wdl.git): 
```
$ git clone https://github.com/openwdl/learn-wdl.git
```

6. Try opening the WDL code in the Explorer such as learn-wdl/1_script_examples/1_hello_worlds/3_hello_input_task/input-task.wdl. It will ask you to install the WDL syntax highlighter. I recommend you do, as it will make it easier to read the code.

7. Try out the examples inside. For example:
```
$ cd learn-wdl/1_script_examples/1_hello_worlds/3_hello_input_task
$ miniwdl run input-task.wdl "WriteGreeting.name=Mike WDL Schatz"
...
$ cat _LAST/out/WriteGreeting.response/stdout.txt 
hello Mike WDL Schatz!
```

![helloworld](https://github.com/schatzlab-teaching/wdl101/raw/main/hello.png)

8. If you close the window, navigage to [https://github.com/schatzlab-teaching](https://github.com/schatzlab-teaching) and go to your private repo. From there you can relaunch your code environment. You can also navigate to [https://github.com/codespaces](https://github.com/codespaces) to see your active codespaces.

9. Make sure to review the codespaces documentation, especially how to sync code inside the virtual machine back to the repo: [https://docs.github.com/en/codespaces/getting-started/quickstart](https://docs.github.com/en/codespaces/getting-started/quickstart)
