
<VersionBlock firstVersion="1.6">

- Have a dbt Cloud Team or Enterprise account. Suitable for both Multi-tenant and Single-tenant deployment. 
    - Note: Single-tenant accounts should contact their account representative for necessary setup and enablement.
- Have both your production and development environments running [dbt version 1.6 or higher](/docs/dbt-versions/upgrade-core-in-cloud).
- Use Snowflake, BigQuery, Databricks, or Redshift.
-  Create a successful run in the environment where you configure the Semantic Layer. 
   - **Note:** Semantic Layer currently supports the Deployment environment for querying. (_development querying experience coming soon_) 
- Set up the [Semantic Layer API](/docs/dbt-cloud-apis/sl-api-overview) in the integrated tool to import metric definitions. 
  - dbt Core or Developer accounts can define metrics but won't be able to dynamically query them.<br />
- Understand [MetricFlow's](/docs/build/about-metricflow) key concepts, which powers the latest dbt Semantic Layer.  
- Note that SSH tunneling for [Postgres and Redshift](/docs/cloud/connect-data-platform/connect-redshift-postgresql-alloydb) connections, [PrivateLink](/docs/cloud/secure/about-privatelink), and [Single sign-on (SSO)](/docs/cloud/manage-access/sso-overview) doesn't supported the dbt Semantic Layer yet.

</VersionBlock>


<VersionBlock firstVersion="1.3" lastVersion="1.5" >

- Have a multi-tenant dbt Cloud instance, <a href="https://docs.getdbt.com/docs/cloud/about-cloud/regions-ip-addresses">hosted</a> in North America <br />
- Have both your production and development environments running dbt version 1.3 or higher <br />
- Use Snowflake data platform <br />
- Install the <a href="https://hub.getdbt.com/dbt-labs/metrics/latest/">dbt metrics package</a> version <code>>=1.3.0, <1.4.0</code> in your dbt project <br />
  * **Note** &mdash; After installing the dbt metrics package and updating the `packages.yml` file, make sure you run at least one model.
- Set up the <a href="https://docs.getdbt.com/docs/dbt-cloud-apis/discovery-api">Discovery API</a> in the integrated tool to import metric definitions 
  * Developer accounts will be able to query the Proxy Server using SQL, but will not be able to browse pre-populated dbt metrics in external tools, which requires access to the Discovery API <br />

</VersionBlock>

<VersionBlock lastVersion="1.2">

- Have a multi-tenant dbt Cloud instance, <a href="https://docs.getdbt.com/docs/cloud/about-cloud/regions-ip-addresses">hosted</a> in North America <br /> 
- Have both your production and development environments running dbt version 1.2 <br />
- Use Snowflake data platform <br />
- Install the <a href="https://hub.getdbt.com/dbt-labs/metrics/latest/">dbt metrics package</a> version <code>>=0.3.0, <0.4.0</code> in your dbt project <br />
  * **Note** &mdash; After installing the dbt metrics package and updating the `packages.yml` file, make sure you run at least one model.
- Set up the <a href="https://docs.getdbt.com/docs/dbt-cloud-apis/discovery-api">Discovery API</a> in the integrated tool to import metric definitions 
  * Developer accounts will be able to query the Proxy Server using SQL, but will not be able to browse pre-populated dbt metrics in external tools, which requires access to the Discovery API <br />

</VersionBlock>
