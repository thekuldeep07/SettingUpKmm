**<u>Setting Up KMM</u>**

-   Install Xcode and Android studio

-   Open terminal and type Brew , if your mac have brew then it will  print something else install brew using
-   Command /bin/bash -c "$(curl -fsSL
> [<u>https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh</u>](https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh))"
>
-   You can get this comment from brew.sh

-   Now install “kdoctor” using command “brew install doctor”

-   Open android studio and from plugins install “kotlin multiplatform mobile” plugin

-   Now run “kdoctor “ command to check requirements installed or not for KMM

-   Most Probably You will get the cocoapods error , for that you need  to install ruby first

-   Use command

-   brew install ruby

-   Add your new version of ruby to the PATH

> echo 'export PATH="/opt/homebrew/opt/ruby/bin:$PATH"' \| sudo tee -a
> \~/.zshrc

-   Restart the terminal

-   Now you can check which ruby version is running by command “which
    > ruby” , it should be

-   /opt/homebrew/opt/ruby/bin/ruby

-   Now install cocoapods using command “sudo gem install cocoapods

-   Again run kdoctor command if you still getting cooapods error then
    > you might have to change the path of cocoapods

-   Check path by “gem which cocoapods”

-   If you get output like
    > “/opt/homebrew/lib/ruby/gems/3.2.0/gems/cocoapods-1.14.3/lib/cocoapods.rb”
-   this than you need to change the path

-   Use command

-   sudo echo 'export
    > PATH="/opt/homebrew/lib/ruby/gems/3.2.0/bin:$PATH"' \>\> \~/.zshrc

-   You might get error regarding UTF-8 encoding , in my case i got this  
    > “CocoaPods requires your terminal to be using UTF-8 encoding.

-Consider adding the following to \~/.zprofile
> export LANG=en_US.UTF-8
> export LC_ALL=en_US.UTF-8”

-   You can use below command to solve this problem

  >  echo 'export LANG=en_US.UTF-8' \>\> \~/.zprofile

  > echo 'export LC_ALL=en_US.UTF-8' \>\> \~/.zprofile

-   Restart your terminal and run “kdoctor” , now you will good to go.
