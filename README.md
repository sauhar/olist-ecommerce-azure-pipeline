# ecommerce-azure-pipeline

<h2>📊 Project Overview</h2>
<p>
End-to-end <strong> Data pipeline</strong> for e-commerce orders built using 
<strong>Microsoft Azure cloud services</strong>, integrating multiple data sources and performing advanced ETL and analytics 
on the <strong>Olist dataset</strong>.
</p>

<h2>Architecture</h2>
<p>
<strong>GitHub (Raw Data)</strong> → <strong>filess.io (MySQL / MongoDB)</strong> → <strong>Azure Data Factory</strong> → 
<strong>Azure Databricks</strong> → <strong>Azure Synapse Analytics</strong>
</p>

<h2>Tech Stack</h2>

<h3>Cloud & Data Platform</h3>
<ul>
  <li><strong>Cloud Platform:</strong> Microsoft Azure</li>
  <li><strong>Orchestration:</strong> Azure Data Factory (ADF)</li>
  <li><strong>Processing:</strong> Azure Databricks (PySpark)</li>
  <li><strong>Data Warehouse:</strong> Azure Synapse Analytics</li>
</ul>

<h3>Data Sources & Storage</h3>
<ul>
  <li><strong>Source Repository:</strong> GitHub</li>
  <li><strong>Database Hosting:</strong> filess.io</li>
  <li><strong>Databases:</strong> MySQL, MongoDB</li>
  <li><strong>Languages:</strong> Python, SQL, PySpark</li>
</ul>

<h2>Pipeline Workflow</h2>

<h3>Data Sourcing</h3>
<ul>
  <li>Fetched raw e-commerce dataset files from <strong>GitHub</strong>.</li>
  <li>Hosted and structured data in <strong>MySQL</strong> and <strong>MongoDB</strong> via filess.io.</li>
  <li>Created a hybrid storage architecture combining relational and NoSQL data sources.</li>
</ul>

<h3>Data Ingestion (Azure Data Factory)</h3>
<ul>
  <li>Configured linked services for <strong>MySQL</strong> and <strong>MongoDB</strong> connections.</li>
  <li>Built <strong>copy activities</strong> to extract data from both sources.</li>
  <li>Automated pipelines to ingest data into <strong>Azure Data Lake Storage</strong>.</li>
  <li>Scheduled and monitored ingestion jobs using ADF triggers and monitoring tools.</li>
</ul>

<h3>Data Transformation (Azure Databricks)</h3>
<ul>
  <li>Loaded raw data from Azure Data Lake into <strong>Databricks notebooks</strong>.</li>
  <li>Performed data cleaning and validation — removed duplicates and handled nulls.</li>
  <li>Converted data types and standardized schema formats.</li>
  <li>Executed <strong>feature engineering</strong> and data aggregations for analytics.</li>
  <li>Merged <strong>MySQL</strong> and <strong>MongoDB</strong> datasets into unified tables.</li>
  <li>Created <strong>fact</strong> and <strong>dimension</strong> tables following a Star Schema model.</li>
  <li>Applied business logic transformations to prepare analytical data models.</li>
</ul>

<h3>Data Warehousing (Azure Synapse Analytics)</h3>
<ul>
  <li>Loaded transformed data into <strong>Azure Synapse dedicated SQL pools</strong>.</li>
  <li>Designed optimized <strong>star schema</strong> for high-performance analytics.</li>
  <li>Created fact tables (<strong>Orders</strong>, <strong>Payments</strong>) and dimension tables 
      (<strong>Customers</strong>, <strong>Products</strong>, <strong>Sellers</strong>).</li>
  <li>Implemented <strong>distribution strategies</strong> and <strong>indexing</strong> for faster query performance.</li>
  <li>Developed <strong>views</strong> for Business Intelligence reporting and dashboarding.</li>
</ul>

<hr>

