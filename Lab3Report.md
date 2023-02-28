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
When `-name` is used with the find command, the system looks through the different directories and files to find the specific names of files or directories and it lists the absolute path needed to reach that directory or file. This part of the find command is useful for quickly finding the specific name of the file or directory you need without having to go through all of the files, saving you lots of time.

***Source:*** [digitalocean.com](https://www.digitalocean.com/community/tutorials/how-to-use-find-and-locate-to-search-for-files-on-linux)

2. Use the find command to search for empty files within directories with `-empty`

```
$ find written_2 -empty
written_2/find-results.txt
```
```
$ find non-fiction/ -empty

```
When `-empty` is used with the find command, the system looks through the indicated directory in order to find empty files within them. This is useful for quickly finding files that are created that are still empty when they should have data in them. The first example above shows that there is one file that is empty within the written_2/ directory. The second example above shows us that within the non-fiction/ directory, there is no files that are currently empty within the directory.

***Source:*** [geeksforgeeks.org](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

3. Use the find command to search for any file despite its capitalization with `-iname`

```
$ find written_2/ -iname algarve-history.txt
written_2/travel_guides/berlitz2/Algarve-History.txt
```
```
$ find berlitz1/ -iname whattohawaii.txt
berlitz1/WhatToHawaii.txt
```
When `-iname` is used with the find command, the system looks through any directories listed within the commandline for any files with the given name disreguarding its capitalization. This is useful for finding specific files despite their name being uppercased or lowercased in case the file was created with created mistakenly with both uppercase and lowercase letters, or in case it was forgotten if the file name contained an uppercase letter.

***Source:*** [tecmint.com/](https://www.tecmint.com/35-practical-examples-of-linux-find-command/)

4. Use the find command to search for any readable file with `-perm /u=r`
```
$ find Abernathy/ -perm /u=r
Abernathy/
Abernathy/ch1.txt
Abernathy/ch14.txt
Abernathy/ch15.txt
Abernathy/ch2.txt
Abernathy/ch3.txt
Abernathy/ch6.txt
Abernathy/ch7.txt
Abernathy/ch8.txt
Abernathy/ch9.txt
```
```
$ find Berk/ -perm /u=r
Berk/
Berk/ch1.txt
Berk/ch2.txt
Berk/CH4.txt
Berk/ch7.txt
```
When `-perm /u=r` is used with the find command, we are given a list of readable files such as .txt files that are located within a specific directory. This is useful for us because it gives us the ability to separate any readable files from other files with similar names. Examples of this include separating readable files such as .txt files from any exectable file that may have the same name as the readable file. 

***Source:*** [tecmint.com/](https://www.tecmint.com/35-practical-examples-of-linux-find-command/)
