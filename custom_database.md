---

copyright:
  years: 2022, 2024
lastupdated: "2024-04-03"

keywords: lakehouse, database, watsonx.data

subcollection: watsonxdata

---

{:javascript: #javascript .ph data-hd-programlang='javascript'}
{:java: #java .ph data-hd-programlang='java'}
{:ruby: #ruby .ph data-hd-programlang='ruby'}
{:php: #php .ph data-hd-programlang='php'}
{:python: #python .ph data-hd-programlang='python'}
{:external: target="_blank" .external}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:important: .important}
{:note: .note}
{:deprecated: .deprecated}
{:pre: .pre}
{:video: .video}


# Custom database feature
{: #custom_database}

A database is one of the data sources that you can register and use in IBM® {{site.data.keyword.lakehouse_full}}. A catalog defines the schemas and metadata for a data source. You can now use the custom catalog to create connections to data stores that are not provided by the built-in connectors. Custom database feature can be used for connectors that are already supported by Presto but not listed in IBM {{site.data.keyword.lakehouse_full}} supported connectors or databases.
{: shortdesc}


To add a custom database-catalog pair, complete the following steps.

1. Log in to the {{site.data.keyword.lakehouse_short}} console.
2. From the navigation menu, select **Infrastructure manager**.
3. To add a database, click **Add component** and select **Add database**.
4. In the **Add database** window, select custom database from the **Database type** drop-down list.
5. Configure the following deatils for Custom database:


    Two databases with the same name cannot be added.
   {: note}

    Custom databases do not support SSL configuration.
   {: note}


    | Field           | Description        |
    |------------------|--------------------|
    | Display name    | Enter the database name to be displayed on the screen. |
    | connector.name     | Enter the name of the database connector that you want to add.  |
    | Property value             | Enter the properties (and their values) to be configured for the database. Enter the property name-value pair as specified in Presto. |
    | Port           | Enter the port number.  |
    | Encryption           | Encrypting values of the keys are stored.  |
    | Associated catalog definition | Enter the name of the catalog. This catalog is automatically associated with your database. |
    {: caption="Table 1. Register database" caption-side="bottom"}

6. Click **Add**.

    **The following is the list of additional data sources from Presto that Custom database supports:**
    -Prometheus
    -AWS Redshift
    -BigQuery
    -Apache Pinot
    -ClickHouse
    -Cassandra
    -Apache Druid
    -Thrift
    -Redis
    -Apache Accumulo
    -Apache Kudu
    -Local File
    -Black Hole
    -Lark Sheets
