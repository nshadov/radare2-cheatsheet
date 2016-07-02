# Radare2 Basics: Unofficial Guide

## Disallembly (static analysis)

### Getting on right track

Opening binary in radare2:
```
r2 crkme1sys
```

Finding appropriate function to look at (**main**, **sym.main**, **entry0**):
```
s main
```

Displaying what's inside (20 instructions at a time):
```
pd 20
[enter]
[enter]
...
```

> If you're intrested in opcodes (bytes), rather than in instructions: ```pD 20```

### Seeing rather than reading (visual mode)

### Naming things

Saving current work (project) is done ```Ps <project_name>``` and could be loaded again by ```Po <project_name>```.

Flag ```-p``` could be added during runtime, to load project.

Rename function local variable (base pointer argument). We need to first analyze binary ```aa```, and then:

```
afvbn local_8h buffer
```

> I'm pretty sure this command was called called ```afvn``` before. nvm.

## Debugging (dynamic analysis)

### Getting on right track


## Other tips & tricks

### I hate how it looks
