# Lab Report 5

# How I could've done lab report 4 a different way

Last time I did the task very quickly by using the command `fc -e true -12 -1` after signing in which only worked because my last 12 commands were the exact ones needed to do the task. But let's say that wasn't the case, and that they weren't my last 12 commands. I could use the `history` command to look for where I had executed those commands before.

Here I found it in my history from 332-343

![wowie](https://user-images.githubusercontent.com/122561998/224909298-0c7e13a3-f58d-469c-a167-bb89abbb84a5.PNG)


from there I can run `fc -e true 332 343` instead to execute the commands.

![ehe](https://user-images.githubusercontent.com/122561998/224909464-64fa6098-76d8-41a2-bc5d-e16bd2cb4030.PNG)


I could've also made a bash script before even starting the task. I made a new script with `touch run.sh`. Then I copy pasted the old commands I ran from my history. I displayed them without line numbers using the `cat ~/.bash_history` command. From there find the place where the old commands where and select them and `Ctrl-c`. Then `nano run.sh` and `Ctrl-v`, then `Ctrl-x`, ,`y`, and then `enter`.

![huh](https://user-images.githubusercontent.com/122561998/224911208-05250bf2-e2dd-44e4-a7c1-4c5f5a20f3eb.PNG)

![hee](https://user-images.githubusercontent.com/122561998/224911317-fe3b684c-e366-40a4-b68b-6376d5261782.PNG)

After that you can do `bash run.sh` after signing in as usual. It'll do basically the same thing as my original method but it's faster to type than `fc -e true -12 -1` because I can press `tab` after typing `bash r` and it'll autofill the command.

![welp](https://user-images.githubusercontent.com/122561998/224912127-cea363be-8ac6-44a9-bf48-4660f98af60b.PNG)

