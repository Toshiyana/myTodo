platform :ios, '9.0'

target 'myTodo' do
  use_frameworks!

  # Pods for myTodo
  pod 'RealmSwift'
  pod 'SwipeCellKit' 

  pod 'ChameleonFramework/Swift', :git => 'https://github.com/wowansm/Chameleon.git',
      :branch => 'swift5'

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '9.0'
    end
  end
end


  target 'myTodoTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'myTodoUITests' do
    # Pods for testing
  end

end