# Histórias do SVN

Eu bem que tentei defender até o final, porém, não há mais o que fazer, é hora de chutar cachorro morto. Então, vamos para as histórias do SVN que me fizeram mudar de idéia.

Nota: O objetivo não é falar mal do SVN e sim fazer você refletir sobre se vale a pena sofrer para defender algo que teoricamente é ingrato com você.

```bash
svn: E155009: Failed to run the WC DB work queue associated with /folder/bla/bla/bla/folder/file.php
```
Cara, eu só queria fazer um update :(

```bash
svn: E200030: sqlite[S10]: disk I/O error
```
Esta até hoje não descobri o que é

```bash
svn: E155004: Run 'svn cleanup' to remove locks (type 'svn help cleanup' for details)
svn: E155004: Working copy '/folder/folder/folder/bla/bla/bla/folder' locked.
svn: E155004: '/folder/folder/folder/bla/bla/bla/folder' is already locked.
dev@devel01:$ svn cleanup /folder/folder/folder/bla/bla/bla/folder
svn: E155007: '/folder/folder/folder/bla/bla/bla/folder' is not a working copy
dev@devel01:$ svn status /folder/folder/folder/bla/bla/bla/folder
! L     /folder/folder/folder/bla/bla/bla/folder
```
Como assim? A pasta está bloqueada, o svn pede para limpar, tu vai limpar e não é working copy? svn se autotrolando?

```bash
svn: E200033: sqlite[S5]: database is locked
svn: E200042: Additional errors:
svn: E200033: sqlite[S5]: database is locked
```
svn guloso, quer o banco só pra ele

```bash
svn: E155009: Failed to run the WC DB work queue associated with '/folder/folder/folder/bla/bla/bla/', work item 1178 (file-commit bla/MyAwesomeClass.php)
svn: E000013: Não foi possível modificar as permissões do arquivo '/folder/folder/folder/bla/bla/bla/bla/MyAwesomeClass.php': Permissão negada
```
Okay, não tenho mais controle sobre meus próprios arquivos, o SVN é comunista, quer controlar tudo
