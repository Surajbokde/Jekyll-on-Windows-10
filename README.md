#  Jekyll on Windows 10

Hi! I struggle a lot to get Jekyll on my laptop which is having windows 10.
You need to just follow the steps given below ...

# Steps

## Install Windows Subsystem for Linux

 

 

- Checked Windows Subsystem for Linux .Boot Your pc if require.

![enter image description here](https://www.howtogeek.com/wp-content/uploads/2018/03/img_5aaaba04b2766.png)

- Open microsoft store 

- Download Ubuntu and launch

![enter image description here](https://assets.ubuntu.com/v1/ecc8acb4-installubuntu.png)

 -  After launching you need to set User and password (*If asked*).
 - (**OPTIONAL** if you want to navigate to go to another drive)
 - `cd /mnt/(drive)/(folder)`
 - Example
 - `cd /mnt/d/dev_suraj`
 
 - ##  Run command carefully
 

```
sudo apt-get install software-properties-common
sudo apt update
sudo apt install gnupg2
```
**Install GPG Keys used to verify installation package**


    gpg --keyserver hkp://pool.sks-keyservers.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB


**Add PPA and Install RVM Package**
```
sudo apt-add-repository -y ppa:rael-gc/rvm
sudo apt-get update
sudo apt-get install rvm
```
 **Change terminal window** 
 `echo 'source "/etc/profile.d/rvm.sh"' >> ~/.bashrc`


**Reboot Your PC**

**Install Ruby:**  

    rvm install ruby

    sudo apt-get install npm

**Go the the Repo**

    cd repo

 

   `bundle install`
    
     make site  

  (either use make site or bundle exec jekyll serve)
  
  `bundle exec jekyll serve`



