```sh
[root@ip-172-31-5-105 ~]# curl -u hugorodrigues-cds:cloudera 'http://ip-172-31-5-105.ec2.internal:7180/api/v2/cm/deployent'
{
  "timestamp" : "2017-04-05T14:22:09.796Z",
  "clusters" : [ {
    "name" : "hugorodrigues-cds",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "639631360"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "639631360"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "3432356249"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "577"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-5-105.ec2.internal"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_P@ssw0rd"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-16dbafb87f56b5571024e355679848bf",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "06f822fa-07d8-4487-bcf1-45faf63da4b7"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-7849b33c8c86f9da899c0452960fc603",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "66a777e0-eb7f-4a92-9944-7cefd6b97deb"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-a074160b7df867001bcb215fc5121baf",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "655a5ff3-fa44-426f-850c-24ceb713d837"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-fbe0badd547b4715e81ebbbaad4fee46",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "9750544f-fea7-49c2-aba0-a61c2936eae5"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bmpnxadyj4xvz9yjhhbjpeuyb"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1k6tbyxl6x8xl79283xjqzibf"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-16dbafb87f56b5571024e355679848bf",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "06f822fa-07d8-4487-bcf1-45faf63da4b7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dd3sm7on9ybhscqt81qcxsvm2"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-7849b33c8c86f9da899c0452960fc603",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "66a777e0-eb7f-4a92-9944-7cefd6b97deb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "btjlmplucyul2spau7zc4pibh"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-a074160b7df867001bcb215fc5121baf",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "655a5ff3-fa44-426f-850c-24ceb713d837"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dfm7xsyv7mnp1r79wkakcoxz8"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-5-105.ec2.internal"
        }, {
          "name" : "database_password",
          "value" : "hue_P@ssw0rd"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-fbe0badd547b4715e81ebbbaad4fee46"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "colctun6fxwzc4zu5xa4xbbbg"
          }, {
            "name" : "secret_key",
            "value" : "TzcEjuNr8MSZR4zrmlQ0YLR3CP94LK"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-5-105.ec2.internal"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie_P@ssw0rd"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "639631360"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2k8w0tpkmtnnwarlq9wvocztc"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "639631360"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "rm_cpu_shares",
            "value" : "1800"
          }, {
            "name" : "rm_io_weight",
            "value" : "900"
          }, {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm,/data0/yarn/nm,/mnt/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs,/data0/yarn/container-logs,/mnt/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "3"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "2942"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "639631360"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "3480"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "eUXqEepTPzKdQeWDw414G4EwWgMvDe"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c0z04dvs05rbtcdvbhs2q4h8m"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-16dbafb87f56b5571024e355679848bf",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "06f822fa-07d8-4487-bcf1-45faf63da4b7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "74wrklu77grqqv5a0a9myhdom"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-7849b33c8c86f9da899c0452960fc603",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "66a777e0-eb7f-4a92-9944-7cefd6b97deb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6y5kwhk7r4pwpqtdtgp9ll1jo"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-a074160b7df867001bcb215fc5121baf",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "655a5ff3-fa44-426f-850c-24ceb713d837"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8e2cg5q62k3u1cn8latpzyt2c"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-fbe0badd547b4715e81ebbbaad4fee46",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "9750544f-fea7-49c2-aba0-a61c2936eae5"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "10aklr1bdm3kh1y3qfep71xjj"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "53"
          }, {
            "name" : "role_jceks_password",
            "value" : "96iiwghj7fdde1m5q7fvogo1j"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "639631360"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn,/data0/dfs/dn,/mnt/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "8588506316"
          }, {
            "name" : "dfs_datanode_failed_volumes_tolerated",
            "value" : "1"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "200"
          }, {
            "name" : "rm_io_weight",
            "value" : "100"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn,/data0/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "639631360"
          }, {
            "name" : "role_config_suppression_namenode_java_heapsize_minimum_validator",
            "value" : "true"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "639631360"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_block_size",
          "value" : "33554432"
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "Lt8RNuEnXmkx6gIXpPlggdlixJjk47"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "VamNyhJTpHyUtFSBl89ifd5YeST365"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "9GZSv03kNIdsvb0wRhQ973OIgtKBen"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-16dbafb87f56b5571024e355679848bf",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "06f822fa-07d8-4487-bcf1-45faf63da4b7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bcpz8047ug4jzuai1ma6og3tt"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-7849b33c8c86f9da899c0452960fc603",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "66a777e0-eb7f-4a92-9944-7cefd6b97deb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1ysy8hnla5yrnfshujn30rig5"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-a074160b7df867001bcb215fc5121baf",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "655a5ff3-fa44-426f-850c-24ceb713d837"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1o2edqj9qbuawpjsbuwkd3sl4"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-fbe0badd547b4715e81ebbbaad4fee46",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "9750544f-fea7-49c2-aba0-a61c2936eae5"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8ak92wnpssi61f22xe1mucd7q"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5di0qqqecij9a1odvy5x58hhl"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-fbe0badd547b4715e81ebbbaad4fee46",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "9750544f-fea7-49c2-aba0-a61c2936eae5"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6dqot3uw6mxua55i87al0g6b5"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-fbe0badd547b4715e81ebbbaad4fee46",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "9750544f-fea7-49c2-aba0-a61c2936eae5"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ab8mhdngtke2zwvvo5pdv312"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-16dbafb87f56b5571024e355679848bf",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "06f822fa-07d8-4487-bcf1-45faf63da4b7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "51z6nees4zb8ocvdgy5ksk5xf"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-7849b33c8c86f9da899c0452960fc603",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "66a777e0-eb7f-4a92-9944-7cefd6b97deb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "518po8g9xxsw8ylp2trcq91zi"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-a074160b7df867001bcb215fc5121baf",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "655a5ff3-fa44-426f-850c-24ceb713d837"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2aipkgcds5fykhuaghvrwl9a8"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-a5deea7f5e935d5d10f6b75347f62aed",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "9wcf9m1zanjva633ln3cznzwy"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-fbe0badd547b4715e81ebbbaad4fee46",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "9750544f-fea7-49c2-aba0-a61c2936eae5"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "61"
          }, {
            "name" : "role_jceks_password",
            "value" : "1qg2hfyihdppcghu7xcre01mi"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "655a5ff3-fa44-426f-850c-24ceb713d837",
    "ipAddress" : "172.31.1.146",
    "hostname" : "ip-172-31-1-146.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "06f822fa-07d8-4487-bcf1-45faf63da4b7",
    "ipAddress" : "172.31.1.2",
    "hostname" : "ip-172-31-1-2.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "9750544f-fea7-49c2-aba0-a61c2936eae5",
    "ipAddress" : "172.31.12.22",
    "hostname" : "ip-172-31-12-22.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331",
    "ipAddress" : "172.31.5.105",
    "hostname" : "ip-172-31-5-105.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "66a777e0-eb7f-4a92-9944-7cefd6b97deb",
    "ipAddress" : "172.31.9.225",
    "hostname" : "ip-172-31-9-225.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-a5deea7f5e935d5d10f6b75347f62aed",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "42bcc5d22d1fea6bf72dd03afe18d83eed8e53d7bfbbf9575e658be197561701",
    "pwSalt" : 8254673274829037092,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-a5deea7f5e935d5d10f6b75347f62aed",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "0488be0b4ea6bb42549d74dedc832e7f2ae04166a1665dc6a9bd66fdab75dbdb",
    "pwSalt" : 3231613990054359169,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-a5deea7f5e935d5d10f6b75347f62aed",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "02a4bf94eab5062439e18b486cf9539d2bae1fca800d6707e7d47f55438c004d",
    "pwSalt" : -4009944994320424332,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-a5deea7f5e935d5d10f6b75347f62aed",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "06ebe01d5c824eadbc7667793ce81177d0c5b60ef8f4a9a2742a4260d181dc51",
    "pwSalt" : 6821893954821822287,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "db12060e8c5f712d7727e05ffb52d4a6602b84c53cafc34669f20912dc0af927",
    "pwSalt" : 1044616840971067803,
    "pwLogin" : true
  }, {
    "name" : "hugorodrigues-cds",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "d1bf807f5a8eafc8d5512f11c02f790043ce28422c789677ef1798048a78d89a",
    "pwSalt" : -6624667891260995394,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "2fb6bae182daeb45c6895fa051f9f0b2596ebaf3e257802be5242f602a86a0d4",
    "pwSalt" : 3650218694718828266,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.10.1",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170319-2001",
    "gitHash" : "f226435f6fa5f545543c00245900ae43bea7a29c",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "639631360"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "639631360"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "831520768"
        }, {
          "name" : "role_config_suppression_firehose_heap_size_validator",
          "value" : "true"
        }, {
          "name" : "role_config_suppression_firehose_non_java_memory_validator",
          "value" : "true"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-5-105.ec2.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_P@ssw0rd"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "639631360"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "639631360"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "831520768"
        }, {
          "name" : "role_config_suppression_firehose_heap_size_validator",
          "value" : "true"
        }, {
          "name" : "role_config_suppression_firehose_non_java_memory_validator",
          "value" : "true"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-a5deea7f5e935d5d10f6b75347f62aed",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "77u2yrgvz0g4h0st55ry0o1vh"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-a5deea7f5e935d5d10f6b75347f62aed",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "8yxip3v9fy1v29edgwgv8ch4x"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-a5deea7f5e935d5d10f6b75347f62aed",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "6i540gn5z9gjhwemxvtlpcdd4"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-a5deea7f5e935d5d10f6b75347f62aed",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3jl3zp1xktqduluw3vosjzcfg"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-a5deea7f5e935d5d10f6b75347f62aed",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "4c2ba4f6-49e6-4bb5-9338-e9e2c988b331"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "1teaqdyssn4h3wb1vs45ijhz5"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/23/2012 7:20"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}
```
