# Install Rails on Mac

These instructions will work if you have a recent version of Mac OSX installed (Yosemite or later).

Open your terminal (Cmd + Space, type 'term' and hit enter)

Copy each of the commands below into the terminal and hit enter. You need to wait for each command to finish running before doing the next.

You will know a command has finished running because you see the `$` (the prompt).

You will be asked for your computer password during some of the steps below so keep an eye on the installation processes. When you type your password, it may look like nothing is happening — but it is :)

The tools you are installing are:

1. Homebrew — a package manager for Mac. This makes it easy to download, install and update code libraries which you will do regularly as a developer.
2. RVM (Ruby Version Manager) — is a tool for managing different versions of Ruby and Rails on your computer. This is useful as new versions come out over time and you want to be able to access new and old versions.
3. Ruby — this is the main Ruby interpreter. You're downloading the latest stable version: 2.4.3
4. Rails — lastly you download and install the Rails gems. This gives you the ability to create Rails applications.


01. Install HomeBrew
    ```
    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    ```

02. When that finishes, run `brew doctor`

03. Install RVM by copying this into your terminal:
    ```
    \curl -sSL https://get.rvm.io | bash -s stable
    ```

04. Copy the following into the terminal:
    ```
    source ~/.rvm/scripts/rvm
    ```

05. Install the latest Ruby by typing this in your terminal:
    ```
    rvm install 2.4.3
    ```

06. Install Rails

  In your terminal type:
    ```
    rvm use ruby-2.4.3@rails514 --create
    ```

07. Now install the latest Rails:
    ```
    gem install rails --version=5.1.4 --no-ri --no-rdoc
    ```

  When it's finished, check the version with `rails -v`. It should be 5.1.4

08. Now set this as the default gemset:
    ```
    rvm use ruby-2.4.3@rails14 --default
    ```

You're done!
