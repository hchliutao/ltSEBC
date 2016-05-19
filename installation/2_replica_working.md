mysql> show slave status\G<br>
*************************** 1. row ***************************<br>
               Slave_IO_State: Waiting for master to send event<br>
                  Master_Host: 192.168.60.70<br>
                  Master_User: root<br>
                  Master_Port: 3306<br>
                Connect_Retry: 60<br>
              Master_Log_File: mysql-bin.000004<br>
          Read_Master_Log_Pos: 246<br>
               Relay_Log_File: mysql-relay-bin.000005<br>
                Relay_Log_Pos: 175<br>
        Relay_Master_Log_File: mysql-bin.000004<br>
             Slave_IO_Running: Yes<br>
            Slave_SQL_Running: Yes<br>
              Replicate_Do_DB: tecmint<br>
          Replicate_Ignore_DB: <br>
           Replicate_Do_Table: <br>
       Replicate_Ignore_Table: <br>
      Replicate_Wild_Do_Table: <br>
  Replicate_Wild_Ignore_Table: <br>
                   Last_Errno: 0<br>
                   Last_Error: <br>
                 Skip_Counter: 0<br>
          Exec_Master_Log_Pos: 198<br>
              Relay_Log_Space: 543<br>
              Until_Condition: None<br>
               Until_Log_File: <br>
                Until_Log_Pos: 0<br>
           Master_SSL_Allowed: No<br>
           Master_SSL_CA_File: <br>
           Master_SSL_CA_Path: <br>
              Master_SSL_Cert: <br>
            Master_SSL_Cipher: <br>
               Master_SSL_Key: <br>
        Seconds_Behind_Master: 0<br>
Master_SSL_Verify_Server_Cert: No<br>
                Last_IO_Errno: 0<br>
                Last_IO_Error: <br>
               Last_SQL_Errno: 0<br>
               Last_SQL_Error: <br>
1 row in set (0.00 sec)<br>
