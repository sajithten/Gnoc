```
git checkout master
git pull
git checkout -b CHANGE-2001257
git rm config/audc1/syd10/c4u1/racks/zs4_4_exmtc_v1_r602.yaml
git rm config/audc1/syd10/c4u1/racks/zs4_4_exmtc_v1_r111.yaml
git rm config/audc1/syd10/c4u1/racks/zs4_4_exmtc_v1_r502.yaml
git add config/audc1/syd10/c4u1/fabric-definitions.yaml
git commit -am "CHANGE-2001257 removing OS rack 602,111 and 502 from fabric-yaml SYD10"
git push -u origin CHANGE-2001257
```
