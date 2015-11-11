# Listing_4_16_Project_1412 

##Intro

Working on Listing 4.16 to generate a random character using Math.random().

##Code

```public class RandomCharacter {
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
} ```


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
Microsoft Windows [Version 10.0.10240]
(c) 2015 Microsoft Corporation. All rights reserved.

C:\Users\denise>cd desktop

C:\Users\denise\Desktop>cd workspace

C:\Users\denise\Desktop\workspace>cd RandomCharacter1

C:\Users\denise\Desktop\workspace\RandomCharacter1>echo # Listing_4_16_Project_1412 >> README.md

C:\Users\denise\Desktop\workspace\RandomCharacter1>git init
Initialized empty Git repository in C:/Users/denise/Desktop/workspace/RandomCharacter1/.git/

C:\Users\denise\Desktop\workspace\RandomCharacter1>git add README.md

C:\Users\denise\Desktop\workspace\RandomCharacter1>git commit -m "first commit"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'denise@denise-PC.(none)')

C:\Users\denise\Desktop\workspace\RandomCharacter1>git config user.name "Sarah VanLeeuwen"

C:\Users\denise\Desktop\workspace\RandomCharacter1>git config user.email "vanleeuwens@student.swosu.edu"

C:\Users\denise\Desktop\workspace\RandomCharacter1>

C:\Users\denise\Desktop\workspace\RandomCharacter1>git commit -m "first commit"
[master (root-commit) 9314f97] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

C:\Users\denise\Desktop\workspace\RandomCharacter1>git remote add origin https://github.com/54r4hv/Listing_4_16_Project_1412.git

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

C:\Users\denise\Desktop\workspace\RandomCharacter1>

```

##Report

