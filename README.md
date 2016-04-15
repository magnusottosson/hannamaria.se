# hannamaria.se

# Start development server
```
bundle exec middleman server
```

# Deploy Instructions
To deploy the site to github pages perform the following commands
```
rm -rf build/
bundle exec middleman build
bundle exec middleman deploy
```
Note: You need to remove the build folder before deploy becuase if there is a previous deploy left then the git repo is fucked up. See https://github.com/middleman-contrib/middleman-deploy/issues/114

# Nokogiri install issues
Fix with
```
gem install nokogiri -- --use-system-libraries --with-xml2-include=/usr/local/opt/libxml2/include/libxml2
```

