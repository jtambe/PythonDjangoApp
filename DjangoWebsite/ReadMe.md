1.
To setup conda in vs code, use *ctrl+shift+p* and add following settings.json file with `Open Workspace Settings (JSON)` 

```
{
    "python.terminal.activateEnvironment": true,
    //"terminal.integrated.shell.windows": "C:\\Windows\\System32\\cmd.exe",
    "python.condaPath": "C:\\Users\\your_user_name\\Anaconda3\\Scripts\\conda.exe"
}
```

Open a new terminal and it will open up a command prompt with either `base` env or whichever env is currently activated in conda. <br/>
This process is shown in this video: https://www.youtube.com/watch?v=J8jLHgw-bFQ
<br/>

2.
To solve Open SSL  error for installing using `conda install -c anaconda django` , you will need to copy following 2 files from *C:\Users\your_user_name\anaconda3\Library\bin* to *C:\Users\your_user_name\anaconda3\DLLs* <br/>
file1: libcrypto-1_1-x64.dll <br/>
file2: libssl-1_1-x64.dll <br/>
This process is shown in this video: https://www.youtube.com/watch?v=hfKAV6OYaKw

3.

run following command in your terminal <br/>
*python .\DjangoWebsite\manage.py runserver*

