source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'

def ads_pods
    pod 'GoogleAnalytics-iOS-SDK'
end

def debugging_pods
    pod 'HSTestingBackchannel', :configuration => ['Testing']
end

target 'iZurvive' do
    inhibit_all_warnings!
    ads_pods
    debugging_pods
end

target 'iZurviveTests' do 
    # Pods for testing
    inhibit_all_warnings!
    ads_pods
    debugging_pods     
end

target 'iZurviveUITests' do
    # Pods for UI testing
    inhibit_all_warnings!
    ads_pods
    debugging_pods
    pod 'HSTestingBackchannel', :configuration => ['Testing']
end