# OnUbuntu
## Setting up git on Ubuntu (Linux)

Install git:
```
sudo apt install git
```
Configure name and email:

```
git config --global unser.name <user name>
```

```
git config --global unser.email <user email>
```
To verify:
```
git config --list
```
Clone repo

```
git clone <repo link>
```
To read README.md file:

```
cat README.md
```
To create a file:
```
touch <file name with extension>
```
To check status of branch and files:

```
git status
```
To save the file from local repo to github respo:
- track the untrack file:
  ```
  git add <file>
  ```
- commit the file with a message:
  ```
  git commit -m ""
  ```
- push the file to the desired brach:
  ```
  git push origin main
  ```
  Error:
  ```
  remote: Support for password authentication was removed on August 13, 2021.
  remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-   repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
  ```
  - To fix this generate a token -> `Settings` -> `Developer Settings` -> `tokens`
  - Set remote access using token:
    ```
    git remote set-url origin https://<token>@github.com/<username>/<repository>
    ```
  - Push:
    ```
    git push origin <branch>
    ```

  ## Setting up python

  ```
  sudo apt install python3
  ```

  - To install pip:
    ```
    sudo apt install python3-pip
    ```
    
