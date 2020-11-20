Local Database

service :
- mysql 
    image : latest
    port : 3306 => 3306
    volumes : local
    root : secret
    database : d
    user : d
    pass : d
    tty : true
- phpMySql
    port : 80 => 81
- postgres:
    image : latest
    port : 5432 => 5432
    volume : local
    user : d
    pass : d
- pgAdmin
    port : 5050 => 51
    user : d@localhost
    pass : d