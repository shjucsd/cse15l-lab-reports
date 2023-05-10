# Lab Report 3 - Researching Commands

## Command Line Options with `grep`

1. `grep -i`

*
```
$ grep -i "evidence" technical/biomed/ar68.txt
```
```
       Evidence in support of T-cell involvement in rheumatoid
          evidence for cellular activation (either selective or
```
*
```
$ grep -i "MacRo" technical/biomed/ar79.txt
```
```
        In the joint, MMP-9 is expressed in macrophages in the
        macrophages and vascular structures have previously
```

2. `grep -w`

*
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
*
```
$ grep -w "mono" technical/biomed/rr74.txt
```
```
          for 45 min at 37°C (1:1500 anti-eNOS mono [BD
          Golden, CO, USA]; and 1:1500 anti-β-actin mono [Sigma
```

3. `grep -v`

*
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
*
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

4. `grep -c`

*
```
$ grep -c "we" technical/911report/preface.txt
```
```
29
```
*
```
$ grep -c "in" technical/plos/pmed.0020088.txt
```
```
58
```
