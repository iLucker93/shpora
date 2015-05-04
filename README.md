http://stackoverflow.com/questions/18289366/postgres-no-permission-to-create-user
http://guruadmin.ru/page/15-practical-postgresql-database-administration-commands   
https://github.com/dokku-alt/dokku-alt/issues/66

service postresql restart 
 
Connect as Admin
 
sudo -u postgres psql -d template1
Alter role
 
ALTER ROLE gitlab_ci WITH CREATEDB;
Re-run the task
 
sudo -u gitlab_ci -H bundle exec rake db:setup RAILS_ENV=production
 
 
sudo su postgres -c "psql samara-photo_development -c 'CREATE EXTENSION hstore;'"


 
gem update --system 
 
bundle update

====================================================================================================================
