namespace :greeting do
desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

desc 'outputs hello with sazon!'
  task :hola do
    puts "hola de Rake!"
  end
end

desc 'gives access to environment'
  task :environment do
    require_relative './config/environment.rb'
  end

desc 'gives access to Pry console'
  task :console => :environment do
    Pry.start
  end

namespace :db do
desc 'migration, caw,caw!'
  task :migrate => :environment do
    Student.create_table
  end

desc 'when I saw watermelon, you say??'
  task :seed do
    require_relative './db/seeds.rb'
  end
end
