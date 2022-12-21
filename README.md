# clean-firefox
🦊 A set of minimalist configurations for the Firefox browser! 


### Example
![windows-example](https://user-images.githubusercontent.com/14153661/208849296-a944cd5e-b66a-4a83-9021-3a76a85da52f.png)

### Recommended addons:
* [KeePassXC Browser](https://addons.mozilla.org/en-US/firefox/addon/keepassxc-browser/)
* [uBlock Origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)
* [Tree Style Tab](https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/)

### Recommended themes:
* [Gruvbox](https://addons.mozilla.org/en-US/firefox/addon/gruvboxgruvboxgruvboxgruvboxgr/) 

### Adding and applying custom CSS to Firefox
Follow these steps to cleanly style your Tree Style Tab addon. These steps will remove the large 
"Tree Style Tab" title bar, remove the tabs from the top of your browser, and will correctly reposition 
your minimize, maximize, and close window buttons.
1. Clone this repository
    - `git clone https://github.com/OliverAbdulrahim/clean-firefox.git`
2. Open Firefox
3. In the address bar, navigate to "about:profiles"
4. Find the profile that's under use
    - _Hint:_ Look for a message like "This is the profile in use and it cannot be deleted" 
5. Under that profile, find "Root Directory" and copy it
6. Into this directory, copy the "chrome" folder for your operating system 
    - `cp -clean-firefox/<your OS name>/chrome/ <profile-dir>`
7. If you haven't already, [enable CSS customization within Firefox](#enable-custom-css-within-firefox)
    
### Enable custom CSS within Firefox
1. Open Firefox
2. In the address bar, navigate to "about:config"
3. If prompted with a warning, confirm that you'll be careful!
4. Search for the rule `toolkit.legacyUserProfileCustomizations.stylesheets`
5. Set the value of this rule to `true`
6. Close and reopen Firefox
7. You're all done!

