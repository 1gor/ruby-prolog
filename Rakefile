# Look in the tasks/setup.rb file for the various options that can be
# configured in this Rakefile. The .rake files in the tasks directory
# are where the options are used.

begin
  require 'bones'
  Bones.setup
rescue LoadError
  begin
    load 'tasks/setup.rb'
  rescue LoadError
    raise RuntimeError, '### please install the "bones" gem ###'
  end
end

ensure_in_path 'lib'
require 'ruby_prolog'

task :default => 'spec:run'

PROJ.name = 'ruby_prolog'
PROJ.authors = 'Preston Lee'
PROJ.email = 'preston.lee@openrain.com'
PROJ.url = 'http://openrain.com'
PROJ.version = RubyProlog::VERSION
PROJ.rubyforge.name = 'ruby_prolog'

PROJ.spec.opts << '--color'

# EOF
