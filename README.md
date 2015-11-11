# Listing_4_16_Project_1412 

##Intro

Working on Listing 4.16 to generate a random character using Math.random().

##Code

``` java 
public class RandomCharacter {
    public static void main(String[] args) {
        // Call a method to generate a random number in the range of a character.
        int randomUpperCaseLetterNumber = makeRandomUpperLetter();

        // Note that (char) in front of our variable recasts it as 
        System.out.println("The random upper case letter of the day is: " + (char)randomUpperCaseLetterNumber);
    }
    public static int makeRandomUpperLetter(){
        // Range of Character values, page 125, table 4.4
        //Characters ('A' to 'Z'), Code Value in Decimal (65 to 90)

        // How to use a random number Page 122, bottom of the page, 4.2.5 The random Method
        // Also use the example on page 87.

        int lowerLimit = 65;
        int upperLimit = 90;
        int Range = upperLimit-lowerLimit + 1;
        int randomUpperCaseLetterNumber = lowerLimit + (int)(Math.random()*Range);
        System.out.println(randomUpperCaseLetterNumber);
        return randomUpperCaseLetterNumber;
        
        
        
        
        
    }
} 

```


##Console Output

```
71
The random upper case letter of the day is: G

77
The random upper case letter of the day is: M

90
The random upper case letter of the day is: Z

69
The random upper case letter of the day is: E

```


##Command Prompt



```
C:\Users\denise\Desktop\workspace\RandomCharacter1>git push -u origin master
Username for 'https://github.com': 54r4hv
Password for 'https://54r4hv@github.com':
Counting objects: 3, done.
Writing objects: 100% (3/3), 252 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/54r4hv/Listing_4_16_Project_1412.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.

C:\Users\denise\Desktop\workspace\RandomCharacter1>git add .

C:\Users\denise\Desktop\workspace\RandomCharacter1>git commit -m "added stuff"
[master 45738f9] added stuff
 4 files changed, 48 insertions(+)
 create mode 100644 .classpath
 create mode 100644 .project
 create mode 100644 bin/RandomCharacter.class
 create mode 100644 src/RandomCharacter.java

C:\Users\denise\Desktop\workspace\RandomCharacter1>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': 54r4hv
Password for 'https://54r4hv@github.com':
Counting objects: 8, done.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (8/8), 1.90 KiB | 0 bytes/s, done.
Total 8 (delta 0), reused 0 (delta 0)
To https://github.com/54r4hv/Listing_4_16_Project_1412.git
   9314f97..45738f9  master -> master

C:\Users\denise\Desktop\workspace\RandomCharacter1>git branch
* master

C:\Users\denise\Desktop\workspace\RandomCharacter1>git checkout -b "dev"
Switched to a new branch 'dev'

C:\Users\denise\Desktop\workspace\RandomCharacter1>git add .

C:\Users\denise\Desktop\workspace\RandomCharacter1>git commit -m "uhhhhh"
On branch dev
nothing to commit, working directory clean

C:\Users\denise\Desktop\workspace\RandomCharacter1>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev


C:\Users\denise\Desktop\workspace\RandomCharacter1>git checkout

C:\Users\denise\Desktop\workspace\RandomCharacter1>git checkout "master"
Switched to branch 'master'
Your branch is up-to-date with 'origin/master'.

C:\Users\denise\Desktop\workspace\RandomCharacter1>git status
On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working directory clean

C:\Users\denise\Desktop\workspace\RandomCharacter1>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': 54r4hv
Password for 'https://54r4hv@github.com':
Everything up-to-date

C:\Users\denise\Desktop\workspace\RandomCharacter1>git add .

C:\Users\denise\Desktop\workspace\RandomCharacter1>git commit -m "eeeerrrrrr"
[master caf085f] eeeerrrrrr
 1 file changed, 5 insertions(+)

C:\Users\denise\Desktop\workspace\RandomCharacter1>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': 54r4hv
Password for 'https://54r4hv@github.com':
Counting objects: 4, done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 360 bytes | 0 bytes/s, done.
Total 4 (delta 2), reused 0 (delta 0)
To https://github.com/54r4hv/Listing_4_16_Project_1412.git
   45738f9..caf085f  master -> master

C:\Users\denise\Desktop\workspace\RandomCharacter1>dir
 Volume in drive C has no label.
 Volume Serial Number is 5A0A-2F66

 Directory of C:\Users\denise\Desktop\workspace\RandomCharacter1

11/10/2015  10:53 PM    <DIR>          .
11/10/2015  10:53 PM    <DIR>          ..
11/10/2015  07:33 PM               232 .classpath
11/10/2015  07:33 PM               392 .project
11/10/2015  07:38 PM    <DIR>          bin
11/10/2015  10:51 PM                30 README.md
11/10/2015  07:38 PM    <DIR>          src
               3 File(s)            654 bytes
               4 Dir(s)  95,364,829,184 bytes free

C:\Users\denise\Desktop\workspace\RandomCharacter1>J:\COMSC_1033_Workspace\Listing_4_16_project>echo # Listing_4_16_project >> README.md
The system cannot find the drive specified.

C:\Users\denise\Desktop\workspace\RandomCharacter1>git add .

C:\Users\denise\Desktop\workspace\RandomCharacter1>git commit -m "uhmmmmm"
[master 75022cf] uhmmmmm
 1 file changed, 272 insertions(+)

C:\Users\denise\Desktop\workspace\RandomCharacter1>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': 54r4hv
Password for 'https://54r4hv@github.com':
Counting objects: 3, done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 2.28 KiB | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
To https://github.com/54r4hv/Listing_4_16_Project_1412.git
   caf085f..75022cf  master -> master

C:\Users\denise\Desktop\workspace\RandomCharacter1>git add .

C:\Users\denise\Desktop\workspace\RandomCharacter1>git commit -m "errrrmmmmm"
[master 97ee89d] errrrmmmmm
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\denise\Desktop\workspace\RandomCharacter1>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': 54r4hv
Password for 'https://54r4hv@github.com':
Counting objects: 3, done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 297 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To https://github.com/54r4hv/Listing_4_16_Project_1412.git
   75022cf..97ee89d  master -> master

C:\Users\denise\Desktop\workspace\RandomCharacter1>git add .

C:\Users\denise\Desktop\workspace\RandomCharacter1>git add .

C:\Users\denise\Desktop\workspace\RandomCharacter1>git commit -m "omg"
[master 484504b] omg
 1 file changed, 5 insertions(+), 2 deletions(-)

C:\Users\denise\Desktop\workspace\RandomCharacter1>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': 54r4hv
Password for 'https://54r4hv@github.com':
Counting objects: 3, done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 307 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To https://github.com/54r4hv/Listing_4_16_Project_1412.git
   97ee89d..484504b  master -> master

C:\Users\denise\Desktop\workspace\RandomCharacter1>
```


##Report

