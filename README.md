# JPMC Task 1
Starter repo for task 1 of the JPMC software engineering program


## How to make a patch file

### Scenario 1: One commit

Run the command below:

```git format-patch -1 HEAD```

### Scenario 2: Multiple commits

Run the command below:

```git format-patch -n –stdout > multi_commit.patch```

- note: the n in -n must be replaced with a number which represents the number of commits you made for the
task.

So the real command if you made 4 commits on top of the old commits should be

```git format-patch -4 --stdout > multi_commit.patch```
    
After executing the command, a .patch file will be produced in the directory where you executed the command