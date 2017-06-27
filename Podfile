source 'git@git.innovaptor.at:cocoapods/specs.git'
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'

def shared_pods
    pod 'Crashlytics'
    pod 'Mapbox-iOS-SDK@sputnik', :git => 'git@github.com:iv-mexx/Mapbox-iOS-SDK-1.git', :branch => 'master'
    pod 'AFNetworking'
    pod 'AFDownloadRequestOperation'
    pod 'Appirater'
    pod 'CargoBay', '~> 2.1'
    pod 'SVProgressHUD', '~> 1.0'
    pod 'ViewDeck', '~> 2.4'
    pod 'UIView+AutoLayout', '~> 1.3.0'
    pod 'ReactiveCocoa', '~> 2.5'
    pod 'PureLayout', '~> 3.0'
    
    pod 'Shimmer' # Only used for the Offer-Banner, might be removed when the Offer is over..
    # Tools
#    pod 'R.swift', '~> 3.0.0'  // Use as soon as we abandon iOS 7
end

def logging_pods
    pod 'CocoaLumberjack', '~> 1.9'
    pod 'CrashlyticsLumberjack', '~> 1.0.1'
end

def ads_pods
    pod 'ChartboostSDK'
    pod 'Google-Mobile-Ads-SDK'
    pod 'GoogleAnalytics-iOS-SDK'
    pod 'GoogleConversionTracking'
    pod 'mopub-ios-sdk'
end

def inhouse_pods
    pod 'IVLogFormatter', '~> 1.0'
    pod 'IVCategories', '~> 1.0'
    pod 'IVCustomViews', '~> 1.0'
    pod 'IVBase64', '~> 1.0'
    pod 'IVMacros', '~> 1.0'
end

def debugging_pods
    pod 'Reveal-SDK', :configurations => ['Debug']
    pod 'Jibber-Framework', :configurations => ['Debug']
    pod 'HSTestingBackchannel', :configuration => ['Testing']
end

target 'iZurvive' do
    inhibit_all_warnings!
    shared_pods
    logging_pods
    ads_pods
    inhouse_pods
    debugging_pods

    target 'iZurviveTests' do 
        # Pods for testing
        inherit! :search_paths        
    end

    target 'iZurviveUITests' do
        # Pods for UI testing
        inherit! :search_paths
        pod 'HSTestingBackchannel', :configuration => ['Testing']
    end
end