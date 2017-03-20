# GitAliases
Below are some useful git aliases for any repo.  To use, simply paste the aliases below into a .gitconfig file, after the `[alias]` line.  You must have whitespace (tabs or spaces) before each alias.  For best results, you should paste into the _global_ .gitconfig file (located at "C:\Users\<UserName>\.gitconfig" on Windows 7, 8, and 10 machines), and not just into repository .gitconfig files.


  a = add  
  aa = add -A  
  ah = add -h  
  ap = add --patch  
  aas = !"f() { git add -A; git status; }; f"  
  b = branch  
  ba = branch --all  
  bd = branch --delete  
  bh = branch -h  
  bl = branch --list  
  bu = branch --set-upstream-to  
  bv = branch --verbose  
  bvv = branch -vv  
  c = commit  
  ca = commit --all  
  ch = commit -h  
  cm = commit --message  
  cam = commit --all --message  
  csq = commit --no-edit --squash  
  casq = commit --all --no-edit --squash  
  ch = checkout  
  chb = checkout -b  
  chh = checkout -h  
  chm = checkout master  
  chps = !"f() { git checkout $1; git pull --rebase=true --autostash; }; f"  
  co = config  
  cog = config --global  
  cogr = !"f() { git config --global --get-regexp $1 | sed 's|'$1'.||'; }; f"  
  cogra = !"f() { git config --global --get-regexp alias | sed 's|alias.||'; }; f"  
  cogg = config --global --get  
  cogga = !"f() { git config --global --get alias.$1; }; f"  
  cogl = config --global --list  
  col = config --local  
  colr = !"f() { git config --local --get-regexp $1 | sed 's|'$1'.||'; }; f"  
  colra = !"f() { git config --local --get-regexp alias | sed 's|alias.||'; }; f"  
  colg = config --global --get  
  colga = !"f() { git config --local --get alias.$1; }; f"  
  coll = config --local --list  
  d = diff  
  f = fetch  
  fh = fetch -h  
  fp = fetch --prune  
  logn = log --oneline -n  
  m = merge  
  ma = merge --abort  
  mh = merge -h  
  mm = merge master  
  mnf = merge --no-ff  
  pd = push --delete  
  pf = push --force  
  pu = push --set-upstream  
  pp = pull --prune  
  pr = pull --rebase=true  
  ps = pull --rebase=true --autostash  
  pt = pull --tags  
  r = reset  
  rb = rebase  
  rba = rebase --abort  
  rbc = rebase --continue
  rbh = rebase -h  
  rbi = rebase --interactive  
  rbsq = rebase --interactive --autosquash  
  rs = reset --soft  
  rh = reset --hard  
  s = status  
  sa = stash apply  
  sb = stash branch  
  sc = stash clear  
  sd = stash drop  
  sp = stash pop  
  sl = stash list  
  ss = stash save  
  sski = stash save --keep-index  
  ssnki = stash save --no-keep-index  
  ssu = stash save --include-untracked
  ta = tag --annotate
	tam = !"f() { set -x; git tag --annotate $1 --message \"$2\"; }; f"
  td = tag --delete
  th = tag -h
  tl = tag --list
