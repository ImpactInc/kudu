```
// Licensed to the Apache Software Foundation (ASF) under one
// or more contributor license agreements.  See the NOTICE file
// distributed with this work for additional information
// regarding copyright ownership.  The ASF licenses this file
// to you under the Apache License, Version 2.0 (the
// "License"); you may not use this file except in compliance
// with the License.  You may obtain a copy of the License at
//
//   http://www.apache.org/licenses/LICENSE-2.0
//
// Unless required by applicable law or agreed to in writing,
// software distributed under the License is distributed on an
// "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
// KIND, either express or implied.  See the License for the
// specific language governing permissions and limitations
// under the License.
```

## This is a fork of:
[Apache Kudu Repo](https://github.com/apache/kudu)

## Publishing Locally
Produces an artifact `com.impact:kudu-spark2_2.11-1.9.1:alpaqa-VERSION`
```
cd java
./gradlew kudu-spark:publishToMavenLocal -DBUILD_NUMBER=17
ls -alR ~/.m2/repository/com/impact/kudu-spark2_2.11-1.9.1/
```

## Publishing from Jenkins to Nexus
There is a [Jenkins Job](https://data-jenkins-ci.gcp.inf-impact.net/view/Scoring/job/alpaqa-publish-kudu/) to publish shc jar to nexus thirdparty url. To publish a kudu jar, simply go to the alpaqa-publish-kudu job, click release and input the branch you want to release from and a custom version number if applicable.