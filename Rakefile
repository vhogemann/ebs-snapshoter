
begin
  require 'bones'
rescue LoadError
  abort '### Please install the "bones" gem ###'
end

task :default => 'test:run'
task 'gem:release' => 'test:run'

Bones {
  name     'snapshoter'
  authors  'Kris Rasmussen'
  email    'victor.hogemann@gmail.com'
  url      'https://github.com/vhogemann/ebs-snapshoter'
  
  depend_on 'mysql'
  depend_on 'right_aws', '~> 3.0.0'
}
