# wfly-9129-reproducer
Reproducer for WFLY-9129

Start Wildfly with enabled Security Manager <br />
<ul>
  <li>export SECMGR=true;</li>
  <li>on the cmd-line -DSECMGR=true</li>
  <li>edit bin/standalone.conf and uncomment line SECMGR="true"</li>
</ul>
Deploy reproducer <br />
Go to http://localhost:8080/wfly-9129-reproducer/Print <br />
"Permission check failed" exception should be thrown <br />
