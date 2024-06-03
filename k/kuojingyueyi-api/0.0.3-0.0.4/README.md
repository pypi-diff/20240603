# Comparing `tmp/kuojingyueyi-api-0.0.3.tar.gz` & `tmp/kuojingyueyi-api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuojingyueyi-api-0.0.3.tar", last modified: Fri Feb  2 08:40:27 2024, max compression
+gzip compressed data, was "kuojingyueyi-api-0.0.4.tar", last modified: Mon Jun  3 09:03:59 2024, max compression
```

## Comparing `kuojingyueyi-api-0.0.3.tar` & `kuojingyueyi-api-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-02 08:40:27.257590 kuojingyueyi-api-0.0.3/
--rw-rw-rw-   0        0        0      898 2024-02-02 08:40:27.256619 kuojingyueyi-api-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-10-31 08:19:44.000000 kuojingyueyi-api-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-02 08:40:27.247490 kuojingyueyi-api-0.0.3/kuojingyueyi_api/
--rw-rw-rw-   0        0        0       31 2023-11-01 01:23:23.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api/__init__.py
--rw-rw-rw-   0        0        0     8747 2024-01-31 03:17:28.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api/api.py
--rw-rw-rw-   0        0        0      853 2023-08-22 10:24:45.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api/exception.py
--rw-rw-rw-   0        0        0    18796 2024-02-02 08:37:30.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api/fields.py
--rw-rw-rw-   0        0        0     9671 2023-08-23 11:13:46.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-02 08:40:27.254593 kuojingyueyi-api-0.0.3/kuojingyueyi_api.egg-info/
--rw-rw-rw-   0        0        0      898 2024-02-02 08:40:27.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-02-02 08:40:27.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-02 08:40:27.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-02-02 08:40:27.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-02-02 08:40:27.000000 kuojingyueyi-api-0.0.3/kuojingyueyi_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-02 08:40:27.257590 kuojingyueyi-api-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     5246 2024-02-02 08:39:17.000000 kuojingyueyi-api-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:03:59.717774 kuojingyueyi-api-0.0.4/
+-rw-rw-rw-   0        0        0      898 2024-06-03 09:03:59.716777 kuojingyueyi-api-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-10-31 08:19:44.000000 kuojingyueyi-api-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 09:03:59.710773 kuojingyueyi-api-0.0.4/kuojingyueyi_api/
+-rw-rw-rw-   0        0        0       31 2023-11-01 01:23:23.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api/__init__.py
+-rw-rw-rw-   0        0        0     9947 2024-06-03 08:58:54.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api/api.py
+-rw-rw-rw-   0        0        0      833 2024-06-03 08:03:45.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api/exception.py
+-rw-rw-rw-   0        0        0    23040 2024-06-03 08:57:45.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api/fields.py
+-rw-rw-rw-   0        0        0     9671 2023-08-23 11:13:46.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:03:59.715777 kuojingyueyi-api-0.0.4/kuojingyueyi_api.egg-info/
+-rw-rw-rw-   0        0        0      898 2024-06-03 09:03:59.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-06-03 09:03:59.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 09:03:59.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 09:03:59.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-06-03 09:03:59.000000 kuojingyueyi-api-0.0.4/kuojingyueyi_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 09:03:59.717774 kuojingyueyi-api-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     5246 2024-06-03 09:02:34.000000 kuojingyueyi-api-0.0.4/setup.py
```

### Comparing `kuojingyueyi-api-0.0.3/PKG-INFO` & `kuojingyueyi-api-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuojingyueyi-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: 抖音官方开放接口
 Home-page: https://github.com/ldsxp/kuojingyueyi-api
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/kuojingyueyi-api
 Description: # kuojingyueyi-api
```

### Comparing `kuojingyueyi-api-0.0.3/kuojingyueyi_api/api.py` & `kuojingyueyi-api-0.0.4/kuojingyueyi_api/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -215,14 +215,45 @@
 
         网址:
         """
         url = f"{self.base_url}/api/admin/cp-contract/detail-settlement/list/{contract_id}"
         r = self._session.get(url)
         return self.get_response_data(r)
 
+    def settlement_payment_document_list(self, page=1, page_size=20, **kwargs):
+        """
+        支付单列表
+
+        结算管理/支付单
+        网址: https://ds.kuojingyueyi.cn/app/settle-manage/pay-bill-manage?current=1&pageSize=20
+
+        # 支持的参数
+        "pageNo": 2,  # 可不用
+        "current": 1,  # 可不用
+        "pageSize": 20,  # 可不用
+        # 内部合约编号
+        "docIdOrName": "P724_20230401_20230930_Z16OXKY"
+        """
+        # https://ds.kuojingyueyi.cn/api/admin//list?pageNo=1&pageSize=20
+        # print(kwargs)
+        url = f"{self.base_url}/api/admin/settlement-payment-document/list?pageNo={page}&pageSize={page_size}"
+        r = self._session.post(url, json=kwargs)
+        return self.get_response_data(r)
+
+    def settlement_payment_document_detail(self, pk):
+        """
+        支付单详情
+
+        结算管理/支付单/支付单信息
+        网址: https://ds.kuojingyueyi.cn/app/settle-manage/pay-bill-detail/3682
+        """
+        url = f"{self.base_url}/api/admin/settlement-payment-document/detail/{pk}"
+        r = self._session.get(url)
+        return self.get_response_data(r)
+
     def song_list(self, page=1, page_size=20, **kwargs):
         """
         歌曲列表
 
         内容管理/歌曲管理
         网址: https://ds-test.kuojingyueyi.cn/app/content-manage/song-manage?current=1&pageSize=20
```

### Comparing `kuojingyueyi-api-0.0.3/kuojingyueyi_api/exception.py` & `kuojingyueyi-api-0.0.4/kuojingyueyi_api/exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # __all__ = [
 #     # warnings
 #     # exceptions
-#     'DouYinException',
+#     'KJException',
 #     'NeedLoginException',
 # ]
 
 
-class DouYinException(Exception):
+class KJException(Exception):
     pass
 
 
-class NeedLoginException(DouYinException):
+class NeedLoginException(KJException):
     def __init__(self, what):
         """
         使用某方法需要登录而当前客户端未登录
 
         :param str|unicode what: 当前试图调用的方法名
         """
         self.what = what
 
     def __repr__(self):
         return '需要登录才能使用 [{self.what}] 方法。'.format(self=self)
 
     __str__ = __repr__
 
 
-class NeedAccessTokenException(DouYinException):
+class NeedAccessTokenException(KJException):
 
     def __repr__(self):
         return '需要用户 access-token 才能使用这个接口！'.format(self=self)
 
     __str__ = __repr__
 
 
-class LoginError(DouYinException):
+class LoginError(KJException):
     """
     所有登录中发生的错误
     """
```

### Comparing `kuojingyueyi-api-0.0.3/kuojingyueyi_api/fields.py` & `kuojingyueyi-api-0.0.4/kuojingyueyi_api/fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     'contractStatus': '内部合同编号状态',
     'cpDisplayName': '所属公司显示名字',
     'cpId': '所属公司Id',
     'cpName': '所属公司名字',
     'ctime': '创建时间',
     'deDeposit': '扣减保底金',
     'deOtherAmount': '扣减其他费用',
-    'divisionMethod': '_divisionMethod',
+    'divisionMethod': '合作模式Id',
     'divisionMethodName': '合作模式',
     'endTime': '结算结束时间',
     'frozenStatus': '冻结状态',
     'id': '供应商结算单ID',
     'isCanApprove': '可以审核',
     'liableManName': '合约负责人',
     'name': '名字',
@@ -247,14 +247,120 @@
     'status': '合约状态',
     'type': '资产类型',  # 列表
     'uid': '更新用户ID',
     'uname': '更新用户',
     'utime': '更新时间',
 }
 
+# 支付单列表
+SETTLEMENT_PAYMENT_DOCUMENT_LIST_FIELDS = {
+    'accountName': '收款方名字',
+    'accountNum': '收款方银行账号',
+    'bankName': '_bankName',
+    'bfDeDepositBalance': '扣减前保底金余额',
+    'bfDeOtherAmountBalance': '扣减前其他费用余额',
+    'cname': '创建者',
+    'code': '支付单CODE',
+    'confirmInfo': '_confirmInfo',
+    'confirmStatus': '_confirmStatus',
+    'contractCode': '内部合同Code',
+    'contractId': '内部合同ID',
+    'contractName': '内部合同名称',
+    'contractOfflineCode': '内部合同编号',
+    'contractStatus': '内部合同编号状态',
+    'cpDisplayName': '所属公司显示名字',
+    'cpId': '所属公司Id',
+    'cpName': '所属公司名字',
+    'ctime': '创建时间',
+    'deDeposit': '扣减保底金',
+    'deOtherAmount': '扣减其他费用',
+    'divisionMethod': '合作模式Id',
+    'divisionMethodName': '合作模式',
+    'endTime': '结算结束时间',
+    'id': '支付单Id',
+    'isCanApprove': '可以审核',
+    'liableManName': '合约负责人',
+    'name': '支付单名称',
+    'ogTotleAmount': '原始分成总计',
+    'payTotleAmount': '实际分成合计',
+    'paymentAttachments': '_paymentAttachments',
+    'paymentInvoiceAttachments': '_paymentInvoiceAttachments',
+    'paymentReceiptAttachments': '_paymentReceiptAttachments',
+    'settleFormula': '结算公式',
+    'settlementCurrency': '结算货币ID',
+    'settlementCurrencyStr': '结算货币名字',
+    'shareAchievedAmount': '_shareAchievedAmount',
+    'shareProportion': '合同分成比例',
+    'spDisplayName': '结算渠道显示名字',
+    'spId': '结算渠道Id',
+    'spName': '结算渠道名字',
+    'startTime': '结算开始时间',
+    'status': '状态',
+    'statusStr': '当前状态名字',
+    'supplierDisplayName': '供应商显示名字',
+    'supplierId': '供应商ID',
+    'supplierName': '供应商名字',
+    'totleAmount': '实际分成合计',
+    'uname': '更新用户',
+    'utime': '更新时间'}
+
+# 支付单详情
+SETTLEMENT_PAYMENT_DOCUMENT_DETAIL_FIELDS = {
+    'accountName': '收款方名字',
+    'accountNum': '收款方银行账号',
+    'bankName': '收款方开户行名字',
+    'bfDeDepositBalance': '扣减前保底金余额',
+    'bfDeOtherAmountBalance': '扣减前其他费用余额',
+    'cname': '创建者',
+    'code': '支付单CODE',
+    'confirmInfo': '_confirmInfo',
+    'confirmStatus': '_confirmStatus',
+    'contractCode': '内部合同Code',
+    'contractId': '内部合同ID',
+    'contractName': '内部合同名称',
+    'contractOfflineCode': '内部合同编号',
+    'contractStatus': '内部合同编号状态',
+    'cpDisplayName': '所属公司显示名字',
+    'cpId': '所属公司Id',
+    'cpName': '所属公司名字',
+    'ctime': '创建时间',
+    'deDeposit': '扣减保底金',
+    'deOtherAmount': '扣减其他费用',
+    'divisionMethod': '合作模式Id',
+    'divisionMethodName': '合作模式',
+    'endTime': '结算结束时间',
+    'id': '支付单Id',
+    'isCanApprove': '可以审核',
+    'liableManName': '合约负责人',
+    'name': '支付单名称',
+    'ogTotleAmount': '原始分成总计',
+    'payTotleAmount': '实际分成合计',
+    'paymentAttachments': '支付单附件',  # 支付单附件 一个包含字典的列表
+    'paymentInvoiceAttachments': '_paymentInvoiceAttachments',
+    'paymentReceiptAttachments': '_paymentReceiptAttachments',
+    'settleFormula': '结算公式',
+    'settlementCurrency': '结算货币ID',
+    'settlementCurrencyStr': '结算货币名字',
+    'shareAchievedAmount': '_shareAchievedAmount',
+    'shareProportion': '合同分成比例',
+    'spDisplayName': '结算渠道显示名字',
+    'spId': '结算渠道Id',
+    'spName': '结算渠道名字',
+    'startTime': '结算开始时间',
+
+    'status': '状态',
+    'statusStr': '当前状态名字',
+    'supplierDisplayName': '供应商显示名字',
+    'supplierId': '供应商ID',
+    'supplierName': '供应商名字',
+    'totleAmount': '实际分成合计',
+    'uname': '更新用户',
+    'utime': '更新时间',
+}
+
 # 歌曲列表
 SONG_LIST_FIELDS = {
     'advertPublishBeginDate': '_advertPublishBeginDate',
     'advertPublishEndDate': '_advertPublishEndDate',
     'albumCode': '专辑CODE',
     'albumCopyrightOrgId': '_albumCopyrightOrgId',
     'albumCopyrightOrgName': '_albumCopyrightOrgName',
```

### Comparing `kuojingyueyi-api-0.0.3/kuojingyueyi_api/utils.py` & `kuojingyueyi-api-0.0.4/kuojingyueyi_api/utils.py`

 * *Files identical despite different names*

### Comparing `kuojingyueyi-api-0.0.3/kuojingyueyi_api.egg-info/PKG-INFO` & `kuojingyueyi-api-0.0.4/kuojingyueyi_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuojingyueyi-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: 抖音官方开放接口
 Home-page: https://github.com/ldsxp/kuojingyueyi-api
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/kuojingyueyi-api
 Description: # kuojingyueyi-api
```

### Comparing `kuojingyueyi-api-0.0.3/setup.py` & `kuojingyueyi-api-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
-version = '0.0.3'
+version = '0.0.4'
 
 # 创建一个源码包
 # python setup.py sdist
 # 对于 Windows，可以执行python setup.py bdist_wininst 生成一个exe文件；
 # 若要生成 RPM 包，执行 python setup.py bdist_rpm，但系统必须有 rpm 命令的支持。
 # 可以运行下面的命令查看所有格式的支持：
 # python setup.py bdist --help-formats
```

