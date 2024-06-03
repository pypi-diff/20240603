# Comparing `tmp/ocpp-2.0.0rc0.tar.gz` & `tmp/ocpp-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocpp-2.0.0rc0.tar", max compression
+gzip compressed data, was "ocpp-2.0.0rc1.tar", max compression
```

## Comparing `ocpp-2.0.0rc0.tar` & `ocpp-2.0.0rc1.tar`

### file list

```diff
@@ -1,226 +1,226 @@
--rw-r--r--   0        0        0     1075 2024-05-22 09:38:52.650504 ocpp-2.0.0rc0/LICENSE
--rw-r--r--   0        0        0     6872 2024-05-22 09:38:52.650504 ocpp-2.0.0rc0/README.rst
--rw-r--r--   0        0        0        0 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/__init__.py
--rw-r--r--   0        0        0    16380 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/charge_point.py
--rw-r--r--   0        0        0     4451 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/exceptions.py
--rw-r--r--   0        0        0      221 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/experimental/v21/README.rst
--rw-r--r--   0        0        0    14821 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/messages.py
--rw-r--r--   0        0        0     4106 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/routing.py
--rw-r--r--   0        0        0      186 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/__init__.py
--rw-r--r--   0        0        0    20548 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/call.py
--rw-r--r--   0        0        0    19232 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/call_result.py
--rw-r--r--   0        0        0     3968 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/datatypes.py
--rw-r--r--   0        0        0    23663 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/enums.py
--rw-r--r--   0        0        0      306 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/Authorize.json
--rw-r--r--   0        0        0     1062 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/AuthorizeResponse.json
--rw-r--r--   0        0        0     1139 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/BootNotification.json
--rw-r--r--   0        0        0      655 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/BootNotificationResponse.json
--rw-r--r--   0        0        0      302 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/CancelReservation.json
--rw-r--r--   0        0        0      423 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/CancelReservationResponse.json
--rw-r--r--   0        0        0      352 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/CertificateSigned.json
--rw-r--r--   0        0        0      505 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/CertificateSignedResponse.json
--rw-r--r--   0        0        0      512 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ChangeAvailability.json
--rw-r--r--   0        0        0      453 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ChangeAvailabilityResponse.json
--rw-r--r--   0        0        0      418 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ChangeConfiguration.json
--rw-r--r--   0        0        0      491 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ChangeConfigurationResponse.json
--rw-r--r--   0        0        0      174 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ClearCache.json
--rw-r--r--   0        0        0      416 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ClearCacheResponse.json
--rw-r--r--   0        0        0      637 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ClearChargingProfile.json
--rw-r--r--   0        0        0      425 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ClearChargingProfileResponse.json
--rw-r--r--   0        0        0      466 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/DataTransfer.json
--rw-r--r--   0        0        0      547 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/DataTransferResponse.json
--rw-r--r--   0        0        0     1156 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/DeleteCertificate.json
--rw-r--r--   0        0        0      523 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/DeleteCertificateResponse.json
--rw-r--r--   0        0        0      491 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/DiagnosticsStatusNotification.json
--rw-r--r--   0        0        0      194 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/DiagnosticsStatusNotificationResponse.json
--rw-r--r--   0        0        0      760 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ExtendedTriggerMessage.json
--rw-r--r--   0        0        0      530 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json
--rw-r--r--   0        0        0      591 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/FirmwareStatusNotification.json
--rw-r--r--   0        0        0      191 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/FirmwareStatusNotificationResponse.json
--rw-r--r--   0        0        0      539 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetCompositeSchedule.json
--rw-r--r--   0        0        0     2139 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetCompositeScheduleResponse.json
--rw-r--r--   0        0        0      344 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetConfiguration.json
--rw-r--r--   0        0        0     1066 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetConfigurationResponse.json
--rw-r--r--   0        0        0      642 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetDiagnostics.json
--rw-r--r--   0        0        0      275 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetDiagnosticsResponse.json
--rw-r--r--   0        0        0      552 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetInstalledCertificateIds.json
--rw-r--r--   0        0        0     1566 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json
--rw-r--r--   0        0        0      183 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetLocalListVersion.json
--rw-r--r--   0        0        0      301 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetLocalListVersionResponse.json
--rw-r--r--   0        0        0     1184 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetLog.json
--rw-r--r--   0        0        0      566 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/GetLogResponse.json
--rw-r--r--   0        0        0      173 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/Heartbeat.json
--rw-r--r--   0        0        0      325 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/HeartbeatResponse.json
--rw-r--r--   0        0        0      639 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/InstallCertificate.json
--rw-r--r--   0        0        0      526 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/InstallCertificateResponse.json
--rw-r--r--   0        0        0      667 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/LogStatusNotification.json
--rw-r--r--   0        0        0      173 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/LogStatusNotificationResponse.json
--rw-r--r--   0        0        0     6758 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/MeterValues.json
--rw-r--r--   0        0        0      176 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/MeterValuesResponse.json
--rw-r--r--   0        0        0     4383 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/RemoteStartTransaction.json
--rw-r--r--   0        0        0      428 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/RemoteStartTransactionResponse.json
--rw-r--r--   0        0        0      306 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/RemoteStopTransaction.json
--rw-r--r--   0        0        0      427 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/RemoteStopTransactionResponse.json
--rw-r--r--   0        0        0      704 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ReserveNow.json
--rw-r--r--   0        0        0      502 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ReserveNowResponse.json
--rw-r--r--   0        0        0      398 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/Reset.json
--rw-r--r--   0        0        0      411 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/ResetResponse.json
--rw-r--r--   0        0        0      464 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SecurityEventNotification.json
--rw-r--r--   0        0        0      177 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SecurityEventNotificationResponse.json
--rw-r--r--   0        0        0     2146 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SendLocalList.json
--rw-r--r--   0        0        0      484 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SendLocalListResponse.json
--rw-r--r--   0        0        0     4310 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SetChargingProfile.json
--rw-r--r--   0        0        0      456 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SetChargingProfileResponse.json
--rw-r--r--   0        0        0      287 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SignCertificate.json
--rw-r--r--   0        0        0      483 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SignCertificateResponse.json
--rw-r--r--   0        0        0      876 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SignedFirmwareStatusNotification.json
--rw-r--r--   0        0        0      184 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SignedFirmwareStatusNotificationResponse.json
--rw-r--r--   0        0        0     1212 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SignedUpdateFirmware.json
--rw-r--r--   0        0        0      590 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json
--rw-r--r--   0        0        0      676 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/StartTransaction.json
--rw-r--r--   0        0        0     1162 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/StartTransactionResponse.json
--rw-r--r--   0        0        0     1805 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/StatusNotification.json
--rw-r--r--   0        0        0      183 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/StatusNotificationResponse.json
--rw-r--r--   0        0        0     7313 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/StopTransaction.json
--rw-r--r--   0        0        0     1023 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/StopTransactionResponse.json
--rw-r--r--   0        0        0      678 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/TriggerMessage.json
--rw-r--r--   0        0        0      454 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/TriggerMessageResponse.json
--rw-r--r--   0        0        0      296 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/UnlockConnector.json
--rw-r--r--   0        0        0      457 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/UnlockConnectorResponse.json
--rw-r--r--   0        0        0      572 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/UpdateFirmware.json
--rw-r--r--   0        0        0      179 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v16/schemas/UpdateFirmwareResponse.json
--rw-r--r--   0        0        0      189 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v201/__init__.py
--rw-r--r--   0        0        0    34073 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v201/call.py
--rw-r--r--   0        0        0    32301 2024-05-22 09:38:52.814506 ocpp-2.0.0rc0/ocpp/v201/call_result.py
--rw-r--r--   0        0        0    22081 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/datatypes.py
--rw-r--r--   0        0        0    80113 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/enums.py
--rwxr-xr-x   0        0        0     4203 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/AuthorizeRequest.json
--rwxr-xr-x   0        0        0     7208 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/AuthorizeResponse.json
--rwxr-xr-x   0        0        0     3161 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/BootNotificationRequest.json
--rwxr-xr-x   0        0        0     2270 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/BootNotificationResponse.json
--rwxr-xr-x   0        0        0      775 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/CancelReservationRequest.json
--rwxr-xr-x   0        0        0     1758 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/CancelReservationResponse.json
--rwxr-xr-x   0        0        0     1914 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/CertificateSignedRequest.json
--rwxr-xr-x   0        0        0     1752 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/CertificateSignedResponse.json
--rwxr-xr-x   0        0        0     1811 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ChangeAvailabilityRequest.json
--rwxr-xr-x   0        0        0     1783 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ChangeAvailabilityResponse.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearCacheRequest.json
--rwxr-xr-x   0        0        0     1735 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearCacheResponse.json
--rwxr-xr-x   0        0        0     2574 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearChargingProfileRequest.json
--rwxr-xr-x   0        0        0     1752 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearChargingProfileResponse.json
--rwxr-xr-x   0        0        0      787 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearDisplayMessageRequest.json
--rwxr-xr-x   0        0        0     1735 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearDisplayMessageResponse.json
--rwxr-xr-x   0        0        0      865 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearVariableMonitoringRequest.json
--rwxr-xr-x   0        0        0     2327 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearVariableMonitoringResponse.json
--rwxr-xr-x   0        0        0     1087 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearedChargingLimitRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ClearedChargingLimitResponse.json
--rwxr-xr-x   0        0        0     1121 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/CostUpdatedRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/CostUpdatedResponse.json
--rwxr-xr-x   0        0        0     4659 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/CustomerInformationRequest.json
--rwxr-xr-x   0        0        0     1740 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/CustomerInformationResponse.json
--rwxr-xr-x   0        0        0     1101 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/DataTransferRequest.json
--rwxr-xr-x   0        0        0     1869 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/DataTransferResponse.json
--rwxr-xr-x   0        0        0     1808 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/DeleteCertificateRequest.json
--rwxr-xr-x   0        0        0     1747 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/DeleteCertificateResponse.json
--rwxr-xr-x   0        0        0     1539 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json
--rwxr-xr-x   0        0        0     1424 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/Get15118EVCertificateRequest.json
--rwxr-xr-x   0        0        0     1915 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/Get15118EVCertificateResponse.json
--rwxr-xr-x   0        0        0     1105 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetBaseReportRequest.json
--rwxr-xr-x   0        0        0     1794 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetBaseReportResponse.json
--rwxr-xr-x   0        0        0     1957 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetCertificateStatusRequest.json
--rwxr-xr-x   0        0        0     2089 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetCertificateStatusResponse.json
--rwxr-xr-x   0        0        0     3622 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetChargingProfilesRequest.json
--rwxr-xr-x   0        0        0     1859 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetChargingProfilesResponse.json
--rwxr-xr-x   0        0        0     1329 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetCompositeScheduleRequest.json
--rwxr-xr-x   0        0        0     5095 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetCompositeScheduleResponse.json
--rwxr-xr-x   0        0        0     1874 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetDisplayMessagesRequest.json
--rwxr-xr-x   0        0        0     1841 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetDisplayMessagesResponse.json
--rwxr-xr-x   0        0        0     1204 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json
--rwxr-xr-x   0        0        0     3997 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetLocalListVersionRequest.json
--rwxr-xr-x   0        0        0      840 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetLocalListVersionResponse.json
--rwxr-xr-x   0        0        0     2802 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetLogRequest.json
--rwxr-xr-x   0        0        0     1954 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetLogResponse.json
--rwxr-xr-x   0        0        0     4175 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetMonitoringReportRequest.json
--rwxr-xr-x   0        0        0     1800 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetMonitoringReportResponse.json
--rwxr-xr-x   0        0        0     4143 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetReportRequest.json
--rwxr-xr-x   0        0        0     1800 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetReportResponse.json
--rwxr-xr-x   0        0        0      784 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetTransactionStatusRequest.json
--rwxr-xr-x   0        0        0      910 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetTransactionStatusResponse.json
--rwxr-xr-x   0        0        0     3931 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetVariablesRequest.json
--rwxr-xr-x   0        0        0     5581 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/GetVariablesResponse.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/HeartbeatRequest.json
--rwxr-xr-x   0        0        0      802 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/HeartbeatResponse.json
--rwxr-xr-x   0        0        0     1226 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/InstallCertificateRequest.json
--rwxr-xr-x   0        0        0     1751 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/InstallCertificateResponse.json
--rwxr-xr-x   0        0        0     1361 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/LogStatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/LogStatusNotificationResponse.json
--rwxr-xr-x   0        0        0     7709 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/MeterValuesRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/MeterValuesResponse.json
--rwxr-xr-x   0        0        0    11333 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyChargingLimitRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyChargingLimitResponse.json
--rwxr-xr-x   0        0        0     1542 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyCustomerInformationRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyCustomerInformationResponse.json
--rwxr-xr-x   0        0        0     6512 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json
--rwxr-xr-x   0        0        0     5943 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json
--rwxr-xr-x   0        0        0     1870 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json
--rwxr-xr-x   0        0        0    10370 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json
--rwxr-xr-x   0        0        0     1780 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json
--rwxr-xr-x   0        0        0     6614 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEventRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEventResponse.json
--rwxr-xr-x   0        0        0     7005 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyMonitoringReportRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyMonitoringReportResponse.json
--rwxr-xr-x   0        0        0     8608 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyReportRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyReportResponse.json
--rwxr-xr-x   0        0        0     1668 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/PublishFirmwareRequest.json
--rwxr-xr-x   0        0        0     1691 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/PublishFirmwareResponse.json
--rwxr-xr-x   0        0        0     1631 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json
--rwxr-xr-x   0        0        0    14700 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ReportChargingProfilesRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.818506 ocpp-2.0.0rc0/ocpp/v201/schemas/ReportChargingProfilesResponse.json
--rwxr-xr-x   0        0        0    15964 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/RequestStartTransactionRequest.json
--rwxr-xr-x   0        0        0     2080 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/RequestStartTransactionResponse.json
--rwxr-xr-x   0        0        0      844 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/RequestStopTransactionRequest.json
--rwxr-xr-x   0        0        0     1760 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/RequestStopTransactionResponse.json
--rwxr-xr-x   0        0        0     1133 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/ReservationStatusUpdateRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/ReservationStatusUpdateResponse.json
--rwxr-xr-x   0        0        0     3649 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/ReserveNowRequest.json
--rwxr-xr-x   0        0        0     1758 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/ReserveNowResponse.json
--rwxr-xr-x   0        0        0     1144 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/ResetRequest.json
--rwxr-xr-x   0        0        0     1730 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/ResetResponse.json
--rwxr-xr-x   0        0        0     1120 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SecurityEventNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SecurityEventNotificationResponse.json
--rwxr-xr-x   0        0        0     7733 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SendLocalListRequest.json
--rwxr-xr-x   0        0        0     1810 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SendLocalListResponse.json
--rwxr-xr-x   0        0        0    13730 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetChargingProfileRequest.json
--rwxr-xr-x   0        0        0     1913 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetChargingProfileResponse.json
--rwxr-xr-x   0        0        0     5989 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetDisplayMessageRequest.json
--rwxr-xr-x   0        0        0     1848 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetDisplayMessageResponse.json
--rwxr-xr-x   0        0        0     1005 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetMonitoringBaseRequest.json
--rwxr-xr-x   0        0        0     1789 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetMonitoringBaseResponse.json
--rwxr-xr-x   0        0        0     2087 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetMonitoringLevelRequest.json
--rwxr-xr-x   0        0        0     1718 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetMonitoringLevelResponse.json
--rwxr-xr-x   0        0        0     7613 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetNetworkProfileRequest.json
--rwxr-xr-x   0        0        0     1710 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetNetworkProfileResponse.json
--rwxr-xr-x   0        0        0     5959 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetVariableMonitoringRequest.json
--rwxr-xr-x   0        0        0     6923 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetVariableMonitoringResponse.json
--rwxr-xr-x   0        0        0     4272 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetVariablesRequest.json
--rwxr-xr-x   0        0        0     5035 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SetVariablesResponse.json
--rwxr-xr-x   0        0        0     1481 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SignCertificateRequest.json
--rwxr-xr-x   0        0        0     1699 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/SignCertificateResponse.json
--rwxr-xr-x   0        0        0     1570 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/StatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/StatusNotificationResponse.json
--rwxr-xr-x   0        0        0    14824 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/TransactionEventRequest.json
--rwxr-xr-x   0        0        0     7606 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/TransactionEventResponse.json
--rwxr-xr-x   0        0        0     1996 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/TriggerMessageRequest.json
--rwxr-xr-x   0        0        0     1772 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/TriggerMessageResponse.json
--rwxr-xr-x   0        0        0      970 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/UnlockConnectorRequest.json
--rwxr-xr-x   0        0        0     1776 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/UnlockConnectorResponse.json
--rwxr-xr-x   0        0        0      837 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/UnpublishFirmwareRequest.json
--rwxr-xr-x   0        0        0     1059 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/UnpublishFirmwareResponse.json
--rwxr-xr-x   0        0        0     2765 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/UpdateFirmwareRequest.json
--rwxr-xr-x   0        0        0     1824 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/ocpp/v201/schemas/UpdateFirmwareResponse.json
--rw-r--r--   0        0        0     1581 2024-05-22 09:38:52.822506 ocpp-2.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 ocpp-2.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-06-03 14:39:03.801852 ocpp-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     6872 2024-06-03 14:39:03.801852 ocpp-2.0.0rc1/README.rst
+-rw-r--r--   0        0        0        0 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/__init__.py
+-rw-r--r--   0        0        0    16539 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/charge_point.py
+-rw-r--r--   0        0        0     4451 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/exceptions.py
+-rw-r--r--   0        0        0      221 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/experimental/v21/README.rst
+-rw-r--r--   0        0        0    14821 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/messages.py
+-rw-r--r--   0        0        0     4106 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/routing.py
+-rw-r--r--   0        0        0      186 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/__init__.py
+-rw-r--r--   0        0        0    20548 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/call.py
+-rw-r--r--   0        0        0    19232 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/call_result.py
+-rw-r--r--   0        0        0     3968 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/datatypes.py
+-rw-r--r--   0        0        0    23663 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/enums.py
+-rw-r--r--   0        0        0      306 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/Authorize.json
+-rw-r--r--   0        0        0     1062 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/AuthorizeResponse.json
+-rw-r--r--   0        0        0     1139 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/BootNotification.json
+-rw-r--r--   0        0        0      655 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/BootNotificationResponse.json
+-rw-r--r--   0        0        0      302 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/CancelReservation.json
+-rw-r--r--   0        0        0      423 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/CancelReservationResponse.json
+-rw-r--r--   0        0        0      352 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/CertificateSigned.json
+-rw-r--r--   0        0        0      505 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/CertificateSignedResponse.json
+-rw-r--r--   0        0        0      512 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ChangeAvailability.json
+-rw-r--r--   0        0        0      453 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ChangeAvailabilityResponse.json
+-rw-r--r--   0        0        0      418 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ChangeConfiguration.json
+-rw-r--r--   0        0        0      491 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ChangeConfigurationResponse.json
+-rw-r--r--   0        0        0      174 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ClearCache.json
+-rw-r--r--   0        0        0      416 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ClearCacheResponse.json
+-rw-r--r--   0        0        0      637 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ClearChargingProfile.json
+-rw-r--r--   0        0        0      425 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ClearChargingProfileResponse.json
+-rw-r--r--   0        0        0      466 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/DataTransfer.json
+-rw-r--r--   0        0        0      547 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/DataTransferResponse.json
+-rw-r--r--   0        0        0     1156 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/DeleteCertificate.json
+-rw-r--r--   0        0        0      523 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/DeleteCertificateResponse.json
+-rw-r--r--   0        0        0      491 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/DiagnosticsStatusNotification.json
+-rw-r--r--   0        0        0      194 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/DiagnosticsStatusNotificationResponse.json
+-rw-r--r--   0        0        0      760 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ExtendedTriggerMessage.json
+-rw-r--r--   0        0        0      530 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json
+-rw-r--r--   0        0        0      591 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/FirmwareStatusNotification.json
+-rw-r--r--   0        0        0      191 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/FirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0      539 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetCompositeSchedule.json
+-rw-r--r--   0        0        0     2139 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetCompositeScheduleResponse.json
+-rw-r--r--   0        0        0      344 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetConfiguration.json
+-rw-r--r--   0        0        0     1066 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetConfigurationResponse.json
+-rw-r--r--   0        0        0      642 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetDiagnostics.json
+-rw-r--r--   0        0        0      275 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetDiagnosticsResponse.json
+-rw-r--r--   0        0        0      552 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetInstalledCertificateIds.json
+-rw-r--r--   0        0        0     1566 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json
+-rw-r--r--   0        0        0      183 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetLocalListVersion.json
+-rw-r--r--   0        0        0      301 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetLocalListVersionResponse.json
+-rw-r--r--   0        0        0     1184 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetLog.json
+-rw-r--r--   0        0        0      566 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/GetLogResponse.json
+-rw-r--r--   0        0        0      173 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/Heartbeat.json
+-rw-r--r--   0        0        0      325 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/HeartbeatResponse.json
+-rw-r--r--   0        0        0      639 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/InstallCertificate.json
+-rw-r--r--   0        0        0      526 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/InstallCertificateResponse.json
+-rw-r--r--   0        0        0      667 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/LogStatusNotification.json
+-rw-r--r--   0        0        0      173 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/LogStatusNotificationResponse.json
+-rw-r--r--   0        0        0     6758 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/MeterValues.json
+-rw-r--r--   0        0        0      176 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/MeterValuesResponse.json
+-rw-r--r--   0        0        0     4383 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/RemoteStartTransaction.json
+-rw-r--r--   0        0        0      428 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/RemoteStartTransactionResponse.json
+-rw-r--r--   0        0        0      306 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/RemoteStopTransaction.json
+-rw-r--r--   0        0        0      427 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/RemoteStopTransactionResponse.json
+-rw-r--r--   0        0        0      704 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ReserveNow.json
+-rw-r--r--   0        0        0      502 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ReserveNowResponse.json
+-rw-r--r--   0        0        0      398 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/Reset.json
+-rw-r--r--   0        0        0      411 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/ResetResponse.json
+-rw-r--r--   0        0        0      464 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SecurityEventNotification.json
+-rw-r--r--   0        0        0      177 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SecurityEventNotificationResponse.json
+-rw-r--r--   0        0        0     2146 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SendLocalList.json
+-rw-r--r--   0        0        0      484 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SendLocalListResponse.json
+-rw-r--r--   0        0        0     4310 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SetChargingProfile.json
+-rw-r--r--   0        0        0      456 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SetChargingProfileResponse.json
+-rw-r--r--   0        0        0      287 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SignCertificate.json
+-rw-r--r--   0        0        0      483 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SignCertificateResponse.json
+-rw-r--r--   0        0        0      876 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SignedFirmwareStatusNotification.json
+-rw-r--r--   0        0        0      184 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SignedFirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0     1212 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SignedUpdateFirmware.json
+-rw-r--r--   0        0        0      590 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json
+-rw-r--r--   0        0        0      676 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/StartTransaction.json
+-rw-r--r--   0        0        0     1162 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/StartTransactionResponse.json
+-rw-r--r--   0        0        0     1805 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/StatusNotification.json
+-rw-r--r--   0        0        0      183 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/StatusNotificationResponse.json
+-rw-r--r--   0        0        0     7313 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/StopTransaction.json
+-rw-r--r--   0        0        0     1023 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/StopTransactionResponse.json
+-rw-r--r--   0        0        0      678 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/TriggerMessage.json
+-rw-r--r--   0        0        0      454 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/TriggerMessageResponse.json
+-rw-r--r--   0        0        0      296 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/UnlockConnector.json
+-rw-r--r--   0        0        0      457 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/UnlockConnectorResponse.json
+-rw-r--r--   0        0        0      572 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/UpdateFirmware.json
+-rw-r--r--   0        0        0      179 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v16/schemas/UpdateFirmwareResponse.json
+-rw-r--r--   0        0        0      189 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v201/__init__.py
+-rw-r--r--   0        0        0    34073 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v201/call.py
+-rw-r--r--   0        0        0    32301 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v201/call_result.py
+-rw-r--r--   0        0        0    22081 2024-06-03 14:39:03.961852 ocpp-2.0.0rc1/ocpp/v201/datatypes.py
+-rw-r--r--   0        0        0    80113 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/enums.py
+-rwxr-xr-x   0        0        0     4203 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/AuthorizeRequest.json
+-rwxr-xr-x   0        0        0     7208 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/AuthorizeResponse.json
+-rwxr-xr-x   0        0        0     3161 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/BootNotificationRequest.json
+-rwxr-xr-x   0        0        0     2270 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/BootNotificationResponse.json
+-rwxr-xr-x   0        0        0      775 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/CancelReservationRequest.json
+-rwxr-xr-x   0        0        0     1758 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/CancelReservationResponse.json
+-rwxr-xr-x   0        0        0     1914 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/CertificateSignedRequest.json
+-rwxr-xr-x   0        0        0     1752 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/CertificateSignedResponse.json
+-rwxr-xr-x   0        0        0     1811 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ChangeAvailabilityRequest.json
+-rwxr-xr-x   0        0        0     1783 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ChangeAvailabilityResponse.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearCacheRequest.json
+-rwxr-xr-x   0        0        0     1735 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearCacheResponse.json
+-rwxr-xr-x   0        0        0     2574 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearChargingProfileRequest.json
+-rwxr-xr-x   0        0        0     1752 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearChargingProfileResponse.json
+-rwxr-xr-x   0        0        0      787 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearDisplayMessageRequest.json
+-rwxr-xr-x   0        0        0     1735 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearDisplayMessageResponse.json
+-rwxr-xr-x   0        0        0      865 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearVariableMonitoringRequest.json
+-rwxr-xr-x   0        0        0     2327 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearVariableMonitoringResponse.json
+-rwxr-xr-x   0        0        0     1087 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearedChargingLimitRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ClearedChargingLimitResponse.json
+-rwxr-xr-x   0        0        0     1121 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/CostUpdatedRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/CostUpdatedResponse.json
+-rwxr-xr-x   0        0        0     4659 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/CustomerInformationRequest.json
+-rwxr-xr-x   0        0        0     1740 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/CustomerInformationResponse.json
+-rwxr-xr-x   0        0        0     1101 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/DataTransferRequest.json
+-rwxr-xr-x   0        0        0     1869 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/DataTransferResponse.json
+-rwxr-xr-x   0        0        0     1808 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/DeleteCertificateRequest.json
+-rwxr-xr-x   0        0        0     1747 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/DeleteCertificateResponse.json
+-rwxr-xr-x   0        0        0     1539 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json
+-rwxr-xr-x   0        0        0     1424 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/Get15118EVCertificateRequest.json
+-rwxr-xr-x   0        0        0     1915 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/Get15118EVCertificateResponse.json
+-rwxr-xr-x   0        0        0     1105 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetBaseReportRequest.json
+-rwxr-xr-x   0        0        0     1794 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetBaseReportResponse.json
+-rwxr-xr-x   0        0        0     1957 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetCertificateStatusRequest.json
+-rwxr-xr-x   0        0        0     2089 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetCertificateStatusResponse.json
+-rwxr-xr-x   0        0        0     3622 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetChargingProfilesRequest.json
+-rwxr-xr-x   0        0        0     1859 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetChargingProfilesResponse.json
+-rwxr-xr-x   0        0        0     1329 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetCompositeScheduleRequest.json
+-rwxr-xr-x   0        0        0     5095 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetCompositeScheduleResponse.json
+-rwxr-xr-x   0        0        0     1874 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetDisplayMessagesRequest.json
+-rwxr-xr-x   0        0        0     1841 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetDisplayMessagesResponse.json
+-rwxr-xr-x   0        0        0     1204 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json
+-rwxr-xr-x   0        0        0     3997 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetLocalListVersionRequest.json
+-rwxr-xr-x   0        0        0      840 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetLocalListVersionResponse.json
+-rwxr-xr-x   0        0        0     2802 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetLogRequest.json
+-rwxr-xr-x   0        0        0     1954 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetLogResponse.json
+-rwxr-xr-x   0        0        0     4175 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetMonitoringReportRequest.json
+-rwxr-xr-x   0        0        0     1800 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetMonitoringReportResponse.json
+-rwxr-xr-x   0        0        0     4143 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetReportRequest.json
+-rwxr-xr-x   0        0        0     1800 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetReportResponse.json
+-rwxr-xr-x   0        0        0      784 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetTransactionStatusRequest.json
+-rwxr-xr-x   0        0        0      910 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetTransactionStatusResponse.json
+-rwxr-xr-x   0        0        0     3931 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetVariablesRequest.json
+-rwxr-xr-x   0        0        0     5581 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/GetVariablesResponse.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/HeartbeatRequest.json
+-rwxr-xr-x   0        0        0      802 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/HeartbeatResponse.json
+-rwxr-xr-x   0        0        0     1226 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/InstallCertificateRequest.json
+-rwxr-xr-x   0        0        0     1751 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/InstallCertificateResponse.json
+-rwxr-xr-x   0        0        0     1361 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/LogStatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/LogStatusNotificationResponse.json
+-rwxr-xr-x   0        0        0     7709 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/MeterValuesRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/MeterValuesResponse.json
+-rwxr-xr-x   0        0        0    11333 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyChargingLimitRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyChargingLimitResponse.json
+-rwxr-xr-x   0        0        0     1542 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyCustomerInformationRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyCustomerInformationResponse.json
+-rwxr-xr-x   0        0        0     6512 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json
+-rwxr-xr-x   0        0        0     5943 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json
+-rwxr-xr-x   0        0        0     1870 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json
+-rwxr-xr-x   0        0        0    10370 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json
+-rwxr-xr-x   0        0        0     1780 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json
+-rwxr-xr-x   0        0        0     6614 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEventRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEventResponse.json
+-rwxr-xr-x   0        0        0     7005 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyMonitoringReportRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyMonitoringReportResponse.json
+-rwxr-xr-x   0        0        0     8608 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyReportRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyReportResponse.json
+-rwxr-xr-x   0        0        0     1668 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/PublishFirmwareRequest.json
+-rwxr-xr-x   0        0        0     1691 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/PublishFirmwareResponse.json
+-rwxr-xr-x   0        0        0     1631 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json
+-rwxr-xr-x   0        0        0    14700 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ReportChargingProfilesRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/ReportChargingProfilesResponse.json
+-rwxr-xr-x   0        0        0    15964 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/RequestStartTransactionRequest.json
+-rwxr-xr-x   0        0        0     2080 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/RequestStartTransactionResponse.json
+-rwxr-xr-x   0        0        0      844 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/RequestStopTransactionRequest.json
+-rwxr-xr-x   0        0        0     1760 2024-06-03 14:39:03.965852 ocpp-2.0.0rc1/ocpp/v201/schemas/RequestStopTransactionResponse.json
+-rwxr-xr-x   0        0        0     1133 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/ReservationStatusUpdateRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/ReservationStatusUpdateResponse.json
+-rwxr-xr-x   0        0        0     3649 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/ReserveNowRequest.json
+-rwxr-xr-x   0        0        0     1758 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/ReserveNowResponse.json
+-rwxr-xr-x   0        0        0     1144 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/ResetRequest.json
+-rwxr-xr-x   0        0        0     1730 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/ResetResponse.json
+-rwxr-xr-x   0        0        0     1120 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SecurityEventNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SecurityEventNotificationResponse.json
+-rwxr-xr-x   0        0        0     7733 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SendLocalListRequest.json
+-rwxr-xr-x   0        0        0     1810 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SendLocalListResponse.json
+-rwxr-xr-x   0        0        0    13730 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetChargingProfileRequest.json
+-rwxr-xr-x   0        0        0     1913 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetChargingProfileResponse.json
+-rwxr-xr-x   0        0        0     5989 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetDisplayMessageRequest.json
+-rwxr-xr-x   0        0        0     1848 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetDisplayMessageResponse.json
+-rwxr-xr-x   0        0        0     1005 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetMonitoringBaseRequest.json
+-rwxr-xr-x   0        0        0     1789 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetMonitoringBaseResponse.json
+-rwxr-xr-x   0        0        0     2087 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetMonitoringLevelRequest.json
+-rwxr-xr-x   0        0        0     1718 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetMonitoringLevelResponse.json
+-rwxr-xr-x   0        0        0     7613 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetNetworkProfileRequest.json
+-rwxr-xr-x   0        0        0     1710 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetNetworkProfileResponse.json
+-rwxr-xr-x   0        0        0     5959 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetVariableMonitoringRequest.json
+-rwxr-xr-x   0        0        0     6923 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetVariableMonitoringResponse.json
+-rwxr-xr-x   0        0        0     4272 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetVariablesRequest.json
+-rwxr-xr-x   0        0        0     5035 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SetVariablesResponse.json
+-rwxr-xr-x   0        0        0     1481 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SignCertificateRequest.json
+-rwxr-xr-x   0        0        0     1699 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/SignCertificateResponse.json
+-rwxr-xr-x   0        0        0     1570 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/StatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/StatusNotificationResponse.json
+-rwxr-xr-x   0        0        0    14824 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/TransactionEventRequest.json
+-rwxr-xr-x   0        0        0     7606 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/TransactionEventResponse.json
+-rwxr-xr-x   0        0        0     1996 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/TriggerMessageRequest.json
+-rwxr-xr-x   0        0        0     1772 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/TriggerMessageResponse.json
+-rwxr-xr-x   0        0        0      970 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/UnlockConnectorRequest.json
+-rwxr-xr-x   0        0        0     1776 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/UnlockConnectorResponse.json
+-rwxr-xr-x   0        0        0      837 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/UnpublishFirmwareRequest.json
+-rwxr-xr-x   0        0        0     1059 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/UnpublishFirmwareResponse.json
+-rwxr-xr-x   0        0        0     2765 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/UpdateFirmwareRequest.json
+-rwxr-xr-x   0        0        0     1824 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/ocpp/v201/schemas/UpdateFirmwareResponse.json
+-rw-r--r--   0        0        0     1581 2024-06-03 14:39:03.969852 ocpp-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 ocpp-2.0.0rc1/PKG-INFO
```

### Comparing `ocpp-2.0.0rc0/LICENSE` & `ocpp-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/README.rst` & `ocpp-2.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/charge_point.py` & `ocpp-2.0.0rc1/ocpp/charge_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 
     Inspired by: https://stackoverflow.com/a/1176023/1073222
 
     """
     if isinstance(data, dict):
         snake_case_dict = {}
         for key, value in data.items():
-            key = key.replace("ocppCSMS", "ocpp_csms")
-            key = key.replace("V2X", "_v2x")
+            key = key.replace("ocppCSMSURL", "ocpp_csms_url")
             key = key.replace("V2X", "_v2x").replace("V2G", "_v2g")
             s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", key)
             key = re.sub("([a-z0-9])([A-Z])(?=\\S)", r"\1_\2", s1).lower()
 
             snake_case_dict[key] = camel_to_snake_case(value)
 
         return snake_case_dict
@@ -53,15 +52,18 @@
     Inspired by: https://stackoverflow.com/a/19053800/1073222
     """
     if isinstance(data, dict):
         camel_case_dict = {}
         for key, value in data.items():
             key = key.replace("soc", "SoC")
             key = key.replace("_v2x", "V2X")
-            key = key.replace("ocpp_csms", "ocppCSMS")
+            # The spec uses inconsent casing for "csms" and "url".
+            # E.g. "OcppCsmsUrl" vs "ResponderURL" and "CSMSRootCertificate"
+            key = key.replace("ocpp_csms_url", "ocppCsmsUrl")
+            key = key.replace("csms", "CSMS")
             key = key.replace("_url", "URL")
             key = key.replace("soc", "SoC").replace("_SoCket", "Socket")
             key = key.replace("_v2x", "V2X")
             key = key.replace("soc_limit_reached", "SOCLimitReached")
             key = key.replace("_v2x", "V2X").replace("_v2g", "V2G")
             components = key.split("_")
             key = components[0] + "".join(x[:1].upper() + x[1:] for x in components[1:])
```

### Comparing `ocpp-2.0.0rc0/ocpp/exceptions.py` & `ocpp-2.0.0rc1/ocpp/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/messages.py` & `ocpp-2.0.0rc1/ocpp/messages.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/routing.py` & `ocpp-2.0.0rc1/ocpp/routing.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/call.py` & `ocpp-2.0.0rc1/ocpp/v16/call.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/call_result.py` & `ocpp-2.0.0rc1/ocpp/v16/call_result.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/datatypes.py` & `ocpp-2.0.0rc1/ocpp/v16/datatypes.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/enums.py` & `ocpp-2.0.0rc1/ocpp/v16/enums.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/AuthorizeResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/AuthorizeResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/BootNotification.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/BootNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/BootNotificationResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/BootNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/ChangeAvailability.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/ChangeAvailability.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/ClearChargingProfile.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/ClearChargingProfile.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/DataTransferResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/DataTransferResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/DeleteCertificate.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/DeleteCertificate.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/DeleteCertificateResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/DeleteCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/ExtendedTriggerMessage.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/ExtendedTriggerMessage.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/FirmwareStatusNotification.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/FirmwareStatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/GetCompositeSchedule.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/GetCompositeSchedule.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/GetCompositeScheduleResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/GetCompositeScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/GetConfigurationResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/GetConfigurationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/GetDiagnostics.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/GetDiagnostics.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/GetInstalledCertificateIds.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/GetInstalledCertificateIds.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/GetLog.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/GetLog.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/GetLogResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/GetLogResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/InstallCertificate.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/InstallCertificate.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/InstallCertificateResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/InstallCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/LogStatusNotification.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/LogStatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/MeterValues.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/MeterValues.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/RemoteStartTransaction.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/RemoteStartTransaction.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/ReserveNow.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/ReserveNow.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/SendLocalList.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/SendLocalList.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/SetChargingProfile.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/SetChargingProfile.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/SignedFirmwareStatusNotification.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/SignedFirmwareStatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/SignedUpdateFirmware.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/SignedUpdateFirmware.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/StartTransaction.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/StartTransaction.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/StartTransactionResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/StartTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/StatusNotification.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/StatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/StopTransaction.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/StopTransaction.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/StopTransactionResponse.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/StopTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/TriggerMessage.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/TriggerMessage.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v16/schemas/UpdateFirmware.json` & `ocpp-2.0.0rc1/ocpp/v16/schemas/UpdateFirmware.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/call.py` & `ocpp-2.0.0rc1/ocpp/v201/call.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/call_result.py` & `ocpp-2.0.0rc1/ocpp/v201/call_result.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/datatypes.py` & `ocpp-2.0.0rc1/ocpp/v201/datatypes.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/enums.py` & `ocpp-2.0.0rc1/ocpp/v201/enums.py`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/AuthorizeRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/AuthorizeRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/AuthorizeResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/AuthorizeResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/BootNotificationRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/BootNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/BootNotificationResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/BootNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/CancelReservationRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/CancelReservationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/CancelReservationResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/CancelReservationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/CertificateSignedRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/CertificateSignedRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/CertificateSignedResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/CertificateSignedResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ChangeAvailabilityRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ChangeAvailabilityRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ChangeAvailabilityResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ChangeAvailabilityResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearCacheRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearCacheRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearCacheResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearCacheResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearChargingProfileRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearChargingProfileRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearChargingProfileResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearChargingProfileResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearDisplayMessageRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearDisplayMessageRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearDisplayMessageResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearDisplayMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearVariableMonitoringRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearVariableMonitoringRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearVariableMonitoringResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearVariableMonitoringResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearedChargingLimitRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearedChargingLimitRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ClearedChargingLimitResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ClearedChargingLimitResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/CostUpdatedRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/CostUpdatedRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/CostUpdatedResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/CostUpdatedResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/CustomerInformationRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/CustomerInformationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/CustomerInformationResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/CustomerInformationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/DataTransferRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/DataTransferRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/DataTransferResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/DataTransferResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/DeleteCertificateRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/DeleteCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/DeleteCertificateResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/DeleteCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/Get15118EVCertificateRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/Get15118EVCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/Get15118EVCertificateResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/Get15118EVCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetBaseReportRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetBaseReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetBaseReportResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetBaseReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetCertificateStatusRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetCertificateStatusRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetCertificateStatusResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetCertificateStatusResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetChargingProfilesRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetChargingProfilesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetChargingProfilesResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetChargingProfilesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetCompositeScheduleRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetCompositeScheduleRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetCompositeScheduleResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetCompositeScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetDisplayMessagesRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetDisplayMessagesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetDisplayMessagesResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetDisplayMessagesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetLocalListVersionRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetLocalListVersionRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetLocalListVersionResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetLocalListVersionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetLogRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetLogRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetLogResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetLogResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetMonitoringReportRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetMonitoringReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetMonitoringReportResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetMonitoringReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetReportRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetReportResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetTransactionStatusRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetTransactionStatusRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetTransactionStatusResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetTransactionStatusResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetVariablesRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetVariablesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/GetVariablesResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/GetVariablesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/HeartbeatRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/HeartbeatRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/HeartbeatResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/HeartbeatResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/InstallCertificateRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/InstallCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/InstallCertificateResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/InstallCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/LogStatusNotificationRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/LogStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/LogStatusNotificationResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/LogStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/MeterValuesRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/MeterValuesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/MeterValuesResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/MeterValuesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyChargingLimitRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyChargingLimitRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyChargingLimitResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyChargingLimitResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyCustomerInformationRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyCustomerInformationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyCustomerInformationResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyCustomerInformationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEventRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEventRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyEventResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyEventResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyMonitoringReportRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyMonitoringReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyMonitoringReportResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyMonitoringReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyReportRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/NotifyReportResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/NotifyReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/PublishFirmwareRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/PublishFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/PublishFirmwareResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/PublishFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ReportChargingProfilesRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ReportChargingProfilesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ReportChargingProfilesResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ReportChargingProfilesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/RequestStartTransactionRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/RequestStartTransactionRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/RequestStartTransactionResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/RequestStartTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/RequestStopTransactionRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/RequestStopTransactionRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/RequestStopTransactionResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/RequestStopTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ReservationStatusUpdateRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ReservationStatusUpdateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ReservationStatusUpdateResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ReservationStatusUpdateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ReserveNowRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ReserveNowRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ReserveNowResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ReserveNowResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ResetRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ResetRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/ResetResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/ResetResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SecurityEventNotificationRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SecurityEventNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SecurityEventNotificationResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SecurityEventNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SendLocalListRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SendLocalListRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SendLocalListResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SendLocalListResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetChargingProfileRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetChargingProfileRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetChargingProfileResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetChargingProfileResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetDisplayMessageRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetDisplayMessageRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetDisplayMessageResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetDisplayMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetMonitoringBaseRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetMonitoringBaseRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetMonitoringBaseResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetMonitoringBaseResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetMonitoringLevelRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetMonitoringLevelRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetMonitoringLevelResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetMonitoringLevelResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetNetworkProfileRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetNetworkProfileRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetNetworkProfileResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetNetworkProfileResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetVariableMonitoringRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetVariableMonitoringRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetVariableMonitoringResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetVariableMonitoringResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetVariablesRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetVariablesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SetVariablesResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SetVariablesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SignCertificateRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SignCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/SignCertificateResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/SignCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/StatusNotificationRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/StatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/StatusNotificationResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/StatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/TransactionEventRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/TransactionEventRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/TransactionEventResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/TransactionEventResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/TriggerMessageRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/TriggerMessageRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/TriggerMessageResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/TriggerMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/UnlockConnectorRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/UnlockConnectorRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/UnlockConnectorResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/UnlockConnectorResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/UnpublishFirmwareRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/UnpublishFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/UnpublishFirmwareResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/UnpublishFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/UpdateFirmwareRequest.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/UpdateFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/ocpp/v201/schemas/UpdateFirmwareResponse.json` & `ocpp-2.0.0rc1/ocpp/v201/schemas/UpdateFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-2.0.0rc0/pyproject.toml` & `ocpp-2.0.0rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ocpp"
-version = "2.0.0-rc.0"
+version = "2.0.0-rc.1"
 description = "Python package implementing the JSON version of the Open Charge Point Protocol (OCPP)."
 authors = [
 	"André Duarte <andre15x@gmail.com>",
 	"Auke Willem Oosterhoff <aukewillem.oosterhoff@mobilityhouse.com>",
 	"Greg Lutostanski <greg.luto@gmail.com>",
 	"Jared Newell <jared.newell@mobilityhouse.com>",
 	"Jonathan Herrmann <jonathan.herrmann@mobilityhouse.com>",
```

### Comparing `ocpp-2.0.0rc0/PKG-INFO` & `ocpp-2.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocpp
-Version: 2.0.0rc0
+Version: 2.0.0rc1
 Summary: Python package implementing the JSON version of the Open Charge Point Protocol (OCPP).
 Home-page: https://github.com/mobilityhouse/ocpp
 License: MIT
 Author: André Duarte
 Author-email: andre15x@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

