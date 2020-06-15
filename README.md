# wfly-9129-reproducer
Reproducer for WFLY-9129

Start Wildfly with enabled Security Manager
  export SECMGR=true;
  on the cmd-line -DSECMGR=true
  edit bin/standalone.conf and uncomment line SECMGR="true"
Deploy reproducer
Go to http://localhost:8080/wfly-9129-reproducer/Print
"Permission check failed" exception should be thrown
