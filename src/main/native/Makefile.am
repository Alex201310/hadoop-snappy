#
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
ACLOCAL_AMFLAGS = -I m4

AM_CPPFLAGS = @JNI_CPPFLAGS@ -I$(HADOOP_NATIVE_SRCDIR)/src -Isrc/org/apache/hadoop/io/compress/snappy
AM_LDFLAGS = @JNI_LDFLAGS@
AM_CFLAGS = -g -Wall -fPIC -O2 -m$(JVM_DATA_MODEL)

lib_LTLIBRARIES = libhadoopsnappy.la

libhadoopsnappy_la_SOURCES = src/org/apache/hadoop/io/compress/snappy/SnappyCompressor.c src/org/apache/hadoop/io/compress/snappy/SnappyDecompressor.c
libhadoopsnappy_la_LDFLAGS = $(AM_LDFLAGS) -version-info 0:1:0
