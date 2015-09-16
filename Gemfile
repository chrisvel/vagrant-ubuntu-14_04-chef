source 'https://rubygems.org'

gem 'berkshelf'
gem 'passenger'
gem 'rails'

# Uncomment these lines if you want to live on the Edge:
#
# group :development do
#   gem "berkshelf", github: "berkshelf/berkshelf"
#   gem "vagrant", github: "mitchellh/vagrant", tag: "v1.6.3"
# end
#
# group :plugins do
#   gem "vagrant-berkshelf", github: "berkshelf/vagrant-berkshelf"
#   gem "vagrant-omnibus", github: "schisamo/vagrant-omnibus"
# end

rvm_shell "passenger_module" do
  ruby_string "ruby-2.2.0-p0"
  code        "passenger-install-nginx-module --auto"
  creates node[:passenger][:module_path]
end
