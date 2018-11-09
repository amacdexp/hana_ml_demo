# hana_ml_demo
Examples using Hana ML  library

API Docs:
[Python Client API for machine learning algorithms](https://help.sap.com/http.svc/rc/3f0dbe754b194c42a6bf3405697b711f/2.0.03/en-US/html/index.html)


Dowload instrauction for Hana Express:
https://developers.sap.com/uk/topics/sap-hana-express.html

Related: 
[Setting up a HANA Express Python Machine Learning API Demo VMs](https://blogs.sap.com/2018/11/03/setting-up-a-hana-express-python-machine-learning-api-demo-vm/)


# Additional extra steps   enabling DI builder if using for 'ML' space
di-space-enablement-ui        STOPPED           0/1         16.0 MB   <unlimited>   https://hxehost:51027


# Test user setup after building the DB
create user MLUSER Password Password1 NO FORCE_FIRST_PASSWORD_CHANGE;
grant AFL__SYS_AFL_AFLPAL_EXECUTE to  MLUSER;
grant "HANA_ML_DEMO_HDI_DB_1"."pythonML" to MLUSER;
