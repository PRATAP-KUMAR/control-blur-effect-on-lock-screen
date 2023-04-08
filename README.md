# control-blur-effect-on-lock-screen
Control Blur Effect on Lock Screen for GNOME Shell

Please follow this [issue link](https://github.com/PRATAP-KUMAR/control-blur-effect-on-lock-screen/issues/3) for changing the password entry filed background color to default theme.

![image](https://user-images.githubusercontent.com/40719899/230716380-65c96419-85e1-407e-879d-e47786da2be6.png)

to edit the extensions `stylesheet.css` file with `nano` run below command
````
nano $HOME/.local/share/gnome-shell/extensions/ControlBlurEffectOnLockScreen@pratap.fastmail.fm/stylesheet.css
````

````
/* Delete this styleshet.css file if you wish to have default color/transperency set by GNOME for password entry
or you can change the background-color to your choice.
*/

.login-dialog-prompt-entry {
    background-color: #000;
}
````

Please note that any changes to the `stylesheet.css` file will reflect only after a gnome-shell restart.

Sometimes, turning off and on the extension will do the trick. You may try this first.

To restart gnome-shell,  
If you are on `xorg` - Use Alt+F2 r enter method.  
on `wayland` you need to logout and login.
