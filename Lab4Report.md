***3 Differet Ways to Use the Grep Command in Bash***
---
1. Use the grep command to search and display the total number of times a string appears in a file with `-c`

```
$ grep -c 'apple' ch1.txt
0
```
```
$ grep -c 'the' ch1.txt
153
```
When `-c` is used with the grep command, the system looks through the specified file searching for how many times a string may appear in that file. 
It then lists an integer indicating how many times that specified word is within that file. This part of the grep command is useful for quickly searching through specific files
in hopes of finding a specific string or word that may be in it, saving you a lot of time from just manually reading through the file and finding the specific string that 
you are looking for. 

***Source:*** [cyberciti.biz](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)

2. Use the grep command to look words within a file without it being case sensitive with `-i`

```
$ grep -i CiviliZATION written_2/non-fiction/OUP/Berk/ch1.txt
Whether on the scene, or behind the scenes, parents have jointly created the institutions that train and inspire children: apprenticeships, schools, 
works of art and literature, religious classes, playing ﬁelds, and even forms of resistance and rebellion. These institutions, and the adults who run them, 
sustain civilization and provide the disciplines—however fragile they may seem—that keep our societies from reverting to barbarism.77
```
```
$ grep -i AIRpoDS written_2/non-fiction/OUP/Berk/ch1.txt

```

When `-i` is used with the grep command, the system looks through the specified file path for a word no matter how case sensitive it is. This part of the grep command is useful
for finding words within the inidicated file path no matter how case sensitive it is. This means that you will be able to find the word as long as the word is spelled exactly
the same. This can help you save a lot of time from manually going through each file and .txt file looking for a word. It even gived you the specific lines in where the word 
has been found. 

***Source:*** [cyberciti.biz](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)

3. Use the grep command to look for the specific lines in which the words is located on with `-n`

```
$ grep -n teaching written_2/non-fiction/OUP/Berk/ch1.txt
5:In my three decades of teaching university courses in child development, I have come to know thousands of students, 
many of whom were parents or who became parents soon after completing my class. I also served on boards of directors and advisory committees for 
child-care centers, preschools, elementary schools, and parent organizations. And my research continually drew me into classrooms, where for countless 
hours I observed and recorded preschool and school-age children’s activities, social interactions, and solitary behaviors, in hopes of answering central 
questions about how they learn.
60:Piaget’s contribution to the ﬁeld of child development is enormous. He inspired more research on children’s thinking than any other single theorist. 
Especially important, Piaget convinced the academic community—as well as many parents and teachers—that children are active contributors to their own development,
have their own ways of understanding the world, and must be developmentally ready if teaching is to be successful.
61:In the ﬁeld of early childhood education, Piaget’s theory sparked preschool classrooms emphasizing discovery learning through children’s spontaneous 
interaction with the environment. Rather than teaching didactically, teachers in Piagetian-based settings provide a rich variety of hands-on activities and 
encourage children’s exploration and experimentation. Educators inspired by Piaget’s work hope that by repeatedly applying cognitive structures in stimulating
environments, children will notice and amend deﬁciencies in their thinking.
64:As our discussion already suggests, a central Piagetian tenet is that it is foolhardy to try to speed up development. If children are masters of their own learning, then adult eorts to teach them new skills before they indicate they are interested or ready are doomed to failure. Because Piaget stressed the supremacy of children’s engagement with their surroundings over adult teaching, parents’ and teachers’ contributions to development are severely reduced relative to the child’s. In sum, compared to the behaviorist, adult-supremacy perspective, the Piagetian view stands at the opposite pole.
67:Finally, many studies show that children’s performance on tasks such as conservation can be improved with training.37 This, along with the cross-cultural 
ﬁndings just described, raises doubts about Piaget’s assumption that discovery learning rather than adult teaching is the most eective way to foster development.
154:In all the ways just mentioned, parents and other adults are vital conveyers of culture, through direct teaching of attitudes and values and through the 
pervasive imprint of culture on the settings and activities they provide for children. In the hands of parents and teachers lies the awesome responsibility of 
conveying to the next generation the intellectual, scientiﬁc, aesthetic, and moral achievements that dierentiate our species from others. From the simplest 
preliterate society to the most technologically advanced nation, adults are charged with ensuring that children acquire competencies that enable them to assume a 
responsible place in their society and, ultimately, participate in transmitting its values and practices to future generations.
216:The importance of activity contexts reminds us that all children do not face identical tasks. Cultures, and adults within them responsible for socialization,
select dierent tasks for children’s learning. As a result, children’s cognition is contextualized; it emerges and derives meaning from particular activities and social experiences. Parents who spend little time in joint pursuits and conversation with their children convey to them a very dierent set of cultural values, practices, and cognitive strategies than do parents who involve their children in constructive play and projects; encourage them to participate in family routines and duties, such as meal preparation and cleaning; and plan parent–child outings. Similarly, teachers who require mostly solitary desk work from children, isolating the skills taught from their everyday use, promote values and competencies strikingly dierent from those cultivated by teachers who embed teaching and learning in meaningful collaborative activities.
```
```
$ grep -n shrimp written_2/non-fiction/OUP/Berk/ch1.txt

```

When `-n` is used with the grep command, the system looks through the file path for a specified string and it prints the line that is is on followed with
the line number of where it is. This is useful for us as it can help us locate a specific file and file line in where our code could have the specific method which leads to an error.
With this feature, we can immediantly locate the line that is causing the error and fix it almost immediantly, instead of wasting time searching for the error manually.

***Source:*** [cyberciti.biz](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)
