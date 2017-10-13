<p>The command and output for hdfs dfs -ls /user</p>

<pre><code>
	[hdfs@ip-172-31-3-113 centos]$ hdfs dfs -ls /user
	Found 6 items
	drwxr-xr-x   - beltran astros           0 2017-10-13 18:08 /user/beltran
	drwxrwxrwx   - mapred  hadoop           0 2017-10-13 18:01 /user/history
	drwxrwxr-t   - hive    hive             0 2017-10-13 18:02 /user/hive
	drwxrwxr-x   - hue     hue              0 2017-10-13 18:02 /user/hue
	drwxr-xr-x   - jimenez rangers          0 2017-10-13 18:08 /user/jimenez
	drwxrwxr-x   - oozie   oozie            0 2017-10-13 18:03 /user/oozie
</code></pre>

<p>The command and output from the CM API call ../api/v5/hosts</p>

<pre><code>
	[hdfs@ip-172-31-3-113 centos]$ curl -u admin:admin 'http://35.165.10.154:7180/api/v5/hosts'
	{
	  "items" : [ {
	    "hostId" : "f390d6c8-7c1f-4c1f-b89c-3852b36286da",
	    "ipAddress" : "172.31.12.173",
	    "hostname" : "ip-172-31-12-173.us-west-2.compute.internal",
	    "rackId" : "/default",
	    "hostUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/hostRedirect/f390d6c8-7c1f-4c1f-b89c-3852b36286da",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "commissionState" : "COMMISSIONED",
	    "numCores" : 4,
	    "totalPhysMemBytes" : 15600140288
	  }, {
	    "hostId" : "237510c4-7a99-4865-90fc-6bad570f3ffc",
	    "ipAddress" : "172.31.13.157",
	    "hostname" : "ip-172-31-13-157.us-west-2.compute.internal",
	    "rackId" : "/default",
	    "hostUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/hostRedirect/237510c4-7a99-4865-90fc-6bad570f3ffc",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "commissionState" : "COMMISSIONED",
	    "numCores" : 4,
	    "totalPhysMemBytes" : 15600140288
	  }, {
	    "hostId" : "dd1e360a-6c0a-4055-a065-aede9a0aaaf3",
	    "ipAddress" : "172.31.14.253",
	    "hostname" : "ip-172-31-14-253.us-west-2.compute.internal",
	    "rackId" : "/default",
	    "hostUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/hostRedirect/dd1e360a-6c0a-4055-a065-aede9a0aaaf3",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "commissionState" : "COMMISSIONED",
	    "numCores" : 4,
	    "totalPhysMemBytes" : 15600140288
	  }, {
	    "hostId" : "f6c5ce2d-c12a-4bc5-ba99-9a808f905b27",
	    "ipAddress" : "172.31.3.113",
	    "hostname" : "ip-172-31-3-113.us-west-2.compute.internal",
	    "rackId" : "/default",
	    "hostUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/hostRedirect/f6c5ce2d-c12a-4bc5-ba99-9a808f905b27",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "commissionState" : "COMMISSIONED",
	    "numCores" : 4,
	    "totalPhysMemBytes" : 15600140288
	  }, {
	    "hostId" : "4d502482-c367-4771-8131-76f619f74e92",
	    "ipAddress" : "172.31.6.74",
	    "hostname" : "ip-172-31-6-74.us-west-2.compute.internal",
	    "rackId" : "/default",
	    "hostUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/hostRedirect/4d502482-c367-4771-8131-76f619f74e92",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "commissionState" : "COMMISSIONED",
	    "numCores" : 4,
	    "totalPhysMemBytes" : 15600140288
	  } ]
	}[hdfs@ip-172-31-3-113 centos]$ 
	
</code></pre>

<p>The command and output from the CM API call ../api/v11/clusters/<githubName>/services</p>

<pre><code>
	[hdfs@ip-172-31-3-113 centos]$ curl -u admin:admin 'http://35.165.10.154:7180/api/v11/clusters/satyar-lenka/services'
	{
	  "items" : [ {
	    "name" : "hive",
	    "type" : "HIVE",
	    "clusterRef" : {
	      "clusterName" : "cluster"
	    },
	    "serviceUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive",
	    "roleInstancesUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive/instances",
	    "serviceState" : "STARTED",
	    "healthSummary" : "GOOD",
	    "healthChecks" : [ {
	      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "HIVE_HIVESERVER2S_HEALTHY",
	      "summary" : "GOOD",
	      "suppressed" : false
	    } ],
	    "configStalenessStatus" : "FRESH",
	    "clientConfigStalenessStatus" : "FRESH",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "displayName" : "Hive",
	    "entityStatus" : "GOOD_HEALTH"
	  }, {
	    "name" : "hbase",
	    "type" : "HBASE",
	    "clusterRef" : {
	      "clusterName" : "cluster"
	    },
	    "serviceUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/hbase",
	    "roleInstancesUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/hbase/instances",
	    "serviceState" : "STARTED",
	    "healthSummary" : "GOOD",
	    "healthChecks" : [ {
	      "name" : "HBASE_MASTER_HEALTH",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "HBASE_REGION_SERVERS_HEALTHY",
	      "summary" : "GOOD",
	      "suppressed" : false
	    } ],
	    "configStalenessStatus" : "FRESH",
	    "clientConfigStalenessStatus" : "FRESH",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "displayName" : "HBase",
	    "entityStatus" : "GOOD_HEALTH"
	  }, {
	    "name" : "zookeeper",
	    "type" : "ZOOKEEPER",
	    "clusterRef" : {
	      "clusterName" : "cluster"
	    },
	    "serviceUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/zookeeper",
	    "roleInstancesUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/zookeeper/instances",
	    "serviceState" : "STARTED",
	    "healthSummary" : "GOOD",
	    "healthChecks" : [ {
	      "name" : "ZOOKEEPER_CANARY_HEALTH",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
	      "summary" : "GOOD",
	      "suppressed" : false
	    } ],
	    "configStalenessStatus" : "FRESH",
	    "clientConfigStalenessStatus" : "FRESH",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "displayName" : "ZooKeeper",
	    "entityStatus" : "GOOD_HEALTH"
	  }, {
	    "name" : "hue",
	    "type" : "HUE",
	    "clusterRef" : {
	      "clusterName" : "cluster"
	    },
	    "serviceUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/hue",
	    "roleInstancesUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/hue/instances",
	    "serviceState" : "STARTED",
	    "healthSummary" : "GOOD",
	    "healthChecks" : [ {
	      "name" : "HUE_HUE_SERVERS_HEALTHY",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "HUE_LOAD_BALANCER_HEALTHY",
	      "summary" : "GOOD",
	      "suppressed" : false
	    } ],
	    "configStalenessStatus" : "FRESH",
	    "clientConfigStalenessStatus" : "FRESH",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "displayName" : "Hue",
	    "entityStatus" : "GOOD_HEALTH"
	  }, {
	    "name" : "oozie",
	    "type" : "OOZIE",
	    "clusterRef" : {
	      "clusterName" : "cluster"
	    },
	    "serviceUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/oozie",
	    "roleInstancesUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/oozie/instances",
	    "serviceState" : "STARTED",
	    "healthSummary" : "GOOD",
	    "healthChecks" : [ {
	      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
	      "summary" : "GOOD",
	      "suppressed" : false
	    } ],
	    "configStalenessStatus" : "FRESH",
	    "clientConfigStalenessStatus" : "FRESH",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "displayName" : "Oozie",
	    "entityStatus" : "GOOD_HEALTH"
	  }, {
	    "name" : "yarn",
	    "type" : "YARN",
	    "clusterRef" : {
	      "clusterName" : "cluster"
	    },
	    "serviceUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/yarn",
	    "roleInstancesUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/yarn/instances",
	    "serviceState" : "STARTED",
	    "healthSummary" : "GOOD",
	    "healthChecks" : [ {
	      "name" : "YARN_JOBHISTORY_HEALTH",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "YARN_NODE_MANAGERS_HEALTHY",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
	      "summary" : "DISABLED",
	      "suppressed" : false
	    } ],
	    "configStalenessStatus" : "FRESH",
	    "clientConfigStalenessStatus" : "FRESH",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "displayName" : "YARN (MR2 Included)",
	    "entityStatus" : "GOOD_HEALTH"
	  }, {
	    "name" : "hdfs",
	    "type" : "HDFS",
	    "clusterRef" : {
	      "clusterName" : "cluster"
	    },
	    "serviceUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/hdfs",
	    "roleInstancesUrl" : "http://ip-172-31-3-113.us-west-2.compute.internal:7180/cmf/serviceRedirect/hdfs/instances",
	    "serviceState" : "STARTED",
	    "healthSummary" : "GOOD",
	    "healthChecks" : [ {
	      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "HDFS_CANARY_HEALTH",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "HDFS_DATA_NODES_HEALTHY",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "HDFS_FREE_SPACE_REMAINING",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "HDFS_HA_NAMENODE_HEALTH",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "HDFS_MISSING_BLOCKS",
	      "summary" : "GOOD",
	      "suppressed" : false
	    }, {
	      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
	      "summary" : "GOOD",
	      "suppressed" : false
	    } ],
	    "configStalenessStatus" : "FRESH",
	    "clientConfigStalenessStatus" : "FRESH",
	    "maintenanceMode" : false,
	    "maintenanceOwners" : [ ],
	    "displayName" : "HDFS",
	    "entityStatus" : "GOOD_HEALTH"
	  } ]
	}[hdfs@ip-172-31-3-113 centos]$ 
	
</code></pre>