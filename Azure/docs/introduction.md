https://learn.microsoft.com/en-us/azure/databricks/introduction/

* see [README](/README.md)
* Databricks 
  * 👀manages and deploys cloud infrastructure / ON your behalf 👀
    * -- via -- integrates | your cloud account, with
      * cloud storage
      * cloud security 
  * provides
    * Data processing scheduling and management (_Example:_ ETL)
    * Generating dashboards and visualizations
    * Managing security, governance, high availability, and disaster recovery
    * Data discovery, annotation, and exploration
    * Machine learning (ML) modeling, tracking, and model serving
    * Generative AI solutions
  * keeps -- updated with -- open source integrations (SOME -- were originally created by -- Databricks employees)
    * [Delta Lake](https://delta.io/) and [Delta Sharing](https://delta.io/sharing/)
    * [MLflow](https://mlflow.org/)
    * [Apache Spark](https://spark.apache.org/) and Structured Streaming
    * [Redash](https://redash.io/)
  * ways to interact with it
    * workspace UI
    * REST API
    * CLI
    * Terraform
  * how does it work?
    * generative AI + data lakehouse
    * connecting ALL your sources of data -- to -- Databricks platform / apply solutions ([BI, generative AI])
  * uses 
    * understand the unique semantics -- of -- YOUR data
    * automatically 
      * optimizes performance
      * manages infrastructure / -- match your -- business needs
    * about ALL your sources of data | Databricks platform, to
      * process
      * store,
      * share,
      * analyze,
      * model,
      * monetize
    * -- integrate with -- APIs (_Example:_ OpenAI) / NOT compromising data privacy and IP control
  * proprietary tools / integrate and expand technologies
    * [Jobs](jobs.md)
    * [Unity Catalog](data-governance.unity-catalog.md)
    * [Delta Live Tables](delta-live-tables.md)
    * [Databricks SQL](sql.md)
    * [Photon compute clusters](compute.photon.md)

* Azure Databricks == Databricks | Azure
  * Azure Databricks platform architecture == 
    * infrastructure / used by Azure Databricks
      * allows, about the platform and services
        * deploy,
        * configure,
        * manage 
    * customer-owned infrastructure / managed by Azure Databricks + your company
  * requirements
    * 👀NOT force you to migrate your data | proprietary storage systems 👀
    * configure an Azure Databricks workspace / secure integrations between Azure Databricks platform -- & -- your cloud account
  * how does it work?
    * Azure Databricks -- via your account's cloud resources -- deploys compute clusters /
      * process
      * store data | object storage & other integrated services | your control
  * use cases
    * == # of data processed & employees
    * build an enterprise data lakehouse

* data lakehouse
  * == enterprise data warehouses + data lakes
  * allows, about enterprise data solutions / distributed,
    * accelerate, 
    * simplify (building, maintaining, and syncing) 
    * unify
  * uses
    * single source of truth for
      * Data engineers,
      * data scientists,
      * analysts,
      * production systems

* Unity Catalog
  * extends the relationship, Azure Databricks -- & -- your account
    * _Example:_ access data -- via -- familiar SQL syntax

* Natural language
  * processing
    * learns your business’s language / asking a question | your own words -> you can
      * search data
      * discover data
  * assistance helps you
    * write code,
    * troubleshoot errors,
    * find answers | documentation

* TODO: ETL and data engineering