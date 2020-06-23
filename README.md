### Install NextFlow

https://www.nextflow.io/

### Run the pipeline

```
./nextflow run pipe.nf --in1 "sample1" --in2 "sample2"
```

Sample output:
```
N E X T F L O W  ~  version 20.04.1
Launching `pipe.nf` [astonishing_gautier] - revision: 02ecaa4986
executor >  local (4)
[fe/ef41d3] process > make_file (sample1)      [100%] 2 of 2 ✔
[30/3a175e] process > print_file (sample1.txt) [100%] 2 of 2 ✔
[print_file] contents of sample2.txt: [print_sample] sample2

[print_file] contents of sample1.txt: [print_sample] sample1
```

### Change the input arguments

```
./nextflow run pipe.nf --in1 "antigen" --in2 "cell"
```

```
N E X T F L O W  ~  version 20.04.1
Launching `pipe.nf` [irreverent_hugle] - revision: 02ecaa4986
executor >  local (4)
[b1/b70e10] process > make_file (cell)         [100%] 2 of 2 ✔
[c7/b6b86f] process > print_file (antigen.txt) [100%] 2 of 2 ✔
[print_file] contents of cell.txt: [print_sample] cell

[print_file] contents of antigen.txt: [print_sample] antigen
```