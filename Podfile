# Uncomment the next line to define a global platform for your project
platform :ios, '17.0'

target 'CM_NATIVE_IOS' do

    pod 'AFNetworking', '~> 3.0'
    pod 'FBSDKCoreKit', '~> 4.9'

  use_frameworks!

  # Pods for CM_NATIVE_IOS

  target 'CM_NATIVE_IOSTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'CM_NATIVE_IOSUITests' do
    # Pods for testing
  end
  post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings["IPHONEOS_DEPLOYMENT_TARGET"] = "17.0"
      end
    end
  end

end
