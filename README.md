# udacity_fullstack_project2
udacity 
To be sure that the database tournament works

vagrant@vagrant-ubuntu-trusty-32:/vagrant/tournament$ psql
psql (9.3.5)
Type "help" for help.

vagrant=> CREATE DATABASE tournament;
CREATE DATABASE
vagrant=> \q

use SQL schema

vagrant@vagrant-ubuntu-trusty-32:/vagrant/tournament$ psql tournament < tournament.sql 


run the test
vagrant@vagrant-ubuntu-trusty-32:/vagrant/tournament$ python tournament_test.py 
1. Old matches can be deleted.
2. Player records can be deleted.
3. After deleting, countPlayers() returns zero.
4. After registering a player, countPlayers() returns 1.
5. Players can be registered and deleted.
6. Newly registered players appear in the standings with no matches.
7. After a match, players have updated standings.
8. After one match, players with one win are paired.
Success!  All tests pass!