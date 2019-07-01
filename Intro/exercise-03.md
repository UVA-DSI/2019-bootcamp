# Exercise 3

## Part 1

1. Change back into the Documents directory.
1. Enter the command `wget https://raw.githubusercontent.com/ontoligent/2019-bootcamp/master/Intro/pg105.txt`
2. How many words does the file have?
2. How many lines does the file have?

## Part 2

1. Enter the command  `more pg105.txt`. What is the  text about? 
2. Find where the real text begins.
3. Enter the command `more pg105.txt | grep happiness`. What do you see?
4. Try this: `more pg105.txt | grep happiness > happiness.txt`. Then look at the directory contents. What do you see?
5. Try this: `more pg105.txt | grep Chapter` and then `more pg105.txt | grep Chapter | wc`. What does the result tell you?

## Part 3

1. Use `vi` to remove the Gutenberg boilerplate from the beginning of `pg105.txt`.
2. Use `vi`'s search command -- `/` -- and search for `Finis`. Remove the extra lines from the end of the file. Save the file.
3. Now count how many lines the text has.
4. What does this do? `more pg105.txt | grep ^\s*$ | wc -l`

## Part 4

1. Enter `mv pg105.txt persuasion.txt`
2. Look at the Directory and see what happened.
3. Enter `cp persuasion.txt foo`. Go into `foo` directory and list its contents.
4. Enter `cd ..`. List the contents of the directory. Where are you?
5. Enter `rmdir foo`. What happens?
6. Enter `rm -rf foo`. What happens?
