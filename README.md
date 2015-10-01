# First Lab Ruby - Git CLI - OSX

## Objectives

1. Fork the lab via GitHub.
2. Clone your fork via the `git` CLI.
3. Run the lab's tests with the `learn` CLI command.
4. Make a change to your local copy of this lab and pass the tests using the `learn` CLI command.
5. Stage and Commit your changes via the `git` CLI.
6. Push your changes to GitHub via the `git` CLI
7. Open a Pull Request on GitHub

## Instructions

### 1. Forking from Github

Forking is the process of making a personal remote copy of the Learn lab.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/git-workflow-1.png" alt="Git Workflow 1">

To get started, in Learn click "View on GitHub".

![View on GitHub](https://dl.dropboxusercontent.com/s/4wmbuywfusq8l51/2015-09-30%20at%208.17%20PM.png)

Next on Flatiron's Github page for the lab click the Fork button.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/ironboard-labs-step-1.jpg" alt="Ironboard Labs Step 1">

Then select your personal Github account as the location to fork to.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/ironboard-labs-step-1b.jpg" alt="Ironboard Labs Step 1B">

### 2. Clone Your Fork

Cloning is the process of making a local copy of the lab from your personal remote on GitHub.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/git-workflow-2.png" alt="Git Workflow 2">

To clone, make sure you've first clicked on the SSH link, then click the
copy button next to the Clone URL to copy it to your clipboard.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/ironboard-labs-step-2.jpg" alt="Ironboard Labs Step 2">

Next, in Terminal navigate to the parent directory where you would like to place this lab. Then type:  `git clone <paste the clone URL here>`  

Note: You should replace the `<paste the clone URL here>` including the `<` and `>` symbols in the snippet above with your actual clone URL by pressing command+v on mac or ctrl+v on windows. Example: `git clone git@github.com:jongrover/first-lab-000.git`

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/ironboard-labs-step-2b.png" alt="Ironboard Labs Step 2b">

Don't forget to `cd` into the lab directory that was made when you cloned the lab. Once in the directory, open the directory with your favorite text editor. Try `subl .` to open in Sublime or `atom .` to open in Atom.

![Work mode](https://dl.dropboxusercontent.com/s/je5pazo2edy5cwl/2015-09-30%20at%207.34%20PM.png)

This setup, a terminal in the lab's directory and the lab directory open in an editor like Sublime or Atom, that's the state you want to be in when working on a lab on Learn. It means you're ready.

### 3. First test run with `learn`

From your terminal, run the test suite by typing `learn` and hitting enter. You'll see something similar to:

![Failing Test](https://dl.dropboxusercontent.com/s/0ik01a1urmuw7o6/2015-09-30%20at%207.46%20PM.png)

*Note: My prompt is `// ♥`, yours might be different. You'll see a terminal prompt generally represented by a `$`. That indicates you're suppose to be typing in terminal.*

You can see your test is currently failing, which is fine, we haven't done any work yet, so it makes sense.

The failure reads: `Make sure you have added a new file or edited edit-me.txt`

### 4. Passing the lab with `learn`

To pass this lab, either make any change to the content of `edit-me.txt` or create a new file.

You can open `edit-me.txt` and you'll see it is currently empty. Add anything to that file, save the file, and then run `learn`, everything should pass.

You can also pass this lab by creating a new file. From Terminal, you can run `touch new-file` to create a new file. Or use your text editor to create a new file and save it. If a new file is added to this lab, when you run `learn`, your tests should pass.

![Passing Tests](https://dl.dropboxusercontent.com/s/op46jyoc228ji62/2015-09-30%20at%207.53%20PM.png)

### 5. Stage and Commit Your Changes with `git` CLI

Now that the lab is solved, we need to commit your changes. Don't worry if all these commands don't make total sense yet.

To stage your changes for a commit, type.

`git add .`

![1](https://dl.dropboxusercontent.com/s/kesh225ztp4owbk/2015-05-03%20at%209.12%20PM.png)

5. Commit the file.

`git commit -am "My first commit"`

![1](https://dl.dropboxusercontent.com/s/9y3zt153pvaabh0/2015-05-03%20at%209.14%20PM.png)

## 4. Push Your Code to Github

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/git-workflow-4.png" alt="Git Workflow 4">

After adding and commiting your most recent work next we want to push our work up to our personal Github remote (origin).

`git push origin master`

![1](https://dl.dropboxusercontent.com/s/7qta395mpnmst7x/2015-05-03%20at%209.15%20PM.png)

Go to github and confirm the push.

![1](http://flatiron-videos.s3.amazonaws.com/ironboard/ironboard-tutorial/7-solving-the-lab.png)

## 5. Opening a Pull Request

Submitting a pull request can be described as the process of asking the maintainer of the Learn lab (upstream remote) to consider pulling (fetching & merging) in your work from your personal remote copy (origin remote). This enables your instructor to see your solution for the lab.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/git-workflow-5.png" alt="Git Workflow 5">

To do so, in Learn click the title of the lab to go to your forked copy on Github.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/ironboard-labs-step-0b.jpg" alt="Ironboard Labs Step 0b">

Then click the green Pull Request button.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/ironboard-labs-step-4.jpg" alt="Ironboard Labs Step 4">

After reviewing the comparison code and making sure it shows your solution, click the Create pull request button.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/ironboard-labs-step-4e.jpg" alt="Ironboard Labs Step 4e">

Then click Create pull request button again.

<img width="100%" height="auto" src="http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/ironboard-labs-step-4f.jpg" alt="Ironboard Labs Step 4f">
