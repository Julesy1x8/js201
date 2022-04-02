# Coding Nomads JavaScript 201 Labs

Steps to get set up:

1. Clone this repository to your machine.
2. Create a _new_ repository on your GitHub account. _Don't_ fork this repository, don't clone it either. Take note of the URL of your new, blank GitHub repository:

    ```
    git@github.com:<YOUR_USERNAME>/<YOUR_REPOSITORY_NAME>.git
    ```
    
3. From the command line, navigate to the local clone of this repository:

    ```bash
    $ git remote -v
    ```
    
    This should show you the URL of the Coding Nomads 201 repository, you'll be changing this to your new empty repository.
    
    ```bash
    $ git remote set-url origin git@github.com:<YOUR_USERNAME>/<YOUR_REPOSITORY_NAME>.git
    ```
    
    Then run `git remote -v` to check that it's been replaced.
    
    Finally:
    
    ```bash
    $ git push
    ```
    
    To update your new repository with the labs.
    
4. Create a branch to work on, and once you are ready for your mentor to look over your work, create a pull request and request a review from them. Then you'll merge it together. Start new branches and pull requests for each section.