To add 3 fingers touch and slide, need to install fusuma.
Steps -

  1)  Install Fusuma
        a) The first thing you must do is add your user to the input group with the command. Without this fusuma can’t read the touchpad inputs.
        
          sudo gpasswd -a $USER input
         $USER will be replaced by username.
         Log out, then log back in.

        b) Install some dependencies.
        
          sudo apt-get install libinput-tools  
          sudo apt-get install xdotool

        c) Now install ruby (if not already on your machine), and then fusuma.
                          
          sudo apt-get install ruby
          sudo gem install fusuma
  2)  Change Config File
  
        a) Copy the "config.yml" file at this path: ~/.config/fusuma/config.yml
                          
          sudo cp ~/config.yml ~/.config/fusuma/config.yml
        
        Create or modify the shorcuts in Settings => Keyboard & Shortcuts as your preference.
  
  3) Add Fusuma at Startup
        command:          
        
          fusuma -d
        
        
Logout and then log back in.

You are good to go now.

    


