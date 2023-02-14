***4 Differet Ways to Use the Find Command in Bash***
---
1. Use the find command to search for files by name with `-name`

```
$ find -name "Castro"
./written_2/non-fiction/OUP/Castro
```
```
$ find -name "non-fiction"
./written_2/non-fiction
```
This feature of the find command is looking through the different directories and files to find the specific names of files or directories and it lists the absolute path needed to reach that directory or file. This part of the find command is useful for quickly finding the specific name of the file or directory you need without having to go through all of the files, saving you lots of time.

***Source:*** [digitalocean.com](https://www.digitalocean.com/community/tutorials/how-to-use-find-and-locate-to-search-for-files-on-linux)

2. Use the find command to search for all files ending in a specific keyword

```
$ find berlitz2/ -type f -name "*.txt"
berlitz2/Algarve-History.txt
berlitz2/Algarve-Intro.txt
berlitz2/Algarve-WhatToDo.txt
berlitz2/Algarve-WhereToGo.txt
berlitz2/Amsterdam-History.txt
berlitz2/Amsterdam-Intro.txt
berlitz2/Amsterdam-WhatToDo.txt
berlitz2/Amsterdam-WhereToGo.txt
berlitz2/Athens-History.txt
berlitz2/Athens-Intro.txt
berlitz2/Athens-WhatToDo.txt
berlitz2/Athens-WhereToGo.txt
berlitz2/Bahamas-History.txt
berlitz2/Bahamas-Intro.txt
berlitz2/Bahamas-WhatToDo.txt
berlitz2/Bahamas-WhereToGo.txt
berlitz2/Bali-History.txt
berlitz2/Bali-WhatToDo.txt
berlitz2/Bali-WhereToGo.txt
berlitz2/Barcelona-History.txt
berlitz2/Barcelona-WhatToDo.txt
berlitz2/Barcelona-WhereToGo.txt
berlitz2/Beijing-History.txt
berlitz2/Beijing-WhatToDo.txt
berlitz2/Beijing-WhereToGo.txt
berlitz2/Berlin-History.txt
berlitz2/Berlin-WhatToDo.txt
berlitz2/Berlin-WhereToGo.txt
berlitz2/Bermuda-history.txt
berlitz2/Bermuda-WhatToDo.txt
berlitz2/Bermuda-WhereToGo.txt
berlitz2/Boston-WhereToGo.txt
berlitz2/Budapest-History.txt
berlitz2/Budapest-WhatToDo.txt
berlitz2/Budapest-WhereoGo.txt
berlitz2/California-History.txt
berlitz2/California-WhatToDo.txt
berlitz2/California-WhereToGo.txt
berlitz2/Canada-History.txt
berlitz2/Canada-WhereToGo.txt
berlitz2/CanaryIslands-History.txt        
berlitz2/CanaryIslands-WhatToDo.txt       
berlitz2/CanaryIslands-WhereToGo.txt      
berlitz2/Cancun-History.txt
berlitz2/Cancun-WhatToDo.txt
berlitz2/Cancun-WhereToGo.txt
berlitz2/China-History.txt
berlitz2/China-WhatToDo.txt
berlitz2/China-WhereToGo.txt
berlitz2/Costa-History.txt
berlitz2/Costa-WhatToDo.txt
berlitz2/Costa-WhereToGo.txt
berlitz2/CostaBlanca-History.txt
berlitz2/CostaBlanca-WhatToDo.txt
berlitz2/Crete-History.txt
berlitz2/Crete-WhatToDo.txt
berlitz2/Crete-WhereToGo.txt
berlitz2/CstaBlanca-WhereToGo.txt
berlitz2/Cuba-History.txt
berlitz2/Cuba-WhatToDo.txt
berlitz2/Cuba-WhereToGo.txt
berlitz2/Nepal-History.txt
berlitz2/Nepal-WhatToDo.txt
berlitz2/Nepal-WhereToGo.txt
berlitz2/NewOrleans-History.txt
berlitz2/Paris-WhatToDo.txt
berlitz2/Paris-WhereToGo.txt
berlitz2/Poland-History.txt
berlitz2/Poland-WhatToDo.txt
berlitz2/Portugal-History.txt
berlitz2/Portugal-WhatToDo.txt
berlitz2/Portugal-WhereToGo.txt
berlitz2/PuertoRico-History.txt
berlitz2/PuertoRico-WhatToDo.txt
berlitz2/PuertoRico-WhereToGo.txt
berlitz2/Vallarta-History.txt
berlitz2/Vallarta-WhatToDo.txt
berlitz2/Vallarta-WhereToGo.txt
```

```
