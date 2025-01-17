https://learn.microsoft.com/en-us/azure/databricks/init-scripts/global


* run | 
  * concrete workspace's clusters
    * == those / configured with 
      * single user access mode or
      * no-isolation shared access mode
  * BEFORE [cluster-scope init scripts](init-scripts.cluster-scoped.md)
* cons
  * ⚠️can cause unexpected issues ⚠️
    * _Example:_ library conflicts
* restrictions
  * ONLY can be created -- by -- workspace admin users
* ways to create them -- via --
  * UI
    * TODO:
  * REST api
* recommendations
  * use better [cluster-scoped init scripts](init-scripts.cluster-scoped.md) 
  * 👀check that your global init scripts do NOT output sensitive information 👀
* allows
  * viewing the global init scripts' output `stderr` and `stdout` -- by -- ANY user / 
    * creates the cluster
    * enables cluster log delivery 
* if you have got problems -> see 
  * [init script logging](init-scripts.logs.md)
  * [cluster log delivery](compute.configure.md)

* TODO: