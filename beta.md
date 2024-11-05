# Otázky Beta / Beta Questions

## Jaký příkaz slouží ke změně branche? / Which git command switches between branches?

Git checkout. Např.: mám branche main list beta-branch.
input: git status
Output:On branch main
        Your branch is up to date with 'origin/main'.
input: git checkout beta-branch
output: Switched to branch 'beta-branch'
input git status
output: On branch beta-branch
        Your branch is up to date with 'origin/beta-branch'.

## Jaký jsou rozdíly mezi příkazy 'git init' a 'git clone' ? / What are differencies between command 'git init' and 'git clone'?

**git init** = vytvoří LOKÁLNÍ repozitář který není spojený s zádným remote repozitářem
            pokud chci lokální repozitář spojit společne s remote
            **input:** git remote add origin https://github.com/petrhornik/test.git
            **input:** git fetch
            **output:** remote: Enumerating objects: 24, done.
                    remote: Counting objects: 100% (24/24), done.
                    remote: Compressing objects: 100% (15/15), done.
                    remote: Total 24 (delta 6), reused 20 (delta 2), pack-reused 0 (from 0)
                    Unpacking objects: 100% (24/24), 1.92 KiB | 0 bytes/s, done.
                    From https://github.com/petrhornik/test
                    * [new branch]      master     -> origin/master
            **input:** git pull origin master
            **output:** From https://github.com/petrhornik/test
                     * branch            master     -> FETCH_HEAD
            v tuto chvíli už můžu s repozitářem pracovat
**git clone** = naklonuje repozitář z githubu a už můžu dálkově spravovat bez dalšího nastasvení.
            např.: v repozitáři najdu zelené tračítko CODE po kliknutí na něj zkopíruju HTTPS odkaz a následně napíšu git clone https://github.com/petrhornik/Git-test-G2.git a po stazění všech souborů už můžu ihned pracovat
