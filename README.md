## Removing a remote repository from local git repo

Let's say you've created a local git repository and connected it to a remote GitHub repository by running the command `git remote add origin "your-github-repository"`.

You can check whether or not this connection was successful by running the command `git remote -v` on your command line from within your local directory. This command should list the remote you added twice; once for (fetch) and once for (push).

To remove your local respository's connection with this remote GitHub repository, you would run `git remote rm origin`, since you connected this local repository to your remote repository by running `git remote add origin "your-github-repository"`. If you had instead run the command `git remote add thing "your-remote-repository"` to connect your local repository to your remote repository, you would run `git remote rm thing` to sever the connection.

To make sure your connection was successfully severed, you can run `git remote -v` again. You should get an empty response from your terminal.
