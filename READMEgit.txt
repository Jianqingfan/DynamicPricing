For Git:

To turn a local folder into a Git repository, you start by initializing it.

git init

Next, you "stage” or add files, which tells Git which files to include in the commit.  In this example, we include all files (the “.” ).

git add .

Finally, commit the changes within the staged files to history with a descriptive message.

git commit -m "Initial commit: setting up the project"

Because you typically want to add and commit at once, I like to use a command that combines the two.

git commit -am "Testing a second commit"

For the public/private SSH key pair, check to see if you have any files ending in .pub.

ls ~/.ssh

If you do, you can add it as a key for authentication in the SSH and GPG keys section of GitHub settings.
