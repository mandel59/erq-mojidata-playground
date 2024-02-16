# Set up

Let's prepare to play with Erq and Mojidata.

1. Set up Git.

   - Follow the steps in [Set up Git](https://docs.github.com/en/get-started/getting-started-with-git/set-up-git).
   - Git is a version control system. We use it to download the files we need to play with Erq and Mojidata.
   - The nice thing about Git is that it's easy to update to the latest version, not just download files.

2. Set up Node.js.

    - Download and install Node.js from [Node.js](https://nodejs.org/en).
    - There are LTS and latest versions, but if you're not sure, I recommend the LTS version.
    - Node.js is used to run applications made with JavaScript. `mojidata` and `erq` commands are made with JavaScript, so you need Node.js to run them.

3. Set up jq.

    - Download and install jq from [jq](https://jqlang.github.io/jq/).
    - `jq` is a command for handling JSON data. We use it to make the output of the `mojidata` command easier to read.

4. Start the terminal.

   - If you're using Windows, start Git Bash.

5. Enter the command to clone (download) this repository.

   - Command: `git clone https://github.com/mandel59/erq-mojidata-playground.git`
   - Follow the steps in [Cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) to clone the repository.

6. Move to the cloned repository.

   - Command: `cd erq-mojidata-playground`

7. Use NPM to install the dependent libraries.

   - Command: `npm install`

Now you're ready to play!
