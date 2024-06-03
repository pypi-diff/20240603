# Comparing `tmp/RocketSim-2.1.0a6.tar.gz` & `tmp/RocketSim-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RocketSim-2.1.0a6.tar", last modified: Sun May  5 18:57:46 2024, max compression
+gzip compressed data, was "RocketSim-2.1.1.tar", last modified: Mon Jun  3 02:12:06 2024, max compression
```

## Comparing `RocketSim-2.1.0a6.tar` & `RocketSim-2.1.1.tar`

### file list

```diff
@@ -1,335 +1,347 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.347940 RocketSim-2.1.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 18:57:46.347940 RocketSim-2.1.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.307940 RocketSim-2.1.0a6/RocketSim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29474 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.303940 RocketSim-2.1.0a6/libsrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.311940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.303940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.311940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    37735 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    40585 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h
--rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h
--rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)    27531 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.319940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    22714 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    48206 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18241 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h
--rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    24106 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h
--rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.323940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h
--rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h
--rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.327940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h
--rw-r--r--   0 runner    (1001) docker     (127)    26341 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h
--rw-r--r--   0 runner    (1001) docker     (127)    26567 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h
--rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h
--rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h
--rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.303940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.327940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h
--rw-r--r--   0 runner    (1001) docker     (127)    86089 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.331940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)    34628 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h
--rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19955 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.331940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.335940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.335940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/
--rw-r--r--   0 runner    (1001) docker     (127)    20707 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h
--rw-r--r--   0 runner    (1001) docker     (127)    28888 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHull.h
--rw-r--r--   0 runner    (1001) docker     (127)    56111 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btHashMap.h
--rw-r--r--   0 runner    (1001) docker     (127)    24434 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btList.h
--rw-r--r--   0 runner    (1001) docker     (127)    43774 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMatrixX.h
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMinMax.h
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMotionState.h
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuadWord.h
--rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuaternion.h
--rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuickprof.h
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btRandom.h
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btReducedVector.h
--rw-r--r--   0 runner    (1001) docker     (127)    24915 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btScalar.h
--rw-r--r--   0 runner    (1001) docker     (127)   128666 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer.h
--rw-r--r--   0 runner    (1001) docker     (127)   128676 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h
--rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btThreads.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btThreads.h
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btTransform.h
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    57838 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btVector3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    38269 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btVector3.h
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/btBulletCollisionCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/btBulletDynamicsCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.339940 RocketSim-2.1.0a6/python-mtheall/
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Angle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    94546 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Arena.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Array.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Array.h
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Ball.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/BallHitInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/BallState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/BoostPad.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/BoostPadState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13598 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Car.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/CarConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/CarControls.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    36056 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/CarState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/DemoMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/GameMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/MemoryWeightMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Module.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Module.h
--rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/MutatorConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/PyRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/RotMat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Team.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Vec.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/WheelPairConfig.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     7834 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/regression_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73848 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/unit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:57:46.347940 RocketSim-2.1.0a6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.339940 RocketSim-2.1.0a6/src/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/BaseInc.h
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/BulletLink.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/BulletLink.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.339940 RocketSim-2.1.0a6/src/CollisionMeshFile/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/CollisionMeshFile/CollisionMeshFile.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/CollisionMeshFile/CollisionMeshFile.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/DataStream/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/DataStream/DataStreamIn.h
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/DataStream/DataStreamOut.h
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/DataStream/SerializeObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Framework.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Math/
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Math/Math.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Math/Math.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Math/MathTypes/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Math/MathTypes/MathTypes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Math/MathTypes/MathTypes.h
--rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/RLConst.h
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/RocketSim.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/RocketSim.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/Arena/
--rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Arena/Arena.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Arena/Arena.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/Ball/
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Ball/Ball.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Ball/Ball.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/BallHitInfo/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BallHitInfo/BallHitInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BallHitInfo/BallHitInfo.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/BallPredTracker/
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BallPredTracker/BallPredTracker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BallPredTracker/BallPredTracker.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/BoostPad/
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPad.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPad.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/Car/
--rw-r--r--   0 runner    (1001) docker     (127)    28015 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Car/Car.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Car/Car.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/Car/CarConfig/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Car/CarConfig/CarConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Car/CarConfig/CarConfig.h
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/CarControls.h
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/CollisionMasks.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/GameEventTracker/
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/GameEventTracker/GameEventTracker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/GameEventTracker/GameEventTracker.h
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/GameMode.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/MutatorConfig/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/MutatorConfig/MutatorConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/MutatorConfig/MutatorConfig.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/PhysState/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/PhysState/PhysState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/PhysState/PhysState.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/
--rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.347940 RocketSim-2.1.0a6/src/Sim/btVehicleRL/
--rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/btVehicleRL/btVehicleRL.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/btVehicleRL/btVehicleRL.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-03 02:11:56.000000 RocketSim-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-03 02:11:56.000000 RocketSim-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-03 02:12:06.109908 RocketSim-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-06-03 02:11:56.000000 RocketSim-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.073907 RocketSim-2.1.1/RocketSim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-03 02:12:06.000000 RocketSim-2.1.1/RocketSim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-06-03 02:12:06.000000 RocketSim-2.1.1/RocketSim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 02:12:06.000000 RocketSim-2.1.1/RocketSim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 02:12:06.000000 RocketSim-2.1.1/RocketSim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 02:12:06.000000 RocketSim-2.1.1/RocketSim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.065907 RocketSim-2.1.1/libsrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.073907 RocketSim-2.1.1/libsrc/bullet3-3.24/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.065907 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.077907 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btAxisSweep3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btAxisSweep3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btAxisSweep3Internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37735 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    40585 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27531 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btRSBroadphase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btRSBroadphase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btSimpleBroadphase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btSimpleBroadphase.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.081907 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22714 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16311 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48206 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18241 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24106 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.089908 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.093907 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26341 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26567 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.065907 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.093907 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    86089 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.093907 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34628 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20060 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.093907 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.101908 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.101908 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/TaskScheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)    20707 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28888 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btConvexHull.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56111 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btHashMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24434 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btList.h
+-rw-r--r--   0 runner    (1001) docker     (127)    44060 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btMatrixX.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btMinMax.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btMotionState.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btQuadWord.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btQuaternion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btQuickprof.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btRandom.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btReducedVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24935 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btScalar.h
+-rw-r--r--   0 runner    (1001) docker     (127)   128666 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btSerializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)   128676 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btThreads.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btThreads.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btTransform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57838 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btVector3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    38453 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btVector3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/btBulletCollisionCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-06-03 02:11:56.000000 RocketSim-2.1.1/libsrc/bullet3-3.24/btBulletDynamicsCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 02:11:56.000000 RocketSim-2.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.105908 RocketSim-2.1.1/python-mtheall/
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Angle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    96861 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Arena.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/ArenaConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Array.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Ball.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11980 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/BallHitInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/BallPredictor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/BallState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/BoostPad.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/BoostPadState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Car.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/CarConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/CarControls.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    36182 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/CarState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/DemoMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/GameMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/MemoryWeightMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Module.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31165 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Module.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25482 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/MutatorConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/PyRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/RotMat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Team.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/Vec.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/WheelPairConfig.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8774 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/regression_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    79117 2024-06-03 02:11:56.000000 RocketSim-2.1.1/python-mtheall/unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 02:12:06.109908 RocketSim-2.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2598 2024-06-03 02:11:56.000000 RocketSim-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.105908 RocketSim-2.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/BaseInc.h
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/BulletLink.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/BulletLink.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.105908 RocketSim-2.1.1/src/CollisionMeshFile/
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/CollisionMeshFile/CollisionMeshFile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/CollisionMeshFile/CollisionMeshFile.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.105908 RocketSim-2.1.1/src/DataStream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/DataStream/DataStreamIn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/DataStream/DataStreamOut.h
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/DataStream/SerializeObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Framework.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.105908 RocketSim-2.1.1/src/Math/
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Math/Math.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Math/Math.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.105908 RocketSim-2.1.1/src/Math/MathTypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Math/MathTypes/MathTypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Math/MathTypes/MathTypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/RLConst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/RocketSim.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/RocketSim.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.105908 RocketSim-2.1.1/src/Sim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.105908 RocketSim-2.1.1/src/Sim/Arena/
+-rw-r--r--   0 runner    (1001) docker     (127)    35780 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Arena/Arena.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Arena/Arena.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.105908 RocketSim-2.1.1/src/Sim/Arena/ArenaConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Arena/ArenaConfig/ArenaConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Arena/ArenaConfig/ArenaConfig.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/Ball/
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Ball/Ball.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Ball/Ball.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/BallHitInfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/BallHitInfo/BallHitInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/BallHitInfo/BallHitInfo.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/BallPredTracker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/BallPredTracker/BallPredTracker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/BallPredTracker/BallPredTracker.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/BoostPad/
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/BoostPad/BoostPad.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/BoostPad/BoostPad.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/BoostPad/BoostPadGrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/Car/
+-rw-r--r--   0 runner    (1001) docker     (127)    28033 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Car/Car.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Car/Car.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/Car/CarConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Car/CarConfig/CarConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/Car/CarConfig/CarConfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/CarControls.h
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/CollisionMasks.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/GameEventTracker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/GameEventTracker/GameEventTracker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/GameEventTracker/GameEventTracker.h
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/GameMode.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/MutatorConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/MutatorConfig/MutatorConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/MutatorConfig/MutatorConfig.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/PhysState/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/PhysState/PhysState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/PhysState/PhysState.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/SuspensionCollisionGrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 02:12:06.109908 RocketSim-2.1.1/src/Sim/btVehicleRL/
+-rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/btVehicleRL/btVehicleRL.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-06-03 02:11:56.000000 RocketSim-2.1.1/src/Sim/btVehicleRL/btVehicleRL.h
```

### Comparing `RocketSim-2.1.0a6/LICENSE` & `RocketSim-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/README.md` & `RocketSim-2.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 **A C++ library for simulating Rocket League games at maximum efficiency**
 
 RocketSim is a complete simulation of Rocket League's gameplay logic and physics that is completely standalone.
 RocketSim supports the game modes: Soccar, Hoops, Heatseeker, and Snowday.
 
 # Speed
 RocketSim is designed to run extremely fast, even when complex collisions and suspension calculations are happening every tick.
-On an average PC running a single thread of RocketSim with two cars, RocketSim can simulate around 10 minutes of game time every second.
-This means that with 12 threads running RocketSim, you can simulate around 5 days of game time every minute!
+On an average PC running a single thread of RocketSim with two cars, RocketSim can simulate around 20 minutes of game time every second.
+This means that with 12 threads running RocketSim, you can simulate around 10 days of game time every minute!
 
 # Accuracy
-RocketSim is not a perfectly accurate replication of Rocket League, but is close enough for most applications.
+RocketSim is not a perfectly accurate replication of Rocket League, but is close enough for most applications (such as training ML bots).
 Perceivable differences between the simulation and the real game usually take at least a second to accumulate from an initial state.
 This means RocketSim is accurate enough to:
 - *Train machine learning bots*
 - *Simulate different shots on the ball at different angles to find the best input combination*
 - *Simulate air control to find the optimal orientation input*
 - *Simulate ground and floor pinches*
 
 However, RocketSim is NOT accurate enough to:
-- *Simulate entire games from inputs alone*
+- *Accurately re-create entire games from inputs alone*
 - *Perfectly simulate long sequences of jumps and landings*
 
 ## Installation
 - Clone this repo and build it
 - Use https://github.com/ZealanL/RLArenaCollisionDumper to dump all of Rocket League's arena collision meshes
 - Move those assets into RocketSim's executing directory
 
@@ -53,20 +53,18 @@
 Cars: 2 on each team (2v2)
 Inputs: Randomly pre-generated, changed every 2-60 ticks for each car
 =================================
 Single-thread performance (calculated using average CPU cycles per tick on the RocketSim thread) (1M ticks simulated):
 v1.0.0 = 30,334tps
 v1.1.0 = 48,191tps
 v1.2.0 = 50,763tps
+v2.0.0 = ~50,000tps
+v2.1.0 = 114,481tps
 ```
 
-## Simulation Accuracy
-RocketSim is not perfectly accurate, but it's close enough that it shouldn't matter (for ML bots or humans).
-Bots that work well in RocketSim will work well in the actual game and visa-versa.
-
 ## Example Usage
 ```python
 #!/usr/bin/env python3
 
 import RocketSim as rs
 
 # Make an arena instance (this is where our simulation takes place, has its own btDynamicsWorld instance)
```

### Comparing `RocketSim-2.1.0a6/RocketSim.egg-info/SOURCES.txt` & `RocketSim-2.1.1/RocketSim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+/home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btAxisSweep3.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp
+/home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btRSBroadphase.cpp
+/home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btSimpleBroadphase.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp
@@ -84,17 +87,19 @@
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/LinearMath/btThreads.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/LinearMath/btVector3.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp
 /home/runner/work/RocketSim/RocketSim/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/Angle.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/Arena.cpp
+/home/runner/work/RocketSim/RocketSim/python-mtheall/ArenaConfig.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/Array.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/Ball.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/BallHitInfo.cpp
+/home/runner/work/RocketSim/RocketSim/python-mtheall/BallPredictor.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/BallState.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/BoostPad.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/BoostPadState.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/Car.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/CarConfig.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/CarControls.cpp
 /home/runner/work/RocketSim/RocketSim/python-mtheall/CarState.cpp
@@ -109,14 +114,15 @@
 /home/runner/work/RocketSim/RocketSim/python-mtheall/WheelPairConfig.cpp
 /home/runner/work/RocketSim/RocketSim/src/BulletLink.cpp
 /home/runner/work/RocketSim/RocketSim/src/RocketSim.cpp
 /home/runner/work/RocketSim/RocketSim/src/CollisionMeshFile/CollisionMeshFile.cpp
 /home/runner/work/RocketSim/RocketSim/src/Math/Math.cpp
 /home/runner/work/RocketSim/RocketSim/src/Math/MathTypes/MathTypes.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/Arena/Arena.cpp
+/home/runner/work/RocketSim/RocketSim/src/Sim/Arena/ArenaConfig/ArenaConfig.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/Ball/Ball.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/BallHitInfo/BallHitInfo.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/BallPredTracker/BallPredTracker.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/BoostPad/BoostPad.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/Car/Car.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/Car/CarConfig/CarConfig.cpp
@@ -132,14 +138,17 @@
 RocketSim.egg-info/top_level.txt
 libsrc/bullet3-3.24/LICENSE.txt
 libsrc/bullet3-3.24/MANIFEST.in
 libsrc/bullet3-3.24/README.md
 libsrc/bullet3-3.24/VERSION
 libsrc/bullet3-3.24/btBulletCollisionCommon.h
 libsrc/bullet3-3.24/btBulletDynamicsCommon.h
+libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btAxisSweep3.cpp
+libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btAxisSweep3.h
+libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btAxisSweep3Internal.h
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h
@@ -147,14 +156,18 @@
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp
 libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h
+libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btRSBroadphase.cpp
+libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btRSBroadphase.h
+libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btSimpleBroadphase.cpp
+libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btSimpleBroadphase.h
 libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp
 libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h
 libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp
 libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h
 libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp
 libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h
 libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp
@@ -344,18 +357,20 @@
 libsrc/bullet3-3.24/LinearMath/btVector3.h
 libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp
 libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h
 libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp
 libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp
 python-mtheall/Angle.cpp
 python-mtheall/Arena.cpp
+python-mtheall/ArenaConfig.cpp
 python-mtheall/Array.cpp
 python-mtheall/Array.h
 python-mtheall/Ball.cpp
 python-mtheall/BallHitInfo.cpp
+python-mtheall/BallPredictor.cpp
 python-mtheall/BallState.cpp
 python-mtheall/BoostPad.cpp
 python-mtheall/BoostPadState.cpp
 python-mtheall/Car.cpp
 python-mtheall/CarConfig.cpp
 python-mtheall/CarControls.cpp
 python-mtheall/CarState.cpp
@@ -390,14 +405,16 @@
 src/Math/MathTypes/MathTypes.cpp
 src/Math/MathTypes/MathTypes.h
 src/Sim/CarControls.h
 src/Sim/CollisionMasks.h
 src/Sim/GameMode.h
 src/Sim/Arena/Arena.cpp
 src/Sim/Arena/Arena.h
+src/Sim/Arena/ArenaConfig/ArenaConfig.cpp
+src/Sim/Arena/ArenaConfig/ArenaConfig.h
 src/Sim/Ball/Ball.cpp
 src/Sim/Ball/Ball.h
 src/Sim/BallHitInfo/BallHitInfo.cpp
 src/Sim/BallHitInfo/BallHitInfo.h
 src/Sim/BallPredTracker/BallPredTracker.cpp
 src/Sim/BallPredTracker/BallPredTracker.h
 src/Sim/BoostPad/BoostPad.cpp
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 ///The btBroadphaseInterface class provides an interface to detect aabb-overlapping object pairs.
 ///Some implementations for this broadphase interface include btAxisSweep3, bt32BitAxisSweep3 and btDbvtBroadphase.
 ///The actual overlapping pair management, storage, adding and removing of pairs is dealt by the btOverlappingPairCache class.
 class btBroadphaseInterface
 {
 public:
+
 	virtual ~btBroadphaseInterface() {}
 
 	virtual btBroadphaseProxy* createProxy(const btVector3& aabbMin, const btVector3& aabbMax, int shapeType, void* userPtr, int collisionFilterGroup, int collisionFilterMask, btCollisionDispatcher* dispatcher) = 0;
 	virtual void destroyProxy(btBroadphaseProxy* proxy, btCollisionDispatcher* dispatcher) = 0;
 	virtual void setAabb(btBroadphaseProxy* proxy, const btVector3& aabbMin, const btVector3& aabbMax, btCollisionDispatcher* dispatcher) = 0;
 	virtual void getAabb(btBroadphaseProxy* proxy, btVector3& aabbMin, btVector3& aabbMax) const = 0;
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 2. Altered source versions must be plainly marked as such, and must not be misrepresented as being the original software.
 3. This notice may not be removed or altered from any source distribution.
 */
 
 #include "btCollisionObject.h"
 #include "../BroadphaseCollision/btBroadphaseProxy.h"
 
+#include "../CollisionShapes/btCollisionShape.h"
+
 btCollisionObject::btCollisionObject()
 	: m_interpolationLinearVelocity(0.f, 0.f, 0.f),
 	  m_interpolationAngularVelocity(0.f, 0.f, 0.f),
 	  m_anisotropicFriction(1.f, 1.f, 1.f),
 	  m_hasAnisotropicFriction(false),
 	  m_contactProcessingThreshold(BT_LARGE_FLOAT),
 	  m_broadphaseHandle(0),
@@ -71,8 +73,15 @@
 void btCollisionObject::activate(bool forceActivation) const
 {
 	if (forceActivation || !(m_collisionFlags & (CF_STATIC_OBJECT | CF_KINEMATIC_OBJECT)))
 	{
 		setActivationState(ACTIVE_TAG);
 		m_deactivationTime = btScalar(0.);
 	}
+}
+
+void btCollisionObject::setWorldTransform(const btTransform& worldTrans) {
+	m_updateRevision++;
+	m_worldTransform = worldTrans;
+	if (m_collisionShape)
+		m_collisionShape->m_aabbCached = false;
 }
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,18 @@
 
 /// btCollisionObject can be used to manage collision detection objects.
 /// btCollisionObject maintains all information that is needed for a collision detection: Shape, Transform and AABB proxy.
 /// They can be added to the btCollisionWorld.
 ATTRIBUTE_ALIGNED16(class)
 btCollisionObject
 {
-public:
+private:
 	btTransform m_worldTransform;
 
+public:
 	///m_interpolationWorldTransform is used for CCD and interpolation
 	///it can be either previous or future (predicted) transform
 	btTransform m_interpolationWorldTransform;
 	//those two are experimental: just added for bullet time effect, so you can still apply impulses (directly modifying velocities)
 	//without destroying the continuous interpolated motion (which uses this interpolation velocities)
 	btVector3 m_interpolationLinearVelocity;
 	btVector3 m_interpolationAngularVelocity;
@@ -86,14 +87,17 @@
 	btScalar m_friction;
 	btScalar m_restitution;
 	btScalar m_rollingFriction;   //torsional friction orthogonal to contact normal (useful to stop spheres rolling forever)
 	btScalar m_spinningFriction;  // torsional friction around the contact normal (useful for grasping)
 	btScalar m_contactDamping;
 	btScalar m_contactStiffness;
 
+	// Rotation updates will be skipped
+	int m_noRot = false;
+
 	///m_internalType is reserved to distinguish Bullet's btCollisionObject, btRigidBody, btSoftBody, btGhostObject etc.
 	///do not assign your own m_internalType unless you write a new dynamics object class.
 	int m_internalType;
 
 	///users can point to their objects, m_userPointer is not used by Bullet, see setUserPointer/getUserPointer
 
 	void* m_userObjectPointer;
@@ -393,19 +397,15 @@
 	}
 
 	const btTransform& getWorldTransform() const
 	{
 		return m_worldTransform;
 	}
 
-	void setWorldTransform(const btTransform& worldTrans)
-	{
-		m_updateRevision++;
-		m_worldTransform = worldTrans;
-	}
+	void setWorldTransform(const btTransform& worldTrans);
 
 	SIMD_FORCE_INLINE btBroadphaseProxy* getBroadphaseHandle()
 	{
 		return m_broadphaseHandle;
 	}
 
 	SIMD_FORCE_INLINE const btBroadphaseProxy* getBroadphaseHandle() const
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -100,30 +100,30 @@
 
 	btConvexShape* convexShape = (btConvexShape*)convexObjWrap->getCollisionShape();
 	btStaticPlaneShape* planeShape = (btStaticPlaneShape*)planeObjWrap->getCollisionShape();
 
 	bool hasCollision = false;
 	const btVector3& planeNormal = planeShape->getPlaneNormal();
 	const btScalar& planeConstant = planeShape->getPlaneConstant();
+
 	btTransform planeInConvex;
-	planeInConvex = convexObjWrap->getWorldTransform().inverse() * planeObjWrap->getWorldTransform();
 	btTransform convexInPlaneTrans;
+	planeInConvex = convexObjWrap->getWorldTransform().inverse() * planeObjWrap->getWorldTransform();
 	convexInPlaneTrans = planeObjWrap->getWorldTransform().inverse() * convexObjWrap->getWorldTransform();
 
 	btVector3 vtx = convexShape->localGetSupportingVertex(planeInConvex.getBasis() * -planeNormal);
 	btVector3 vtxInPlane = convexInPlaneTrans(vtx);
 	btScalar distance = (planeNormal.dot(vtxInPlane) - planeConstant);
-
-	btVector3 vtxInPlaneProjected = vtxInPlane - distance * planeNormal;
-	btVector3 vtxInPlaneWorld = planeObjWrap->getWorldTransform() * vtxInPlaneProjected;
-
 	hasCollision = distance < m_manifoldPtr->getContactBreakingThreshold()+ resultOut->m_closestPointDistanceThreshold;
 	resultOut->setPersistentManifold(m_manifoldPtr);
 	if (hasCollision)
 	{
+		btVector3 vtxInPlaneProjected = vtxInPlane - distance * planeNormal;
+		btVector3 vtxInPlaneWorld = planeObjWrap->getWorldTransform() * vtxInPlaneProjected;
+
 		/// report a contact. internally this will be kept persistent, and contact reduction is done
 		btVector3 normalOnSurfaceB = planeObjWrap->getWorldTransform().getBasis() * planeNormal;
 		btVector3 pOnB = vtxInPlaneWorld;
 		resultOut->addContactPoint(normalOnSurfaceB, pOnB, distance);
 	}
 
 	//the perturbation algorithm doesn't work well with implicit surfaces such as spheres, cylinder and cones:
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /*
 Bullet Continuous Collision Detection and Physics Library
 Copyright (c) 2003-2009 Erwin Coumans  http://bulletphysics.org
 
 This software is provided 'as-is', without any express or implied warranty.
 In no event will the authors be held liable for any damages arising from the use of this software.
-Permission is granted to anyone to use this software for any purpose, 
-including commercial applications, and to alter it and redistribute it freely, 
+Permission is granted to anyone to use this software for any purpose,
+including commercial applications, and to alter it and redistribute it freely,
 subject to the following restrictions:
 
 1. The origin of this software must not be misrepresented; you must not claim that you wrote the original software. If you use this software in a product, an acknowledgment in the product documentation would be appreciated but is not required.
 2. Altered source versions must be plainly marked as such, and must not be misrepresented as being the original software.
 3. This notice may not be removed or altered from any source distribution.
 */
 #include "../CollisionShapes/btCollisionShape.h"
@@ -31,31 +31,61 @@
 {
 	void btBulletCollisionProbe();
 
 	void btBulletCollisionProbe() {}
 }
 
 void btCollisionShape::getAabb(const btTransform& t, btVector3& aabbMin, btVector3& aabbMax) const {
-	switch (m_shapeType) {
-	case BOX_SHAPE_PROXYTYPE:
-		return ((btBoxShape*)this)->getAabb(t, aabbMin, aabbMax);
-	case TRIANGLE_SHAPE_PROXYTYPE:
-		return ((btTriangleShape*)this)->getAabb(t, aabbMin, aabbMax);
-	case SPHERE_SHAPE_PROXYTYPE:
+
+	// If we're a sphere, its faster to just re-calculate
+	if (m_shapeType == SPHERE_SHAPE_PROXYTYPE)
 		return ((btSphereShape*)this)->getAabb(t, aabbMin, aabbMax);
-	case STATIC_PLANE_PROXYTYPE:
-		return ((btStaticPlaneShape*)this)->getAabb(t, aabbMin, aabbMax);
-	case TRIANGLE_MESH_SHAPE_PROXYTYPE:
-		return ((btTriangleMeshShape*)this)->getAabb(t, aabbMin, aabbMax);
-	case COMPOUND_SHAPE_PROXYTYPE:
-		return ((btCompoundShape*)this)->getAabb(t, aabbMin, aabbMax);
-	case CONVEX_HULL_SHAPE_PROXYTYPE:
-		return ((btConvexHullShape*)this)->getAabb(t, aabbMin, aabbMax);
-	default:
-		btAssert(false);
+
+	constexpr auto fnFastCompareTransforms = [](const btTransform& a, const btTransform& b) -> bool {
+		return
+			(a.m_origin == b.m_origin) &&
+			(a.m_basis[0] == b.m_basis[0]) &&
+			(a.m_basis[1] == b.m_basis[1]);
+			// Don't need to compare the last row of the basis
+	};
+
+	if (!fnFastCompareTransforms(t, m_aabbCacheTrans) || !m_aabbCached) {
+		switch (m_shapeType) {
+		case BOX_SHAPE_PROXYTYPE:
+			((btBoxShape*)this)->getAabb(t, aabbMin, aabbMax);
+			break;
+		case TRIANGLE_SHAPE_PROXYTYPE:
+			((btTriangleShape*)this)->getAabb(t, aabbMin, aabbMax);
+			break;
+		case SPHERE_SHAPE_PROXYTYPE:
+			((btSphereShape*)this)->getAabb(t, aabbMin, aabbMax);
+			break;
+		case STATIC_PLANE_PROXYTYPE:
+			((btStaticPlaneShape*)this)->getAabb(t, aabbMin, aabbMax);
+			break;
+		case TRIANGLE_MESH_SHAPE_PROXYTYPE:
+			((btTriangleMeshShape*)this)->getAabb(t, aabbMin, aabbMax);
+			break;
+		case COMPOUND_SHAPE_PROXYTYPE:
+			((btCompoundShape*)this)->getAabb(t, aabbMin, aabbMax);
+			break;
+		case CONVEX_HULL_SHAPE_PROXYTYPE:
+			((btConvexHullShape*)this)->getAabb(t, aabbMin, aabbMax);
+			break;
+		default:
+			btAssert(false);
+		}
+
+		m_aabbCached = true;
+		m_aabbMinCache = aabbMin;
+		m_aabbMaxCache = aabbMax;
+		m_aabbCacheTrans = t;
+	} else {
+		aabbMin = m_aabbMinCache;
+		aabbMax = m_aabbMaxCache;
 	}
 }
 
 btScalar btCollisionShape::getMargin() const {
 	switch (m_shapeType) {
 	case BOX_SHAPE_PROXYTYPE:
 		return ((btBoxShape*)this)->getMargin();
@@ -91,16 +121,15 @@
 	case COMPOUND_SHAPE_PROXYTYPE:
 		return ((btCompoundShape*)this)->setMargin(margin);
 	default:
 		btAssert(false);
 	}
 }
 
-void btCollisionShape::getBoundingSphere(btVector3& center, btScalar& radius) const
-{
+void btCollisionShape::getBoundingSphere(btVector3& center, btScalar& radius) const {
 	switch (m_shapeType) {
 	case SPHERE_SHAPE_PROXYTYPE:
 		center = btVector3(0, 0, 0);
 		radius = ((btSphereShape*)this)->getRadius() + 0.08;
 		break;
 	default:
 		btTransform tr;
@@ -110,31 +139,28 @@
 		getAabb(tr, aabbMin, aabbMax);
 
 		radius = (aabbMax - aabbMin).length() * btScalar(0.5);
 		center = (aabbMin + aabbMax) * btScalar(0.5);
 	}
 }
 
-btScalar btCollisionShape::getContactBreakingThreshold(btScalar defaultContactThreshold) const
-{
+btScalar btCollisionShape::getContactBreakingThreshold(btScalar defaultContactThreshold) const {
 	return getAngularMotionDisc() * defaultContactThreshold;
 }
 
-btScalar btCollisionShape::getAngularMotionDisc() const
-{
+btScalar btCollisionShape::getAngularMotionDisc() const {
 	///@todo cache this value, to improve performance
 	btVector3 center;
 	btScalar disc;
 	getBoundingSphere(center, disc);
 	disc += (center).length();
 	return disc;
 }
 
-void btCollisionShape::calculateTemporalAabb(const btTransform& curTrans, const btVector3& linvel, const btVector3& angvel, btScalar timeStep, btVector3& temporalAabbMin, btVector3& temporalAabbMax) const
-{
+void btCollisionShape::calculateTemporalAabb(const btTransform& curTrans, const btVector3& linvel, const btVector3& angvel, btScalar timeStep, btVector3& temporalAabbMin, btVector3& temporalAabbMax) const {
 	//start with static aabb
 	getAabb(curTrans, temporalAabbMin, temporalAabbMax);
 
 	btScalar temporalAabbMaxx = temporalAabbMax.getX();
 	btScalar temporalAabbMaxy = temporalAabbMax.getY();
 	btScalar temporalAabbMaxz = temporalAabbMax.getZ();
 	btScalar temporalAabbMinx = temporalAabbMin.getX();
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h`

 * *Files 12% similar despite different names*

```diff
@@ -21,24 +21,29 @@
 #include "../../LinearMath/btMatrix3x3.h"
 #include "../BroadphaseCollision/btBroadphaseProxy.h"  //for the shape types
 
 ///The btCollisionShape class provides an interface for collision shapes that can be shared among btCollisionObjects.
 ATTRIBUTE_ALIGNED16(class)
 btCollisionShape
 {
-protected:
+public:
+
 	int m_shapeType;
 	void* m_userPointer;
 	int m_userIndex;
 	int m_userIndex2;
 
-public:
+	mutable bool m_aabbCached = false;
+	mutable btVector3 m_aabbMinCache, m_aabbMaxCache;
+	mutable btTransform m_aabbCacheTrans;
+
 	BT_DECLARE_ALIGNED_ALLOCATOR();
 
-	btCollisionShape() : m_shapeType(INVALID_SHAPE_PROXYTYPE), m_userPointer(0), m_userIndex(-1), m_userIndex2(-1)
+	btCollisionShape() : 
+		m_shapeType(INVALID_SHAPE_PROXYTYPE), m_userPointer(0), m_userIndex(-1), m_userIndex2(-1)
 	{
 	}
 
 	virtual ~btCollisionShape()
 	{
 	}
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -32,25 +32,24 @@
 	{
 		supportVerticesOut[i].setValue(btScalar(0.), btScalar(0.), btScalar(0.));
 	}
 }
 
 btVector3 btSphereShape::localGetSupportingVertex(const btVector3& vec) const
 {
-	btVector3 supVertex;
-	supVertex = localGetSupportingVertexWithoutMargin(vec);
-
 	btVector3 vecnorm = vec;
 	if (vecnorm.length2() < (SIMD_EPSILON * SIMD_EPSILON))
 	{
-		vecnorm.setValue(btScalar(-1.), btScalar(-1.), btScalar(-1.));
+		static thread_local btVector3 invalidVecNorm = btVector3(-1, -1, -1).normalized();
+		vecnorm = invalidVecNorm;
+	} else {
+		vecnorm.normalize();
 	}
-	vecnorm.normalize();
-	supVertex += getMargin() * vecnorm;
-	return supVertex;
+
+	return getMargin() * vecnorm;
 }
 
 //broken due to scaling
 void btSphereShape::getAabb(const btTransform& t, btVector3& aabbMin, btVector3& aabbMax) const
 {
 	const btVector3& center = t.getOrigin();
 	btScalar margin = getMargin() + 0.08f;
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,73 @@
 /*
 Bullet Continuous Collision Detection and Physics Library
-Copyright (c) 2003-2009 Erwin Coumans  http://bulletphysics.org
+Copyright (c) 2010 Erwin Coumans  http://bulletphysics.org
 
 This software is provided 'as-is', without any express or implied warranty.
 In no event will the authors be held liable for any damages arising from the use of this software.
 Permission is granted to anyone to use this software for any purpose, 
 including commercial applications, and to alter it and redistribute it freely, 
 subject to the following restrictions:
 
 1. The origin of this software must not be misrepresented; you must not claim that you wrote the original software. If you use this software in a product, an acknowledgment in the product documentation would be appreciated but is not required.
 2. Altered source versions must be plainly marked as such, and must not be misrepresented as being the original software.
 3. This notice may not be removed or altered from any source distribution.
 */
 
-#include "btStaticPlaneShape.h"
+#ifndef _BT_TRIANGLE_INFO_MAP_H
+#define _BT_TRIANGLE_INFO_MAP_H
 
-#include "../../LinearMath/btTransformUtil.h"
+#include "../../LinearMath/btHashMap.h"
 
-btStaticPlaneShape::btStaticPlaneShape(const btVector3& planeNormal, btScalar planeConstant)
-	: btConcaveShape(), m_planeNormal(planeNormal.normalized()), m_planeConstant(planeConstant)
+///for btTriangleInfo m_flags
+#define TRI_INFO_V0V1_CONVEX 1
+#define TRI_INFO_V1V2_CONVEX 2
+#define TRI_INFO_V2V0_CONVEX 4
+
+#define TRI_INFO_V0V1_SWAP_NORMALB 8
+#define TRI_INFO_V1V2_SWAP_NORMALB 16
+#define TRI_INFO_V2V0_SWAP_NORMALB 32
+
+///The btTriangleInfo structure stores information to adjust collision normals to avoid collisions against internal edges
+///it can be generated using
+struct btTriangleInfo
 {
-	m_shapeType = STATIC_PLANE_PROXYTYPE;
-	//	btAssert( btFuzzyZero(m_planeNormal.length() - btScalar(1.)) );
-}
+	btTriangleInfo()
+	{
+		m_edgeV0V1Angle = SIMD_2_PI;
+		m_edgeV1V2Angle = SIMD_2_PI;
+		m_edgeV2V0Angle = SIMD_2_PI;
+		m_flags = 0;
+	}
+
+	int m_flags;
+
+	btScalar m_edgeV0V1Angle;
+	btScalar m_edgeV1V2Angle;
+	btScalar m_edgeV2V0Angle;
+};
 
-btStaticPlaneShape::~btStaticPlaneShape()
-{
-}
-
-void btStaticPlaneShape::getAabb(const btTransform& t, btVector3& aabbMin, btVector3& aabbMax) const
-{
-	(void)t;
-	/*
-	btVector3 infvec (btScalar(BT_LARGE_FLOAT),btScalar(BT_LARGE_FLOAT),btScalar(BT_LARGE_FLOAT));
-
-	btVector3 center = m_planeNormal*m_planeConstant;
-	aabbMin = center + infvec*m_planeNormal;
-	aabbMax = aabbMin;
-	aabbMin.setMin(center - infvec*m_planeNormal);
-	aabbMax.setMax(center - infvec*m_planeNormal); 
-	*/
-
-	aabbMin.setValue(btScalar(-BT_LARGE_FLOAT), btScalar(-BT_LARGE_FLOAT), btScalar(-BT_LARGE_FLOAT));
-	aabbMax.setValue(btScalar(BT_LARGE_FLOAT), btScalar(BT_LARGE_FLOAT), btScalar(BT_LARGE_FLOAT));
-}
-
-void btStaticPlaneShape::processAllTriangles(btTriangleCallback* callback, const btVector3& aabbMin, const btVector3& aabbMax) const
-{
-	btVector3 halfExtents = (aabbMax - aabbMin) * btScalar(0.5);
-	btScalar radius = halfExtents.length();
-	btVector3 center = (aabbMax + aabbMin) * btScalar(0.5);
-
-	//this is where the triangles are generated, given AABB and plane equation (normal/constant)
-
-	btVector3 tangentDir0, tangentDir1;
+typedef btHashMap<btHashInt, btTriangleInfo> btInternalTriangleInfoMap;
 
-	//tangentDir0/tangentDir1 can be precalculated
-	btPlaneSpace1(m_planeNormal, tangentDir0, tangentDir1);
-
-	btVector3 projectedCenter = center - (m_planeNormal.dot(center) - m_planeConstant) * m_planeNormal;
-
-	btVector3 triangle[3];
-	triangle[0] = projectedCenter + tangentDir0 * radius + tangentDir1 * radius;
-	triangle[1] = projectedCenter + tangentDir0 * radius - tangentDir1 * radius;
-	triangle[2] = projectedCenter - tangentDir0 * radius - tangentDir1 * radius;
-
-	callback->processTriangle(triangle, 0, 0);
-
-	triangle[0] = projectedCenter - tangentDir0 * radius - tangentDir1 * radius;
-	triangle[1] = projectedCenter - tangentDir0 * radius + tangentDir1 * radius;
-	triangle[2] = projectedCenter + tangentDir0 * radius + tangentDir1 * radius;
-
-	callback->processTriangle(triangle, 0, 1);
-}
-
-void btStaticPlaneShape::calculateLocalInertia(btScalar mass, btVector3& inertia) const
+///The btTriangleInfoMap stores edge angle information for some triangles. You can compute this information yourself or using btGenerateInternalEdgeInfo.
+struct btTriangleInfoMap : public btInternalTriangleInfoMap
 {
-	(void)mass;
-
-	//moving concave objects not supported
+	btScalar m_convexEpsilon;          ///used to determine if an edge or contact normal is convex, using the dot product
+	btScalar m_planarEpsilon;          ///used to determine if a triangle edge is planar with zero angle
+	btScalar m_equalVertexThreshold;   ///used to compute connectivity: if the distance between two vertices is smaller than m_equalVertexThreshold, they are considered to be 'shared'
+	btScalar m_edgeDistanceThreshold;  ///used to determine edge contacts: if the closest distance between a contact point and an edge is smaller than this distance threshold it is considered to "hit the edge"
+	btScalar m_maxEdgeAngleThreshold;  //ignore edges that connect triangles at an angle larger than this m_maxEdgeAngleThreshold
+	btScalar m_zeroAreaThreshold;      ///used to determine if a triangle is degenerate (length squared of cross product of 2 triangle edges < threshold)
+
+	btTriangleInfoMap()
+	{
+		m_convexEpsilon = 0.00f;
+		m_planarEpsilon = 0.0001f;
+		m_equalVertexThreshold = btScalar(0.0001) * btScalar(0.0001);
+		m_edgeDistanceThreshold = btScalar(0.1);
+		m_zeroAreaThreshold = btScalar(0.0001) * btScalar(0.0001);
+		m_maxEdgeAngleThreshold = SIMD_2_PI;
+	}
+	virtual ~btTriangleInfoMap() {}
+};
 
-	inertia.setValue(btScalar(0.), btScalar(0.), btScalar(0.));
-}
+#endif
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,25 @@
 
 #include "btConcaveShape.h"
 
 ///The btStaticPlaneShape simulates an infinite non-moving (static) collision plane.
 ATTRIBUTE_ALIGNED16(class)
 btStaticPlaneShape : public btConcaveShape
 {
-protected:
+public:
 	btVector3 m_localAabbMin;
 	btVector3 m_localAabbMax;
 
 	btVector3 m_planeNormal;
 	btScalar m_planeConstant;
+	
+	// Plane only exists along a single axis
+	bool m_isSingleAxis;
+	int m_singleAxisIdx;
+	bool m_singleAxisBackwards;
 
 public:
 	BT_DECLARE_ALIGNED_ALLOCATOR();
 
 	btStaticPlaneShape() {}
 
 	btStaticPlaneShape(const btVector3& planeNormal, btScalar planeConstant);
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #include "btTriangleMeshShape.h"
 #include "../../LinearMath/btVector3.h"
 #include "../../LinearMath/btQuaternion.h"
 #include "btStridingMeshInterface.h"
 #include "../../LinearMath/btAabbUtil2.h"
 #include "../CollisionShapes/btCollisionMargin.h"
 
+#include <cstring>
+
 btTriangleMeshShape::btTriangleMeshShape(btStridingMeshInterface* meshInterface)
 	: btConcaveShape(), m_meshInterface(meshInterface)
 {
 	m_shapeType = TRIANGLE_MESH_SHAPE_PROXYTYPE;
 	if (meshInterface->hasPremadeAabb())
 	{
 		meshInterface->getPremadeAabb(&m_localAabbMin, &m_localAabbMax);
@@ -34,15 +36,15 @@
 	}
 }
 
 btTriangleMeshShape::~btTriangleMeshShape()
 {
 }
 
-void btTriangleMeshShape::getAabb(const btTransform& trans, btVector3& aabbMin, btVector3& aabbMax) const
+void btTriangleMeshShape::getAabb(const btTransform& trans, btVector3& aabbMin, btVector3& aabbMax)
 {
 	btVector3 localHalfExtents = btScalar(0.5) * (m_localAabbMax - m_localAabbMin);
 	localHalfExtents += btVector3(getMargin(), getMargin(), getMargin());
 	btVector3 localCenter = btScalar(0.5) * (m_localAabbMax + m_localAabbMin);
 
 	btMatrix3x3 abs_b = trans.getBasis().absolute();
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 	{
 		btAssert(0);
 		return localGetSupportingVertex(vec);
 	}
 
 	void recalcLocalAabb();
 
-	void getAabb(const btTransform& t, btVector3& aabbMin, btVector3& aabbMax) const;
+	void getAabb(const btTransform& t, btVector3& aabbMin, btVector3& aabbMax);
 
 	void processAllTriangles(btTriangleCallback * callback, const btVector3& aabbMin, const btVector3& aabbMax) const;
 
 	void calculateLocalInertia(btScalar mass, btVector3 & inertia) const;
 
 	btStridingMeshInterface* getMeshInterface()
 	{
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 class btRigidBody;
 #include "../../LinearMath/btVector3.h"
 #include "../../LinearMath/btMatrix3x3.h"
 
 #include "../../LinearMath/btAlignedAllocator.h"
 #include "../../LinearMath/btTransformUtil.h"
 
+#include "../Dynamics/btRigidBody.h"
+
 ///Until we get other contributions, only use SIMD on Windows, when using Visual Studio 2008 or later, and not double precision
 #ifdef BT_USE_SSE
 #define USE_SIMD 1
 #endif  //
 
 #ifdef USE_SIMD
 
@@ -268,16 +270,19 @@
 			m_linearVelocity += m_deltaLinearVelocity;
 			m_angularVelocity += m_deltaAngularVelocity;
 
 			//correct the position/orientation based on push/turn recovery
 			btTransform newTransform;
 			if (m_pushVelocity[0] != 0.f || m_pushVelocity[1] != 0 || m_pushVelocity[2] != 0 || m_turnVelocity[0] != 0.f || m_turnVelocity[1] != 0 || m_turnVelocity[2] != 0)
 			{
-				//	btQuaternion orn = m_worldTransform.getRotation();
-				btTransformUtil::integrateTransform(m_worldTransform, m_pushVelocity, m_turnVelocity * splitImpulseTurnErp, timeStep, newTransform);
+				if (m_originalBody->m_noRot) {
+					btTransformUtil::integrateTransformNoRot(m_worldTransform, m_pushVelocity, m_turnVelocity * splitImpulseTurnErp, timeStep, newTransform);
+				} else {
+					btTransformUtil::integrateTransform(m_worldTransform, m_pushVelocity, m_turnVelocity * splitImpulseTurnErp, timeStep, newTransform);
+				}
 				m_worldTransform = newTransform;
 			}
 			//m_worldTransform.setRotation(orn);
 			//m_originalBody->setCompanionId(-1);
 		}
 	}
 };
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -59,22 +59,22 @@
 	m_additionalDampingFactor = constructionInfo.m_additionalDampingFactor;
 	m_additionalLinearDampingThresholdSqr = constructionInfo.m_additionalLinearDampingThresholdSqr;
 	m_additionalAngularDampingThresholdSqr = constructionInfo.m_additionalAngularDampingThresholdSqr;
 	m_additionalAngularDampingFactor = constructionInfo.m_additionalAngularDampingFactor;
 
 	if (m_optionalMotionState)
 	{
-		m_optionalMotionState->getWorldTransform(m_worldTransform);
+		m_optionalMotionState->getWorldTransform(getWorldTransform());
 	}
 	else
 	{
-		m_worldTransform = constructionInfo.m_startWorldTransform;
+		setWorldTransform(constructionInfo.m_startWorldTransform);
 	}
 
-	m_interpolationWorldTransform = m_worldTransform;
+	m_interpolationWorldTransform = getWorldTransform();
 	m_interpolationLinearVelocity.setValue(0, 0, 0);
 	m_interpolationAngularVelocity.setValue(0, 0, 0);
 
 	//moved to btCollisionObject
 	m_friction = constructionInfo.m_friction;
 	m_rollingFriction = constructionInfo.m_rollingFriction;
 	m_spinningFriction = constructionInfo.m_spinningFriction;
@@ -94,38 +94,43 @@
 	m_invMass = m_inverseMass * m_linearFactor;
 	m_pushVelocity.setZero();
 	m_turnVelocity.setZero();
 }
 
 void btRigidBody::predictIntegratedTransform(btScalar timeStep, btTransform& predictedTransform)
 {
-	btTransformUtil::integrateTransform(m_worldTransform, m_linearVelocity, m_angularVelocity, timeStep, predictedTransform);
+
+	if (m_noRot) {
+		btTransformUtil::integrateTransformNoRot(getWorldTransform(), m_linearVelocity, m_angularVelocity, timeStep, predictedTransform);
+	} else {
+		btTransformUtil::integrateTransform(getWorldTransform(), m_linearVelocity, m_angularVelocity, timeStep, predictedTransform);
+	}
 }
 
 void btRigidBody::saveKinematicState(btScalar timeStep)
 {
 	//todo: clamp to some (user definable) safe minimum timestep, to limit maximum angular/linear velocities
 	if (timeStep != btScalar(0.))
 	{
 		//if we use motionstate to synchronize world transforms, get the new kinematic/animated world transform
 		if (getMotionState())
-			getMotionState()->getWorldTransform(m_worldTransform);
+			getMotionState()->getWorldTransform(getWorldTransform());
 		btVector3 linVel, angVel;
 
-		btTransformUtil::calculateVelocity(m_interpolationWorldTransform, m_worldTransform, timeStep, m_linearVelocity, m_angularVelocity);
+		btTransformUtil::calculateVelocity(m_interpolationWorldTransform, getWorldTransform(), timeStep, m_linearVelocity, m_angularVelocity);
 		m_interpolationLinearVelocity = m_linearVelocity;
 		m_interpolationAngularVelocity = m_angularVelocity;
-		m_interpolationWorldTransform = m_worldTransform;
+		m_interpolationWorldTransform = getWorldTransform();
 		//printf("angular = %f %f %f\n",m_angularVelocity.getX(),m_angularVelocity.getY(),m_angularVelocity.getZ());
 	}
 }
 
 void btRigidBody::getAabb(btVector3& aabbMin, btVector3& aabbMax) const
 {
-	getCollisionShape()->getAabb(m_worldTransform, aabbMin, aabbMax);
+	getCollisionShape()->getAabb(getWorldTransform(), aabbMin, aabbMax);
 }
 
 void btRigidBody::setGravity(const btVector3& acceleration)
 {
 	if (m_inverseMass != btScalar(0.0))
 	{
 		m_gravity = acceleration * (btScalar(1.0) / m_inverseMass);
@@ -243,15 +248,15 @@
 							   inertia.z() != btScalar(0.0) ? btScalar(1.0) / inertia.z() : btScalar(0.0));
 
 	m_invMass = m_linearFactor * m_inverseMass;
 }
 
 void btRigidBody::updateInertiaTensor()
 {
-	m_invInertiaTensorWorld = m_worldTransform.getBasis().scaled(m_invInertiaLocal) * m_worldTransform.getBasis().transpose();
+	m_invInertiaTensorWorld = getWorldTransform().getBasis().scaled(m_invInertiaLocal) * getWorldTransform().getBasis().transpose();
 }
 
 btVector3 btRigidBody::getLocalInertia() const
 {
 	btVector3 inertiaLocal;
 	const btVector3 inertia = m_invInertiaLocal;
 	inertiaLocal.setValue(inertia.x() != btScalar(0.0) ? btScalar(1.0) / inertia.x() : btScalar(0.0),
@@ -338,16 +343,16 @@
 	// calculate using implicit euler step so it's stable.
 
 	const btVector3 inertiaLocal = getLocalInertia();
 	const btVector3 w0 = getAngularVelocity();
 
 	btMatrix3x3 I;
 
-	I = m_worldTransform.getBasis().scaled(inertiaLocal) *
-		m_worldTransform.getBasis().transpose();
+	I = getWorldTransform().getBasis().scaled(inertiaLocal) *
+		getWorldTransform().getBasis().transpose();
 
 	// use newtons method to find implicit solution for new angular velocity (w')
 	// f(w') = -(T*step + Iw) + Iw' + w' + w'xIw'*step = 0
 	// df/dw' = I + 1xIw'*step + w'xI*step
 
 	btVector3 w1 = w0;
 
@@ -387,31 +392,31 @@
 	clampVelocity(m_angularVelocity);
 	#endif
 }
 
 btQuaternion btRigidBody::getOrientation() const
 {
 	btQuaternion orn;
-	m_worldTransform.getBasis().getRotation(orn);
+	getWorldTransform().getBasis().getRotation(orn);
 	return orn;
 }
 
 void btRigidBody::setCenterOfMassTransform(const btTransform& xform)
 {
 	if (isKinematicObject())
 	{
-		m_interpolationWorldTransform = m_worldTransform;
+		m_interpolationWorldTransform = getWorldTransform();
 	}
 	else
 	{
 		m_interpolationWorldTransform = xform;
 	}
 	m_interpolationLinearVelocity = getLinearVelocity();
 	m_interpolationAngularVelocity = getAngularVelocity();
-	m_worldTransform = xform;
+	setWorldTransform(xform);
 	updateInertiaTensor();
 }
 
 void btRigidBody::addConstraintRef(btTypedConstraint* c)
 {
 	///disable collision with the 'other' body
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h`

 * *Files 1% similar despite different names*

```diff
@@ -427,21 +427,21 @@
 		m_totalTorque.setValue(btScalar(0.0), btScalar(0.0), btScalar(0.0));
 	}
 
 	void updateInertiaTensor();
 
 	const btVector3& getCenterOfMassPosition() const
 	{
-		return m_worldTransform.getOrigin();
+		return getWorldTransform().getOrigin();
 	}
 	btQuaternion getOrientation() const;
 
 	const btTransform& getCenterOfMassTransform() const
 	{
-		return m_worldTransform;
+		return getWorldTransform();
 	}
 	const btVector3& getLinearVelocity() const
 	{
 		return m_linearVelocity;
 	}
 	const btVector3& getAngularVelocity() const
 	{
@@ -481,15 +481,17 @@
     {
         //we also calculate lin/ang velocity for kinematic objects
         return m_pushVelocity + m_turnVelocity.cross(rel_pos);
     }
 
 	void translate(const btVector3& v)
 	{
-		m_worldTransform.getOrigin() += v;
+		btTransform newWorldTransform = getWorldTransform();
+		newWorldTransform.getOrigin() += v;
+		setWorldTransform(newWorldTransform);
 	}
 
 	void getAabb(btVector3& aabbMin, btVector3& aabbMax) const;
 
 	SIMD_FORCE_INLINE btScalar computeImpulseDenominator(const btVector3& pos, const btVector3& normal) const
 	{
 		btVector3 r0 = pos - getCenterOfMassPosition();
@@ -565,15 +567,15 @@
 	{
 		return m_optionalMotionState;
 	}
 	void setMotionState(btMotionState* motionState)
 	{
 		m_optionalMotionState = motionState;
 		if (m_optionalMotionState)
-			motionState->getWorldTransform(m_worldTransform);
+			motionState->getWorldTransform(getWorldTransform());
 	}
 
 	//for experimental overriding of friction/contact solver func
 	int m_contactSolverType;
 	int m_frictionSolverType;
 
 	void setAngularFactor(const btVector3& angFac)
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LICENSE.txt` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h`

 * *Files 3% similar despite different names*

```diff
@@ -54,22 +54,22 @@
 SIMD_FORCE_INLINE bool TestTriangleAgainstAabb2(const btVector3* vertices,
 												const btVector3& aabbMin, const btVector3& aabbMax)
 {
 	const btVector3& p1 = vertices[0];
 	const btVector3& p2 = vertices[1];
 	const btVector3& p3 = vertices[2];
 
-	if (btMin(btMin(p1[0], p2[0]), p3[0]) > aabbMax[0]) return false;
-	if (btMax(btMax(p1[0], p2[0]), p3[0]) < aabbMin[0]) return false;
+	// First check Z, then X, then Y
+	constexpr int INDEX_ORDER[] = { 2, 0, 1 };
 
-	if (btMin(btMin(p1[2], p2[2]), p3[2]) > aabbMax[2]) return false;
-	if (btMax(btMax(p1[2], p2[2]), p3[2]) < aabbMin[2]) return false;
-
-	if (btMin(btMin(p1[1], p2[1]), p3[1]) > aabbMax[1]) return false;
-	if (btMax(btMax(p1[1], p2[1]), p3[1]) < aabbMin[1]) return false;
+	for (int i : INDEX_ORDER) {
+		if (btMin(btMin(p1[i], p2[i]), p3[i]) > aabbMax[i]) return false;
+		if (btMax(btMax(p1[i], p2[i]), p3[i]) < aabbMin[i]) return false;
+	}
+	
 	return true;
 }
 
 SIMD_FORCE_INLINE int btOutcode(const btVector3& p, const btVector3& halfExtent)
 {
 	return (p.getX() < -halfExtent.getX() ? 0x01 : 0x0) |
 		   (p.getX() > halfExtent.getX() ? 0x08 : 0x0) |
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHull.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btConvexHull.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btHashMap.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btHashMap.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btList.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btList.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h`

 * *Files 1% similar despite different names*

```diff
@@ -799,14 +799,23 @@
 	* @param c1 The second column to use for calculating the cofactor
 	* See http://en.wikipedia.org/wiki/Cofactor_(linear_algebra) for more details
 	*/
 	btScalar cofac(int r1, int c1, int r2, int c2) const
 	{
 		return m_el[r1][c1] * m_el[r2][c2] - m_el[r1][c2] * m_el[r2][c1];
 	}
+
+	friend std::ostream& operator<<(std::ostream& stream, const btMatrix3x3& mat) {
+		stream << "(" << std::endl;
+		stream << "  " << mat[0] << "," << std::endl;
+		stream << "  " << mat[1] << "," << std::endl;
+		stream << "  " << mat[2] << std::endl;
+		stream << ")";
+		return stream;
+	}
 };
 
 SIMD_FORCE_INLINE btMatrix3x3&
 btMatrix3x3::operator*=(const btMatrix3x3& m)
 {
 #if defined BT_USE_SIMD_VECTOR3 && defined(BT_USE_SSE_IN_API) && defined(BT_USE_SSE)
 	__m128 rv00, rv01, rv02;
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMatrixX.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btMatrixX.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMinMax.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btMinMax.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMotionState.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btMotionState.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuadWord.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btQuadWord.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuaternion.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btQuaternion.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuickprof.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btQuickprof.h`

 * *Files 1% similar despite different names*

```diff
@@ -191,10 +191,11 @@
 {
 public:
 	CProfileSample(const char* name);
 
 	~CProfileSample(void);
 };
 
-#define BT_PROFILE(name) CProfileSample __profile(name)
+//#define BT_PROFILE(name) CProfileSample __profile(name)
+#define BT_PROFILE(name)
 
 #endif  //BT_QUICK_PROF_H
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btRandom.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btRandom.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btReducedVector.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btReducedVector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btScalar.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btScalar.h`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 //Aligned data types not supported in managed code
 #pragma unmanaged
 #endif
 
 #include <math.h>
 #include <stdlib.h>  //size_t for MSVC 6.0
 #include <float.h>
+#include <iostream>
 
 /* SVN $Revision$ on $Date$ from http://bullet.googlecode.com*/
 #define BT_BULLET_VERSION 324
 
 inline int btGetVersion()
 {
 	return BT_BULLET_VERSION;
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btSerializer.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btThreads.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btThreads.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btThreads.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btThreads.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btTransform.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btTransform.h`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,19 @@
 
 	/**@brief Return an identity transform */
 	static const btTransform& getIdentity()
 	{
 		static const btTransform identityTransform(btMatrix3x3::getIdentity());
 		return identityTransform;
 	}
+
+	friend std::ostream& operator<<(std::ostream& stream, const btTransform& trans) {
+		stream << "[" << trans.getBasis() << ", " << trans.getOrigin() << "]";
+		return stream;
+	}
 };
 
 SIMD_FORCE_INLINE btVector3
 btTransform::invXform(const btVector3& inVec) const
 {
 	btVector3 v = inVec - m_origin;
 	return (m_basis.transpose() * v);
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 					 supportDir.z() < btScalar(0.0) ? -halfExtents.z() : halfExtents.z());
 }
 
 /// Utils related to temporal transforms
 class btTransformUtil
 {
 public:
+	static void integrateTransformNoRot(const btTransform& curTrans, const btVector3& linvel, const btVector3& angvel, btScalar timeStep, btTransform& predictedTransform) {
+		predictedTransform.setOrigin(curTrans.getOrigin() + linvel * timeStep);
+		predictedTransform.setBasis(curTrans.getBasis());
+	}
+
 	static void integrateTransform(const btTransform& curTrans, const btVector3& linvel, const btVector3& angvel, btScalar timeStep, btTransform& predictedTransform)
 	{
 		predictedTransform.setOrigin(curTrans.getOrigin() + linvel * timeStep);
 		//	#define QUATERNION_DERIVATIVE
 #ifdef QUATERNION_DERIVATIVE
 		btQuaternion predictedOrn = curTrans.getRotation();
 		predictedOrn += (angvel * predictedOrn) * (timeStep * btScalar(0.5));
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btVector3.cpp` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btVector3.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btVector3.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/LinearMath/btVector3.h`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #ifndef BT_VECTOR3_H
 #define BT_VECTOR3_H
 
 //#include <stdint.h>
 #include "btScalar.h"
 #include "btMinMax.h"
 #include "btAlignedAllocator.h"
+#include <sstream>
 
 #ifdef BT_USE_DOUBLE_PRECISION
 #define btVector3Data btVector3DoubleData
 #define btVector3DataName "btVector3DoubleData"
 #else
 #define btVector3Data btVector3FloatData
 #define btVector3DataName "btVector3FloatData"
@@ -746,14 +747,19 @@
 		float32x2_t b0 = vadd_f32(vpadd_f32(vget_low_f32(a0), vget_low_f32(a1)), zLo.val[0]);
 		float32x2_t b1 = vpadd_f32(vpadd_f32(vget_low_f32(a2), vget_high_f32(a2)), vdup_n_f32(0.0f));
 		return btVector3(vcombine_f32(b0, b1));
 #else
 		return btVector3(dot(v0), dot(v1), dot(v2));
 #endif
 	}
+
+	friend std::ostream& operator<<(std::ostream& stream, const btVector3& v) {
+		stream << "[" << v.x() << ", " << v.y() << ", " << v.z() << "]";
+		return stream;
+	}
 };
 
 /**@brief Return the sum of two vectors (Point symantics)*/
 SIMD_FORCE_INLINE btVector3
 operator+(const btVector3& v1, const btVector3& v2)
 {
 #if defined(BT_USE_SSE_IN_API) && defined(BT_USE_SSE)
```

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/MANIFEST.in` & `RocketSim-2.1.1/libsrc/bullet3-3.24/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/README.md` & `RocketSim-2.1.1/libsrc/bullet3-3.24/README.md`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/btBulletCollisionCommon.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/btBulletCollisionCommon.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/libsrc/bullet3-3.24/btBulletDynamicsCommon.h` & `RocketSim-2.1.1/libsrc/bullet3-3.24/btBulletDynamicsCommon.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/python-mtheall/Angle.cpp` & `RocketSim-2.1.1/python-mtheall/Angle.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 PyType_Slot Angle::Slots[] = {
     {Py_tp_new, (void *)&Angle::New},
     {Py_tp_init, (void *)&Angle::Init},
     {Py_tp_dealloc, (void *)&Angle::Dealloc},
     {Py_tp_repr, (void *)&Angle::Repr},
     {Py_tp_members, &Angle::Members},
     {Py_tp_methods, &Angle::Methods},
+    {Py_sq_length, (void *)&Angle::Length},
+    {Py_sq_item, (void *)&Angle::GetItem},
+    {Py_sq_ass_item, (void *)&Angle::SetItem},
     {Py_tp_doc, (void *)R"(Tait-Bryan angle rotation in the order ZYX (yaw/pitch/roll)
 __init__(self, yaw: float = 0.0, pitch: float = 0.0, roll: float = 0.0))"},
     {0, nullptr},
 };
 
 PyType_Spec Angle::Spec = {
     .name      = "RocketSim.Angle",
@@ -206,14 +209,20 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *Angle::Unpickle (Angle *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
 
@@ -226,14 +235,68 @@
 }
 
 PyObject *Angle::DeepCopy (Angle *self_, PyObject *memo_) noexcept
 {
 	return NewFromAngle (self_->angle).giftObject ();
 }
 
+Py_ssize_t Angle::Length (Angle *self_) noexcept
+{
+	return 3;
+}
+
+PyObject *Angle::GetItem (Angle *self_, Py_ssize_t index_) noexcept
+{
+	switch (index_)
+	{
+	case 0:
+		return PyFloat_FromDouble (self_->angle.yaw);
+
+	case 1:
+		return PyFloat_FromDouble (self_->angle.pitch);
+
+	case 2:
+		return PyFloat_FromDouble (self_->angle.roll);
+	}
+
+	PyErr_SetString (PyExc_IndexError, "index out of range");
+	return nullptr;
+}
+
+int Angle::SetItem (Angle *self_, Py_ssize_t index_, PyObject *value_) noexcept
+{
+	if (!value_)
+	{
+		PyErr_SetString (PyExc_TypeError, "'RocketSim.Angle' object doesn't support item deletion");
+		return -1;
+	}
+
+	auto const val = PyFloat_AsDouble (value_);
+	if (val == -1.0 && PyErr_Occurred ())
+		return -1;
+
+	switch (index_)
+	{
+	case 0:
+		self_->angle.yaw = val;
+		return 0;
+
+	case 1:
+		self_->angle.pitch = val;
+		return 0;
+
+	case 2:
+		self_->angle.roll = val;
+		return 0;
+	}
+
+	PyErr_SetString (PyExc_IndexError, "index out of range");
+	return -1;
+}
+
 PyObject *Angle::AsTuple (Angle *self_) noexcept
 {
 	return Py_BuildValue ("fff", self_->angle.yaw, self_->angle.pitch, self_->angle.roll);
 }
 
 PyObject *Angle::AsRotMat (Angle *self_) noexcept
 {
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/Arena.cpp` & `RocketSim-2.1.1/python-mtheall/Arena.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -131,67 +131,68 @@
 	auto const it = map_.find (makeKey (pad_->pos.x, pad_->pos.y));
 	if (it == std::end (map_))
 		return -1;
 
 	return it->second;
 }
 
-std::pair<std::uint32_t const *, std::size_t> getIndexMapping (RocketSim::GameMode gameMode_) noexcept
-{
-	if (gameMode_ == RocketSim::GameMode::HOOPS)
-		return {hoopsIndexMapping.data (), hoopsIndexMapping.size ()};
-
-	return {soccarIndexMapping.data (), soccarIndexMapping.size ()};
-}
-
 std::unordered_map<std::uint64_t, unsigned> const &getBoostMapping (RocketSim::GameMode gameMode_) noexcept
 {
 	if (gameMode_ == RocketSim::GameMode::HOOPS)
 		return hoopsBoostMapping;
 
 	return soccarBoostMapping;
 }
 
 bool ensureBoostPadByIndex (RocketSim::Python::Arena *arena_) noexcept
 {
-	if (arena_->boostPads->empty () || arena_->boostPadsByIndex)
+	if (arena_->arena->GetArenaConfig ().customBoostPads)
 		return true;
 
-	arena_->boostPadsByIndex = new (std::nothrow)
-	    std::vector<RocketSim::Python::PyRef<RocketSim::Python::BoostPad>> (arena_->boostPads->size ());
-	if (!arena_->boostPadsByIndex)
-	{
-		PyErr_NoMemory ();
-		return false;
-	}
+	if (arena_->boostPads->empty ())
+		return true;
 
-	auto const &boostMapping = getBoostMapping (arena_->arena->gameMode);
-	for (auto const &[ptr, pad] : *arena_->boostPads)
+	try
 	{
-		auto const index = getBoostPadIndex (ptr, boostMapping);
-		if (index < 0 || static_cast<unsigned> (index) > arena_->boostPads->size ())
+		auto boostPadsByIndex = std::make_unique<std::vector<RocketSim::Python::PyRef<RocketSim::Python::BoostPad>>> (
+		    arena_->boostPads->size ());
+
+		auto const &boostMapping = getBoostMapping (arena_->arena->gameMode);
+		for (auto const &[ptr, pad] : *arena_->boostPads)
 		{
-			delete arena_->boostPadsByIndex;
-			arena_->boostPadsByIndex = nullptr;
-			PyErr_SetString (PyExc_ValueError, "Failed to map boost pad index");
-			return false;
-		}
+			auto const index = getBoostPadIndex (ptr, boostMapping);
+			if (index < 0 || static_cast<unsigned> (index) > arena_->boostPads->size ())
+			{
+				PyErr_SetString (PyExc_ValueError, "Failed to map boost pad index");
+				return false;
+			}
 
-		(*arena_->boostPadsByIndex)[index] = pad;
-	}
+			boostPadsByIndex->operator[] (index) = pad;
+		}
 
-	for (auto const &pad : *arena_->boostPadsByIndex)
-	{
-		if (!pad)
+		for (auto const &pad : *boostPadsByIndex)
 		{
-			delete arena_->boostPadsByIndex;
-			arena_->boostPadsByIndex = nullptr;
-			PyErr_SetString (PyExc_ValueError, "Failed to map boost pad index");
-			return false;
+			if (!pad)
+			{
+				PyErr_SetString (PyExc_ValueError, "Failed to map boost pad index");
+				return false;
+			}
 		}
+
+		*arena_->boostPadsByIndex = std::move (*boostPadsByIndex);
+	}
+	catch (std::exception const &err)
+	{
+		PyErr_SetString (PyExc_RuntimeError, err.what ());
+		return false;
+	}
+	catch (...)
+	{
+		PyErr_SetString (PyExc_RuntimeError, "Unknown exception");
+		return false;
 	}
 
 	return true;
 }
 
 void assign (RocketSim::Python::PyArrayRef &array_, unsigned row_, unsigned col_, btVector3 const &value_) noexcept
 {
@@ -472,14 +473,18 @@
         .ml_meth  = (PyCFunction)&Arena::Clone,
         .ml_flags = METH_VARARGS | METH_KEYWORDS,
         .ml_doc   = R"(clone(self, copy_callbacks: bool = False) -> RocketSim.Arena)"},
     {.ml_name     = "clone_into",
         .ml_meth  = (PyCFunction)&Arena::CloneInto,
         .ml_flags = METH_VARARGS | METH_KEYWORDS,
         .ml_doc   = R"(clone_into(self, target: RocketSim.Arena, copy_callbacks: bool = False))"},
+    {.ml_name     = "get_config",
+        .ml_meth  = (PyCFunction)&Arena::GetConfig,
+        .ml_flags = METH_NOARGS,
+        .ml_doc   = R"(get_config(self) -> RocketSim.ArenaConfig)"},
     {.ml_name     = "get_car_from_id",
         .ml_meth  = (PyCFunction)&Arena::GetCarFromId,
         .ml_flags = METH_VARARGS | METH_KEYWORDS,
         .ml_doc   = R"(get_car_from_id(self, car_id: int) -> RocketSim.Car
 Raises KeyError if car doesn't exist
 
 get_car_from_id(self, car_id: int, default) -> RocketSim.Car
@@ -488,15 +493,15 @@
         .ml_meth  = (PyCFunction)&Arena::GetCars,
         .ml_flags = METH_NOARGS,
         .ml_doc   = R"(get_cars(self) -> List[RocketSim.Car])"},
     {.ml_name     = "get_ball_prediction",
         .ml_meth  = (PyCFunction)&Arena::GetBallPrediction,
         .ml_flags = METH_VARARGS | METH_KEYWORDS,
         .ml_doc =
-            R"(get_ball_prediction(self, num_ticks: int = 120, tick_skip: int = 1) -> List[Tuple[float, RocketSim.BallState]])"},
+            R"(get_ball_prediction(self, num_ticks: int = 120, tick_interval: int = 1) -> List[RocketSim.BallState])"},
     {.ml_name     = "get_boost_pads",
         .ml_meth  = (PyCFunction)&Arena::GetBoostPads,
         .ml_flags = METH_NOARGS,
         .ml_doc   = R"(get_boost_pads(self) -> List[RocketSim.BoostPad])"},
     {.ml_name     = "get_gym_state",
         .ml_meth  = (PyCFunction)&Arena::GetGymState,
         .ml_flags = METH_NOARGS,
@@ -622,15 +627,15 @@
         .ml_flags = METH_VARARGS | METH_KEYWORDS,
         .ml_doc   = R"(step(self, ticks: int = 1))"},
     {.ml_name = "stop", .ml_meth = (PyCFunction)&Arena::Stop, .ml_flags = METH_NOARGS, .ml_doc = R"(stop(self)
 This can be called from within a callback to stop simulation early)"},
     {.ml_name     = "multi_step",
         .ml_meth  = (PyCFunction)&Arena::MultiStep,
         .ml_flags = METH_VARARGS | METH_KEYWORDS | METH_STATIC,
-        .ml_doc   = R"(multi_step(arenas: list[RocketSim.Arena] = [], ticks: int = 1))"},
+        .ml_doc   = R"(multi_step(arenas: Sequence[RocketSim.Arena] = [], ticks: int = 1))"},
     {.ml_name = "__getstate__", .ml_meth = (PyCFunction)&Arena::Pickle, .ml_flags = METH_NOARGS, .ml_doc = nullptr},
     {.ml_name = "__setstate__", .ml_meth = (PyCFunction)&Arena::Unpickle, .ml_flags = METH_O, .ml_doc = nullptr},
     {.ml_name     = "__copy__",
         .ml_meth  = (PyCFunction)&Arena::Copy,
         .ml_flags = METH_NOARGS,
         .ml_doc   = R"(__copy__(self) -> RocketSim.Arena
 Shallow copy)"},
@@ -654,15 +659,20 @@
     {Py_tp_new, (void *)&Arena::New},
     {Py_tp_init, (void *)&Arena::Init},
     {Py_tp_dealloc, (void *)&Arena::Dealloc},
     {Py_tp_methods, &Arena::Methods},
     {Py_tp_members, &Arena::Members},
     {Py_tp_getset, &Arena::GetSet},
     {Py_tp_doc, (void *)R"(Arena
-__init__(self, game_mode: int = RocketSim.GameMode.SOCCAR, memory_weight_mode = RocketSim.MemoryWeightMode.HEAVY, tick_rate: float = 120.0))"},
+__init__(self,
+	game_mode: int = RocketSim.GameMode.SOCCAR,
+	memory_weight_mode: int = RocketSim.MemoryWeightMode.HEAVY,
+	tick_rate: float = 120.0,
+	config: RocketSim.ArenaConfig = RocketSim.ArenaConfig())
+	Note: memory_weight_mode overrides config.memory_weight_mode if specified)"},
     {0, nullptr},
 };
 
 PyType_Spec Arena::Spec = {
     .name      = "RocketSim.Arena",
     .basicsize = sizeof (Arena),
     .itemsize  = 0,
@@ -678,15 +688,15 @@
 	if (!self)
 		return nullptr;
 
 	new (&self->arena) std::shared_ptr<RocketSim::Arena>{};
 	new (&self->threadPool) std::shared_ptr<Arena::ThreadPool>{};
 	self->cars                        = new (std::nothrow) std::map<std::uint32_t, PyRef<Car>>{};
 	self->boostPads                   = new (std::nothrow) std::unordered_map<RocketSim::BoostPad *, PyRef<BoostPad>>{};
-	self->boostPadsByIndex            = nullptr;
+	self->boostPadsByIndex            = new (std::nothrow) std::vector<PyRef<BoostPad>>{};
 	self->ballPrediction              = nullptr;
 	self->gameEvent                   = nullptr;
 	self->ball                        = nullptr;
 	self->ballTouchCallback           = nullptr;
 	self->ballTouchCallbackUserData   = nullptr;
 	self->boostPickupCallback         = nullptr;
 	self->boostPickupCallbackUserData = nullptr;
@@ -706,40 +716,46 @@
 	self->orangeScore                 = 0;
 	self->lastGoalTick                = 0;
 	self->lastGymStateTick            = 0;
 	self->stepExceptionType           = nullptr;
 	self->stepExceptionValue          = nullptr;
 	self->stepExceptionTraceback      = nullptr;
 
-	if (!self->cars || !self->boostPads)
+	if (!self->cars || !self->boostPads || !self->boostPadsByIndex)
 	{
 		self->arena.~shared_ptr ();
 		self->threadPool.~shared_ptr ();
 		delete self->cars;
 		delete self->boostPads;
+		delete self->boostPadsByIndex;
 
 		return PyErr_NoMemory ();
 	}
 
 	return self.giftObject ();
 }
 
 int Arena::Init (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept
 {
+	RocketSim::ArenaConfig arenaConfig{};
+
+	PyObject *config     = nullptr; // borrowed reference
 	int gameMode         = static_cast<int> (RocketSim::GameMode::SOCCAR);
-	int memoryWeightMode = static_cast<int> (RocketSim::ArenaMemWeightMode::HEAVY);
+	int memoryWeightMode = static_cast<int> (arenaConfig.memWeightMode);
 	float tickRate       = 120.0f;
 
 	static char gameModeKwd[]         = "game_mode";
 	static char memoryWeightModeKwd[] = "memory_weight_mode";
 	static char tickRateKwd[]         = "tick_rate";
+	static char configKwd[]           = "config";
 
-	static char *dict[] = {gameModeKwd, memoryWeightModeKwd, tickRateKwd, nullptr};
+	static char *dict[] = {gameModeKwd, memoryWeightModeKwd, tickRateKwd, configKwd, nullptr};
 
-	if (!PyArg_ParseTupleAndKeywords (args_, kwds_, "|iif", dict, &gameMode, &memoryWeightMode, &tickRate))
+	if (!PyArg_ParseTupleAndKeywords (
+	        args_, kwds_, "|iifO!", dict, &gameMode, &memoryWeightMode, &tickRate, ArenaConfig::Type, &config))
 		return -1;
 
 	try
 	{
 		switch (static_cast<RocketSim::GameMode> (gameMode))
 		{
 		case RocketSim::GameMode::SOCCAR:
@@ -752,27 +768,53 @@
 			break;
 
 		case RocketSim::GameMode::HEATSEEKER:
 		case RocketSim::GameMode::THE_VOID:
 			break;
 
 		default:
-			PyErr_SetString (PyExc_RuntimeError, "Invalid game mode");
+			PyErr_Format (PyExc_RuntimeError, "Invalid game mode '%d'", gameMode);
 			return -1;
 		}
 	}
 	catch (...)
 	{
 		PyErr_NoMemory ();
 		return -1;
 	}
 
+	// check if config was specified
+	if (config)
+	{
+		auto result = ArenaConfig::ToArenaConfig (PyCast<ArenaConfig> (config));
+		if (!result.has_value ())
+			return -1;
+
+		arenaConfig = std::move (result.value ());
+	}
+
+	// check if memory_weight_mode was specified
+	if ((args_ && PyTuple_Size (args_) >= 2 && PyTuple_GetItem (args_, 1)) ||
+	    (kwds_ && PyDict_GetItemString (kwds_, "memory_weight_mode")))
+		arenaConfig.memWeightMode = static_cast<RocketSim::ArenaMemWeightMode> (memoryWeightMode);
+
+	switch (arenaConfig.memWeightMode)
+	{
+	case RocketSim::ArenaMemWeightMode::LIGHT:
+	case RocketSim::ArenaMemWeightMode::HEAVY:
+		break;
+
+	default:
+		PyErr_Format (PyExc_ValueError, "Invalid arena memory weight mode '%d'", memoryWeightMode);
+		return -1;
+	}
+
 	if (tickRate < 15.0f || tickRate > 120.0f)
 	{
-		PyErr_SetString (PyExc_RuntimeError, "Invalid tick rate");
+		PyErr_Format (PyExc_RuntimeError, "Invalid tick rate '%f'", tickRate);
 		return -1;
 	}
 
 	try
 	{
 		// default initialization if it hasn't been done yet
 		InitInternal (nullptr);
@@ -781,18 +823,16 @@
 	{
 		PyErr_SetString (PyExc_RuntimeError, err.what ());
 		return -1;
 	}
 
 	try
 	{
-		auto arena =
-		    std::shared_ptr<RocketSim::Arena> (RocketSim::Arena::Create (static_cast<RocketSim::GameMode> (gameMode),
-		        static_cast<RocketSim::ArenaMemWeightMode> (memoryWeightMode),
-		        tickRate));
+		auto arena = std::shared_ptr<RocketSim::Arena> (
+		    RocketSim::Arena::Create (static_cast<RocketSim::GameMode> (gameMode), arenaConfig, tickRate));
 		if (!arena)
 			throw -1;
 
 		arena->SetCarBumpCallback (&Arena::HandleCarBumpCallback, self_);
 
 		if (arena->gameMode != RocketSim::GameMode::THE_VOID)
 		{
@@ -800,29 +840,32 @@
 			arena->SetGoalScoreCallback (&Arena::HandleGoalScoreCallback, self_);
 		}
 
 		auto ball = PyRef<Ball>::steal (Ball::New ());
 		if (!ball)
 			throw -1;
 
-		auto boostPads = std::unordered_map<RocketSim::BoostPad *, PyRef<BoostPad>>{};
+		auto boostPads        = std::unordered_map<RocketSim::BoostPad *, PyRef<BoostPad>>{};
+		auto boostPadsByIndex = std::vector<PyRef<BoostPad>>{};
 		for (auto const &pad : arena->GetBoostPads ())
 		{
 			auto ref = PyRef<BoostPad>::steal (BoostPad::New ());
 			if (!ref)
 				throw -1;
 
 			ref->pad = pad;
-			boostPads.emplace (pad, std::move (ref));
+			boostPads.emplace (pad, ref);
+			boostPadsByIndex.emplace_back (std::move (ref));
 		}
 
 		// no exceptions thrown after this point
 		self_->arena = arena;
 		self_->cars->clear ();
-		*self_->boostPads = std::move (boostPads);
+		*self_->boostPads        = std::move (boostPads);
+		*self_->boostPadsByIndex = std::move (boostPadsByIndex);
 
 		PyRef<Ball>::assign (self_->ball, ball.borrowObject ());
 		self_->ball->arena = self_->arena;
 		self_->ball->ball  = self_->arena->ball;
 
 		PyObjectRef::assign (self_->ballTouchCallback, Py_None);
 		PyObjectRef::assign (self_->ballTouchCallbackUserData, Py_None);
@@ -851,15 +894,17 @@
 	catch (std::exception const &err)
 	{
 		PyErr_SetString (PyExc_RuntimeError, err.what ());
 		return -1;
 	}
 	catch (...)
 	{
-		PyErr_SetString (PyExc_RuntimeError, "Unknown exception");
+		if (!PyErr_Occurred ())
+			PyErr_SetString (PyExc_RuntimeError, "Unknown exception");
+
 		return -1;
 	}
 }
 
 void Arena::Dealloc (Arena *self_) noexcept
 {
 	self_->arena.~shared_ptr ();
@@ -924,53 +969,46 @@
 				return nullptr;
 		}
 
 		if (!DictSetValue (dict.borrow (), "cars", cars.gift ()))
 			return nullptr;
 	}
 
-	if (!self_->boostPads->empty ())
+	if (!self_->boostPadsByIndex->empty ())
 	{
-		auto pads = PyObjectRef::steal (PyList_New (self_->boostPads->size ()));
+		auto pads = PyObjectRef::steal (PyList_New (self_->boostPadsByIndex->size ()));
 		if (!pads)
 			return nullptr;
 
-		auto const &boostMapping = getBoostMapping (self_->arena->gameMode);
-		for (auto const &[ptr, pad] : *self_->boostPads)
+		for (unsigned idx = 0; idx < self_->boostPadsByIndex->size (); ++idx)
 		{
-			auto entry = BoostPadState::NewFromBoostPadState (pad->pad->GetState ());
+			auto const pad = self_->boostPadsByIndex->operator[] (idx)->pad;
+
+			auto entry = BoostPadState::NewFromBoostPadState (pad->GetState ());
 			if (!entry)
 				return nullptr;
 
-			auto const index = getBoostPadIndex (ptr, boostMapping);
-			if (index < 0 || index >= PyList_Size (pads.borrow ()))
-				continue;
-
 			// steals ref
-			if (PyList_SetItem (pads.borrow (), index, entry.giftObject ()) < 0)
-				return nullptr;
-		}
-
-		for (unsigned i = 0; i < PyList_Size (pads.borrow ()); ++i)
-		{
-			if (!PyList_GetItem (pads.borrow (), i))
-			{
-				PyErr_SetString (PyExc_RuntimeError, "Failed to enumerate all boost pads");
+			if (PyList_SetItem (pads.borrow (), idx, entry.giftObject ()) < 0)
 				return nullptr;
-			}
 		}
 
 		if (!DictSetValue (dict.borrow (), "boost_pads", pads.gift ()))
 			return nullptr;
 	}
 
 	if (self_->arena->gameMode != RocketSim::GameMode::SOCCAR &&
 	    !DictSetValue (dict.borrow (), "game_mode", PyLong_FromLong (static_cast<long> (self_->arena->gameMode))))
 		return nullptr;
 
+	if (!DictSetValue (dict.borrow (),
+	        "arena_config",
+	        ArenaConfig::NewFromArenaConfig (self_->arena->GetArenaConfig ()).giftObject ()))
+		return nullptr;
+
 	if (self_->arena->_lastCarID &&
 	    !DictSetValue (dict.borrow (), "last_car_id", PyLong_FromUnsignedLong (self_->arena->_lastCarID)))
 		return nullptr;
 
 	if (self_->arena->tickTime != 1.0f / 120.0f &&
 	    !DictSetValue (dict.borrow (), "tick_time", PyFloat_FromDouble (self_->arena->tickTime)))
 		return nullptr;
@@ -1060,27 +1098,28 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *Arena::Unpickle (Arena *self_, PyObject *dict_) noexcept
 {
-	if (!Py_IS_TYPE (dict_, &PyDict_Type))
+	if (!PyDict_Check (dict_))
 	{
 		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
 		return nullptr;
 	}
 
 	auto const dummy = PyObjectRef::steal (PyTuple_New (0));
 	if (!dummy)
 		return nullptr;
 
 	static char gameModeKwd[]                    = "game_mode";
 	static char memoryWeightModeKwd[]            = "memory_weight_mode";
 	static char lastCarIDKwd[]                   = "last_car_id";
+	static char arenaConfigKwd[]                 = "arena_config";
 	static char mutatorConfigKwd[]               = "mutator_config";
 	static char tickTimeKwd[]                    = "tick_time";
 	static char tickCountKwd[]                   = "tick_count";
 	static char ballStateKwd[]                   = "ball_state";
 	static char carsKwd[]                        = "cars";
 	static char boostPadsKwd[]                   = "boost_pads";
 	static char blueScoreKwd[]                   = "blue_score";
@@ -1103,14 +1142,15 @@
 	static char goalEventCallbackUserDataKwd[]   = "goal_score_callback_user_data";
 	static char saveEventCallbackKwd[]           = "save_score_callback";
 	static char saveEventCallbackUserDataKwd[]   = "save_score_callback_user_data";
 
 	static char *dict[] = {gameModeKwd,
 	    memoryWeightModeKwd,
 	    lastCarIDKwd,
+	    arenaConfigKwd,
 	    mutatorConfigKwd,
 	    tickTimeKwd,
 	    tickCountKwd,
 	    ballStateKwd,
 	    carsKwd,
 	    boostPadsKwd,
 	    blueScoreKwd,
@@ -1131,59 +1171,60 @@
 	    shotEventCallbackUserDataKwd,
 	    goalEventCallbackKwd,
 	    goalEventCallbackUserDataKwd,
 	    saveEventCallbackKwd,
 	    saveEventCallbackUserDataKwd,
 	    nullptr};
 
-	PyObject *mutatorConfig               = nullptr; // borrowed references
+	PyObject *arenaConfig                 = nullptr; // borrowed references
+	PyObject *mutatorConfig               = nullptr;
 	PyObject *ballState                   = nullptr;
 	PyObject *cars                        = nullptr;
 	PyObject *pads                        = nullptr;
-	PyObject *ballTouchCallback           = nullptr;
-	PyObject *ballTouchCallbackUserData   = nullptr;
-	PyObject *boostPickupCallback         = nullptr;
-	PyObject *boostPickupCallbackUserData = nullptr;
-	PyObject *carBumpCallback             = nullptr;
-	PyObject *carBumpCallbackUserData     = nullptr;
-	PyObject *carDemoCallback             = nullptr;
-	PyObject *carDemoCallbackUserData     = nullptr;
-	PyObject *goalScoreCallback           = nullptr;
-	PyObject *goalScoreCallbackUserData   = nullptr;
-	PyObject *shotEventCallback           = nullptr;
-	PyObject *shotEventCallbackUserData   = nullptr;
-	PyObject *goalEventCallback           = nullptr;
-	PyObject *goalEventCallbackUserData   = nullptr;
-	PyObject *saveEventCallback           = nullptr;
-	PyObject *saveEventCallbackUserData   = nullptr;
+	PyObject *ballTouchCallback           = Py_None;
+	PyObject *ballTouchCallbackUserData   = Py_None;
+	PyObject *boostPickupCallback         = Py_None;
+	PyObject *boostPickupCallbackUserData = Py_None;
+	PyObject *carBumpCallback             = Py_None;
+	PyObject *carBumpCallbackUserData     = Py_None;
+	PyObject *carDemoCallback             = Py_None;
+	PyObject *carDemoCallbackUserData     = Py_None;
+	PyObject *goalScoreCallback           = Py_None;
+	PyObject *goalScoreCallbackUserData   = Py_None;
+	PyObject *shotEventCallback           = Py_None;
+	PyObject *shotEventCallbackUserData   = Py_None;
+	PyObject *goalEventCallback           = Py_None;
+	PyObject *goalEventCallbackUserData   = Py_None;
+	PyObject *saveEventCallback           = Py_None;
+	PyObject *saveEventCallbackUserData   = Py_None;
 	unsigned long long tickCount          = 0;
 	unsigned long long lastGoalTick       = 0;
 	unsigned long long lastGymStateTick   = 0;
 	unsigned long lastCarID               = 0;
 	float tickTime                        = 1.0f / 120.0f;
 	unsigned blueScore                    = 0;
 	unsigned orangeScore                  = 0;
 	int gameMode                          = static_cast<int> (RocketSim::GameMode::SOCCAR);
 	int memoryWeightMode                  = static_cast<int> (RocketSim::ArenaMemWeightMode::HEAVY);
 	if (!PyArg_ParseTupleAndKeywords (dummy.borrow (),
 	        dict_,
-	        "|iikO!fKO!O!O!IIKKOOOOOOOOOOOOOO",
+	        "|iikO!O!fKO!OOIIKKOOOOOOOOOOOOOO",
 	        dict,
 	        &gameMode,
 	        &memoryWeightMode,
 	        &lastCarID,
+	        ArenaConfig::Type,
+	        &arenaConfig,
 	        MutatorConfig::Type,
 	        &mutatorConfig,
 	        &tickTime,
 	        &tickCount,
 	        BallState::Type,
 	        &ballState,
-	        &PyList_Type,
 	        &cars,
-	        &PyList_Type,
 	        &pads,
 	        &blueScore,
 	        &orangeScore,
 	        &lastGoalTick,
 	        &lastGymStateTick,
 	        &ballTouchCallback,
 	        &ballTouchCallbackUserData,
@@ -1212,17 +1253,23 @@
 	case RocketSim::GameMode::THE_VOID:
 		break;
 
 	default:
 		return PyErr_Format (PyExc_ValueError, "Invalid game mode '%d'", gameMode);
 	}
 
-	if (static_cast<RocketSim::ArenaMemWeightMode> (memoryWeightMode) != RocketSim::ArenaMemWeightMode::LIGHT &&
-	    static_cast<RocketSim::ArenaMemWeightMode> (memoryWeightMode) != RocketSim::ArenaMemWeightMode::HEAVY)
+	switch (static_cast<RocketSim::ArenaMemWeightMode> (memoryWeightMode))
+	{
+	case RocketSim::ArenaMemWeightMode::LIGHT:
+	case RocketSim::ArenaMemWeightMode::HEAVY:
+		break;
+
+	default:
 		return PyErr_Format (PyExc_ValueError, "Invalid arena memory weight mode '%d'", memoryWeightMode);
+	}
 
 	// make sure callback are None or callable
 	if (ballTouchCallback && ballTouchCallback != Py_None && !PyCallable_Check (ballTouchCallback))
 	{
 		PyErr_SetString (PyExc_ValueError, "Invalid ball touch callback");
 		return nullptr;
 	}
@@ -1278,18 +1325,30 @@
 	{
 		PyErr_SetString (PyExc_RuntimeError, err.what ());
 		return nullptr;
 	}
 
 	try
 	{
-		auto arena =
-		    std::shared_ptr<RocketSim::Arena> (RocketSim::Arena::Create (static_cast<RocketSim::GameMode> (gameMode),
-		        static_cast<RocketSim::ArenaMemWeightMode> (memoryWeightMode),
-		        1.0f / tickTime));
+		RocketSim::ArenaConfig config{};
+
+		// backwards compatibility
+		config.memWeightMode = static_cast<RocketSim::ArenaMemWeightMode> (memoryWeightMode);
+
+		if (arenaConfig)
+		{
+			auto result = ArenaConfig::ToArenaConfig (PyCast<ArenaConfig> (arenaConfig));
+			if (!result.has_value ())
+				return nullptr;
+
+			config = std::move (result.value ());
+		}
+
+		auto arena = std::shared_ptr<RocketSim::Arena> (
+		    RocketSim::Arena::Create (static_cast<RocketSim::GameMode> (gameMode), config, 1.0f / tickTime));
 		if (!arena)
 			return PyErr_NoMemory ();
 
 		if (mutatorConfig)
 			arena->SetMutatorConfig (MutatorConfig::ToMutatorConfig (PyCast<MutatorConfig> (mutatorConfig)));
 
 		arena->tickTime  = tickTime;
@@ -1297,79 +1356,80 @@
 
 		if (ballState)
 		{
 			arena->ball->SetState (BallState::ToBallState (PyCast<BallState> (ballState)));
 			arena->ball->_internalState.updateCounter = PyCast<BallState> (ballState)->state.updateCounter;
 		}
 
-		auto carMap        = std::map<std::uint32_t, PyRef<Car>>{};
-		auto const numCars = PyList_Size (cars);
-		for (unsigned i = 0; i < numCars; ++i)
+		auto carMap = std::map<std::uint32_t, PyRef<Car>>{};
+		if (cars)
 		{
-			auto car = PyRef<Car>::steal (Car::New ());
-			if (!car)
+			if (!PySequence_Check (cars))
+			{
+				PyErr_SetString (PyExc_TypeError, "cars type must be a sequence");
 				return nullptr;
+			}
 
-			auto result = PyObjectRef::steal (Car::InternalUnpickle (arena, car.borrow (), PyList_GetItem (cars, i)));
-			if (!result)
-				return nullptr;
+			auto const numCars = PySequence_Size (cars);
+			for (unsigned i = 0; i < numCars; ++i)
+			{
+				auto car = PyRef<Car>::steal (Car::New ());
+				if (!car)
+					return nullptr;
+
+				auto result =
+				    PyObjectRef::steal (Car::InternalUnpickle (arena, car.borrow (), PySequence_GetItem (cars, i)));
+				if (!result)
+					return nullptr;
 
-			carMap[car->car->id] = car;
+				carMap[car->car->id] = car;
+			}
 		}
 
 		auto padMap = std::unordered_map<RocketSim::BoostPad *, PyRef<BoostPad>>{};
+		auto padVec = std::vector<PyRef<BoostPad>>{};
 		if (pads)
 		{
-			auto const &[indexMapping, indexMappingSize] = getIndexMapping (arena->gameMode);
+			if (!PySequence_Check (pads))
+			{
+				PyErr_SetString (PyExc_TypeError, "boost_pads type must be a sequence");
+				return nullptr;
+			}
 
-			auto const numPads = PyList_Size (pads);
+			auto const numPads = arena->GetBoostPads ().size ();
 
-			if (numPads != indexMappingSize)
+			if (PySequence_Size (pads) != numPads)
 				return PyErr_Format (PyExc_KeyError,
 				    "Internal mapping error: expected %zu boost pads, got %zu",
-				    indexMappingSize,
-				    numPads);
+				    numPads,
+				    PySequence_Size (pads));
 
 			for (unsigned i = 0; i < numPads; ++i)
 			{
 				auto pad = PyRef<BoostPad>::steal (BoostPad::New ());
 				if (!pad)
 					return nullptr;
 
-				auto const [x, y] = extractKey (indexMapping[i]);
-
-				for (auto const p : arena->GetBoostPads ())
-				{
-					if (static_cast<int> (p->pos.x) == x && static_cast<int> (p->pos.y) == y)
-					{
-						pad->arena = arena;
-						pad->pad   = p;
-						break;
-					}
-				}
-
-				if (!pad->pad)
-				{
-					PyErr_SetString (PyExc_RuntimeError, "Failed to enumerate all boost pads");
-					return nullptr;
-				}
+				pad->arena = arena;
+				pad->pad   = arena->GetBoostPads ()[i];
 
-				auto state = PyList_GetItem (pads, i);
+				auto state = PySequence_GetItem (pads, i);
 				if (!state)
 					return nullptr;
 
 				if (!Py_IS_TYPE (state, BoostPadState::Type))
 				{
 					PyErr_SetString (PyExc_RuntimeError, "Unexpected type");
 					return nullptr;
 				}
 
 				pad->pad->SetState (BoostPadState::ToBoostPadState (PyCast<BoostPadState> (state)));
 
 				padMap[pad->pad] = pad;
+				padVec.emplace_back (std::move (pad));
 			}
 		}
 
 		auto ball = PyRef<Ball>::steal (Ball::New ());
 		if (!ball)
 			return PyErr_NoMemory ();
 
@@ -1386,16 +1446,17 @@
 
 		self_->arena = std::move (arena);
 
 		PyRef<Ball>::assign (self_->ball, ball.borrowObject ());
 		self_->ball->arena = self_->arena;
 		self_->ball->ball  = self_->arena->ball;
 
-		*self_->cars      = std::move (carMap);
-		*self_->boostPads = std::move (padMap);
+		*self_->cars             = std::move (carMap);
+		*self_->boostPads        = std::move (padMap);
+		*self_->boostPadsByIndex = std::move (padVec);
 
 		self_->blueScore        = blueScore;
 		self_->orangeScore      = orangeScore;
 		self_->lastGoalTick     = lastGoalTick;
 		self_->lastGymStateTick = lastGymStateTick;
 
 		PyObjectRef::assign (self_->ballTouchCallback, ballTouchCallback);
@@ -1424,17 +1485,25 @@
 		{
 			self_->arena->SetBoostPickupCallback (&Arena::HandleBoostPickupCallback, self_);
 			self_->arena->SetGoalScoreCallback (&Arena::HandleGoalScoreCallback, self_);
 		}
 
 		Py_RETURN_NONE;
 	}
+	catch (std::exception const &err)
+	{
+		PyErr_SetString (PyExc_RuntimeError, err.what ());
+		return nullptr;
+	}
 	catch (...)
 	{
-		return PyErr_NoMemory ();
+		if (!PyErr_Occurred ())
+			PyErr_SetString (PyExc_RuntimeError, "Unknown exception");
+
+		return nullptr;
 	}
 }
 
 PyObject *Arena::Copy (Arena *self_) noexcept
 {
 	auto args = PyObjectRef::steal (PyTuple_New (1));
 	if (!args)
@@ -1466,15 +1535,15 @@
 	int team;
 	PyObject *config = nullptr; // borrowed reference
 	if (!PyArg_ParseTupleAndKeywords (args_, kwds_, "i|O", dict, &team, &config))
 		return nullptr;
 
 	if (team != static_cast<int> (RocketSim::Team::BLUE) && team != static_cast<int> (RocketSim::Team::ORANGE))
 	{
-		PyErr_SetString (PyExc_RuntimeError, "Invalid team");
+		PyErr_Format (PyExc_RuntimeError, "Invalid team '%d'", team);
 		return nullptr;
 	}
 
 	RocketSim::CarConfig carConfig = CAR_CONFIG_OCTANE;
 	if (config && Py_IS_TYPE (config, CarConfig::Type))
 	{
 		carConfig = reinterpret_cast<CarConfig const *> (config)->config;
@@ -1539,23 +1608,25 @@
 		if (!arena)
 			return PyErr_NoMemory ();
 
 		auto ball = PyRef<Ball>::steal (Ball::New ());
 		if (!ball)
 			return PyErr_NoMemory ();
 
-		auto boostPads = std::unordered_map<RocketSim::BoostPad *, PyRef<BoostPad>>{};
+		auto boostPads        = std::unordered_map<RocketSim::BoostPad *, PyRef<BoostPad>>{};
+		auto boostPadsByIndex = std::vector<PyRef<BoostPad>>{};
 		for (auto const &pad : arena->GetBoostPads ())
 		{
 			auto ref = PyRef<BoostPad>::steal (BoostPad::New ());
 			if (!ref)
 				return PyErr_NoMemory ();
 
 			ref->pad = pad;
-			boostPads.emplace (pad, std::move (ref));
+			boostPads.emplace (pad, ref);
+			boostPadsByIndex.emplace_back (std::move (ref));
 		}
 
 		auto cars = std::map<std::uint32_t, PyRef<Car>>{};
 		for (auto const &car : arena->GetCars ())
 		{
 			auto &carRef = cars[car->id];
 
@@ -1584,18 +1655,19 @@
 				carRef->shots        = 0;
 				carRef->saves        = 0;
 				carRef->assists      = 0;
 			}
 		}
 
 		// no exceptions thrown after this point
-		clone->arena      = arena;
-		clone->threadPool = self_->threadPool;
-		*clone->boostPads = std::move (boostPads);
-		*clone->cars      = std::move (cars);
+		clone->arena             = arena;
+		clone->threadPool        = self_->threadPool;
+		*clone->boostPads        = std::move (boostPads);
+		*clone->boostPadsByIndex = std::move (boostPadsByIndex);
+		*clone->cars             = std::move (cars);
 
 		PyRef<Ball>::assign (clone->ball, ball.borrowObject ());
 		clone->ball->arena = clone->arena;
 		clone->ball->ball  = clone->arena->ball;
 
 		if (copyCallbacks)
 		{
@@ -1868,26 +1940,39 @@
 		if (PyList_SetItem (list.borrow (), index++, car.newObjectRef ()) < 0)
 			return nullptr;
 	}
 
 	return list.gift ();
 }
 
+PyObject *Arena::GetConfig (Arena *self_) noexcept
+{
+	return ArenaConfig::NewFromArenaConfig (self_->arena->GetArenaConfig ()).giftObject ();
+}
+
 PyObject *Arena::GetBallPrediction (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept
 {
-	static char numTicksKwd[] = "num_ticks";
-	static char tickSkipKwd[] = "tick_skip";
+	static char numStatesKwd[]    = "num_states";
+	static char tickIntervalKwd[] = "tick_interval";
 
-	static char *dict[] = {numTicksKwd, tickSkipKwd, nullptr};
+	static char *dict[] = {numStatesKwd, tickIntervalKwd, nullptr};
 
-	unsigned numTicks = 120;
-	unsigned tickSkip = 1;
-	if (!PyArg_ParseTupleAndKeywords (args_, kwds_, "|II", dict, &numTicks, &tickSkip))
+	unsigned numStates    = 120;
+	unsigned tickInterval = 1;
+	if (!PyArg_ParseTupleAndKeywords (args_, kwds_, "|II", dict, &numStates, &tickInterval))
 		return nullptr;
 
+	if (numStates < 1)
+		return PyErr_Format (PyExc_RuntimeError, "Invalid num_states '%u'\n", numStates);
+
+	if (tickInterval < 1)
+		return PyErr_Format (PyExc_RuntimeError, "Invalid tick_interval '%u'\n", tickInterval);
+
+	auto const numTicks = numStates * tickInterval;
+
 	if (!self_->ballPrediction)
 	{
 		try
 		{
 			self_->ballPrediction = new (std::nothrow) RocketSim::BallPredTracker (self_->arena.get (), numTicks);
 			if (!self_->ballPrediction)
 			{
@@ -1898,48 +1983,36 @@
 		catch (std::exception const &err)
 		{
 			PyErr_SetString (PyExc_RuntimeError, err.what ());
 			return nullptr;
 		}
 	}
 
-	auto const count = numTicks / (tickSkip + 1);
-
-	auto list = PyObjectRef::steal (PyList_New (count));
+	auto list = PyObjectRef::steal (PyList_New (numStates));
 	if (!list)
 		return nullptr;
 
-	if (count == 0)
-		return list.gift ();
-
 	try
 	{
 		if (self_->ballPrediction->predData.capacity () < numTicks)
 			self_->ballPrediction->predData.reserve (numTicks);
 
 		self_->ballPrediction->numPredTicks = numTicks;
 
-		self_->ballPrediction->UpdatePred (self_->arena.get ());
+		self_->ballPrediction->UpdatePredFromArena (self_->arena.get ());
 
-		unsigned index = 0;
-		for (unsigned i = 0; i < self_->ballPrediction->predData.size (); i += tickSkip + 1)
+		auto pred = std::begin (self_->ballPrediction->predData);
+		for (unsigned i = 0; i < numStates; ++i, std::advance (pred, tickInterval))
 		{
-			auto time =
-			    PyObjectRef::stealObject (PyFloat_FromDouble ((self_->arena->tickCount + i) * self_->arena->tickTime));
-			auto state = BallState::NewFromBallState (self_->ballPrediction->predData[i]);
-
-			auto tuple = PyObjectRef::steal (PyTuple_New (2));
-			if (!tuple)
+			auto state = BallState::NewFromBallState (*pred);
+			if (!state)
 				return nullptr;
 
-			PyTuple_SetItem (tuple.borrow (), 0, time.giftObject ());
-			PyTuple_SetItem (tuple.borrow (), 1, state.giftObject ());
-
 			// steals ref
-			if (PyList_SetItem (list.borrow (), index++, tuple.newObjectRef ()) < 0)
+			if (PyList_SetItem (list.borrow (), i, state.giftObject ()) < 0)
 				return nullptr;
 		}
 	}
 	catch (std::exception const &err)
 	{
 		PyErr_SetString (PyExc_RuntimeError, err.what ());
 		return nullptr;
@@ -2002,39 +2075,46 @@
 		gameData (1) = ballLastCarHitId;
 		gameData (2) = self_->blueScore;
 		gameData (3) = self_->orangeScore;
 
 		PyTuple_SetItem (tuple.borrow (), 0, gameData.giftObject ());
 	}
 
+	if (!ensureBoostPadByIndex (self_))
+		return nullptr;
+
+	if (self_->boostPadsByIndex)
 	{
-		auto const &boostPads   = self_->arena->GetBoostPads ();
 		auto const numBoostPads = self_->arena->GetBoostPads ().size ();
 
+		if (self_->boostPadsByIndex->size () != numBoostPads)
+		{
+			PyErr_SetString (PyExc_RuntimeError, "Boost pads size mismatch");
+			return nullptr;
+		}
+
 		auto boostPadState = PyArrayRef (2, numBoostPads);
 		if (!boostPadState)
 			return nullptr;
 
-		auto const &boostMapping = getBoostMapping (self_->arena->gameMode);
-		for (unsigned i = 0; i < numBoostPads; ++i)
+		for (unsigned idx = 0; idx < numBoostPads; ++idx)
 		{
-			auto const &pad = boostPads[i];
-
-			auto const idx = getBoostPadIndex (pad, boostMapping);
-			if (idx < 0)
-				continue; // shouldn't happen
+			auto const pad = self_->boostPadsByIndex->operator[] (idx)->pad;
+			assert (pad);
 
 			auto const inv = numBoostPads - idx - 1;
 
 			boostPadState (0, idx) = pad->_internalState.isActive;
 			boostPadState (1, inv) = pad->_internalState.isActive;
 		}
 
 		PyTuple_SetItem (tuple.borrow (), 1, boostPadState.giftObject ());
 	}
+	else
+		assert (self_->arena->GetBoostPads ().empty ());
 
 	{
 		auto ballState = PyArrayRef (2, 25);
 		if (!ballState)
 			return nullptr;
 
 		auto const ball = self_->arena->ball;
@@ -2524,18 +2604,24 @@
 	static char arenasKwd[] = "arenas";
 	static char ticksKwd[]  = "ticks";
 
 	static char *dict[] = {arenasKwd, ticksKwd, nullptr};
 
 	PyObject *arenas    = nullptr;
 	int ticksToSimulate = 1;
-	if (!PyArg_ParseTupleAndKeywords (args_, kwds_, "|O!i", dict, &PyList_Type, &arenas, &ticksToSimulate))
+	if (!PyArg_ParseTupleAndKeywords (args_, kwds_, "O|i", dict, &arenas, &ticksToSimulate))
 		return nullptr;
 
-	auto const count = PyList_Size (arenas);
+	if (!PySequence_Check (arenas))
+	{
+		PyErr_SetString (PyExc_TypeError, "arenas type must be a sequence");
+		return nullptr;
+	}
+
+	auto const count = PySequence_Size (arenas);
 	if (count == 0)
 		Py_RETURN_NONE;
 
 	std::set<PyRef<Arena>> jobs;
 
 	auto pool = Arena::ThreadPool::GetInstance ();
 	if (!pool)
@@ -2544,15 +2630,15 @@
 		return nullptr;
 	}
 
 	try
 	{
 		for (unsigned i = 0; i < count; ++i)
 		{
-			auto obj = PyList_GetItem (arenas, i);
+			auto obj = PySequence_GetItem (arenas, i);
 			if (!obj)
 				return nullptr;
 
 			if (!Py_IS_TYPE (obj, Arena::Type))
 			{
 				PyErr_SetString (PyExc_RuntimeError, "Unexpected type");
 				return nullptr;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/Array.cpp` & `RocketSim-2.1.1/python-mtheall/Array.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/python-mtheall/Array.h` & `RocketSim-2.1.1/python-mtheall/Array.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/python-mtheall/Ball.cpp` & `RocketSim-2.1.1/python-mtheall/Ball.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/python-mtheall/BallHitInfo.cpp` & `RocketSim-2.1.1/python-mtheall/BallHitInfo.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -239,14 +239,20 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *BallHitInfo::Unpickle (BallHitInfo *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/BallState.cpp` & `RocketSim-2.1.1/python-mtheall/BallState.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -279,14 +279,20 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *BallState::Unpickle (BallState *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/BoostPad.cpp` & `RocketSim-2.1.1/python-mtheall/BoostPad.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/python-mtheall/BoostPadState.cpp` & `RocketSim-2.1.1/python-mtheall/BoostPadState.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,20 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *BoostPadState::Unpickle (BoostPadState *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/Car.cpp` & `RocketSim-2.1.1/python-mtheall/Car.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,20 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *Car::InternalUnpickle (std::shared_ptr<RocketSim::Arena> arena_, Car *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const dummy = PyObjectRef::steal (PyTuple_New (0));
 	if (!dummy)
 		return nullptr;
 
 	static char idKwd[]           = "id";
 	static char teamKwd[]         = "team";
 	static char stateKwd[]        = "state";
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/CarConfig.cpp` & `RocketSim-2.1.1/python-mtheall/CarConfig.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,20 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *CarConfig::Unpickle (CarConfig *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/CarControls.cpp` & `RocketSim-2.1.1/python-mtheall/CarControls.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,20 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *CarControls::Unpickle (CarControls *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/CarState.cpp` & `RocketSim-2.1.1/python-mtheall/CarState.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     {Py_tp_doc, (void *)R"(Car state
 __init__(self
 	pos: RocketSim.Vec = RocketSim.Vec(z = 17.0),
 	rot_mat: RocketSim.RotMat = RocketSim.RotMat(),
 	vel: RocketSim.Vec = RocketSim.Vec(),
 	ang_vel: RocketSim.Vec = RocketSim.Vec(),
 	is_on_ground: bool = True,
-	wheels_with_contact: Tuple[bool] = (false, false, false, false),
+	wheels_with_contact: Sequence[bool] = (false, false, false, false),
 	has_jumped: bool = False,
 	has_double_jumped: bool = False,
 	has_flipped: bool = False,
 	flip_rel_torque: RocketSim.Vec = RocketSim.Vec(),
 	jump_time: float = 0.0,
 	flip_time: float = 0.0,
 	is_flipping: bool = False,
@@ -679,14 +679,20 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *CarState::Unpickle (CarState *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/Module.cpp` & `RocketSim-2.1.1/python-mtheall/Module.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,43 @@
 #include <exception>
 
 namespace
 {
 // No data races due to GIL
 bool inited = false;
 
-RocketSim::Python::PyObjectRef CopyModuleObj;
-RocketSim::Python::PyObjectRef DeepCopyObj;
+PyObject *CopyModuleObj = nullptr;
+PyObject *DeepCopyObj   = nullptr;
 
 bool InitDeepCopy () noexcept
 {
 	if (DeepCopyObj)
 		return true;
 
-	CopyModuleObj = RocketSim::Python::PyObjectRef::steal (PyImport_ImportModule ("copy"));
+	CopyModuleObj = PyImport_ImportModule ("copy");
 	if (!CopyModuleObj)
 		return false;
 
-	DeepCopyObj = RocketSim::Python::PyObjectRef::steal (PyObject_GetAttrString (CopyModuleObj.borrow (), "deepcopy"));
+	DeepCopyObj = PyObject_GetAttrString (CopyModuleObj, "deepcopy");
 	if (!DeepCopyObj)
+	{
+		Py_DECREF (CopyModuleObj);
+		CopyModuleObj = nullptr;
+
 		return false;
+	}
 
-	if (!PyCallable_Check (DeepCopyObj.borrow ()))
+	if (!PyCallable_Check (DeepCopyObj))
 	{
-		DeepCopyObj = {};
+		Py_DECREF (DeepCopyObj);
+		DeepCopyObj = nullptr;
+
+		Py_DECREF (CopyModuleObj);
+		CopyModuleObj = nullptr;
+
 		PyErr_SetString (PyExc_ImportError, "Failed to import copy.deepcopy");
 		return false;
 	}
 
 	return true;
 }
 }
@@ -67,15 +77,15 @@
 	if (!InitDeepCopy ())
 		return nullptr;
 
 	auto args = PyObjectRef::steal (PyTuple_Pack (2, obj_, memo_));
 	if (!args)
 		return nullptr;
 
-	return PyObject_Call (DeepCopyObj.borrow (), args.borrow (), nullptr);
+	return PyObject_Call (DeepCopyObj, args.borrow (), nullptr);
 }
 }
 
 namespace
 {
 PyObject *Init (PyObject *self_, PyObject *args_, PyObject *kwds_) noexcept
 {
@@ -104,16 +114,19 @@
 	}
 
 	Py_RETURN_NONE;
 }
 
 void Free (void *)
 {
+	Py_XDECREF (DeepCopyObj);
+	DeepCopyObj = nullptr;
+
+	Py_XDECREF (CopyModuleObj);
 	CopyModuleObj = nullptr;
-	DeepCopyObj   = nullptr;
 }
 
 struct PyMethodDef Methods[] = {
     {.ml_name     = "init",
         .ml_meth  = (PyCFunction)&Init,
         .ml_flags = METH_VARARGS | METH_KEYWORDS,
         .ml_doc   = R"(init(path: str = os.getenv("RS_COLLISION_MESHES", "collision_meshes"))"},
@@ -159,16 +172,18 @@
 		if (PyModule_AddObject (m.borrow (), #x_, type.borrowObject ()) < 0) /* careful! steals ref on success */      \
 			return nullptr;                                                                                            \
 		RocketSim::Python::x_::Type = type.gift (); /* ref belongs to module now */                                    \
 	} while (0)
 
 	MAKE_TYPE (Angle);
 	MAKE_TYPE (Arena);
+	MAKE_TYPE (ArenaConfig);
 	MAKE_TYPE (Ball);
 	MAKE_TYPE (BallHitInfo);
+	MAKE_TYPE (BallPredictor);
 	MAKE_TYPE (BallState);
 	MAKE_TYPE (BoostPad);
 	MAKE_TYPE (BoostPadState);
 	MAKE_TYPE (Car);
 	MAKE_TYPE (CarConfig);
 	MAKE_TYPE (CarControls);
 	MAKE_TYPE (CarState);
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/Module.h` & `RocketSim-2.1.1/python-mtheall/Module.h`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 #include <Python.h>
 #include <structmember.h>
 
 #include "PyRef.h"
 
 #include "Math/Math.h"
 #include "Sim/Arena/Arena.h"
+#include "Sim/Arena/ArenaConfig/ArenaConfig.h"
 #include "Sim/BallPredTracker/BallPredTracker.h"
 #include "Sim/Car/Car.h"
 #include "Sim/GameEventTracker/GameEventTracker.h"
 
 #include <map>
 #include <memory>
+#include <optional>
 #include <span>
 #include <unordered_map>
 #include <vector>
 
 #ifndef Py_UNREACHABLE
 #ifndef NDEBUG
 #define Py_UNREACHABLE() Py_FatalError ("Unreachable C code path reached")
@@ -93,15 +95,18 @@
 {
 void InitInternal (char const *path_);
 
 bool DictSetValue (PyObject *dict_, char const *key_, PyObject *value_) noexcept;
 
 PyObject *PyDeepCopy (void *obj_, PyObject *memo_) noexcept;
 
+double ToFloat (PyObject *obj_) noexcept;
+
 template <typename T, std::size_t Extent>
+    requires (std::is_same_v<T, bool> || std::is_arithmetic_v<T>)
 bool fromSequence (PyObject *obj_, std::span<T, Extent> span_) noexcept
 {
 	if (!PySequence_Check (obj_))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be a sequence");
 		return false;
 	}
@@ -114,15 +119,35 @@
 
 	for (unsigned i = 0; i < span_.size (); ++i)
 	{
 		auto const obj = PyObjectRef::steal (PySequence_GetItem (obj_, i));
 		if (!obj)
 			return false;
 
-		span_[i] = PyObject_IsTrue (obj.borrow ());
+		if constexpr (std::is_same_v<T, bool>)
+			span_[i] = PyObject_IsTrue (obj.borrow ());
+		else if (std::is_same_v<T, long>)
+			span_[i] = PyLong_AsLong (obj.borrow ());
+		else if constexpr (std::is_same_v<T, long long>)
+			span_[i] = PyLong_AsLongLong (obj.borrow ());
+		else if constexpr (std::is_same_v<T, Py_ssize_t>)
+			span_[i] = PyLong_AsSsize_t (obj.borrow ());
+		else if constexpr (std::is_same_v<T, unsigned long>)
+			span_[i] = PyLong_AsUnsignedLong (obj.borrow ());
+		else if constexpr (std::is_same_v<T, std::size_t>)
+			span_[i] = PyLong_AsSize_t (obj.borrow ());
+		else if constexpr (std::is_same_v<T, unsigned long long>)
+			span_[i] = PyLong_AsUnsignedLongLong (obj.borrow ());
+		else if constexpr (std::is_integral_v<T>)
+			span_[i] = PyLong_AsLong (obj.borrow ());
+		else if constexpr (std::is_floating_point_v<T>)
+			span_[i] = PyFloat_AsDouble (obj.borrow ());
+
+		if (PyErr_Occurred ())
+			return false;
 	}
 
 	return true;
 }
 
 class GIL
 {
@@ -199,14 +224,18 @@
 	static PyObject *Repr (Vec *self_) noexcept;
 	static PyObject *Format (Vec *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *Pickle (Vec *self_) noexcept;
 	static PyObject *Unpickle (Vec *self_, PyObject *dict_) noexcept;
 	static PyObject *Copy (Vec *self_) noexcept;
 	static PyObject *DeepCopy (Vec *self_, PyObject *memo_) noexcept;
 
+	static Py_ssize_t Length (Vec *self_) noexcept;
+	static PyObject *GetItem (Vec *self_, Py_ssize_t index_) noexcept;
+	static int SetItem (Vec *self_, Py_ssize_t index_, PyObject *value_) noexcept;
+
 	static PyObject *AsTuple (Vec *self_) noexcept;
 	static PyObject *AsNumpy (Vec *self_) noexcept;
 	static PyObject *Round (Vec *self_, PyObject *args_, PyObject *kwds_) noexcept;
 };
 
 struct RotMat
 {
@@ -232,14 +261,18 @@
 	static PyObject *Repr (RotMat *self_) noexcept;
 	static PyObject *Format (RotMat *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *Pickle (RotMat *self_) noexcept;
 	static PyObject *Unpickle (RotMat *self_, PyObject *dict_) noexcept;
 	static PyObject *Copy (RotMat *self_) noexcept;
 	static PyObject *DeepCopy (RotMat *self_, PyObject *memo_) noexcept;
 
+	static Py_ssize_t Length (RotMat *self_) noexcept;
+	static PyObject *GetItem (RotMat *self_, Py_ssize_t index_) noexcept;
+	static int SetItem (RotMat *self_, Py_ssize_t index_, PyObject *value_) noexcept;
+
 	static PyObject *AsTuple (RotMat *self_) noexcept;
 	static PyObject *AsAngle (RotMat *self_) noexcept;
 	static PyObject *AsNumpy (RotMat *self_) noexcept;
 
 	GETSET_DECLARE (RotMat, forward)
 	GETSET_DECLARE (RotMat, right)
 	GETSET_DECLARE (RotMat, up)
@@ -267,14 +300,18 @@
 	static PyObject *Repr (Angle *self_) noexcept;
 	static PyObject *Format (Angle *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *Pickle (Angle *self_) noexcept;
 	static PyObject *Unpickle (Angle *self_, PyObject *dict_) noexcept;
 	static PyObject *Copy (Angle *self_) noexcept;
 	static PyObject *DeepCopy (Angle *self_, PyObject *memo_) noexcept;
 
+	static Py_ssize_t Length (Angle *self_) noexcept;
+	static PyObject *GetItem (Angle *self_, Py_ssize_t index_) noexcept;
+	static int SetItem (Angle *self_, Py_ssize_t index_, PyObject *value_) noexcept;
+
 	static PyObject *AsTuple (Angle *self_) noexcept;
 	static PyObject *AsRotMat (Angle *self_) noexcept;
 	static PyObject *AsNumpy (Angle *self_) noexcept;
 };
 
 struct BallHitInfo
 {
@@ -612,14 +649,42 @@
 	static PyObject *GetState (Car *self_) noexcept;
 	static PyObject *GetUpDir (Car *self_) noexcept;
 	static PyObject *Respawn (Car *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *SetControls (Car *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *SetState (Car *self_, PyObject *args_, PyObject *kwds_) noexcept;
 };
 
+struct BallPredictor
+{
+	PyObject_HEAD;
+
+	RocketSim::BallPredTracker tracker;
+
+	static PyTypeObject *Type;
+	static PyMethodDef Methods[];
+	static PyType_Slot Slots[];
+	static PyType_Spec Spec;
+
+	static bool InitFromArena (BallPredictor *self_, RocketSim::Arena *arena_) noexcept;
+	static bool InitFromParams (BallPredictor *self_,
+	    RocketSim::GameMode gameMode_,
+	    RocketSim::ArenaMemWeightMode memoryWeightMode_,
+	    float tickRate_) noexcept;
+
+	static PyObject *New (PyTypeObject *subtype_, PyObject *args_, PyObject *kwds_) noexcept;
+	static int Init (BallPredictor *self_, PyObject *args_, PyObject *kwds_) noexcept;
+	static void Dealloc (BallPredictor *self_) noexcept;
+	static PyObject *Pickle (BallPredictor *self_) noexcept;
+	static PyObject *Unpickle (BallPredictor *self_, PyObject *dict_) noexcept;
+	static PyObject *Copy (BallPredictor *self_) noexcept;
+	static PyObject *DeepCopy (BallPredictor *self_, PyObject *memo_) noexcept;
+
+	static PyObject *GetBallPrediction (BallPredictor *self_, PyObject *args_, PyObject *kwds_) noexcept;
+};
+
 struct MutatorConfig
 {
 	PyObject_HEAD;
 
 	RocketSim::MutatorConfig config;
 	Vec *gravity;
 
@@ -643,14 +708,49 @@
 	static PyObject *Unpickle (MutatorConfig *self_, PyObject *dict_) noexcept;
 	static PyObject *Copy (MutatorConfig *self_) noexcept;
 	static PyObject *DeepCopy (MutatorConfig *self_, PyObject *memo_) noexcept;
 
 	GETSET_DECLARE (MutatorConfig, gravity)
 };
 
+struct ArenaConfig
+{
+	PyObject_HEAD;
+
+	RocketSim::ArenaConfig config;
+
+	Vec *minPos;
+	Vec *maxPos;
+	PyObject *customBigBoostPads;
+	PyObject *customSmallBoostPads;
+
+	static PyTypeObject *Type;
+	static PyMemberDef Members[];
+	static PyMethodDef Methods[];
+	static PyGetSetDef GetSet[];
+	static PyType_Slot Slots[];
+	static PyType_Spec Spec;
+
+	static PyRef<ArenaConfig> NewFromArenaConfig (RocketSim::ArenaConfig const &config_ = {}) noexcept;
+	static bool InitFromArenaConfig (ArenaConfig *self_, RocketSim::ArenaConfig const &config_ = {}) noexcept;
+	static std::optional<RocketSim::ArenaConfig> ToArenaConfig (ArenaConfig *self_) noexcept;
+
+	static PyObject *New (PyTypeObject *subtype_, PyObject *args_, PyObject *kwds_) noexcept;
+	static int Init (ArenaConfig *self_, PyObject *args_, PyObject *kwds_) noexcept;
+	static void Dealloc (ArenaConfig *self_) noexcept;
+	static PyObject *Pickle (ArenaConfig *self_) noexcept;
+	static PyObject *Unpickle (ArenaConfig *self_, PyObject *dict_) noexcept;
+	static PyObject *Copy (ArenaConfig *self_) noexcept;
+	static PyObject *DeepCopy (ArenaConfig *self_, PyObject *memo_) noexcept;
+
+	GETSET_DECLARE (ArenaConfig, memory_weight_mode);
+	GETSET_DECLARE (ArenaConfig, min_pos);
+	GETSET_DECLARE (ArenaConfig, max_pos);
+};
+
 struct Arena
 {
 	class ThreadPool;
 
 	PyObject_HEAD;
 
 	std::shared_ptr<RocketSim::Arena> arena;
@@ -707,14 +807,15 @@
 	static PyObject *AddCar (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *Clone (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *CloneInto (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *GetBallPrediction (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *GetBoostPads (Arena *self_) noexcept;
 	static PyObject *GetCarFromId (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *GetCars (Arena *self_) noexcept;
+	static PyObject *GetConfig (Arena *self_) noexcept;
 	static PyObject *GetGymState (Arena *self_) noexcept;
 	static PyObject *GetMutatorConfig (Arena *self_) noexcept;
 	static PyObject *IsBallProbablyGoingIn (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *RemoveCar (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *ResetKickoff (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *SetBallTouchCallback (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static PyObject *SetBoostPickupCallback (Arena *self_, PyObject *args_, PyObject *kwds_) noexcept;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/MutatorConfig.cpp` & `RocketSim-2.1.1/python-mtheall/MutatorConfig.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,19 @@
         .flags  = 0,
         .doc    = "Enable car-car collision"},
     {.name      = "enable_car_ball_collision",
         .type   = TypeHelper<decltype (RocketSim::MutatorConfig::enableCarBallCollision)>::type,
         .offset = offsetof (MutatorConfig, config) + offsetof (RocketSim::MutatorConfig, enableCarBallCollision),
         .flags  = 0,
         .doc    = "Enable car-ball collision"},
+    {.name      = "goal_base_threshold_y",
+        .type   = TypeHelper<decltype (RocketSim::MutatorConfig::goalBaseThresholdY)>::type,
+        .offset = offsetof (MutatorConfig, config) + offsetof (RocketSim::MutatorConfig, goalBaseThresholdY),
+        .flags  = 0,
+        .doc    = "Goal threshold for soccar"},
     {.name = nullptr, .type = 0, .offset = 0, .flags = 0, .doc = nullptr},
 };
 
 PyMethodDef MutatorConfig::Methods[] = {
     {.ml_name     = "__getstate__",
         .ml_meth  = (PyCFunction)&MutatorConfig::Pickle,
         .ml_flags = METH_NOARGS,
@@ -202,15 +207,16 @@
 	bump_force_scale: float = 1.0,
 	ball_radius: float = <dependent on game_mode>,
 	unlimited_flips: bool = False,
 	unlimited_double_jumps: bool = False,
 	demo_mode: int = RocketSim.DemoMode.NORMAL,
 	enable_team_demos: bool = False,
 	enable_car_car_collision: bool = True,
-	enable_car_ball_collision: bool = True))"},
+	enable_car_ball_collision: bool = True),
+	goal_base_threshold_y: float = 5124.25))"},
     {0, nullptr},
 };
 
 PyType_Spec MutatorConfig::Spec = {
     .name      = "RocketSim.MutatorConfig",
     .basicsize = sizeof (MutatorConfig),
     .itemsize  = 0,
@@ -289,14 +295,15 @@
 	static char ballRadiusKwd[]             = "ball_radius";
 	static char unlimitedFlipsKwd[]         = "unlimited_flips";
 	static char unlimitedDoubleJumpsKwd[]   = "unlimited_double_jumps";
 	static char demoModeKwd[]               = "demo_mode";
 	static char enableTeamDemosKwd[]        = "enable_team_demos";
 	static char enableCarCarCollisionKwd[]  = "enable_car_car_collision";
 	static char enableCarBallCollisionKwd[] = "enable_car_ball_collision";
+	static char goalBaseThresholdYKwd[]     = "goal_base_threshold_y";
 
 	static char *dict[] = {gameModeKwd,
 	    gravityKwd,
 	    carMassKwd,
 	    carWorldFrictionKwd,
 	    carWorldRestitutionKwd,
 	    ballMassKwd,
@@ -318,14 +325,15 @@
 	    ballRadiusKwd,
 	    unlimitedFlipsKwd,
 	    unlimitedDoubleJumpsKwd,
 	    demoModeKwd,
 	    enableTeamDemosKwd,
 	    enableCarCarCollisionKwd,
 	    enableCarBallCollisionKwd,
+	    goalBaseThresholdYKwd,
 	    nullptr};
 
 	int gameMode = static_cast<int> (RocketSim::GameMode::SOCCAR);
 
 	// first pass to get game mode, second pass to fill in if not
 	for (int i = 0; i < 2; ++i)
 	{
@@ -352,15 +360,15 @@
 		int unlimitedDoubleJumps   = config.unlimitedDoubleJumps;
 		int enableTeamDemos        = config.enableTeamDemos;
 		int enableCarCarCollision  = config.enableCarCarCollision;
 		int enableCarBallCollision = config.enableCarBallCollision;
 
 		if (!PyArg_ParseTupleAndKeywords (args_,
 		        kwds_,
-		        "|iO!ffffffffffffffffffffppippp",
+		        "|iO!ffffffffffffffffffffppipppf",
 		        dict,
 		        &gameMode,
 		        Vec::Type,
 		        &gravity,
 		        &config.carMass,
 		        &config.carWorldFriction,
 		        &config.carWorldRestitution,
@@ -382,15 +390,16 @@
 		        &config.bumpForceScale,
 		        &config.ballRadius,
 		        &unlimitedFlips,
 		        &unlimitedDoubleJumps,
 		        &demoMode,
 		        &enableTeamDemos,
 		        &enableCarCarCollision,
-		        &enableCarBallCollision))
+		        &enableCarBallCollision,
+		        &config.goalBaseThresholdY))
 			return -1;
 
 		// try again with parsed game mode
 		if (i == 0 && static_cast<RocketSim::GameMode> (gameMode) != RocketSim::GameMode::SOCCAR)
 			continue;
 
 		config.demoMode = static_cast<RocketSim::DemoMode> (demoMode);
@@ -554,19 +563,29 @@
 	    !DictSetValue (dict.borrow (), "enable_car_car_collision", PyBool_FromLong (config.enableCarCarCollision)))
 		return nullptr;
 
 	if (config.enableCarBallCollision != model.enableCarBallCollision &&
 	    !DictSetValue (dict.borrow (), "enable_car_ball_collision", PyBool_FromLong (config.enableCarBallCollision)))
 		return nullptr;
 
+	if (config.goalBaseThresholdY != model.goalBaseThresholdY &&
+	    !DictSetValue (dict.borrow (), "goal_base_threshold_y", PyFloat_FromDouble (config.goalBaseThresholdY)))
+		return nullptr;
+
 	return dict.gift ();
 }
 
 PyObject *MutatorConfig::Unpickle (MutatorConfig *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/PyRef.h` & `RocketSim-2.1.1/python-mtheall/PyRef.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 #pragma once
 
 #include <Python.h>
 
 #include <cassert>
 #include <cstddef>
 
+// Python 3.9
 #if PY_VERSION_HEX < 0x03090000
 #define Py_IS_TYPE(ob_, type_) ((PyObject const *)(ob_)->ob_type == (PyObject const *)(type_))
 #endif
 
+// Python 3.10
+#if PY_VERSION_HEX < 0x030A0000
+#define Py_Is(x_, y_) ((x_) == (y_))
+#define Py_IsNone(ob_) Py_Is ((ob_), Py_None)
+#endif
+
 namespace RocketSim::Python
 {
 /// \brief PyObject reference wrapper
 template <typename T>
 class PyRef
 {
 public:
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/RotMat.cpp` & `RocketSim-2.1.1/python-mtheall/RotMat.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 PyType_Slot RotMat::Slots[] = {
     {Py_tp_new, (void *)&RotMat::New},
     {Py_tp_init, (void *)&RotMat::Init},
     {Py_tp_dealloc, (void *)&RotMat::Dealloc},
     {Py_tp_repr, (void *)&RotMat::Repr},
     {Py_tp_methods, &RotMat::Methods},
     {Py_tp_getset, &RotMat::GetSet},
+    {Py_sq_length, (void *)&RotMat::Length},
+    {Py_sq_item, (void *)&RotMat::GetItem},
+    {Py_sq_ass_item, (void *)&RotMat::SetItem},
     {Py_tp_doc, (void *)R"(Rotation matrix (3x3)
 __init__(self)
 	Identity matrix
 
 __init__(self,
 	forward_x: float, forward_y: float, forward_z: float,
 	right_x: float, right_y: float, right_z: float,
@@ -245,14 +248,20 @@
 PyObject *RotMat::Pickle (RotMat *self_) noexcept
 {
 	return Py_BuildValue ("{sOsOsO}", "forward", self_->forward, "right", self_->right, "up", self_->up);
 }
 
 PyObject *RotMat::Unpickle (RotMat *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
 
@@ -289,14 +298,61 @@
 	PyRef<Vec>::assign (mat->up, PyDeepCopy (self_->up, memo_));
 	if (!mat->up)
 		return nullptr;
 
 	return mat.giftObject ();
 }
 
+Py_ssize_t RotMat::Length (RotMat *self_) noexcept
+{
+	return 3;
+}
+
+PyObject *RotMat::GetItem (RotMat *self_, Py_ssize_t index_) noexcept
+{
+	switch (index_)
+	{
+	case 0:
+		return Getforward (self_, nullptr);
+
+	case 1:
+		return Getright (self_, nullptr);
+
+	case 2:
+		return Getup (self_, nullptr);
+	}
+
+	PyErr_SetString (PyExc_IndexError, "index out of range");
+	return nullptr;
+}
+
+int RotMat::SetItem (RotMat *self_, Py_ssize_t index_, PyObject *value_) noexcept
+{
+	if (!value_)
+	{
+		PyErr_SetString (PyExc_TypeError, "'RocketSim.RotMat' object doesn't support item deletion");
+		return -1;
+	}
+
+	switch (index_)
+	{
+	case 0:
+		return Setforward (self_, value_, nullptr);
+
+	case 1:
+		return Setright (self_, value_, nullptr);
+
+	case 2:
+		return Setup (self_, value_, nullptr);
+	}
+
+	PyErr_SetString (PyExc_IndexError, "index out of range");
+	return -1;
+}
+
 PyObject *RotMat::Getforward (RotMat *self_, void *) noexcept
 {
 	return PyRef<Vec>::incRef (self_->forward).giftObject ();
 }
 
 int RotMat::Setforward (RotMat *self_, PyObject *value_, void *) noexcept
 {
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/Vec.cpp` & `RocketSim-2.1.1/python-mtheall/Vec.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -69,14 +69,17 @@
     {Py_tp_new, (void *)&Vec::New},
     {Py_tp_init, (void *)&Vec::Init},
     {Py_tp_dealloc, (void *)&Vec::Dealloc},
     {Py_tp_richcompare, (void *)&Vec::RichCompare},
     {Py_tp_repr, (void *)&Vec::Repr},
     {Py_tp_members, &Vec::Members},
     {Py_tp_methods, &Vec::Methods},
+    {Py_sq_length, (void *)&Vec::Length},
+    {Py_sq_item, (void *)&Vec::GetItem},
+    {Py_sq_ass_item, (void *)&Vec::SetItem},
     {Py_tp_doc, (void *)R"(3-dimensional vector
 __init__(self, x: float = 0.0, y: float = 0.0, z: float = 0.0))"},
     {0, nullptr},
 };
 
 PyType_Spec Vec::Spec = {
     .name      = "RocketSim.Vec",
@@ -226,14 +229,20 @@
 		return nullptr;
 
 	return dict.gift ();
 }
 
 PyObject *Vec::Unpickle (Vec *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
 
@@ -246,14 +255,68 @@
 }
 
 PyObject *Vec::DeepCopy (Vec *self_, PyObject *memo_) noexcept
 {
 	return NewFromVec (self_->vec).giftObject ();
 }
 
+Py_ssize_t Vec::Length (Vec *self_) noexcept
+{
+	return 3;
+}
+
+PyObject *Vec::GetItem (Vec *self_, Py_ssize_t index_) noexcept
+{
+	switch (index_)
+	{
+	case 0:
+		return PyFloat_FromDouble (self_->vec.x);
+
+	case 1:
+		return PyFloat_FromDouble (self_->vec.y);
+
+	case 2:
+		return PyFloat_FromDouble (self_->vec.z);
+	}
+
+	PyErr_SetString (PyExc_IndexError, "index out of range");
+	return nullptr;
+}
+
+int Vec::SetItem (Vec *self_, Py_ssize_t index_, PyObject *value_) noexcept
+{
+	if (!value_)
+	{
+		PyErr_SetString (PyExc_TypeError, "'RocketSim.Vec' object doesn't support item deletion");
+		return -1;
+	}
+
+	auto const val = PyFloat_AsDouble (value_);
+	if (val == -1.0 && PyErr_Occurred ())
+		return -1;
+
+	switch (index_)
+	{
+	case 0:
+		self_->vec.x = val;
+		return 0;
+
+	case 1:
+		self_->vec.y = val;
+		return 0;
+
+	case 2:
+		self_->vec.z = val;
+		return 0;
+	}
+
+	PyErr_SetString (PyExc_IndexError, "index out of range");
+	return -1;
+}
+
 PyObject *Vec::AsTuple (Vec *self_) noexcept
 {
 	return Py_BuildValue ("fff", self_->vec.x, self_->vec.y, self_->vec.z);
 }
 
 PyObject *Vec::AsNumpy (Vec *self_) noexcept
 {
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/WheelPairConfig.cpp` & `RocketSim-2.1.1/python-mtheall/WheelPairConfig.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,20 @@
 	    self_->config.suspensionRestLength,
 	    "connection_point_offset",
 	    self_->connectionPointOffset);
 }
 
 PyObject *WheelPairConfig::Unpickle (WheelPairConfig *self_, PyObject *dict_) noexcept
 {
+	if (!PyDict_Check (dict_))
+	{
+		PyErr_SetString (PyExc_ValueError, "Pickled object is not a dict");
+		return nullptr;
+	}
+
 	auto const args = PyObjectRef::steal (PyTuple_New (0));
 	if (!args)
 		return nullptr;
 
 	if (Init (self_, args.borrow (), dict_) != 0)
 		return nullptr;
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/regression_test.py` & `RocketSim-2.1.1/python-mtheall/regression_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import RocketSim as rs
 
 import glm
 import math
 import numpy as np
+import pickle
 import unittest
 
 # simple actor that drives straight toward a target
 def target_chase(target_pos: rs.Vec, car: rs.Car):
   target_pos = glm.vec3(*target_pos.as_tuple())
   car_pos    = glm.vec3(*car.get_state().pos.as_tuple())
   car_fwd    = glm.vec3(*car.get_state().rot_mat.forward.as_tuple())
@@ -239,9 +240,45 @@
       arena.step()
 
       if bumped[0]:
         break
 
     self.assertTrue(bumped[0])
 
+  def test_unpickle_no_boostpads(self):
+    pickle.loads(pickle.dumps(rs.Arena(rs.GameMode.THE_VOID)))
+
+  def test_unpickle_no_cars(self):
+    pickle.loads(pickle.dumps(rs.Arena()))
+
+  def test_unpickle_no_callbacks(self):
+    arena = rs.Arena()
+
+    arena = pickle.loads(pickle.dumps(arena))
+
+    ball = arena.ball
+    car  = arena.add_car(rs.Team.BLUE)
+
+    # trigger the ball touch callback
+    for i in range(1000):
+      target_chase(ball.get_state().pos, car)
+      arena.step()
+
+  def test_arena_ball_prediction(self):
+    arena = rs.Arena()
+    arena.get_ball_prediction(4, 2)
+
+  def test_soccar_wall(self):
+    arena = rs.Arena()
+    ball_state = arena.ball.get_state()
+    ball_state.vel = rs.Vec(2000.0, 0.0, 0.0)
+    arena.ball.set_state(ball_state)
+
+    radius = arena.ball.get_radius()
+
+    for i in range(1000):
+      arena.step()
+      x = arena.ball.get_state().pos.x
+      self.assertLess(x + radius, 4096)
+
 if __name__ == "__main__":
   unittest.main()
```

### Comparing `RocketSim-2.1.0a6/python-mtheall/unit_test.py` & `RocketSim-2.1.1/python-mtheall/unit_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 def pickled(v):
   return pickle.loads(pickle.dumps(v))
 
 def random_bool() -> bool:
   return random.randint(0, 1) == 1
 
-def random_int() -> bool:
+def random_int() -> int:
   return random.randint(1, 1000)
 
-def random_float() -> float:
-  return random.uniform(-1.0, 1.0)
+def random_float(lo=-1.0, hi=1.0) -> float:
+  return random.uniform(lo, hi)
 
-def random_vec() -> rs.Vec:
-  return rs.Vec(random_float(), random_float(), random_float())
+def random_vec(lo=-1.0, hi=1.0) -> rs.Vec:
+  return rs.Vec(random_float(lo, hi), random_float(lo, hi), random_float(lo, hi))
 
 def random_mat() -> rs.RotMat:
   return rs.RotMat(random_vec(), random_vec(), random_vec())
 
 def random_angle() -> rs.Vec:
   return rs.Angle(random_float(), random_float(), random_float())
 
@@ -342,26 +342,28 @@
     )
 
     info_b = pickled(info_a)
 
     self.compare(info_a, info_b)
 
 class TestBallState(FuzzyTestCase):
-  def compare(self, state_a, state_b):
+  def compare(self, state_a, state_b, check_update_counter = True):
     self.assertAlmostEqual(state_a.pos,                 state_b.pos, 3)
     self.assertEqual(state_a.rot_mat.forward,           state_b.rot_mat.forward)
     self.assertEqual(state_a.rot_mat.right,             state_b.rot_mat.right)
     self.assertEqual(state_a.rot_mat.up,                state_b.rot_mat.up)
     self.assertAlmostEqual(state_a.vel,                 state_b.vel, 3)
     self.assertEqual(state_a.ang_vel,                   state_b.ang_vel)
     self.assertEqual(state_a.heatseeker_target_dir,     state_b.heatseeker_target_dir)
     self.assertEqual(state_a.heatseeker_target_speed,   state_b.heatseeker_target_speed)
     self.assertEqual(state_a.heatseeker_time_since_hit, state_b.heatseeker_time_since_hit)
     self.assertEqual(state_a.last_hit_car_id,           state_b.last_hit_car_id)
-    self.assertEqual(state_a.update_counter,            state_b.update_counter)
+
+    if check_update_counter:
+      self.assertEqual(state_a.update_counter, state_b.update_counter)
 
   def compare_direct(self, state, pos, vel, ang_vel, car_id):
     self.assertEqual(state.pos, pos)
     self.assertEqual(state.vel, vel)
     self.assertEqual(state.ang_vel, ang_vel)
     self.assertEqual(state.last_hit_car_id, car_id)
 
@@ -985,14 +987,35 @@
       arena.step()
       if len(demo_pos):
         state = car_b.get_state()
         self.assertEqual(state.pos, demo_pos[0])
 
     self.assertNotEqual(len(demo_pos), 0)
 
+class TestBallPredictor(FuzzyTestCase):
+  def test_ball_predictor(self):
+    pred = rs.BallPredictor()
+
+    for skip in range(1, 9):
+      state = rs.BallState(
+        pos             = random_vec(),
+        vel             = random_vec(),
+        ang_vel         = random_vec(),
+        last_hit_car_id = random_int(),
+        update_counter  = random_int()
+      )
+
+      states = pred.get_ball_prediction(state, 0, 10, skip)
+      for i in range(len(states)):
+        s = pred.get_ball_prediction(states[i], skip, 10, skip)
+        j = i
+        while j < len(states) and j - i < len(s):
+          TestBallState.compare(self, states[j], s[j - i], False)
+          j += 1
+
 class TestMutatorConfig(FuzzyTestCase):
   def compare(self, config_a, config_b):
     self.assertEqual(config_a.gravity,                    config_b.gravity)
     self.assertEqual(config_a.car_mass,                   config_b.car_mass)
     self.assertEqual(config_a.car_world_friction,         config_b.car_world_friction)
     self.assertEqual(config_a.car_world_restitution,      config_b.car_world_restitution)
     self.assertEqual(config_a.ball_mass,                  config_b.ball_mass)
@@ -1014,24 +1037,19 @@
     self.assertEqual(config_a.ball_radius,                config_b.ball_radius)
     self.assertEqual(config_a.unlimited_flips,            config_b.unlimited_flips)
     self.assertEqual(config_a.unlimited_double_jumps,     config_b.unlimited_double_jumps)
     self.assertEqual(config_a.demo_mode,                  config_b.demo_mode)
     self.assertEqual(config_a.enable_team_demos,          config_b.enable_team_demos)
     self.assertEqual(config_a.enable_car_car_collision,   config_b.enable_car_car_collision)
     self.assertEqual(config_a.enable_car_ball_collision,  config_b.enable_car_ball_collision)
+    self.assertEqual(config_a.goal_base_threshold_y,      config_b.goal_base_threshold_y)
 
-  def test_basic(self):
-    config = rs.MutatorConfig(rs.GameMode.SOCCAR)
-    config = rs.MutatorConfig(rs.GameMode.HOOPS)
-    config = rs.MutatorConfig(rs.GameMode.HEATSEEKER)
-    config = rs.MutatorConfig(rs.GameMode.SNOWDAY)
-    config = rs.MutatorConfig(rs.GameMode.THE_VOID)
-
-  def test_pickle(self):
-    config_a = rs.MutatorConfig(
+  @staticmethod
+  def random():
+    return rs.MutatorConfig(
       gravity                    = random_vec(),
       car_mass                   = random_float(),
       car_world_friction         = random_float(),
       car_world_restitution      = random_float(),
       ball_mass                  = random_float(),
       ball_max_speed             = random_float(),
       ball_drag                  = random_float(),
@@ -1050,91 +1068,223 @@
       bump_force_scale           = random_float(),
       ball_radius                = random_float(),
       unlimited_flips            = random_bool(),
       unlimited_double_jumps     = random_bool(),
       demo_mode                  = random.randint(0, 2),
       enable_team_demos          = random_bool(),
       enable_car_car_collision   = random_bool(),
-      enable_car_ball_collision  = random_bool()
+      enable_car_ball_collision  = random_bool(),
+      goal_base_threshold_y      = random_float()
     )
+
+  def test_basic(self):
+    config = rs.MutatorConfig(rs.GameMode.SOCCAR)
+    config = rs.MutatorConfig(rs.GameMode.HOOPS)
+    config = rs.MutatorConfig(rs.GameMode.HEATSEEKER)
+    config = rs.MutatorConfig(rs.GameMode.SNOWDAY)
+    config = rs.MutatorConfig(rs.GameMode.THE_VOID)
+
+  def test_pickle(self):
+    config_a = TestMutatorConfig.random()
     config_b = pickled(config_a)
 
     self.assertIsNot(config_a.gravity, config_b.gravity)
     self.compare(config_a, config_b)
 
   def test_copy(self):
-    config_a = rs.MutatorConfig(
-      gravity                    = random_vec(),
-      car_mass                   = random_float(),
-      car_world_friction         = random_float(),
-      car_world_restitution      = random_float(),
-      ball_mass                  = random_float(),
-      ball_max_speed             = random_float(),
-      ball_drag                  = random_float(),
-      ball_world_friction        = random_float(),
-      ball_world_restitution     = random_float(),
-      jump_accel                 = random_float(),
-      jump_immediate_force       = random_float(),
-      boost_accel                = random_float(),
-      boost_used_per_second      = random_float(),
-      respawn_delay              = random_float(),
-      bump_cooldown_time         = random_float(),
-      boost_pad_cooldown_big     = random_float(),
-      boost_pad_cooldown_small   = random_float(),
-      car_spawn_boost_amount     = random_float(),
-      ball_hit_extra_force_scale = random_float(),
-      bump_force_scale           = random_float(),
-      ball_radius                = random_float(),
-      unlimited_flips            = random_bool(),
-      unlimited_double_jumps     = random_bool(),
-      demo_mode                  = random.randint(0, 2),
-      enable_team_demos          = random_bool(),
-      enable_car_car_collision   = random_bool(),
-      enable_car_ball_collision  = random_bool()
-    )
+    config_a = TestMutatorConfig.random()
     config_b = copy.copy(config_a)
 
     self.assertIs(config_a.gravity, config_b.gravity)
     self.compare(config_a, config_b)
 
   def test_deep_copy(self):
-    config_a = rs.MutatorConfig(
-      gravity                    = random_vec(),
-      car_mass                   = random_float(),
-      car_world_friction         = random_float(),
-      car_world_restitution      = random_float(),
-      ball_mass                  = random_float(),
-      ball_max_speed             = random_float(),
-      ball_drag                  = random_float(),
-      ball_world_friction        = random_float(),
-      ball_world_restitution     = random_float(),
-      jump_accel                 = random_float(),
-      jump_immediate_force       = random_float(),
-      boost_accel                = random_float(),
-      boost_used_per_second      = random_float(),
-      respawn_delay              = random_float(),
-      bump_cooldown_time         = random_float(),
-      boost_pad_cooldown_big     = random_float(),
-      boost_pad_cooldown_small   = random_float(),
-      car_spawn_boost_amount     = random_float(),
-      ball_hit_extra_force_scale = random_float(),
-      bump_force_scale           = random_float(),
-      ball_radius                = random_float(),
-      unlimited_flips            = random_bool(),
-      unlimited_double_jumps     = random_bool(),
-      demo_mode                  = random.randint(0, 2),
-      enable_team_demos          = random_bool(),
-      enable_car_car_collision   = random_bool(),
-      enable_car_ball_collision  = random_bool()
-    )
+    config_a = TestMutatorConfig.random()
     config_b = copy.deepcopy(config_a)
-
     self.assertIsNot(config_a.gravity, config_b.gravity)
     self.compare(config_a, config_b)
 
+class TestArenaConfig(FuzzyTestCase):
+  def compare(self, config_a, config_b):
+    self.assertEqual(config_a.memory_weight_mode,    config_b.memory_weight_mode)
+    self.assertEqual(config_a.min_pos,               config_a.min_pos)
+    self.assertEqual(config_a.max_pos,               config_a.max_pos)
+    self.assertEqual(config_a.max_aabb_len,          config_a.max_aabb_len)
+    self.assertEqual(config_a.no_ball_rot,           config_a.no_ball_rot)
+    self.assertEqual(config_a.use_custom_broadphase, config_a.use_custom_broadphase)
+    self.assertEqual(config_a.max_objects,           config_a.max_objects)
+
+    if config_a.custom_big_boost_pads is None and config_a.custom_small_boost_pads is None:
+      self.assertIsNone(config_b.custom_big_boost_pads)
+      self.assertIsNone(config_b.custom_small_boost_pads)
+    else:
+      if not config_a.custom_big_boost_pads is None:
+        self.assertEqual(len(config_a.custom_big_boost_pads), len(config_b.custom_big_boost_pads))
+        for a, b in zip(config_a.custom_big_boost_pads, config_b.custom_big_boost_pads):
+          self.assertEqual(a, b)
+
+      if not config_a.custom_small_boost_pads is None:
+        self.assertEqual(len(config_a.custom_small_boost_pads), len(config_b.custom_small_boost_pads))
+        for a, b in zip(config_a.custom_small_boost_pads, config_b.custom_small_boost_pads):
+          self.assertEqual(a, b)
+
+  @staticmethod
+  def random():
+    a = random_vec(-5000.0, -4000.0)
+    b = rs.Vec(abs(a.x), abs(a.y), abs(a.z))
+    return rs.ArenaConfig(
+      memory_weight_mode = random.randint (0, 1),
+      min_pos = a,
+      max_pos = b,
+      max_aabb_len = random.uniform(400.0, 500.0),
+      no_ball_rot = random_bool(),
+      use_custom_broadphase = random_bool(),
+      max_objects = random_int()
+    )
+
+  def test_basic(self):
+    config = rs.ArenaConfig()
+
+    for i in range(100):
+      config = TestArenaConfig.random()
+      arena = rs.Arena(config=config)
+      self.compare(config, arena.get_config())
+
+  def test_custom_boost_pads(self):
+    for i in range(10):
+      config = TestArenaConfig.random()
+
+      if random_bool():
+        config.custom_big_boost_pads = [random_vec(-4000, 4000) for i in range(random.randint(0, 3))]
+
+      if random_bool():
+        config.custom_small_boost_pads = [random_vec(-4000, 4000) for i in range(random.randint(0, 3))]
+
+      arena = rs.Arena(config=config)
+
+      # make sure this doesn't throw any errors
+      arena.get_gym_state()
+
+      if config.custom_big_boost_pads is None and config.custom_small_boost_pads is None:
+        continue
+
+      big   = config.custom_big_boost_pads or []
+      small = config.custom_small_boost_pads or []
+
+      pads = arena.get_boost_pads()
+      self.assertEqual(len(pads), len(big) + len(small))
+
+      for a, b in zip(pads, big + small):
+        self.assertEqual(a.get_pos(), b)
+
+    config = TestArenaConfig.random()
+    config.custom_big_boost_pads   = [rs.Vec(-2000.0, -2000.0, 73.0)]
+    config.custom_small_boost_pads = [rs.Vec( 2000.0,  2000.0, 70.0)]
+
+    arena = rs.Arena(config=config)
+    car = arena.add_car(rs.Team.BLUE)
+    arena.reset_kickoff(seed=999)
+
+    # drive toward the big boost but deplete
+    while car.get_state().boost > 0:
+      target_chase(config.custom_small_boost_pads[0], car)
+      arena.step()
+
+    # grab the big boost
+    for i in range(1000):
+      target_chase(config.custom_big_boost_pads[0], car)
+      arena.step()
+      if car.get_state().boost > 0:
+        break
+
+    self.assertEqual(car.get_state().boost, 100)
+
+    # drive toward the small boost but deplete
+    while car.get_state().boost > 0:
+      target_chase(config.custom_small_boost_pads[0], car)
+      arena.step()
+
+    # grab the small boost
+    for i in range(1000):
+      target_chase(config.custom_small_boost_pads[0], car)
+      arena.step()
+      if car.get_state().boost > 0:
+        break
+
+    self.assertEqual(car.get_state().boost, 12)
+
+  def test_pickle(self):
+    for i in range(10):
+      config_a = TestArenaConfig.random()
+      config_b = pickled(config_a)
+      self.assertIsNot(config_a.min_pos, config_b.min_pos)
+      self.assertIsNot(config_a.max_pos, config_b.max_pos)
+      self.compare(config_a, config_b)
+
+      if random_bool():
+        config_a.custom_big_boost_pads = [random_vec() for i in range(random_int())]
+
+      if random_bool():
+        config_a.custom_small_boost_pads = [random_vec() for i in range(random_int())]
+
+      config_b = pickled(config_a)
+      self.assertIsNot(config_a.min_pos, config_b.min_pos)
+      self.assertIsNot(config_a.max_pos, config_b.max_pos)
+      if not config_a.custom_big_boost_pads is None:
+        self.assertIsNot(config_a.custom_big_boost_pads, config_b.custom_big_boost_pads)
+      if not config_a.custom_small_boost_pads is None:
+        self.assertIsNot(config_a.custom_small_boost_pads, config_b.custom_small_boost_pads)
+      self.compare(config_a, config_b)
+
+  def test_copy(self):
+    for i in range(10):
+      config_a = TestArenaConfig.random()
+      config_b = copy.copy(config_a)
+      self.assertIs(config_a.min_pos, config_b.min_pos)
+      self.assertIs(config_a.max_pos, config_b.max_pos)
+      self.compare(config_a, config_b)
+
+      if random_bool():
+        config_a.custom_big_boost_pads = [random_vec() for i in range(random_int())]
+
+      if random_bool():
+        config_a.custom_small_boost_pads = [random_vec() for i in range(random_int())]
+
+      config_b = copy.copy(config_a)
+      self.assertIs(config_a.min_pos, config_b.min_pos)
+      self.assertIs(config_a.max_pos, config_b.max_pos)
+      if not config_a.custom_big_boost_pads is None:
+        self.assertIs(config_a.custom_big_boost_pads, config_b.custom_big_boost_pads)
+      if not config_a.custom_small_boost_pads is None:
+        self.assertIs(config_a.custom_small_boost_pads, config_b.custom_small_boost_pads)
+      self.compare(config_a, config_b)
+
+  def test_deep_copy(self):
+    for i in range(10):
+      config_a = TestArenaConfig.random()
+      config_b = copy.deepcopy(config_a)
+      self.assertIsNot(config_a.min_pos, config_b.min_pos)
+      self.assertIsNot(config_a.max_pos, config_b.max_pos)
+      self.compare(config_a, config_b)
+
+      if random_bool():
+        config_a.custom_big_boost_pads = [random_vec() for i in range(random_int())]
+
+      if random_bool():
+        config_a.custom_small_boost_pads = [random_vec() for i in range(random_int())]
+
+      config_b = copy.deepcopy(config_a)
+      self.assertIsNot(config_a.min_pos, config_b.min_pos)
+      self.assertIsNot(config_a.max_pos, config_b.max_pos)
+      if not config_a.custom_big_boost_pads is None:
+        self.assertIsNot(config_a.custom_big_boost_pads, config_b.custom_big_boost_pads)
+      if not config_a.custom_small_boost_pads is None:
+        self.assertIsNot(config_a.custom_small_boost_pads, config_b.custom_small_boost_pads)
+      self.compare(config_a, config_b)
+
 class TestArena(FuzzyTestCase):
   def compare(self, arena_a, arena_b):
     self.assertEqual(arena_a.game_mode,    arena_b.game_mode)
     self.assertEqual(arena_a.tick_time,    arena_b.tick_time)
     self.assertEqual(arena_a.tick_count,   arena_b.tick_count)
     self.assertEqual(arena_a.blue_score,   arena_b.blue_score)
     self.assertEqual(arena_a.orange_score, arena_b.orange_score)
@@ -1432,18 +1582,20 @@
       arena = rs.Arena(mode)
 
       ball_state = arena.ball.get_state()
       ball_state.vel = rs.Vec(x=500.0, y=500.0, z=500.0)
       arena.ball.set_state(ball_state)
 
       pred = arena.get_ball_prediction()
-      self.assertEqual(len(pred), 60)
+      self.assertEqual(len(pred), 120)
+      TestBallState.compare(self, pred[0], arena.ball.get_state())
 
-      pred = arena.get_ball_prediction(num_ticks=240, tick_skip=0)
-      self.assertEqual(len(pred), 240)
+      pred = arena.get_ball_prediction(num_states=50, tick_interval=3)
+      self.assertEqual(len(pred), 50)
+      TestBallState.compare(self, pred[0], arena.ball.get_state())
 
   def test_clone(self):
     for mode in (rs.GameMode.SOCCAR, rs.GameMode.HOOPS, rs.GameMode.HEATSEEKER, rs.GameMode.SNOWDAY, rs.GameMode.THE_VOID):
       arena = rs.Arena(mode)
 
       for i in range(4):
         random_car(arena, rs.Team.BLUE)
```

### Comparing `RocketSim-2.1.0a6/setup.py` & `RocketSim-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,13 +84,13 @@
     ("NO_IMPORT_ARRAY", "1"),
     ("RS_DONT_LOG", "1")
   ]
 )
 
 setup(
   name = "RocketSim",
-  version = "2.1.0a6",
+  version = "2.1.1",
   description = "This is Rocket League!",
   cmdclass = {"build_ext": build_ext_ex},
   ext_modules = [RocketSim],
   install_requires = ["numpy"]
 )
```

### Comparing `RocketSim-2.1.0a6/src/CollisionMeshFile/CollisionMeshFile.cpp` & `RocketSim-2.1.1/src/CollisionMeshFile/CollisionMeshFile.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 #include "../../libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h"
 #include "../../libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h"
 #include "../../libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h"
 
 RS_NS_START
 
-void CollisionMeshFile::ReadFromFile(std::string filePath) {
-	constexpr char ERROR_PREFIX_STR[] = " > CollisionMeshFile::ReadFromFile(): ";
-
-	DataStreamIn in = DataStreamIn(filePath, false);
+void CollisionMeshFile::ReadFromStream(DataStreamIn& in, std::string filePath) {
+	constexpr char ERROR_PREFIX_STR[] = " > CollisionMeshFile::ReadFromStream(): ";
 
+	// If you have more verts or tris then this, I have no idea what you are doing, godspeed
 	constexpr int MAX_VERT_OR_TRI_COUNT = 1000 * 1000;
 
 	// Read triangle/vertex counts
 	int32_t numTris, numVertices;
 	in.Read(numTris);
 	in.Read(numVertices);
```

### Comparing `RocketSim-2.1.0a6/src/CollisionMeshFile/CollisionMeshFile.h` & `RocketSim-2.1.1/src/CollisionMeshFile/CollisionMeshFile.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #pragma once
 #include "../Framework.h"
 #include "../BulletLink.h"
 
+#include "../DataStream/DataStreamIn.h"
+
 #define COLLISION_MESH_BASE_PATH "./collision_meshes/"
 #define COLLISION_MESH_FILE_EXTENSION ".cmf"
 
 class btTriangleMesh;
 
 RS_NS_START
 
@@ -26,13 +28,13 @@
 	};
 
 	std::vector<Triangle> tris;
 	std::vector<Vertex> vertices;
 
 	uint32_t hash;
 
-	void ReadFromFile(std::string filePath);
+	void ReadFromStream(DataStreamIn& in, std::string filePath = "<NO FILE PATH>");
 	btTriangleMesh* MakeBulletMesh();
 	void UpdateHash();
 };
 
 RS_NS_END
```

### Comparing `RocketSim-2.1.0a6/src/DataStream/DataStreamIn.h` & `RocketSim-2.1.1/src/DataStream/DataStreamIn.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/DataStream/DataStreamOut.h` & `RocketSim-2.1.1/src/DataStream/DataStreamOut.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Framework.h` & `RocketSim-2.1.1/src/Framework.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #pragma once
 
-#define RS_VERSION "pre-2.1.0"
+#define RS_VERSION "2.1.1"
 
 #include <cstdint>
 #include <cstdlib>
 #include <iostream>
 #include <string>
 #include <vector>
 #include <algorithm>
@@ -102,7 +102,10 @@
 	for (int i = 0; i < sizeof(RS_VERSION); i++)
 		result = RS_MAX(RS_VERSION[i] - '0' + 1, 0) + (result*10);
 	return result;
 }
 #define RS_VERSION_ID (__RS_GET_VERSION_ID())
 
 #define RS_IS_BIG_ENDIAN (std::endian::native == std::endian::big)
+
+// TODO: Remove more permanently
+#define RS_NO_SUSPCOLGRID
```

### Comparing `RocketSim-2.1.0a6/src/Math/Math.cpp` & `RocketSim-2.1.1/src/Math/Math.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Math/Math.h` & `RocketSim-2.1.1/src/Math/Math.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Math/MathTypes/MathTypes.cpp` & `RocketSim-2.1.1/src/Math/MathTypes/MathTypes.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Math/MathTypes/MathTypes.h` & `RocketSim-2.1.1/src/Math/MathTypes/MathTypes.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/RLConst.h` & `RocketSim-2.1.1/src/RLConst.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/RocketSim.cpp` & `RocketSim-2.1.1/src/RocketSim.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -65,76 +65,110 @@
 		return suspColGrids_soccar[isLight];
 	}
 }
 #endif
 
 void RocketSim::Init(std::filesystem::path collisionMeshesFolder) {
 
+	std::map<GameMode, std::vector<FileData>> meshFileMap = {};
+
+	for (int i = 0; i < 2; i++) { // Load collision meshes for soccar and hoops
+		GameMode gameMode = (i > 0) ? GameMode::HOOPS : GameMode::SOCCAR;
+		auto& meshes = GetArenaCollisionShapes(gameMode);
+
+		std::filesystem::path basePath = collisionMeshesFolder;
+		std::filesystem::path soccarMeshesFolder = basePath / GAMEMODE_STRS[(int)gameMode];
+
+		if (!std::filesystem::exists(soccarMeshesFolder))
+			continue;
+
+		MeshHashSet targetHashes = MeshHashSet(gameMode);
+
+		// Load collision meshes
+		auto dirItr = std::filesystem::directory_iterator(soccarMeshesFolder);
+		for (auto& entry : dirItr) {
+			auto entryPath = entry.path();
+			if (entryPath.has_extension() && entryPath.extension() == COLLISION_MESH_FILE_EXTENSION) {
+				DataStreamIn streamIn = DataStreamIn(entryPath, false);
+				meshFileMap[gameMode].push_back(streamIn.data);
+			}
+		}
+	}
+
+	RocketSim::InitFromMem(meshFileMap);
+
+	_collisionMeshesFolder = collisionMeshesFolder;
+}
+
+void RocketSim::InitFromMem(const std::map<GameMode, std::vector<FileData>>& meshFilesMap) {
+
 	constexpr char MSG_PREFIX[] = "RocketSim::Init(): ";
 
+	_collisionMeshesFolder = "<MESH FILES LOADED FROM MEMORY>";
+
 	_beginInitMutex.lock();
 	{
 		if (stage != RocketSimStage::UNINITIALIZED) {
 			RS_WARN("RocketSim::Init() called again after already initialized, ignoring...");
 			_beginInitMutex.unlock();
 			return;
 		}
 
 		RS_LOG("Initializing RocketSim version " RS_VERSION ", created by ZealanL...");
 
-		_collisionMeshesFolder = collisionMeshesFolder;
+		
 		stage = RocketSimStage::INITIALIZING;
 
 		uint64_t startMS = RS_CUR_MS();
 
-		for (int i = 0; i < 2; i++) { // Load collision meshes for soccar and hoops
-			GameMode gameMode = (i > 0) ? GameMode::HOOPS : GameMode::SOCCAR;
-			auto& meshes = GetArenaCollisionShapes(gameMode);
-
-			std::filesystem::path basePath = collisionMeshesFolder;
-			std::filesystem::path soccarMeshesFolder = basePath / GAMEMODE_STRS[(int)gameMode];
+		for (auto& mapPair : meshFilesMap) { // Load collision meshes for soccar and hoops
+			GameMode gameMode = mapPair.first;
+			auto& meshFiles = mapPair.second;
 
-			RS_LOG("Loading arena meshes from " << soccarMeshesFolder << "...");
+			RS_LOG("Loading arena meshes for " << GAMEMODE_STRS[(int)gameMode] << "...");
 
-			if (!std::filesystem::exists(soccarMeshesFolder)) {
-				RS_LOG("No arena meshes for " << GAMEMODE_STRS[(int)gameMode] << ", skipping...");
+			if (meshFiles.empty()) {
+				RS_LOG(" > No meshes, skipping");
 				continue;
 			}
 
+			auto& meshes = GetArenaCollisionShapes(gameMode);
+
 			MeshHashSet targetHashes = MeshHashSet(gameMode);
 
 			// Load collision meshes
-			auto dirItr = std::filesystem::directory_iterator(soccarMeshesFolder);
-			for (auto& entry : dirItr) {
-				auto entryPath = entry.path();
-				if (entryPath.has_extension() && entryPath.extension() == COLLISION_MESH_FILE_EXTENSION) {
-					CollisionMeshFile meshFile = {};
-					meshFile.ReadFromFile(entryPath.string());
-					int& hashCount = targetHashes[meshFile.hash];
-
-					if (hashCount > 0) {
-						RS_WARN(MSG_PREFIX << "Collision mesh " << entryPath << " is a duplicate (0x" << std::hex << meshFile.hash << "), " <<
-							"already loaded a mesh with the same hash."
-						);
-					} else if (targetHashes.hashes.count(meshFile.hash) == 0) {
-						RS_WARN(MSG_PREFIX <<
-							"Collision mesh " << entryPath << " does not match any known soccar collision file (0x" << std::hex << meshFile.hash << "), " <<
-							"make sure they were dumped from a normal soccar arena."
-						)
-					}
-					hashCount++;
-
-					btTriangleMesh* triMesh = meshFile.MakeBulletMesh();
-
-					auto bvtMesh = new btBvhTriangleMeshShape(triMesh, true);
-					btTriangleInfoMap* infoMap = new btTriangleInfoMap();
-					btGenerateInternalEdgeInfo(bvtMesh, infoMap);
-					bvtMesh->setTriangleInfoMap(infoMap);
-					meshes.push_back(bvtMesh);
+			int idx = 0;
+			for (auto& entry : meshFiles) {
+				DataStreamIn dataStream = {};
+				dataStream.data = entry;
+				CollisionMeshFile meshFile = {};
+				meshFile.ReadFromStream(dataStream);
+				int& hashCount = targetHashes[meshFile.hash];
+
+				if (hashCount > 0) {
+					RS_WARN(MSG_PREFIX << "Collision mesh [" << idx << "] is a duplicate (0x" << std::hex << meshFile.hash << "), " <<
+						"already loaded a mesh with the same hash."
+					);
+				} else if (targetHashes.hashes.count(meshFile.hash) == 0) {
+					RS_WARN(MSG_PREFIX <<
+						"Collision mesh [" << idx << "] does not match any known " << GAMEMODE_STRS[(int)gameMode] << " collision mesh (0x" << std::hex << meshFile.hash << "), " <<
+						"make sure they were dumped from a normal " << GAMEMODE_STRS[(int)gameMode] << " arena."
+					)
 				}
+				hashCount++;
+
+				btTriangleMesh* triMesh = meshFile.MakeBulletMesh();
+
+				auto bvtMesh = new btBvhTriangleMeshShape(triMesh, true);
+				btTriangleInfoMap* infoMap = new btTriangleInfoMap();
+				btGenerateInternalEdgeInfo(bvtMesh, infoMap);
+				bvtMesh->setTriangleInfoMap(infoMap);
+				meshes.push_back(bvtMesh);
+
+				idx++;
 			}
 		}
 
 		RS_LOG(MSG_PREFIX << "Finished loading arena collision meshes:");
 		RS_LOG(" > Soccar: " << GetArenaCollisionShapes(GameMode::SOCCAR).size());
 		RS_LOG(" > Hoops: " << GetArenaCollisionShapes(GameMode::HOOPS).size());
 
@@ -147,16 +181,16 @@
 				if (!meshes.empty()) {
 					RS_LOG("Building collision suspension grids from " << GAMEMODE_STRS[(int)gameMode] << " arena meshes...");
 
 					for (int j = 0; j < 2; j++) {
 						auto& grid = GetDefaultSuspColGrid(gameMode, j);
 						grid.Allocate();
 						grid.SetupWorldCollision(meshes);
-					}
-				}
+	}
+}
 			}
 		}
 #endif
 
 		uint64_t elapsedMS = RS_CUR_MS() - startMS;
 		RS_LOG("Finished initializing RocketSim in " << (elapsedMS / 1000.f) << "s!");
```

### Comparing `RocketSim-2.1.0a6/src/RocketSim.h` & `RocketSim-2.1.1/src/RocketSim.h`

 * *Files 19% similar despite different names*

```diff
@@ -16,18 +16,27 @@
 namespace RocketSim {
 	enum class RocketSimStage : byte {
 		UNINITIALIZED,
 		INITIALIZING,
 		INITIALIZED
 	};
 
+	typedef std::vector<byte> FileData;
+
 	extern std::filesystem::path _collisionMeshesFolder;
 	extern std::mutex _beginInitMutex;
 
+	
 	void Init(std::filesystem::path collisionMeshesFolder);
+
+	// Instead of loading a collision meshes folder, you can pass in the meshes in this memory-only format
+	// The map sorts mesh files to their respective game modes, where each game mode has a list of mesh files
+	// The mesh files themselves are just byte arrays
+	void InitFromMem(const std::map<GameMode, std::vector<FileData>>& meshFilesMap);
+
 	void AssertInitialized(const char* errorMsgPrefix);
 
 	RocketSimStage GetStage();
 
 	std::vector<btBvhTriangleMeshShape*>& GetArenaCollisionShapes(GameMode gameMode);
 
 #ifndef RS_NO_SUSPCOLGRID
```

### Comparing `RocketSim-2.1.0a6/src/Sim/Arena/Arena.cpp` & `RocketSim-2.1.1/src/Sim/Arena/Arena.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 #include "Arena.h"
 #include "../../RocketSim.h"
 
+#include "../../../libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btAxisSweep3.h"
+#include "../../../libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h"
+#include "../../../libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btSimpleBroadphase.h"
+#include "../../../libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btRSBroadphase.h"
+#include "../../../libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h"
 
 #include <array>
+#include <span>
 
 RS_NS_START
 RSAPI void Arena::SetMutatorConfig(const MutatorConfig& mutatorConfig) {
 
 	bool
 		ballChanged = mutatorConfig.ballRadius != this->_mutatorConfig.ballRadius || mutatorConfig.ballMass != this->_mutatorConfig.ballMass,
 		carMassChanged = mutatorConfig.carMass != this->_mutatorConfig.carMass,
@@ -23,15 +29,15 @@
 
 	_bulletWorld.setGravity(mutatorConfig.gravity * UU_TO_BT);
 	
 	if (ballChanged) {
 		// We'll need to remake the ball
 		_bulletWorld.removeCollisionObject(&ball->_rigidBody);
 		delete ball->_collisionShape;
-		ball->_BulletSetup(gameMode, &_bulletWorld, mutatorConfig);
+		ball->_BulletSetup(gameMode, &_bulletWorld, mutatorConfig, _config.noBallRot);
 	}
 
 	if (carMassChanged) {
 		for (Car* car : _cars) {
 			btVector3 newCarInertia;
 			car->_childHitboxShape.calculateLocalInertia(mutatorConfig.carMass, newCarInertia);
 			car->_rigidBody.setMassProps(mutatorConfig.ballMass, newCarInertia);
@@ -438,48 +444,64 @@
 	car->_internalState.worldContact.contactNormal = manifoldPoint.m_normalWorldOnB;
 
 	// Manually override manifold friction/restitution
 	manifoldPoint.m_combinedFriction = _mutatorConfig.carWorldFriction;
 	manifoldPoint.m_combinedRestitution = _mutatorConfig.carWorldRestitution;
 }
 
-Arena::Arena(GameMode gameMode, ArenaMemWeightMode memWeightMode, float tickRate) : _mutatorConfig(gameMode), _suspColGrid(gameMode) {
+Arena::Arena(GameMode gameMode, const ArenaConfig& config, float tickRate) : _mutatorConfig(gameMode), _config(config), _suspColGrid(gameMode) {
 
 	// Tickrate must be from 15 to 120tps
 	assert(tickRate >= 15 && tickRate <= 120);
 
 	RocketSim::AssertInitialized("Cannot create Arena, ");
 
 	this->gameMode = gameMode;
 	this->tickTime = 1 / tickRate;
 
 	{ // Initialize world
 
 		btDefaultCollisionConstructionInfo collisionConfigConstructionInfo = {};
 
 		// These take up a ton of memory normally
-		if (memWeightMode == ArenaMemWeightMode::LIGHT) {
+		if (_config.memWeightMode == ArenaMemWeightMode::LIGHT) {
+			collisionConfigConstructionInfo.m_defaultMaxPersistentManifoldPoolSize /= 32;
+			collisionConfigConstructionInfo.m_defaultMaxCollisionAlgorithmPoolSize /= 64;
+		} else {
 			collisionConfigConstructionInfo.m_defaultMaxPersistentManifoldPoolSize /= 16;
 			collisionConfigConstructionInfo.m_defaultMaxCollisionAlgorithmPoolSize /= 32;
-		} else {
-			collisionConfigConstructionInfo.m_defaultMaxPersistentManifoldPoolSize /= 8;
-			collisionConfigConstructionInfo.m_defaultMaxCollisionAlgorithmPoolSize /= 16;
 		}
 
 		_bulletWorldParams.collisionConfig.setup(collisionConfigConstructionInfo);
 
 		_bulletWorldParams.collisionDispatcher.setup(&_bulletWorldParams.collisionConfig);
 		_bulletWorldParams.constraintSolver = btSequentialImpulseConstraintSolver();
 
-		_bulletWorldParams.overlappingPairCache = new (btAlignedAlloc(sizeof(btHashedOverlappingPairCache), 16)) btHashedOverlappingPairCache();
-		_bulletWorldParams.broadphase = btDbvtBroadphase(_bulletWorldParams.overlappingPairCache);
+		_bulletWorldParams.overlappingPairCache = new btHashedOverlappingPairCache();
+
+		if (_config.useCustomBroadphase) {
+			float cellSizeMultiplier = 1;
+			if (_config.memWeightMode == ArenaMemWeightMode::LIGHT) {
+				// Increase cell size
+				cellSizeMultiplier = 2.0f;
+			}
+
+			_bulletWorldParams.broadphase = new btRSBroadphase(
+				_config.minPos * UU_TO_BT,
+				_config.maxPos * UU_TO_BT,
+				_config.maxAABBLen * UU_TO_BT * cellSizeMultiplier,
+				_bulletWorldParams.overlappingPairCache,
+				_config.maxObjects);
+		} else {
+			_bulletWorldParams.broadphase = new btDbvtBroadphase(_bulletWorldParams.overlappingPairCache);
+		}
 
 		_bulletWorld.setup(
 			&_bulletWorldParams.collisionDispatcher,
-			&_bulletWorldParams.broadphase,
+			_bulletWorldParams.broadphase,
 			&_bulletWorldParams.constraintSolver,
 			&_bulletWorldParams.collisionConfig
 		);
 
 		_bulletWorld.setGravity(_mutatorConfig.gravity * UU_TO_BT);
 
 		// Adjust solver configuration to be closer to older Bullet (Rocket League's Bullet is from somewhere between 2013 and 2015)
@@ -513,56 +535,64 @@
 		_worldCollisionBvhShapes = NULL;
 		_worldCollisionPlaneShapes = NULL;
 	}
 
 	{ // Initialize ball
 		ball = Ball::_AllocBall();
 
-		ball->_BulletSetup(gameMode, &_bulletWorld, _mutatorConfig);
+		ball->_BulletSetup(gameMode, &_bulletWorld, _mutatorConfig, _config.noBallRot);
 		ball->SetState(BallState());
 	}
 
 	if (loadArenaStuff) { // Initialize boost pads
 		using namespace RLConst::BoostPads;
 
 		bool isHoops = gameMode == GameMode::HOOPS;
 
-		int amountSmall = isHoops ? LOCS_AMOUNT_SMALL_HOOPS : LOCS_AMOUNT_SMALL_SOCCAR;
-		_boostPads.reserve(LOCS_AMOUNT_BIG + amountSmall);
+		auto toSpan = [](auto &val) { return std::span<const Vec, std::dynamic_extent> (&*std::begin (val), &*std::end (val)); };
 
-		for (int i = 0; i < (LOCS_AMOUNT_BIG + amountSmall); i++) {
-			bool isBig = i < LOCS_AMOUNT_BIG;
+		std::span<const Vec> big   = isHoops ? toSpan (LOCS_BIG_HOOPS) : toSpan (LOCS_BIG_SOCCAR);
+		std::span<const Vec> small = isHoops ? toSpan (LOCS_SMALL_HOOPS) : toSpan (LOCS_SMALL_SOCCAR);
 
-			btVector3 pos;
-			if (isHoops) {
-				pos = isBig ? LOCS_BIG_HOOPS[i] : LOCS_SMALL_HOOPS[i - LOCS_AMOUNT_BIG];
-			} else {
-				pos = isBig ? LOCS_BIG_SOCCAR[i] : LOCS_SMALL_SOCCAR[i - LOCS_AMOUNT_BIG];
-			}
+		if (config.customBoostPads)
+		{
+			big   = toSpan (config.customBigBoostPads);
+			small = toSpan (config.customSmallBoostPads);
+		}
+
+		_boostPads.reserve(big.size() + small.size());
 
-			BoostPad* pad = BoostPad::_AllocBoostPad();
-			pad->_Setup(isBig, pos);
+		for (auto const &pads : {big, small})
+		{
+			for (auto const &pos : pads)
+			{
+				BoostPad* pad = BoostPad::_AllocBoostPad();
+				pad->_Setup(pads.data () == big.data (), pos);
 
-			_boostPads.push_back(pad);
-			_boostPadGrid.Add(pad);
+				_boostPads.push_back(pad);
+				if (!config.customBoostPads)
+					_boostPadGrid.Add(pad);
+			}
 		}
 	}
 
 	// Set internal tick callback
 	_bulletWorld.setWorldUserInfo(this);
 
 	gContactAddedCallback = &Arena::_BulletContactAddedCallback;
 }
 
-Arena* Arena::Create(GameMode gameMode, ArenaMemWeightMode memWeightMode, float tickRate) {
-	return new Arena(gameMode, memWeightMode, tickRate);
+Arena* Arena::Create(GameMode gameMode, const ArenaConfig& arenaConfig, float tickRate) {
+	return new Arena(gameMode, arenaConfig, tickRate);
 }
 
 void Arena::Serialize(DataStreamOut& out) const {
-	out.WriteMultiple(gameMode, tickTime, tickCount, _lastCarID, _memWeightMode);
+	out.WriteMultiple(gameMode, tickTime, tickCount, _lastCarID);
+
+	_config.Serialize(out);
 
 	{ // Serialize cars
 		out.Write<uint32_t>(_cars.size());
 		for (auto car : _cars) {
 			out.Write(car->team);
 			out.Write(car->id);
 			car->Serialize(out);
@@ -589,17 +619,20 @@
 
 	GameMode gameMode;
 	float tickTime;
 	uint64_t tickCount;
 	uint32_t lastCarID;
 	ArenaMemWeightMode memWeightMode;
 
-	in.ReadMultiple(gameMode, tickTime, tickCount, lastCarID, memWeightMode);
+	in.ReadMultiple(gameMode, tickTime, tickCount, lastCarID);
+
+	ArenaConfig newConfig = {};
+	newConfig.Deserialize(in);
 
-	Arena* newArena = new Arena(gameMode, memWeightMode, 1.f / tickTime);
+	Arena* newArena = new Arena(gameMode, newConfig, 1.f / tickTime);
 	newArena->tickCount = tickCount;
 	
 	{ // Deserialize cars
 		uint32_t carAmount = in.Read<uint32_t>();
 		for (uint32_t i = 0; i < carAmount; i++) {
 			Team team;
 			uint32_t id;
@@ -650,15 +683,15 @@
 		newArena->SetMutatorConfig(newArena->_mutatorConfig);
 	}
 
 	return newArena;
 }
 
 Arena* Arena::Clone(bool copyCallbacks) {
-	Arena* newArena = new Arena(this->gameMode, this->_memWeightMode, this->GetTickRate());
+	Arena* newArena = new Arena(this->gameMode, this->_config, this->GetTickRate());
 	
 	if (copyCallbacks)
 	{
 		newArena->_ballTouchCallback   = this->_ballTouchCallback;
 		newArena->_boostPickupCallback = this->_boostPickupCallback;
 		newArena->_carBumpCallback     = this->_carBumpCallback;
 		newArena->_goalScoreCallback   = this->_goalScoreCallback;
@@ -712,16 +745,19 @@
 			if (ball->_rigidBody.m_linearVelocity.length2() == 0 && ball->_rigidBody.m_angularVelocity.length2() == 0) {
 				ball->_rigidBody.setActivationState(ISLAND_SLEEPING);
 			} else {
 				ball->_rigidBody.setActivationState(ACTIVE_TAG);
 			}
 		}
 
+		bool ballOnly = _cars.empty();
+
 		bool hasArenaStuff = (gameMode != GameMode::THE_VOID);
-		if (hasArenaStuff) {
+		bool shouldUpdateSuspColGrid = hasArenaStuff && !ballOnly;
+		if (shouldUpdateSuspColGrid) {
 #ifndef RS_NO_SUSPCOLGRID
 			{ // Add dynamic bodies to suspension grid
 				for (Car* car : _cars) {
 					if (car->_internalState.isDemoed)
 						continue;
 
 					btVector3 min, max;
@@ -737,61 +773,68 @@
 		}
 
 		for (Car* car : _cars) {
 			SuspensionCollisionGrid* suspColGridPtr;
 #ifdef RS_NO_SUSPCOLGRID
 			suspColGridPtr = NULL;
 #else
-			if (hasArenaStuff) {
+			if (shouldUpdateSuspColGrid) {
 				suspColGridPtr = &_suspColGrid;
 			} else {
 				suspColGridPtr = NULL;
 			}
 #endif
 			car->_PreTickUpdate(gameMode, tickTime, _mutatorConfig, suspColGridPtr);
 		}
 
-		if (hasArenaStuff) {
+		if (shouldUpdateSuspColGrid) {
 #ifndef RS_NO_SUSPCOLGRID
 			_suspColGrid.ClearDynamicCollisions();
 #endif
 		}
 
-		if (hasArenaStuff) {
+		if (hasArenaStuff && !ballOnly) {
 			for (BoostPad* pad : _boostPads)
 				pad->_PreTickUpdate(tickTime);
 		}
 
 		// Update ball
 		ball->_PreTickUpdate(gameMode, tickTime);
 
 		// Update world
 		_bulletWorld.stepSimulation(tickTime, 0, tickTime);
 
 		for (Car* car : _cars) {
 			car->_PostTickUpdate(gameMode, tickTime, _mutatorConfig);
 			car->_FinishPhysicsTick(_mutatorConfig);
-			if (hasArenaStuff)
-				_boostPadGrid.CheckCollision(car);
+			if (hasArenaStuff) {
+				if (_config.customBoostPads)
+				{
+					for (auto &pad : _boostPads)
+						pad->_CheckCollide(car);
+				}
+				else
+					_boostPadGrid.CheckCollision(car);
+			}
 		}
 
-		if (hasArenaStuff)
+		if (hasArenaStuff && !ballOnly)
 		{
 			for (BoostPad* pad : _boostPads)
 			{
 				if (pad->_PostTickUpdate(tickTime, _mutatorConfig) && _boostPickupCallback.func)
 					_boostPickupCallback.func(this, pad->_internalState.curLockedCar, pad, _boostPickupCallback.userInfo);
 			}
 		}
 
 		ball->_FinishPhysicsTick(_mutatorConfig);
 
 		if (_goalScoreCallback.func != NULL) { // Potentially fire goal score callback
 			if (IsBallScored()) {
-				_goalScoreCallback.func(this, RS_TEAM_FROM_Y(-ball->_rigidBody.m_worldTransform.m_origin.y()), _goalScoreCallback.userInfo);
+				_goalScoreCallback.func(this, RS_TEAM_FROM_Y(-ball->_rigidBody.getWorldTransform().m_origin.y()), _goalScoreCallback.userInfo);
 			}
 		}
 
 		tickCount++;
 	}
 }
 
@@ -809,23 +852,23 @@
 
 	float dy = abs(y) * SCALE_Y - OFFSET_Y;
 	float distSq = x * x + dy * dy;
 	return distSq - RADIUS_SQ;
 }
 
 bool Arena::IsBallProbablyGoingIn(float maxTime, float extraMargin, Team* goalTeamOut) const {
-	Vec ballPos = ball->_rigidBody.m_worldTransform.m_origin * BT_TO_UU;
+	Vec ballPos = ball->_rigidBody.getWorldTransform().m_origin * BT_TO_UU;
 	Vec ballVel = ball->_rigidBody.m_linearVelocity * BT_TO_UU;
 
 	if (gameMode == GameMode::SOCCAR || gameMode == GameMode::SNOWDAY) {
 		if (abs(ballVel.y) < FLT_EPSILON)
 			return false;
 
 		float scoreDirSgn = RS_SGN(ballVel.y);
-		float goalY = RLConst::SOCCAR_GOAL_SCORE_BASE_THRESHOLD_Y * scoreDirSgn;
+		float goalY = _mutatorConfig.goalBaseThresholdY * scoreDirSgn;
 		float distToGoal = abs(ballPos.y - goalY);
 
 		float timeToGoal = distToGoal / abs(ballVel.y);
 		
 		if (timeToGoal > maxTime)
 			return false;
 
@@ -936,26 +979,26 @@
 
 RSAPI bool Arena::IsBallScored() const {
 	switch (gameMode) {
 	case GameMode::SOCCAR:
 	case GameMode::HEATSEEKER:
 	case GameMode::SNOWDAY:
 	{
-		float ballPosY = ball->_rigidBody.m_worldTransform.m_origin.y() * BT_TO_UU;
-		return abs(ballPosY) > (RLConst::SOCCAR_GOAL_SCORE_BASE_THRESHOLD_Y + _mutatorConfig.ballRadius);
+		float ballPosY = ball->_rigidBody.getWorldTransform().m_origin.y() * BT_TO_UU;
+		return abs(ballPosY) > (_mutatorConfig.goalBaseThresholdY + _mutatorConfig.ballRadius);
 	}
 	case GameMode::HOOPS:
 	{
-		if (ball->_rigidBody.m_worldTransform.m_origin.z() < RLConst::HOOPS_GOAL_SCORE_THRESHOLD_Z * UU_TO_BT) {
+		if (ball->_rigidBody.getWorldTransform().m_origin.z() < RLConst::HOOPS_GOAL_SCORE_THRESHOLD_Z * UU_TO_BT) {
 			constexpr float
 				SCALE_Y = 0.9f,
 				OFFSET_Y = 2770.f,
 				RADIUS_SQ = 716 * 716;
 
-			Vec ballPos = ball->_rigidBody.m_worldTransform.m_origin * BT_TO_UU;
+			Vec ballPos = ball->_rigidBody.getWorldTransform().m_origin * BT_TO_UU;
 			return BallWithinHoopsGoalXYMarginSq(ballPos.x, ballPos.y) < 0;
 		} else {
 			return false;
 		}
 	}
 	default:
 		return false;
@@ -986,22 +1029,22 @@
 
 	if (_boostPads.size() > 0) {
 		if (ownsBoostPads) {
 			// Remove all boost pads
 			for (BoostPad* boostPad : _boostPads)
 				delete boostPad;
 		}
-
-		delete[] _worldCollisionRBs;
-		delete[] _worldCollisionPlaneShapes;
-		delete[] _worldCollisionBvhShapes;
 	}
 
-	_bulletWorldParams.overlappingPairCache->~btHashedOverlappingPairCache();
-	btAlignedFree(_bulletWorldParams.overlappingPairCache);
+	delete[] _worldCollisionRBs;
+	delete[] _worldCollisionPlaneShapes;
+	delete[] _worldCollisionBvhShapes;
+
+	delete _bulletWorldParams.overlappingPairCache;
+	delete _bulletWorldParams.broadphase;
 }
 
 void Arena::_SetupArenaCollisionShapes() {
 	assert(gameMode != GameMode::THE_VOID);
 	bool isHoops = gameMode == GameMode::HOOPS;
 
 	auto collisionMeshes = RocketSim::GetArenaCollisionShapes(gameMode);
```

### Comparing `RocketSim-2.1.0a6/src/Sim/Arena/Arena.h` & `RocketSim-2.1.1/src/Sim/Arena/Arena.h`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,26 @@
 #include "../BoostPad/BoostPad.h"
 #include "../CollisionMasks.h"
 
 #include "../../CollisionMeshFile/CollisionMeshFile.h"
 #include "../BoostPad/BoostPadGrid/BoostPadGrid.h"
 #include "../SuspensionCollisionGrid/SuspensionCollisionGrid.h"
 #include "../MutatorConfig/MutatorConfig.h"
+#include "ArenaConfig/ArenaConfig.h"
 
 #include "../../../libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h"
 #include "../../../libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h"
 #include "../../../libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h"
 
 RS_NS_START
 
-// Mode of speed/memory optimization for the arena
-// Will affect whether high memory consumption is used to slightly increase speed or not
-enum class ArenaMemWeightMode : byte {
-	HEAVY, // ~611KB per arena with 4 cars
-	LIGHT  // ~397KB per arena with 4 cars
-};
-
 using BallTouchEventFn   = void(*)(class Arena* arena, Car *car, void* userInfo);
 using BoostPickupEventFn = void(*)(class Arena* arena, Car *car, BoostPad *boostPad, void* userInfo);
 using CarBumpEventFn     = void(*)(class Arena* arena, Car* bumper, Car* victim, bool isDemo, void* userInfo);
 using GoalScoreEventFn   = void(*)(class Arena* arena, Team scoringTeam, void* userInfo);
 
 // The container for all game simulation
 // Stores cars, the ball, all arena collisions, and manages the overall game state
@@ -89,23 +83,23 @@
 
 	RSAPI Car* GetCar(uint32_t id);
 
 	btDiscreteDynamicsWorld _bulletWorld;
 	struct {
 		btDefaultCollisionConfiguration collisionConfig;
 		btCollisionDispatcher collisionDispatcher;
-		btHashedOverlappingPairCache* overlappingPairCache;
-		btDbvtBroadphase broadphase;
+		btOverlappingPairCache* overlappingPairCache;
+		btBroadphaseInterface* broadphase;
 		btSequentialImpulseConstraintSolver constraintSolver;
 	} _bulletWorldParams;
 
-	btRigidBody* _worldCollisionRBs;
-	size_t _worldCollisionRBAmount;
-	btBvhTriangleMeshShape* _worldCollisionBvhShapes;
-	btStaticPlaneShape* _worldCollisionPlaneShapes;
+	btRigidBody* _worldCollisionRBs = NULL;
+	size_t _worldCollisionRBAmount = 0;
+	btBvhTriangleMeshShape* _worldCollisionBvhShapes = NULL;
+	btStaticPlaneShape* _worldCollisionPlaneShapes = NULL;
 
 	struct {
 		BallTouchEventFn func = nullptr;
 		void* userInfo = nullptr;
 	} _ballTouchCallback;
 	RSAPI void SetBallTouchCallback(BallTouchEventFn callbackFn, void* userInfo = nullptr);
 
@@ -124,15 +118,15 @@
 	struct {
 		GoalScoreEventFn func = nullptr;
 		void* userInfo = nullptr;
 	} _goalScoreCallback;
 	RSAPI void SetGoalScoreCallback(GoalScoreEventFn callbackFn, void* userInfo = nullptr);
 
 	// NOTE: Arena should be destroyed after use
-	RSAPI static Arena* Create(GameMode gameMode, ArenaMemWeightMode memWeightMode = ArenaMemWeightMode::HEAVY, float tickRate = 120);
+	RSAPI static Arena* Create(GameMode gameMode, const ArenaConfig& arenaConfig = {}, float tickRate = 120);
 	
 	// Serialize entire arena state including cars, ball, and boostpads
 	RSAPI void Serialize(DataStreamOut& out) const;
 
 	// Load new arena from serialized data
 	RSAPI static Arena* DeserializeNew(DataStreamIn& in);
 
@@ -200,26 +194,31 @@
 		const btCollisionObjectWrapper* colObjB, int partID_B, int indexB
 	);
 
 	void _BtCallback_OnCarBallCollision(Car* car, Ball* ball, btManifoldPoint& manifoldPoint, bool ballIsBodyA);
 	void _BtCallback_OnCarCarCollision(Car* car1, Car* car2, btManifoldPoint& manifoldPoint);
 	void _BtCallback_OnCarWorldCollision(Car* car, btCollisionObject* worldObject, btManifoldPoint& manifoldPoint);
 
+	const ArenaConfig& GetArenaConfig() const {
+		return _config;
+	}
+
+	// Backwards compatability
 	ArenaMemWeightMode GetMemWeightMode() {
-		return _memWeightMode;
+		return _config.memWeightMode;
 	}
 
 	void SetCarCarCollision(bool enable);
 	void SetCarBallCollision(bool enable);
 
 private:
 	// Whether to stop
 	bool _stop = false;
 
 	// Constructor for use by Arena::Create()
-	Arena(GameMode gameMode, ArenaMemWeightMode memWeightMode, float tickRate = 120);
+	Arena(GameMode gameMode, const ArenaConfig& config, float tickRate = 120);
 
-	// Making this private because horrible memory overflows would happen if you changed it
-	ArenaMemWeightMode _memWeightMode;
+	// Making this private because horrible memory overflows can happen if you changed it
+	ArenaConfig _config;
 };
 
 RS_NS_END
```

### Comparing `RocketSim-2.1.0a6/src/Sim/Ball/Ball.cpp` & `RocketSim-2.1.1/src/Sim/Ball/Ball.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 	} else {
 		auto shape = new btSphereShape(mutatorConfig.ballRadius * UU_TO_BT);
 		shape->calculateLocalInertia(mutatorConfig.ballMass, localIntertia);
 		return shape;
 	}
 }
 
-void Ball::_BulletSetup(GameMode gameMode, btDynamicsWorld* bulletWorld, const MutatorConfig& mutatorConfig) {
+void Ball::_BulletSetup(GameMode gameMode, btDynamicsWorld* bulletWorld, const MutatorConfig& mutatorConfig, bool noRot) {
 	btVector3 localIneria;
 	_collisionShape = MakeBallCollisionShape(gameMode, mutatorConfig, localIneria);
 
 	btRigidBody::btRigidBodyConstructionInfo constructionInfo =
 		btRigidBody::btRigidBodyConstructionInfo(mutatorConfig.ballMass, NULL, _collisionShape);
 
 	constructionInfo.m_startWorldTransform.setIdentity();
@@ -99,14 +99,16 @@
 	_rigidBody.setUserPointer(this);
 
 	// Trigger the Arena::_BulletContactAddedCallback() when anything touches the ball
 	_rigidBody.m_collisionFlags |= btCollisionObject::CF_CUSTOM_MATERIAL_CALLBACK;
 
 	_rigidBody.m_rigidbodyFlags = 0;
 
+	_rigidBody.m_noRot = noRot && (_collisionShape->getShapeType() == SPHERE_SHAPE_PROXYTYPE);
+
 	int mask = btBroadphaseProxy::AllFilter;
 	if (!mutatorConfig.enableCarBallCollision)
 		mask &= ~btBroadphaseProxy::CharacterFilter;
 	bulletWorld->addRigidBody(&_rigidBody, btBroadphaseProxy::DefaultFilter | CollisionMasks::HOOPS_NET, mask);
 }
 
 void Ball::_FinishPhysicsTick(const MutatorConfig& mutatorConfig) {
```

### Comparing `RocketSim-2.1.0a6/src/Sim/Ball/Ball.h` & `RocketSim-2.1.1/src/Sim/Ball/Ball.h`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 	// For construction by Arena
 	static Ball* _AllocBall() { return new Ball(); }
 
 	// For removal by Arena
 	static void _DestroyBall(Ball* ball) { delete ball; }
 
-	void _BulletSetup(GameMode gameMode, btDynamicsWorld* bulletWorld, const MutatorConfig& mutatorConfig);
+	void _BulletSetup(GameMode gameMode, btDynamicsWorld* bulletWorld, const MutatorConfig& mutatorConfig, bool noRot);
 
 	bool groundStickApplied = false;
 	Vec _velocityImpulseCache = { 0,0,0 };
 	void _FinishPhysicsTick(const MutatorConfig& mutatorConfig);
 
 	RSAPI bool IsSphere() const;
```

### Comparing `RocketSim-2.1.0a6/src/Sim/BallHitInfo/BallHitInfo.h` & `RocketSim-2.1.1/src/Sim/BallHitInfo/BallHitInfo.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPad.cpp` & `RocketSim-2.1.1/src/Sim/BoostPad/BoostPad.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 	_internalState.curLockedCar = NULL;
 }
 
 void BoostPad::_CheckCollide(Car* car) {
 	using namespace RLConst::BoostPads;
 
-	Vec carPosBT = car->_rigidBody.m_worldTransform.m_origin;
+	Vec carPosBT = car->_rigidBody.getWorldTransform().m_origin;
 
 	bool colliding = false;
 	if (_internalState.prevLockedCarID == car->id) {
 		// Check with AABB-hitbox collision
 
 		btVector3 carMinBT, carMaxBT;
 		car->_rigidBody.getAabb(carMinBT, carMaxBT);
```

### Comparing `RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPad.h` & `RocketSim-2.1.1/src/Sim/BoostPad/BoostPad.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp` & `RocketSim-2.1.1/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 RS_NS_START
 
 void BoostPadGrid::CheckCollision(Car* car) {
 	if (car->_internalState.isDemoed || car->_internalState.boost >= 100)
 		return;
 
-	Vec carPos = car->_rigidBody.m_worldTransform.m_origin * BT_TO_UU;
+	Vec carPos = car->_rigidBody.getWorldTransform().m_origin * BT_TO_UU;
 
 	if (carPos.z > EXTENT_Z)
 		return;
 
 	int indexX = carPos.x / CELL_SIZE_X + (CELLS_X / 2);
 	int indexY = carPos.y / CELL_SIZE_Y + (CELLS_Y / 2);
 
-	for (int i = RS_MAX(indexX - 1, 0); i < CELLS_X; i++) {
-		for (int j = RS_MAX(indexY - 1, 0); j < CELLS_Y; j++) {
+	for (int i = RS_MAX(indexX - 1, 0); i <= RS_MIN(indexX + 1, CELLS_X - 1); i++) {
+		for (int j = RS_MAX(indexY - 1, 0); j <= RS_MIN(indexY + 1, CELLS_Y - 1); j++) {
 			BoostPad* pad = pads[i][j];
 			if (pad) {
 				pad->_CheckCollide(car);
 			}
 		}
 	}
 }
```

### Comparing `RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h` & `RocketSim-2.1.1/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Sim/Car/Car.cpp` & `RocketSim-2.1.1/src/Sim/Car/Car.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #include "../../../libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h"
 
 RS_NS_START
 
 // Update our internal state from bullet and return it
 CarState Car::GetState() {
 	if (!_internalState.isDemoed) {
-		_internalState.pos = _rigidBody.m_worldTransform.m_origin * BT_TO_UU;
+		_internalState.pos = _rigidBody.getWorldTransform().m_origin * BT_TO_UU;
 
 		// NOTE: rotMat already updated at the start of Car::_PostTickUpdate()
 
 		_internalState.vel = _rigidBody.m_linearVelocity * BT_TO_UU;
 
 		_internalState.angVel = _rigidBody.m_angularVelocity;
 	}
@@ -23,15 +23,15 @@
 
 // Update our bullet stuff to this new state, replace our internal state with it
 void Car::SetState(const CarState& state) {
 	btTransform rbTransform;
 	rbTransform.setOrigin(state.pos * UU_TO_BT);
 	rbTransform.setBasis(state.rotMat);
 
-	_rigidBody.m_worldTransform = rbTransform;
+	_rigidBody.getWorldTransform() = rbTransform;
 
 	_rigidBody.m_linearVelocity = state.vel * UU_TO_BT;
 	_rigidBody.m_angularVelocity = state.angVel;
 
 	_velocityImpulseCache = { 0, 0, 0 };
 
 	_internalState = state;
@@ -89,15 +89,15 @@
 	if (_internalState.isDemoed)
 		return; // No other updates need to occur
 
 	// Do first part of the btVehicleRL update (update wheel transforms, do traces, calculate friction impulses) 
 	_bulletVehicle.updateVehicleFirst(tickTime, grid);
 
 
-	btMatrix3x3 basis = _rigidBody.m_worldTransform.m_basis;
+	btMatrix3x3 basis = _rigidBody.getWorldTransform().m_basis;
 
 	bool jumpPressed = controls.jump && !_internalState.lastControls.jump;
 
 	int numWheelsInContact = 0;
 	for (int i = 0; i < 4; i++)
 		numWheelsInContact += _bulletVehicle.m_wheelInfo[i].m_raycastInfo.m_isInContact;
 
@@ -127,15 +127,15 @@
 }
 
 void Car::_PostTickUpdate(GameMode gameMode, float tickTime, const MutatorConfig& mutatorConfig) {
 
 	if (_internalState.isDemoed)
 		return;
 
-	_internalState.rotMat = _rigidBody.m_worldTransform.m_basis;
+	_internalState.rotMat = _rigidBody.getWorldTransform().m_basis;
 
 	// Update wheelsWithContact
 	int numWheelsInContact = 0;
 	for (int i = 0; i < 4; i++) {
 		bool inContact = _bulletVehicle.m_wheelInfo[i].m_raycastInfo.m_isInContact;
 		_internalState.wheelsWithContact[i] = inContact;
 		numWheelsInContact += inContact;
@@ -428,15 +428,15 @@
 
 				btVector3
 					latDir = wheel.m_worldTransform.getBasis().getColumn(1),
 					longDir = latDir.cross(wheel.m_raycastInfo.m_contactNormalWS);
 
 				float frictionCurveInput = 0;
 
-				btVector3 wheelDelta = wheel.m_raycastInfo.m_hardPointWS - _rigidBody.m_worldTransform.m_origin;
+				btVector3 wheelDelta = wheel.m_raycastInfo.m_hardPointWS - _rigidBody.getWorldTransform().m_origin;
 
 				auto crossVec = (angularVel.cross(wheelDelta) + vel) * BT_TO_UU;
 
 				float baseFriction = abs(crossVec.dot(latDir));
 
 				// Significant friction results in lateral slip
 				if (baseFriction > 5)
@@ -590,15 +590,15 @@
 					doAirControl = true;
 				}
 			}
 
 			relDodgeTorque.y() *= pitchScale;
 
 			btVector3 dodgeTorque = relDodgeTorque * btVector3(FLIP_TORQUE_X, FLIP_TORQUE_Y, 0);
-			_rigidBody.applyTorque(_rigidBody.m_invInertiaTensorWorld.inverse() * _rigidBody.m_worldTransform.m_basis * dodgeTorque);
+			_rigidBody.applyTorque(_rigidBody.m_invInertiaTensorWorld.inverse() * _rigidBody.getWorldTransform().m_basis * dodgeTorque);
 		} else {
 			// Stall, allow air control
 			doAirControl = true;
 		}
 	} else {
 		doAirControl = true;
 	}
```

### Comparing `RocketSim-2.1.0a6/src/Sim/Car/Car.h` & `RocketSim-2.1.1/src/Sim/Car/Car.h`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 struct CarState : public PhysState {
 
 	// Incremented every update, reset when SetState() is called
 	// Used for telling if a stateset occured
 	// Not serialized
 	uint64_t updateCounter = 0;
 
+	// True if 3 or more wheels have contact
 	bool isOnGround = true;
 
 	// Whether each of the 4 wheels have contact
 	// First two are front
 	bool wheelsWithContact[4] = {}; 
 
 	// Whether we jumped to get into the air
```

### Comparing `RocketSim-2.1.0a6/src/Sim/Car/CarConfig/CarConfig.cpp` & `RocketSim-2.1.1/src/Sim/Car/CarConfig/CarConfig.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Sim/Car/CarConfig/CarConfig.h` & `RocketSim-2.1.1/src/Sim/Car/CarConfig/CarConfig.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Sim/CarControls.h` & `RocketSim-2.1.1/src/Sim/CarControls.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Sim/GameEventTracker/GameEventTracker.cpp` & `RocketSim-2.1.1/src/Sim/GameEventTracker/GameEventTracker.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 		// Goal event
 		if (scored && !_ballScoredLast) {
 			Car* shooter;
 			Car* passer;
 			if (GetShooterPasser(
 				arena,
-				RS_TEAM_FROM_Y(-arena->ball->_rigidBody.m_worldTransform.m_origin.y()),
+				RS_TEAM_FROM_Y(-arena->ball->_rigidBody.getWorldTransform().m_origin.y()),
 				shooter, true, passer,
 				config.goalMaxTouchTime * tickrate,
 				config.passMaxTouchTime * tickrate
 			)) {
 
 				if (_goalCallback.func)
 					_goalCallback.func(arena, shooter, passer, _goalCallback.userInfo);
```

### Comparing `RocketSim-2.1.0a6/src/Sim/GameEventTracker/GameEventTracker.h` & `RocketSim-2.1.1/src/Sim/GameEventTracker/GameEventTracker.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Sim/MutatorConfig/MutatorConfig.cpp` & `RocketSim-2.1.1/src/Sim/MutatorConfig/MutatorConfig.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 		ballWorldRestitution = Snowday::PUCK_RESTITUTION;
 		ballMass = Snowday::PUCK_MASS_BT;
 	} else {
 		ballWorldFriction = BALL_FRICTION;
 		ballWorldRestitution = BALL_RESTITUTION;
 		ballMass = BALL_MASS_BT;
 	}
+
+	if (gameMode == GameMode::HEATSEEKER) {
+		// Infinite boost
+		carSpawnBoostAmount = 100;
+		boostUsedPerSecond = 0;
+	}
 }
 
 void MutatorConfig::Serialize(DataStreamOut& out) const {
 	out.Write<uint16_t>(RS_GET_ARGUMENT_COUNT(MUTATOR_CONFIG_SERIALIZATION_FIELDS));
 	out.WriteMultiple(MUTATOR_CONFIG_SERIALIZATION_FIELDS);
 }
```

### Comparing `RocketSim-2.1.0a6/src/Sim/MutatorConfig/MutatorConfig.h` & `RocketSim-2.1.1/src/Sim/MutatorConfig/MutatorConfig.h`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 enum class DemoMode : byte {
 	NORMAL,
 	ON_CONTACT,
 	DISABLED
 };
 
-struct MutatorConfig {
+RSAPI struct MutatorConfig {
 
 	Vec gravity = Vec(0, 0, RLConst::GRAVITY_Z);
 
 	float
 		carMass = RLConst::CAR_MASS_BT,
 
 		// Friction between car and world (arena)
@@ -53,32 +53,35 @@
 	float
 		ballHitExtraForceScale = 1,
 		bumpForceScale = 1;
 
 	float
 		ballRadius;
 
-	bool 
+	bool
 		unlimitedFlips = false,
 		unlimitedDoubleJumps = false;
 
 	DemoMode demoMode = DemoMode::NORMAL;
 	bool enableTeamDemos = false;
 
 	bool enableCarCarCollision = true;
 	bool enableCarBallCollision = true;
 
+	// Only used if the game mode has soccar goals (i.e. soccar, heatseeker, snowday)
+	float goalBaseThresholdY = RLConst::SOCCAR_GOAL_SCORE_BASE_THRESHOLD_Y;
+
 	MutatorConfig(GameMode gameMode);
 
-	RSAPI void Serialize(DataStreamOut& out) const;
-	RSAPI void Deserialize(DataStreamIn& in);
+	void Serialize(DataStreamOut& out) const;
+	void Deserialize(DataStreamIn& in);
 };
 
 #define MUTATOR_CONFIG_SERIALIZATION_FIELDS \
 gravity, carMass, carWorldFriction, carWorldRestitution, ballMass, \
 ballMaxSpeed, ballDrag, ballWorldFriction, ballWorldRestitution, jumpAccel, \
 jumpImmediateForce, boostAccel, boostUsedPerSecond, respawnDelay, \
 carSpawnBoostAmount, bumpCooldownTime, boostPadCooldown_Big, boostPadCooldown_Small, \
 ballHitExtraForceScale, bumpForceScale, ballRadius, unlimitedFlips, unlimitedDoubleJumps, \
-demoMode, enableTeamDemos, enableCarCarCollision, enableCarBallCollision
+demoMode, enableTeamDemos, enableCarCarCollision, enableCarBallCollision, goalBaseThresholdY
 
 RS_NS_END
```

### Comparing `RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp` & `RocketSim-2.1.1/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h` & `RocketSim-2.1.1/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h`

 * *Files 3% similar despite different names*

```diff
@@ -61,20 +61,14 @@
 	template <bool LIGHT>
 	Cell& Get(int i, int j, int k) {
 		int index = (i * CELL_AMOUNT_Y[LIGHT] * CELL_AMOUNT_Z[LIGHT]) + (j * CELL_AMOUNT_Z[LIGHT]) + k;
 		return cellData[index];
 	}
 
 	template <bool LIGHT>
-	Cell Get(int i, int j, int k) const {
-		int index = (i * CELL_AMOUNT_Y[LIGHT] * CELL_AMOUNT_Z[LIGHT]) + (j * CELL_AMOUNT_Z[LIGHT]) + k;
-		return cellData[index];
-	}
-
-	template <bool LIGHT>
 	Vec GetCellMin(int xIndex, int yIndex, int zIndex) const {
 		return Vec(
 			CELL_SIZE_X[LIGHT] * (xIndex - (CELL_AMOUNT_X[LIGHT] / 2)),
 			CELL_SIZE_Y[LIGHT] * (yIndex - (CELL_AMOUNT_Y[LIGHT] / 2)),
 			CELL_SIZE_Z[LIGHT] * zIndex
 		);
 	}
```

### Comparing `RocketSim-2.1.0a6/src/Sim/btVehicleRL/btVehicleRL.cpp` & `RocketSim-2.1.1/src/Sim/btVehicleRL/btVehicleRL.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 				wheel.m_raycastInfo.m_suspensionLength,
 				wheel.getSuspensionRestLength() - suspensionTravel,
 				wheel.getSuspensionRestLength() + suspensionTravel
 			);
 
 		float denominator = wheel.m_raycastInfo.m_contactNormalWS.dot(getUpVector());
 
-		btVector3 relpos = wheel.m_raycastInfo.m_contactPointWS - m_chassisBody->m_worldTransform.m_origin;
+		btVector3 relpos = wheel.m_raycastInfo.m_contactPointWS - m_chassisBody->getWorldTransform().m_origin;
 		wheel.m_velAtContactPoint = m_chassisBody->getVelocityInLocalPoint(relpos);
 
 		float projVel = wheel.m_raycastInfo.m_contactNormalWS.dot(wheel.m_velAtContactPoint);
 
 		if (denominator > 0.1) {
 			float inv = 1 / denominator;
 			wheel.m_suspensionRelativeVelocity = projVel * inv;
```

### Comparing `RocketSim-2.1.0a6/src/Sim/btVehicleRL/btVehicleRL.h` & `RocketSim-2.1.1/src/Sim/btVehicleRL/btVehicleRL.h`

 * *Files identical despite different names*

