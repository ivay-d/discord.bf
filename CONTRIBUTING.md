# Welcome!
Hello, thanks for considering contributing to this repository!
> **Note**: Contributions to this repository are made by pull requests. If you are new to GitHub please familiarize yourself with the [GitHub Docs](https://docs.github.com/en/pull-requests)

## How To Contribute
In this part we will talk about:
  - [What you need to know](#what-to-know)
  - [Making an issue](#issues)
  - [Setup the project in your terminal](#setup)
  - [Guidelines](#guidelines)
  - [Testing your changes](#testing-your-changes)
  - [Making a pull request](#making-a-pull-request)

### What to know
We appreciate the enthusiasm but before starting to contribute you need to know a few things. This includes (but not limited to):
  - C++
  - Brainfuck
  - GitHub forking/issues/pull requests 

### Issues
Issues are a great way to report bugs or request new features, before making a pull request we ask you to create an issue with the feature you are going to add and reference it in the pull requests you create. (Psst, remember you don't need to create a pull request. Maybe someone will code your idea, who knows.).

### Setup
To begin you first need to install [git](https://git-scm.com/doc).
 
 After installing git open your terminal and run:
 ```bash
 git clone https://github.com/ivay-d/discord.bf
 cd discord.bf 
 ls
 ```
> **Note**: We have a cli to make your contribution smoother. You can install it from [here](https://github.com/ivay-d/discord.bf-cli).

### Guidelines
 To keep the project consistent and easy to read for everyone, please follow the guidelines.

   - Files names must be snake\_case (i.e. file\_name.cpp)
   - Follow the code style, our code style might be a little weird so we made a [file](./CODE_STYLE.md) talking about it.
   - Make the commit messages meaningful (e.g. Fixed the bug where bots couldn't stay in the voice chat for long times)
   - Try to keep the pull requests small, reviewing 200-line change is easier than 4000-line change.
   - Comments are optional but will be very appreciated if you add them. This makes it easier to review the code.

### Testing your changes
First install our cli from [here](https://github.com/ivay-d/discord.bf-cli).

After the cli installs run:
```bash
dbf run-tests
```
This will run every test, make sure nothing fails. If something fails, that can mean your code can be faulty.

**Adding Tests**:
To add tests create a file in the tests folder, and add the content:
```c++
// ...
int test()
{
    // ...
    return 0; // This signals the test has been successful, to make the test fail replace 0 with 1.
}
```
Our cli will automatically detect your test and will run it when you run `dbf run-tests`.
If capable of making a script testing the new feature on your bot.

### Making a pull request
After you added and tested your changes you should be left with the question: "How do I push these changes to the discord.bf?", you will do that with pull requests! This part will briefly explain what you need to do.

First of all run this in your terminal:
```bash
git add .
git commit -m "Commit Message!"
```
It will prompt you to set your GitHub name and GitHub email (it won't prompt you about it if you already set it), make sure you set them.
Then run:
```bash
git push
```
This will ask you for your GitHub name and GitHub password. Now it actually won't accept your GitHub password, you need a token for it to work. To get your token go to https://github.com/settings/tokens and press "Generate New Token".
> **Note:** Do not share your tokens to ANYONE.

Now you need to go to https://github.com/ivay-d/discord.bf/pulls and press "New Pull Request". You should see a text, "compare across forks" click that and select your fork and you should be done!
