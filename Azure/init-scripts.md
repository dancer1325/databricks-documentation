https://learn.microsoft.com/en-us/azure/databricks/init-scripts/


* goal
  * recommendations for 
    * init scripts
    * configuration information 

* init script (initialization script)
  * := shell script / 👀runs | startup of EACH cluster node 👀
    * BEFORE the Apache Spark driver or executor JVM starts 
  * 👀ALTERNATIVES 👀
    * use compute policies / set system properties, environmental variables, and Spark configuration parameters 
      * see [Compute policy reference](admin.clusters.policy-definition.md)
    * add libraries | cluster policies
      * see [add libraries | a policy](admin.clusters.policies.md)
  * recommendations
    * 👀use | higher -- to -- lower recommendation 👀
      * init scripts -- via -- compute policies
      * cluster-scoped init scripts
      * global init scripts
    * if you want to install library | production and interactive environments -> use compute policies
      * ❌NOT use init scripts ❌
    * use shared access mode | ALL workloads
      * if required functionality is NOT supported by shared access mode -> use single user access mode 
    * use NEW Databricks Runtime versions and Unity Catalog | ALL workloads 
      * if you use Databricks Runtime v13.3+ LTS + Unity Catalog ->	store init scripts | [Unity Catalog volumes](ingestion.file-upload.upload-to-volume.md)
      * if you use Databricks Runtime v11.3+ LTS  WITHOUT Unity Catalog -> store init scripts -- as -- workspace files / 's size < 500 MB
      * if you use Databricks Runtime v10.4- LTS ->	store init scripts -- via -- cloud object storage
  * types
    * [Cluster-scoped](init-scripts.cluster-scoped.md)
    * [Global](init-scripts.global.md)
  * if you change type of init script -> you MUST restart ALL clusters / affected by the script

* recommendations
  * 👀use built-in platform features -- instead of -- init scripts 👀 
    * Reason: 🧠overuse init scripts -> can
      * slow down migration to -- NEW Databricks Runtime versions
      * prevent adoption of SOME Databricks optimizations 🧠

* TODO: Where can init scripts be installed?