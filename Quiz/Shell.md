## Unix Shell Quiz

#### Q1. How can you print out "foo" from the variable b?

```bash
a=foo
b=a
```

- [ ] eval echo $$b
- [ ] eval echo ${$b}
- [x] eval echo \$$b
- [x] eval echo '$'$b
- [ ] This is not possible

Explanation:
  - $$ gives the PID, so "echo $$b" or "eval echo $$b" returns for example: 6139b
  - ${$var} is incorrect, so "echo ${$b}" or "eval echo ${$b}" will raise: "bash: ${$b}: bad substitution"
  + But "eval echo \$$b" means "eval echo $a" which returns "foo"
  ! Warning: This may look particular comparing to the above, but "echo $b" returns "a", and "echo \$$b" returns "$a"

Further reading: https://linuxhint.com/bash_eval_command
