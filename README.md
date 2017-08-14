# Welcome to Cloudinary

1. Let's start by sign up to Cloudinary: <br>
https://cloudinary.com/users/register/free <br>
![alt text](http://res.cloudinary.com/shirly/image/upload/f_auto,q_auto,w_200/signup "Sign Up") <br>
** **Tip** Edit your cloud name (you will thank me later :)

2. Create an upload preset: <br>
https://cloudinary.com/console/settings/upload <br>
![alt text](http://res.cloudinary.com/shirly/image/upload/q_auto,f_auto,w_700/v1502674641/preset.png "New Upload preset") <br>
Choose your own upload preset name and choose unsigned for **Mode**

3. Let go to the code and add our cloud name and our upload preset: <br>
Open the file named: AppDelegate+config.swift.copy

![alt text](http://res.cloudinary.com/shirly/image/upload/q_auto/f_auto/w_500/v1502675284/config.png "configure your cloud name")

* Rename the file (delete the .copy) => `AppDelegate+config.swift`
- update the file with your cloud name.
+ Update the file with your upload preset.

4. Let's add Cloudinary to our project with [cocoapods](https://guides.cocoapods.org/using/getting-started.html)<br>
If you never used cocoapods before go ahead and install it by open your terminal and <br>
`$ sudo gem install cocoapods` (if you are not sure feel free to run it and it will just update your cocoapods) <br>
Now let go to our directory: `cd /Users/../../PhotoAlbumApp-Stage1`

In the terminal: `pod init` to create the pod file

Now go ahead and open the Podfile. The Podfile should look like:

```
# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'PhotoAlbum' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for PhotoAlbum
  pod 'GradientCircularProgress', :git => 'https://github.com/keygx/GradientCircularProgress'
  pod 'Cloudinary'
  pod 'QMServices'


end
```

`pod install` will install all the dependecies to our app.

5. Close the project and open the workspace file.

![alt text](http://res.cloudinary.com/shirly/image/upload/z_0.9,c_pad,w_145,h_145,r_max,e_improve,dpr_2.0,bo_4px_solid_rgb:000000/l_profile_shirly_manor,w_38,h_50,r_max,z_0.90,g_north,c_thumb,bo_2px_solid_rgb:000000/fl_layer_apply,g_south_east,x_74,y_37/f_auto,b_white/wwc.png "Having fun @Cloudinary")
