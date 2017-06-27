source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'

def ads_pods
end

def debugging_pods
    pod 'HSTestingBackchannel', :configuration => ['Testing']
end

target 'iZurvive' do
    inhibit_all_warnings!
    ads_pods
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