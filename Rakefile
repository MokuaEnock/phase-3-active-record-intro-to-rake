task :environment do
  require_relative "./config/environment"
end

namespace :db do
  desc 'migrate changes to your database'
  task migrate: :environment do
    Student.create_table
  end

  desc "seed the database with some dummy data"
  task seed: :environment do
    require_relative "./db/seeds"
  end


end


desc "drop into the Pry console"
task console: :environment do
  Pry.start
end
