source 'https://github.com/CocoaPods/Specs.git'

use_frameworks!
platform :ios, '12.0'
inhibit_all_warnings!

target 'PetProject' do
  #pod 'IQKeyboardManagerSwift', '6.5.10'
  pod 'Firebase/Core', '8.8.0'
  pod 'Firebase/Analytics', '8.8.0'
  pod 'Firebase/Messaging', '8.8.0'
  pod 'Firebase/Crashlytics', '8.8.0'
  pod 'Firebase/RemoteConfig', '8.8.0'
  pod 'GoogleMaps', '6.2.1'
  pod 'GooglePlaces', '6.2.1'
  #pod 'Alamofire', '5.4.4'
  #pod 'Kingfisher', '6.3.1'
  #pod 'ObjectMapperAdditions/Realm', '8.0'
  #pod 'Socket.IO-Client-Swift', '~> 15.2.0'
  #pod 'GrowingTextViewHandler-Swift', '1.2'
  #pod 'Tagging', '0.5.0'
  #pod 'AlignedCollectionViewFlowLayout', '1.1.2'
  #pod 'NVActivityIndicatorView/AppExtension', '4.8.0'
  #pod 'SwiftLint', '0.44.0'
  #pod 'MultiSlider', '1.12.3'
  #pod 'ReachabilitySwift', '5.0.0'
  #pod 'KeychainAccess', '4.2.2'

  target 'PetProjectTests' do
    inherit! :search_paths
  end
end

post_install do |installer|
  installer.pods_project.build_configurations.each do |config|
    config.build_settings["EXCLUDED_ARCHS[sdk=iphonesimulator*]"] = "arm64"
  end
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '12.0'
    end
  end
end
