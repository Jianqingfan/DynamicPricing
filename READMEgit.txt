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

If you do, you can add it as a key for authentication in the SSH and GPG keys section of GitHub settings.

# SSH Authentication to GitHub

If you have installed a public SSH key from your working machine onto GitHub, it must be unlocked locally to interact with GitHub from Terminal.

Unlock a private key locally:

ssh-add ~/.ssh/<private_key_name>

See your unlocked private keys with:

ssh-add -l

To validate communication with GitHub:

ssh -T git@github.com

# For Home Machine

Because the repository is “local” via Dropbox, we don’t need to clone or create it.  We can being our add/commit and push.

# Adding Collaborators

This is done via GitHub under the repository’s Settings in Collaborators and Teams > Manage Direct Access (my account name is pubino).
