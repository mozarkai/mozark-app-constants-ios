**MozarkEventConstants** is a sdk is used to define constants to be used in the event sdk, the objective is to define the list of event names and event journey ... to be used for the ui test of an app in order to check later if the scripter has entered valid data before synchronizing them with the server
## Installation :  
To integrate MozarkEventConstants into a new project we have 4 possible steps:
#### 1 - Install cocoapods
If cocoapods is not installed on your Mac try typing this command in the terminal : 
 
     sudo gem install cocoapods
 
#### 2- Generate podfile

    pod init
logically you will have a new file called Podfile generated in your project tree

#### 3- Prepare Podfile
You are just invited to add two lines in the podfile:

    source 'https://github.com/CocoaPods/Specs.git'
    And
    pod 'MozarkEventConstants'
here is an example of the structure of a podfile    

    source 'https://github.com/CocoaPods/Specs.git'
    target 'test_Project' do
     use_frameworks!
     pod "MozarkEventConstants"
    end
    
#### 4- Load MozarkEventConstants

     pod install


## Use :
Import  **MozarkEventConstants**
   
## How to release a new version

To publish a new version, you must:
1. Increment the **spec.version** attribute in the MozarkEventsSDK.podspec file
2. Push the code to branch **main**
3. Create a new tag that corresponds to the version number, for exemple tag number is 2.1 => **git tag 2.1**                  
4. Push the tag => **git push origin 2.1**
5. Check if MozarkEventsSDK.podspec file is valid  => **pod lib lint MozarkEventConstants.podspec --allow-warnings**
6. Publish update : **pod trunk push  MozarkEventConstants.podspec --allow-warnings**  



