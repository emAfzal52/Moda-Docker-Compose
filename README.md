1. # Moda-Docker-Compose
2. # Make a Directory mkdir Project ... Command .. ( mkdir CoxandCox )
3. # Clone git repo into Cox
4. # Copy Your Source Code into src folder
5. # Copy Your database into CoxandCox 
6. # Run Command .. Command ..( bin/start --no-dev )  to pull images and run container on terminal into CoxandCox Directory
7. # Run command ..Command.. ( bin/setup-domain coxandcox.co.uk ) and Open in Browser ..command.. ( open https://coxandcox.co.uk ) on terminal into CoxandCox Directory
8. # Run command to copy your src code into container .. Command.. ( bin/copytocontainer --all )
9. # Run command to import your database into container ..Command .. ( bin/mysql <  <Your-Databse-Name> ) 
10. # From Docker Desktop go to ( -phpfpm-1 ) Note: You can put Admin Names and Password As You wish )  container and Run 
11. # .. Command .. ( php bin/magento setup:install --base-url=http://localhost:80/ --db-host=db --db-name=magento --db-user=root --db-password=magento --admin-firstname=EmAfzal --admin-lastname=Ishaq --admin-email=demotest@gmail.com --admin-user=emafzal --admin-password=Magento@12 --language=en_US --currency=USD --timezone=America/Chicago --use-rewrites=1  )
12. # Go into Database container from Docker Desktop ( -db-1 ) and gointo datbases ..command .. ( mysql -u root -pmagento; ) and then Run ..command.. ( use magento; ) run Following Quries
13. # 1. ( update core_config_data set value = "opensearch" where path = "catalog/search/opensearch_server_hostname"; )
    # 2. ( update core_config_data set value = "opensearch" where path = "catalog/search/engine"; )
    # 3. ( update core_config_data set value = "9200" where path = "catalog/search/opensearch_server_port";  )
14. # Run ..command.. ( bin/magento setup:upgrade ) on terminal into CoxandCox directory 
15. # Run ..command.. ( bin/restart ) on terminal into CoxandCox directory to Restart all Container
16. # Refresh Browser a few second later 
 
 
