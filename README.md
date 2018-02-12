# Install Rails on Mac

Hopefully you have a recent version of Mac OSX installed.

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
