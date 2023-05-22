# Lab Report 3 - Researching Commands

## Command Line Options with `grep`

## 1. `grep -i`

* **Example 1**

```
$ grep -i "evidence" technical/biomed/ar68.txt
```
```
       Evidence in support of T-cell involvement in rheumatoid
          evidence for cellular activation (either selective or
```
* **Example 2**

```
$ grep -i "MacRo" technical/biomed/ar79.txt
```
```
        In the joint, MMP-9 is expressed in macrophages in the
        macrophages and vascular structures have previously
```

`grep -i` option ignores the case of the specified pattern while searching for it in the file. It is useful in case we want to see the number of lines which contain the pattern irrespective of the case. 

---

## 2. `grep -w`

* **Example 1** 

```
$ grep -w "population" technical/biomed/ar140.txt
```
```
        represent an uncommitted precursor population, from which
        the effector population. We have previously demonstrated
        population.
        is restricted to the CD4 +, CD27 -population (Davis L,
        from the memory T-cell population before priming in the
        the initial memory cell population. Recent studies [ 32]
        synovial tissue T cells are a mixed population of recently
```

* **Example 2**

```
$ grep -w "mono" technical/biomed/rr74.txt
```
```
          for 45 min at 37°C (1:1500 anti-eNOS mono [BD
          Golden, CO, USA]; and 1:1500 anti-β-actin mono [Sigma
```

`grep -w` option searches for the exact word specified in the command line instead of treating it as a pattern, so it only prints the sentences which contain that whole word. It is useful because it is not always the case that we have to searcg for a pattern. This option with grep can be used to check the lines which contain exactly the same word we want.

---

## 3. `grep -v`

* **Example 1** 

```
$ grep -v "a" technical/government/Media/Farm_workers.txt
```

```



the workers sick.
heightened her concern.
whether the incident occurred.
nothing.'
rules.
inspections.
often require fieldwork from sunup to sundown during the growing
interpreter.
exposure.
EPA toxicologist in Denver.




```

* **Example 2**

```
$ grep -v "e" technical/government/Env_Prot_Agen/final.txt
```

```



will:


-


-


-
and


-


trading program.


obligations.
hazardous air pollutants (air toxics or HAPs) from fossil






FINE PARTICLE POLLUTION:
annually.
• VISIBILITY AND REGIONAL HAZE IMPACTS:

C OZONE:


C MERCURY:
ACID RAIN:
� NITROGEN DEPOSITION:
productivity.







V. Conclusion
11
this industry.
12




```

`grep -v` stands for the invert option which can be used to print the lines which don't contain the specified pattern. This option can be useful in a case where we would want to ensure that there is a specific pattern in every line. Hence, this option lets us check which lines won't have that pattern so that we can do the needful for our desired task.

---

## 4. `grep -c`

* **Example 1**

```
$ grep -c "we" technical/911report/preface.txt
29
```

* **Example 2** 

```
$ grep -c "in" technical/plos/pmed.0020088.txt
58
```

`grep -c` option returns the count of the lines which contain the specified pattern. This option can be useful in cases we just want to check how many lines contain that pattern. Hence, this provides a good alternative of `wc` command where we first need to redirect the output of `grep` into another file. Using this option, we can directly print out the count of lines.

---

## References

* en.wikibooks.org/wiki/Grep 
* ChatGPT prompt : command line options with grep command
* Its output:

The `grep` command is a powerful tool used to search for patterns in text files. Here are some common command line options that can be used with `grep`:

1. `-i` or `--ignore-case`: This option tells `grep` to ignore case when searching for patterns. For example, if you search for "apple" with `-i` option, it will also match "Apple" and "APPLE".

2. `-v` or `--invert-match`: This option tells `grep` to print lines that do not match the pattern. For example, if you search for "apple" with `-v` option, it will print all lines that do not contain the word "apple".

3. `-w` or `--word-regexp`: This option tells `grep` to search for whole words only. For example, if you search for "cat" with `-w` option, it will only match "cat" and not "catch".

4. `-r` or `--recursive`: This option tells `grep` to search for patterns in all files and directories recursively. For example, if you search for "apple" in a directory with subdirectories using `-r` option, it will search for the pattern in all files in that directory and its subdirectories.

5. `-n` or `--line-number`: This option tells `grep` to print the line number of the matched lines. For example, if you search for "apple" with `-n` option, it will print the line number along with the matched lines.

6. `-c` or `--count`: This option tells `grep` to print the number of times the pattern appears in the file. For example, if you search for "apple" with `-c` option, it will print the number of times the word "apple" appears in the file.

7. `-e` or `--regexp`: This option allows you to specify the pattern to be searched for. For example, if you want to search for "apple" or "orange" in a file, you can use `-e "apple|orange"`.

These are some of the commonly used options with `grep`. For more options, you can check the `grep` manual by typing `man grep` in the terminal.

