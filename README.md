# GitAliases
Below are some useful git aliases for any repo.  To use, simply paste the aliases below into a .gitconfig file, after the `[alias]` line.  You must have whitespace (tabs or spaces) before each alias.  None of these aliases conflict, so you can use as many or as few of them as you like.  For best results, you should paste into the _global_ .gitconfig file (located at "C:\Users\<UserName>\.gitconfig" on Windows 7, 8, and 10 machines), and not just into repository .gitconfig files.  

Note that aliases are meant to be copied _from this README screen_.  Several characters have been escaped in the actual Markdown file so that they will display (and copy) correctly from here.  If you instead copy these aliases while editing the file, you will get the actual character _and_ the escape character, so use caution!


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
  coh = config -h  
  cogl = config --global --list  
  col = config --local  
  colr = !"f() { git config --local --get-regexp $1 | sed 's|'$1'.||'; }; f"  
  colra = !"f() { git config --local --get-regexp alias | sed 's|alias.||'; }; f"  
  colg = config --local --get  
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
  ps = push  
  psa = push --all  
  psd = push --delete  
  psh = push -h  
  psf = push --force  
  pst = push --tags  
  psu = push --set-upstream  
  pl = pull  
  pla = pull --all  
  plh = pull -h  
  plp = pull --prune  
  plr = pull --rebase=true  
  pls = pull --rebase=true --autostash  
  plt = pull --tags  
  rb = rebase  
  rba = rebase --abort  
  rbc = rebase --continue  
  rbh = rebase -h  
  rbi = rebase --interactive  
  rbsq = rebase --interactive --autosquash  
  rbsqs = rebase --interactive --autosquash --autostash  
  r = reset  
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
  tam = !"f() { git tag --annotate $1 --message \\"$2\\"; }; f"  
  td = tag --delete  
  th = tag -h  
  tl = tag --list  
